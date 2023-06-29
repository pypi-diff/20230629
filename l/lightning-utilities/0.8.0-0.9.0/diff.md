# Comparing `tmp/lightning-utilities-0.8.0.tar.gz` & `tmp/lightning-utilities-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-utilities-0.8.0.tar", last modified: Fri Mar 10 11:21:26 2023, max compression
+gzip compressed data, was "lightning-utilities-0.9.0.tar", last modified: Thu Jun 29 18:27:37 2023, max compression
```

## Comparing `lightning-utilities-0.8.0.tar` & `lightning-utilities-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.428289 lightning-utilities-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/requirements/cli.txt
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.428289 lightning-utilities-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.428289 lightning-utilities-0.8.0/src/lightning_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/src/lightning_utilities/core/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/core/rank_zero.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/src/lightning_utilities/install/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/install/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/src/lightning_utilities/test/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-10 11:21:10.000000 lightning-utilities-0.8.0/src/lightning_utilities/test/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:21:26.432289 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-10 11:21:26.000000 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-10 11:21:26.000000 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 11:21:26.000000 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 11:21:26.000000 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-10 11:21:26.000000 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 11:21:26.000000 lightning-utilities-0.8.0/src/lightning_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.292365 lightning-utilities-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-29 18:27:37.292365 lightning-utilities-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/requirements/cli.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/requirements/dev-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/requirements/dev-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:27:37.292365 lightning-utilities-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2969 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.284365 lightning-utilities-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/src/lightning_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/src/lightning_utilities/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/core/rank_zero.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/src/lightning_utilities/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/docs/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/docs/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/src/lightning_utilities/install/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/install/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/src/lightning_utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-29 18:27:22.000000 lightning-utilities-0.9.0/src/lightning_utilities/test/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:27:37.288365 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-29 18:27:37.000000 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-29 18:27:37.000000 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:27:37.000000 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:27:37.000000 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 18:27:37.000000 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 18:27:37.000000 lightning-utilities-0.9.0/src/lightning_utilities.egg-info/top_level.txt
```

### Comparing `lightning-utilities-0.8.0/CHANGELOG.md` & `lightning-utilities-0.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.9.0] - 2023-06-29
+
+### Added
+
+- docs: fetch all external resources for building docs ([#142](https://github.com/Lightning-AI/utilities/pull/142))
+
+### Changed
+
+- CI: allow splitting docs's tests and make ([#141](https://github.com/Lightning-AI/utilities/pull/141))
+
+### Fixed
+
+- Fixed - do not erase function types in decorators ([#135](https://github.com/Lightning-AI/utilities/pull/135))
+- CI: fix passing install flags in package check ([#137](https://github.com/Lightning-AI/utilities/pull/137))
+
 ## [0.8.0] - 2023-03-10
 
 ### Added
 
 - Added requirements parser ([#107](https://github.com/Lightning-AI/utilities/pull/107))
 - Added workflow for checking markdown links ([#81](https://github.com/Lightning-AI/utilities/pull/81))
```

### Comparing `lightning-utilities-0.8.0/LICENSE` & `lightning-utilities-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-utilities-0.8.0/PKG-INFO` & `lightning-utilities-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-utilities
-Version: 0.8.0
+Version: 0.9.0
 Summary: PyTorch Lightning Sample project.
 Home-page: https://github.com/Lightning-AI/utilities
 Download-URL: https://github.com/Lightning-AI/utilities
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/utilities/issues
@@ -19,18 +19,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: cli
-Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: typing
+Provides-Extra: cli
 License-File: LICENSE
 
 # Lightning Utilities
 
 [![UnitTests](https://github.com/Lightning-AI/utilities/actions/workflows/ci-testing.yml/badge.svg?event=push)](https://github.com/Lightning-AI/utilities/actions/workflows/ci-testing.yml)
 [![Apply checks](https://github.com/Lightning-AI/utilities/actions/workflows/ci-use-checks.yaml/badge.svg?event=push)](https://github.com/Lightning-AI/utilities/actions/workflows/ci-use-checks.yaml)
 [![Docs Status](https://readthedocs.org/projects/lit-utilities/badge/?version=latest)](https://lit-utilities.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `lightning-utilities-0.8.0/README.md` & `lightning-utilities-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lightning-utilities-0.8.0/setup.py` & `lightning-utilities-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import find_packages, setup
 
 _PATH_ROOT = os.path.realpath(os.path.dirname(__file__))
 _PATH_SOURCE = os.path.join(_PATH_ROOT, "src")
 _PATH_REQUIRE = os.path.join(_PATH_ROOT, "requirements")
 
 
-def _load_py_module(fname, pkg="lightning_utilities"):
+def _load_py_module(fname: str, pkg: str = "lightning_utilities"):
     spec = spec_from_file_location(os.path.join(pkg, fname), os.path.join(_PATH_SOURCE, pkg, fname))
     py = module_from_spec(spec)
     spec.loader.exec_module(py)
     return py
 
 
 about = _load_py_module("__about__.py")
@@ -23,15 +23,15 @@
 # load basic requirements
 with open(os.path.join(_PATH_REQUIRE, "base.txt")) as fp:
     requirements = list(map(str, parse_requirements(fp.readlines())))
 
 # make extras as automated loading
 requirements_extra = {}
 for fpath in glob.glob(os.path.join(_PATH_REQUIRE, "*.txt")):
-    if os.path.basename(fpath) == "base.txt":
+    if os.path.basename(fpath) in ("base.txt", "dev-docs.txt", "dev-tests.txt"):
         continue
     name, _ = os.path.splitext(os.path.basename(fpath))
     with open(fpath) as fp:
         requirements_extra[name] = list(map(str, parse_requirements(fp.readline())))
 
 # loading readme as description
 with open(os.path.join(_PATH_ROOT, "README.md")) as fp:
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/__about__.py` & `lightning-utilities-0.9.0/src/lightning_utilities/__about__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import time
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2022-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/utilities"
 __docs__ = "PyTorch Lightning Sample project."
 __long_doc__ = """
-What is it?
------------
 This package allows for sharing GH workflows, CI/CD assistance actions, and Python utilities across the Lightning
 ecosystem.
 """
 
 __all__ = [
     "__author__",
     "__author_email__",
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/__init__.py` & `lightning-utilities-0.9.0/src/lightning_utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Root package info."""
 
 import os
 
-from lightning_utilities.__about__ import *  # noqa: F401, F403
+from lightning_utilities.__about__ import *  # noqa: F403
 from lightning_utilities.core.apply_func import apply_to_collection
 from lightning_utilities.core.enums import StrEnum
 from lightning_utilities.core.imports import compare_version, module_available
 from lightning_utilities.core.overrides import is_overridden
 from lightning_utilities.core.rank_zero import WarningCache
 
 _PACKAGE_ROOT = os.path.dirname(__file__)
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/core/apply_func.py` & `lightning-utilities-0.9.0/src/lightning_utilities/core/apply_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright The PyTorch Lightning team.
 # Licensed under the Apache License, Version 2.0 (the "License");
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 import dataclasses
-from collections import defaultdict, OrderedDict
+from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
 
 
 def is_namedtuple(obj: object) -> bool:
     """Check if object is type nametuple."""
     # https://github.com/pytorch/pytorch/blob/v1.8.1/torch/nn/parallel/scatter_gather.py#L4-L8
@@ -181,15 +181,16 @@
                 for k, v in zipped.items()
             }
         )
 
     is_namedtuple_ = is_namedtuple(data1)
     is_sequence = isinstance(data1, Sequence) and not isinstance(data1, str)
     if (is_namedtuple_ or is_sequence) and data2 is not None:
-        assert len(data1) == len(data2), "Sequence collections have different sizes."
+        if len(data1) != len(data2):
+            raise ValueError("Sequence collections have different sizes.")
         out = [
             apply_to_collections(v1, v2, dtype, function, *args, wrong_dtype=wrong_dtype, **kwargs)
             for v1, v2 in zip(data1, data2)
         ]
         return elem_type(*out) if is_namedtuple_ else elem_type(out)
 
     if is_dataclass_instance(data1) and data2 is not None:
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/core/enums.py` & `lightning-utilities-0.9.0/src/lightning_utilities/core/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     @classmethod
     def try_from_str(cls, value: str, source: Literal["key", "value", "any"] = "key") -> Optional["StrEnum"]:
         """Try to create emun and if it does not match any, return `None`."""
         try:
             return cls.from_str(value, source)
         except ValueError:
-            warnings.warn(
+            warnings.warn(  # noqa: B028
                 UserWarning(f"Invalid string: expected one of {cls._allowed_matches(source)}, but got {value}.")
             )
         return None
 
     @classmethod
     def _allowed_matches(cls, source: str) -> List[str]:
         keys, vals = [], []
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/core/imports.py` & `lightning-utilities-0.9.0/src/lightning_utilities/core/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 import functools
 import importlib
 import warnings
 from functools import lru_cache
 from importlib.util import find_spec
 from types import ModuleType
-from typing import Any, Callable, List, Optional
+from typing import Any, Callable, List, Optional, TypeVar
 
 import pkg_resources
 from packaging.requirements import Requirement
 from packaging.version import Version
+from typing_extensions import ParamSpec
+
+T = TypeVar("T")
+P = ParamSpec("P")
 
 try:
     from importlib import metadata
 except ImportError:
     # Python < 3.8
     import importlib_metadata as metadata  # type: ignore
 
@@ -256,15 +260,15 @@
 
     Returns:
         a proxy module object that will be lazily imported when first used
     """
     return LazyModule(module_name, callback=callback)
 
 
-def requires(*module_path: str, raise_exception: bool = True) -> Callable:
+def requires(*module_path: str, raise_exception: bool = True) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """Wrap early import failure with some nice exception message.
 
     Example:
         >>> @requires("libpath", raise_exception=bool(int(os.getenv("LIGHTING_TESTING", "0"))))
         ... def my_cwd():
         ...     from pathlib import Path
         ...     return Path(__file__).parent
@@ -273,21 +277,21 @@
         ...     @requires("math", "random")
         ...     def __init__(self):
         ...         from math import pow
         ...         from random import randint
         ...         self._rnd = pow(randint(1, 9), 2)
     """
 
-    def decorator(func: Callable) -> Callable:
+    def decorator(func: Callable[P, T]) -> Callable[P, T]:
         @functools.wraps(func)
-        def wrapper(*args: Any, **kwargs: Any) -> Any:
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             unavailable_modules = [module for module in module_path if not module_available(module)]
             if any(unavailable_modules):
                 msg = f"Required dependencies not available. Please run `pip install {' '.join(unavailable_modules)}`"
                 if raise_exception:
                     raise ModuleNotFoundError(msg)
-                warnings.warn(msg)
+                warnings.warn(msg, stacklevel=2)
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/core/inheritance.py` & `lightning-utilities-0.9.0/src/lightning_utilities/core/inheritance.py`

 * *Files identical despite different names*

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/core/overrides.py` & `lightning-utilities-0.9.0/src/lightning_utilities/core/overrides.py`

 * *Files identical despite different names*

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/core/rank_zero.py` & `lightning-utilities-0.9.0/src/lightning_utilities/core/rank_zero.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,32 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 """Utilities that can be used for calling functions on a particular rank."""
 import logging
 import warnings
 from functools import wraps
 from platform import python_version
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Optional, TypeVar, Union
+
+from typing_extensions import ParamSpec
 
 log = logging.getLogger(__name__)
 
+T = TypeVar("T")
+P = ParamSpec("P")
+
 
-def rank_zero_only(fn: Callable) -> Callable:
+def rank_zero_only(fn: Callable[P, T]) -> Callable[P, Optional[T]]:
     """Wrap a function to call internal function only in rank zero.
 
     Function that can be used as a decorator to enable a function/method being called only on global rank 0.
     """
 
     @wraps(fn)
-    def wrapped_fn(*args: Any, **kwargs: Any) -> Optional[Any]:
+    def wrapped_fn(*args: P.args, **kwargs: P.kwargs) -> Optional[T]:
         rank = getattr(rank_zero_only, "rank", None)
         if rank is None:
             raise RuntimeError("The `rank_zero_only.rank` needs to be set before use")
         if rank == 0:
             return fn(*args, **kwargs)
         return None
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities/install/requirements.py` & `lightning-utilities-0.9.0/src/lightning_utilities/install/requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 class _RequirementWithComment(Requirement):
     strict_string = "# strict"
 
     def __init__(self, *args: Any, comment: str = "", pip_argument: Optional[str] = None, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.comment = comment
-        assert pip_argument is None or pip_argument  # sanity check that it's not an empty str
+        if not (pip_argument is None or pip_argument):  # sanity check that it's not an empty str
+            raise RuntimeError(f"wrong pip argument: {pip_argument}")
         self.pip_argument = pip_argument
         self.strict = self.strict_string in comment.lower()
 
     def adjust(self, unfreeze: str) -> str:
         """Remove version restrictions unless they are strict.
 
         >>> _RequirementWithComment("arrow<=1.2.2,>=1.2.0", comment="# anything").adjust("none")
@@ -105,12 +106,14 @@
 
     >>> import os
     >>> from lightning_utilities import _PROJECT_ROOT
     >>> path_req = os.path.join(_PROJECT_ROOT, "requirements")
     >>> load_requirements(path_req, "docs.txt", unfreeze="major")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
     ['sphinx<6.0,>=4.0', ...]
     """
-    assert unfreeze in {"none", "major", "all"}
+    if unfreeze not in {"none", "major", "all"}:
+        raise ValueError(f'unsupported option of "{unfreeze}"')
     path = Path(path_dir) / file_name
-    assert path.exists(), (path_dir, file_name, path)
+    if not path.exists():
+        raise FileNotFoundError(f"missing file for {(path_dir, file_name, path)}")
     text = path.read_text()
     return [req.adjust(unfreeze) for req in _parse_requirements(text)]
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities.egg-info/PKG-INFO` & `lightning-utilities-0.9.0/src/lightning_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-utilities
-Version: 0.8.0
+Version: 0.9.0
 Summary: PyTorch Lightning Sample project.
 Home-page: https://github.com/Lightning-AI/utilities
 Download-URL: https://github.com/Lightning-AI/utilities
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/utilities/issues
@@ -19,18 +19,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: cli
-Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: typing
+Provides-Extra: cli
 License-File: LICENSE
 
 # Lightning Utilities
 
 [![UnitTests](https://github.com/Lightning-AI/utilities/actions/workflows/ci-testing.yml/badge.svg?event=push)](https://github.com/Lightning-AI/utilities/actions/workflows/ci-testing.yml)
 [![Apply checks](https://github.com/Lightning-AI/utilities/actions/workflows/ci-use-checks.yaml/badge.svg?event=push)](https://github.com/Lightning-AI/utilities/actions/workflows/ci-use-checks.yaml)
 [![Docs Status](https://readthedocs.org/projects/lit-utilities/badge/?version=latest)](https://lit-utilities.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `lightning-utilities-0.8.0/src/lightning_utilities.egg-info/SOURCES.txt` & `lightning-utilities-0.9.0/src/lightning_utilities.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 requirements/base.txt
 requirements/cli.txt
+requirements/dev-docs.txt
+requirements/dev-tests.txt
 requirements/docs.txt
-requirements/test.txt
 requirements/typing.txt
 src/lightning_utilities/__about__.py
 src/lightning_utilities/__init__.py
 src/lightning_utilities/py.typed
 src/lightning_utilities.egg-info/PKG-INFO
 src/lightning_utilities.egg-info/SOURCES.txt
 src/lightning_utilities.egg-info/dependency_links.txt
@@ -21,10 +22,14 @@
 src/lightning_utilities/core/__init__.py
 src/lightning_utilities/core/apply_func.py
 src/lightning_utilities/core/enums.py
 src/lightning_utilities/core/imports.py
 src/lightning_utilities/core/inheritance.py
 src/lightning_utilities/core/overrides.py
 src/lightning_utilities/core/rank_zero.py
+src/lightning_utilities/docs/__init__.py
+src/lightning_utilities/docs/formatting.py
+src/lightning_utilities/docs/retriever.py
 src/lightning_utilities/install/__init__.py
 src/lightning_utilities/install/requirements.py
+src/lightning_utilities/test/__init__.py
 src/lightning_utilities/test/warning.py
```

