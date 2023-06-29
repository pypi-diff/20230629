# Comparing `tmp/napari-graph-0.1.0.tar.gz` & `tmp/napari-graph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-graph-0.1.0.tar", last modified: Thu Jun  8 15:18:24 2023, max compression
+gzip compressed data, was "napari-graph-0.1.1.tar", last modified: Thu Jun 29 15:46:58 2023, max compression
```

## Comparing `napari-graph-0.1.0.tar` & `napari-graph-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      195 2023-05-12 19:42:43.000000 napari-graph-0.1.0/.coveragerc
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.113741 napari-graph-0.1.0/.github/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/.github/workflows/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      792 2023-05-12 19:42:15.000000 napari-graph-0.1.0/.github/workflows/build-docs.yml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      907 2023-05-12 19:42:16.000000 napari-graph-0.1.0/.github/workflows/deploy-docs.yml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2865 2023-05-12 19:42:43.000000 napari-graph-0.1.0/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1847 2023-05-12 19:42:16.000000 napari-graph-0.1.0/.gitignore
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1356 2023-05-12 19:42:16.000000 napari-graph-0.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1514 2023-05-26 16:03:32.000000 napari-graph-0.1.0/LICENSE
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1160 2023-06-08 15:18:24.117741 napari-graph-0.1.0/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      234 2023-06-08 15:14:59.000000 napari-graph-0.1.0/README.md
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/docs/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      650 2022-05-09 17:57:12.000000 napari-graph-0.1.0/docs/Makefile
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/docs/api/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       60 2022-05-09 17:57:12.000000 napari-graph-0.1.0/docs/api/api.md
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6627 2023-05-12 19:42:16.000000 napari-graph-0.1.0/docs/conf.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      134 2022-05-09 17:57:12.000000 napari-graph-0.1.0/docs/index.md
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      766 2022-05-09 17:57:12.000000 napari-graph-0.1.0/docs/make.bat
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      534 2023-05-12 19:42:16.000000 napari-graph-0.1.0/pyproject.toml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1189 2023-06-08 15:18:24.121741 napari-graph-0.1.0/setup.cfg
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/src/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/src/napari_graph/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      340 2023-05-12 19:42:43.000000 napari-graph-0.1.0/src/napari_graph/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/src/napari_graph/_tests/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     9696 2023-05-26 16:54:35.000000 napari-graph-0.1.0/src/napari_graph/_tests/test_graph.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      160 2023-06-08 15:18:24.000000 napari-graph-0.1.0/src/napari_graph/_version.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    23772 2023-06-08 15:14:59.000000 napari-graph-0.1.0/src/napari_graph/base_graph.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    14969 2023-05-12 19:42:43.000000 napari-graph-0.1.0/src/napari_graph/directed_graph.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     9439 2023-05-12 19:42:43.000000 napari-graph-0.1.0/src/napari_graph/undirected_graph.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-06-08 15:18:24.117741 napari-graph-0.1.0/src/napari_graph.egg-info/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1160 2023-06-08 15:18:24.000000 napari-graph-0.1.0/src/napari_graph.egg-info/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      671 2023-06-08 15:18:24.000000 napari-graph-0.1.0/src/napari_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-06-08 15:18:24.000000 napari-graph-0.1.0/src/napari_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      172 2023-06-08 15:18:24.000000 napari-graph-0.1.0/src/napari_graph.egg-info/requires.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       13 2023-06-08 15:18:24.000000 napari-graph-0.1.0/src/napari_graph.egg-info/top_level.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      857 2023-05-12 19:42:43.000000 napari-graph-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.774985 napari-graph-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.762983 napari-graph-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 15:46:42.000000 napari-graph-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-29 15:46:58.774985 napari-graph-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 15:46:42.000000 napari-graph-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/api/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-29 15:46:42.000000 napari-graph-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-29 15:46:58.774985 napari-graph-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.766984 napari-graph-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/src/napari_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.774985 napari-graph-0.1.1/src/napari_graph/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/_tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/_tests/test_interops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/interops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/undirected_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.774985 napari-graph-0.1.1/src/napari_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-29 15:46:42.000000 napari-graph-0.1.1/tox.ini
```

### Comparing `napari-graph-0.1.0/.github/workflows/build-docs.yml` & `napari-graph-0.1.1/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/.github/workflows/deploy-docs.yml` & `napari-graph-0.1.1/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/.github/workflows/test_and_deploy.yml` & `napari-graph-0.1.1/.github/workflows/test_and_deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,31 @@
   pull_request:
     branches:
       - master
       - main
   workflow_dispatch:
 
 jobs:
+  linting:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v2
+      - uses: actions/setup-python@v2
+
+        with:
+          python-version: "3.10"
+      - name: Install tox
+        run: |
+          pip install tox
+
+      - name: Run pre-commit to check linting and typing
+        run: tox -e linting
+
   test:
+    needs: [linting]
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.8', '3.9', '3.10']
 
@@ -77,16 +93,16 @@
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools setuptools_scm wheel twine
+          pip install -U setuptools setuptools_scm wheel twine build
       - name: Build and publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
         run: |
           git tag
-          python setup.py sdist bdist_wheel
+          python -m build --sdist --wheel
           twine upload dist/*
```

### Comparing `napari-graph-0.1.0/.gitignore` & `napari-graph-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/.pre-commit-config.yaml` & `napari-graph-0.1.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # make every import absolute
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.0
     hooks:
       - id: absolufy-imports
 # sorting imports
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black", "--filter-files"]
 # automatic upgrade to newer python versions syntax
   - repo: https://github.com/asottile/pyupgrade
     rev: v2.30.0
     hooks:
@@ -42,7 +42,13 @@
                --per-file-ignores,
                '__init__.py:F401']
 
   - repo: https://github.com/psf/black
     rev: 22.3.0
     hooks:
       - id: black
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.1.1
+    hooks:
+    - id: mypy
+      args: [--ignore-missing-imports]
```

### Comparing `napari-graph-0.1.0/LICENSE` & `napari-graph-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/PKG-INFO` & `napari-graph-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-graph
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fast editable graphs in Python and numba
 Home-page: https://github.com/napari/napari-graph
 Author: Jordão Bragantini, Jonas Windhager & Juan Nunez-Iglesias
 Author-email: jordao.bragantini@czbiohub.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-graph-0.1.0/docs/Makefile` & `napari-graph-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/docs/conf.py` & `napari-graph-0.1.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # Add the local code to the Python path, so docs are generated for
 # current working copy
 
+from typing import Any, Dict
+
 import napari_graph
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
@@ -152,15 +154,15 @@
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'napari-graph-docs'
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements = {
+latex_elements: Dict[str, Any] = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
```

### Comparing `napari-graph-0.1.0/docs/make.bat` & `napari-graph-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/pyproject.toml` & `napari-graph-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/setup.cfg` & `napari-graph-0.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 [options]
 package_dir = 
 	=src
 include_package_data = True
 packages = find:
 setup_requires = setuptools_scm
 install_requires = 
+	networkx
 	numba
 	numpy
 	pandas
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
```

### Comparing `napari-graph-0.1.0/src/napari_graph/_tests/test_graph.py` & `napari-graph-0.1.1/src/napari_graph/_tests/test_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import product
-from typing import Callable, List, Optional, Type
+from typing import Any, Callable, List, Optional, Protocol, Type
 
 import numpy as np
 import pandas as pd
 import pytest
 from numpy.typing import ArrayLike
 
 from napari_graph import DirectedGraph, UndirectedGraph
@@ -72,43 +72,96 @@
         graph.get_target_edges(np.roll(coords.index, -1))
     )
     assert np.all(source_edges == edges[:, np.newaxis, :])
     assert np.all(target_edges == edges[:, np.newaxis, :])
 
 
 @pytest.mark.parametrize("n_prealloc_nodes", [0, 3, 6, 12])
-def test_node_addition(n_prealloc_nodes: int) -> None:
+def test_node_addition_indices_coords(n_prealloc_nodes: int) -> None:
+    # test node addition with indices and coords and different pre-allocation size
     size = 6
     ndim = 3
 
     indices = np.random.choice(range(100), size=size, replace=False)
     coords = np.random.randn(size, ndim)
 
     graph = DirectedGraph(ndim=ndim, n_nodes=n_prealloc_nodes)
     for i in range(size):
-        graph.add_nodes(indices[i], coords[i])
+        graph.add_nodes(indices=indices[i], coords=coords[i])
         assert len(graph) == i + 1
 
     np.testing.assert_allclose(graph._coords[: len(graph)], coords)
     np.testing.assert_array_equal(graph._buffer2world[: len(graph)], indices)
     np.testing.assert_array_equal(
         graph._map_world2buffer(indices), range(size)
     )
 
 
+def test_node_addition_non_spatial() -> None:
+    graph = DirectedGraph()
+
+    size = 5
+    new_indices = graph.add_nodes(count=size)
+
+    np.testing.assert_array_equal(new_indices, np.arange(size))
+
+    new_indices = graph.add_nodes(indices=[10, 11])
+    nodes = graph.get_nodes()
+
+    np.testing.assert_equal(new_indices, [10, 11])
+    np.testing.assert_array_equal(nodes[:size], np.arange(size))
+    np.testing.assert_array_equal(nodes[size:], [10, 11])
+
+    with pytest.raises(ValueError):
+        graph.add_nodes(coords=[[0, 1], [2, 3]])
+
+    graph.add_nodes(indices=15)
+    assert len(graph) == 8
+
+    with pytest.raises(ValueError):
+        graph.add_nodes(indices=15)
+
+
+def test_node_addition_spatial() -> None:
+    graph = DirectedGraph(ndim=2)
+
+    with pytest.raises(ValueError):
+        graph.add_nodes(indices=5, coords=[0, 0], count=1)
+
+    new_index = graph.add_nodes(coords=[2, 2])
+    assert len(graph) == 1
+    assert new_index == 0
+    np.testing.assert_equal(graph.get_coordinates(), [[2, 2]])
+
+    new_index = graph.add_nodes(indices=[10, 11], coords=[[0, 0], [1, 1]])
+    assert len(graph) == 3
+    np.testing.assert_equal(new_index, [10, 11])
+
+    with pytest.raises(ValueError):
+        graph.add_nodes(indices=13)
+
+    with pytest.raises(ValueError):
+        graph.add_nodes(count=2)
+
+    with pytest.raises(ValueError):
+        graph.add_nodes(indices=[2, 3], coords=[[1, 2]])
+
+    assert len(graph) == 3
+
+
 @pytest.mark.parametrize(
     "graph_type,ndim",
     product([UndirectedGraph, DirectedGraph], [None, 2, 3]),
 )
 def test_empty_graph(graph_type: Type[BaseGraph], ndim: Optional[int]) -> None:
     _ = graph_type(ndim=ndim)
 
 
 class TestGraph:
-    _GRAPH_CLASS: Type[BaseGraph] = ...
+    _GRAPH_CLASS: Type[BaseGraph]
     __test__ = False  # ignored for testing
     _index_shift = 0  # shift used to test special indexing
 
     def setup_method(self, method: Callable) -> None:
         self.coords = pd.DataFrame(
             [
                 [0, 2.5],
@@ -134,15 +187,17 @@
     @staticmethod
     def contains(edge: ArrayLike, edges: List[ArrayLike]) -> bool:
         return any(
             np.allclose(e, edge) if len(e) > 0 else False for e in edges
         )
 
     def teardown_method(self, method: Callable) -> None:
-        self.edges, self.coords, self.graph = None, None, None
+        del self.edges, self.graph
+        if hasattr(self, "coords"):
+            del self.coords
 
     def test_edge_buffers(self) -> None:
         # testing buffer correctness on a non-trivial case when a node was removed
         node_id = 3 + self._index_shift
         self.graph.remove_node(node_id)
 
         valid_edges = np.logical_not(np.any(self.edges == node_id, axis=1))
@@ -154,16 +209,33 @@
         )
 
         indices, edges = self.graph.get_edges_buffers()
 
         assert np.allclose(expected_indices, indices)
         assert np.allclose(expected_edges, edges)
 
+    def test_subgraph_edges(self) -> None:
+        # 3 is disconnected in subgraph
+        nodes_ids = np.asarray([0, 1, 3]) + self._index_shift
+
+        subgraph = self.graph.subgraph_edges(nodes_ids)
+        expected_subgraph = np.asarray([[0, 1]]) + self._index_shift
+
+        np.testing.assert_array_equal(subgraph, expected_subgraph)
+
+        buffer_node_ids = np.asarray([0, 1, 3])
+        buffer_subgraph = self.graph.subgraph_edges(
+            buffer_node_ids, is_buffer_domain=True
+        )
+
+        np.testing.assert_equal(buffer_subgraph, [[0, 1]])
+
 
 class TestDirectedGraph(TestGraph):
+    graph: DirectedGraph  # required by typing
     _GRAPH_CLASS = DirectedGraph
     __test__ = True
 
     def test_edge_removal(self) -> None:
         edge = np.asarray([0, 1]) + self._index_shift
         self.graph.remove_edges(edge)
         assert self.graph.n_edges == 4
@@ -271,15 +343,21 @@
             assert empty_idx + 1 == next_empty_idx
             # skipping one
             empty_idx = self.graph._edges_buffer[
                 next_empty_idx * _UN_EDGE_SIZE + _LL_UN_EDGE_POS
             ]
 
 
-class NonSpatialMixin:
+class NonSpatialMixin(Protocol):
+    # required by typing
+    _GRAPH_CLASS: Any
+    graph: BaseGraph
+    edges: np.ndarray
+    _index_shift: int
+
     def setup_method(self, method: Callable) -> None:
         self.edges = (
             np.asarray([[0, 1], [1, 2], [2, 3], [3, 4], [4, 0]], dtype=int)
             + self._index_shift
         )
 
         self.graph = self._GRAPH_CLASS(edges=self.edges)
```

### Comparing `napari-graph-0.1.0/src/napari_graph/base_graph.py` & `napari-graph-0.1.1/src/napari_graph/base_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from typing import Callable, List, Optional, Tuple, Union
 
+import networkx as nx
 import numpy as np
 import pandas as pd
 from numba import njit, typed
 from numba.core import types
 from numpy.typing import ArrayLike
 
 """
@@ -134,14 +137,26 @@
             edges.append(edges_buffer[buffer_idx + 1])  # tgt
             idx = edges_buffer[buffer_idx + ll_edge_pos]
 
     return edges_list
 
 
 @njit
+def _contains_keys(
+    map: typed.Dict,
+    keys: np.ndarray,
+) -> bool:
+    """Returns true if at least one `key` is present on `map`."""
+    for k in keys:
+        if k in map:
+            return True
+    return False
+
+
+@njit
 def _update_world2buffer(
     world2buffer: typed.Dict,
     world_idx: np.ndarray,
     buffer_idx: np.ndarray,
 ) -> None:
     """Updates `world_idx` (keys) and `buffer_idx` (values) to `world2buffer` mapping."""
     for w, b in zip(world_idx, buffer_idx):
@@ -173,17 +188,17 @@
     n_nodes : int
         Optional number of nodes to pre-allocate in the graph.
     n_edges : int
         Optional number of edges to pre-allocate in the graph.
     """
 
     # abstract constants
-    _EDGE_DUPLICATION: int = ...
-    _EDGE_SIZE: int = ...
-    _LL_EDGE_POS: int = ...
+    _EDGE_DUPLICATION: int
+    _EDGE_SIZE: int
+    _LL_EDGE_POS: int
 
     # allocation constants
     _ALLOC_MULTIPLIER = 1.1
     _ALLOC_MIN = 25
 
     def __init__(
         self,
@@ -229,15 +244,15 @@
         if ndim is not None:
             self._coords = np.empty((n_nodes, ndim), dtype=np.float32)
         else:
             self._coords = None
 
         if coords is not None:
             assert self._coords is not None
-            self.add_nodes(coords.index, coords)
+            self.add_nodes(indices=coords.index, coords=coords)
 
         # validate edges
         edges = np.asarray(edges)
         if len(edges) > 0:
             if edges.ndim != 2:
                 raise ValueError(
                     f"`edges` ({edges.ndim} dimensions) must have 2 dimensions."
@@ -256,15 +271,15 @@
         else:
             n_edges = len(edges)
 
         # initialize edges
         self._init_edge_buffers(n_edges)
         if len(edges) > 0:
             if coords is None:
-                self.add_nodes(np.unique(edges))
+                self.add_nodes(indices=np.unique(edges))
             self.add_edges(edges)
 
     def _init_node_buffers(self, n_nodes: int) -> None:
         self._empty_nodes: List[int] = list(reversed(range(n_nodes)))
         self._node2edges = np.full(
             n_nodes, fill_value=_EDGE_EMPTY_PTR, dtype=int
         )
@@ -311,14 +326,19 @@
     def get_coordinates(
         self, node_indices: Optional[ArrayLike] = None
     ) -> np.ndarray:
         """Coordinates of the given nodes.
 
         If none is provided it returns the coordinates of every node.
         """
+        if self._coords is None:
+            raise ValueError(
+                "`get_coordinates` is only available for spatial graphs."
+            )
+
         node_indices = self._validate_nodes(node_indices)
         node_indices = self._map_world2buffer(node_indices)
         return self._coords[node_indices]
 
     def _realloc_nodes_buffers(self, size: int) -> None:
         """Rellocs the nodes buffers and copies existing data.
 
@@ -351,60 +371,109 @@
         )
         self._buffer2world = np.append(
             self._buffer2world,
             np.full(size_diff, fill_value=_NODE_EMPTY_PTR, dtype=int),
         )
         self._empty_nodes = list(reversed(range(prev_size, size)))
 
+    def get_next_valid_indices(self, count: int) -> ArrayLike:
+        if count <= 0:
+            raise ValueError(
+                f"`count` must be a positive integer. Found {count}"
+            )
+
+        next_indices = self._buffer2world.max() + 1
+        return np.arange(next_indices, next_indices + count)
+
     def add_nodes(
         self,
-        indices: ArrayLike,
+        *,
+        indices: Optional[ArrayLike] = None,
         coords: Optional[ArrayLike] = None,
-    ) -> None:
-        """Adds node to graph.
+        count: Optional[int] = None,
+    ) -> ArrayLike:
+        """
+        Add nodes to graph, at least one of the arguments must be supplied.
+        `count` cannot be supplied with other arguments.
 
         Parameters
         ----------
         index : int
             Node index.
         coords : np.ndarray
             Node coordinates, optional for non-spatial graph.
+        count : int:
+            Number of nodes to be added.
+
+        Returns
+        -------
+        ArrayLike
+            Added nodes indices.
         """
+        if count is not None and (indices is not None or coords is not None):
+            raise ValueError(
+                "`count` cannot be supplied with `indices` and `coords`."
+            )
+
+        if count is None and indices is None and coords is None:
+            raise ValueError(
+                "One of `indices`, `coords` or `count` must be supplied."
+            )
+
+        if coords is not None:
+            coords = np.atleast_2d(coords)
+
+        if indices is None:
+            if count is None:
+                count = coords.shape[0]
+            indices = self.get_next_valid_indices(count)
+
         indices = np.atleast_1d(indices)
         if indices.ndim > 1:
             raise ValueError(
                 f"`indices` must be 1-dimensional. Found {indices.ndim}."
             )
 
         if (self._coords is None) != (coords is None):
             if coords is None:
                 raise ValueError(
                     "`coords` must be provided for spatial graphs."
                 )
             else:
                 raise ValueError(
-                    "`coords` cannot be provided for non spatial graphs."
+                    "`coords` cannot be provided for non-spatial graphs."
                 )
 
+        if _contains_keys(self._world2buffer, indices):
+            raise ValueError(
+                f"One of the nodes {indices} are already present in the buffer."
+            )
+
         if self.n_empty_nodes < len(indices):
             self._realloc_nodes_buffers(
                 self._get_alloc_size(self.n_nodes + len(indices))
             )
 
         # flipping since _empty_nodes is a stack
         buffer_indices = np.flip(self._empty_nodes[-len(indices) :])
 
-        if self._coords is not None:
-            coords = np.atleast_2d(coords)
+        if coords is not None:
+            if indices.shape[0] != coords.shape[0]:
+                raise ValueError(
+                    f"`indices` and `coords` must be equal. Found {len(indices)} and {len(coords)}."
+                )
+
             self._coords[buffer_indices] = coords
 
-        self._empty_nodes = self._empty_nodes[: -len(indices)]
         _update_world2buffer(self._world2buffer, indices, buffer_indices)
+        self._empty_nodes = self._empty_nodes[: -len(indices)]
         self._buffer2world[buffer_indices] = indices
 
+        return indices
+
     def _get_alloc_size(self, size: int) -> int:
         return int(max(size * self._ALLOC_MULTIPLIER, self._ALLOC_MIN))
 
     def remove_node(self, index: int, is_buffer_domain: bool = False) -> None:
         """Remove node of given `index`, by default it's the world index.
 
         Parameters
@@ -739,7 +808,127 @@
             edges = self._buffer2world[edges]
 
         return indices, edges
 
     def __len__(self) -> int:
         """Number of nodes in use."""
         return self.n_nodes
+
+    def initialized_buffer_mask(self) -> np.ndarray:
+        """Compute mask of nodes that have already been initialized.
+
+        Returns
+        -------
+        np.ndarray
+            Boolean array of valid node, it has the same length the buffer.
+        """
+        return self._buffer2world != _NODE_EMPTY_PTR
+
+    @property
+    def coords_buffer(self) -> np.ndarray:
+        """Returns the actual coordinates buffer. It's not a copy."""
+        if self._coords is None:
+            raise ValueError(
+                "graph does not have a `coords` attribute. "
+                "It is not a spatial graph."
+            )
+        return self._coords
+
+    def is_spatial(self) -> bool:
+        """True if self is a spatial graph (has coordinates attribute)."""
+        return self._coords is not None
+
+    @staticmethod
+    def from_networkx(graph: nx.Graph) -> BaseGraph:
+        """Loads a Directed or Undirected napari-graph from a NetworkX graph.
+
+        Parameters
+        ----------
+        graph : nx.Graph
+            The NetworkX graph to be converted.
+        """
+        from napari_graph.directed_graph import DirectedGraph
+        from napari_graph.undirected_graph import UndirectedGraph
+
+        coords_dict = nx.get_node_attributes(graph, "pos")
+        if len(coords_dict) > 0:
+            coords_df = pd.DataFrame.from_dict(coords_dict, orient="index")
+        else:
+            coords_df = None
+
+        edges = graph.edges
+        if len(edges) > 0:
+            edges = np.atleast_2d(edges)
+
+        return (
+            DirectedGraph(edges, coords_df)
+            if graph.is_directed()
+            else UndirectedGraph(edges, coords_df)
+        )
+
+    def to_networkx(self) -> nx.Graph:
+        """Convert it self into NetworkX graph.
+
+        Parameters
+        ----------
+        graph : BaseGraph
+            napari-graph Graph
+
+        Returns
+        -------
+        nx.Graph
+            An equivalent NetworkX graph.
+        """
+        from napari_graph.directed_graph import DirectedGraph
+
+        if isinstance(self, DirectedGraph):
+            out_graph = nx.DiGraph()
+        else:
+            out_graph = nx.Graph()
+
+        if self.is_spatial():
+            for node_id, pos in zip(self.get_nodes(), self.get_coordinates()):
+                out_graph.add_node(node_id, pos=pos)
+        else:
+            out_graph.add_nodes_from(self.get_nodes())
+
+        edges = self.get_edges()
+        if isinstance(edges, list) and len(edges) > 0:
+            edges = np.concatenate(edges, axis=0)
+
+        edges_as_tuples = list(map(tuple, edges))
+        out_graph.add_edges_from(edges_as_tuples)
+
+        return out_graph
+
+    def subgraph_edges(
+        self,
+        node_indices: ArrayLike,
+        is_buffer_domain: bool = False,
+    ) -> ArrayLike:
+        """Returns edges (node pair) where both nodes are presents.
+
+        Parameters
+        ----------
+        nodes_indices : np.ndarray
+            Subset of nodes used for selection.
+        is_buffer_domain : bool
+            When true `node_indices` and returned edges are on buffer domain.
+
+        Returns
+        -------
+        np.ndarray
+            (N x 2) array of nodes indices, where N is the number of valid edges from the induced subgraph.
+        """
+        _, edges = self.get_edges_buffers(is_buffer_domain)
+
+        if is_buffer_domain:
+            mask = np.zeros(self._buffer2world.shape[0], dtype=bool)
+            mask[node_indices] = True
+            subgraph_edges = edges[mask[edges[:, 0]] & mask[edges[:, 1]]]
+
+        else:
+            mask = np.isin(edges, node_indices).all(axis=1)
+            assert mask.shape[0] == edges.shape[0]
+            subgraph_edges = edges[mask]
+
+        return subgraph_edges
```

### Comparing `napari-graph-0.1.0/src/napari_graph/directed_graph.py` & `napari-graph-0.1.1/src/napari_graph/directed_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
-import pandas as pd
 from numba import njit, typed
 from numpy.typing import ArrayLike
 
 from napari_graph.base_graph import (
     _EDGE_EMPTY_PTR,
     _NODE_EMPTY_PTR,
     BaseGraph,
@@ -353,36 +352,14 @@
 
     def _init_node_buffers(self, n_nodes: int) -> None:
         super()._init_node_buffers(n_nodes)
         self._node2tgt_edges = np.full(
             n_nodes, fill_value=_EDGE_EMPTY_PTR, dtype=int
         )
 
-    def init_nodes(
-        self,
-        coords: Union[pd.DataFrame, ArrayLike],
-    ) -> None:
-        """Initialize graph nodes from coordinates data.
-
-        Graph nodes will be indexed by data frame (or array) indices.
-
-        Parameters
-        ----------
-        coords : Union[pd.DataFrame, ArrayLike],
-            2-dim array containing nodes coordinates.
-        """
-        super().init_nodes(coords)
-        n_nodes = len(coords)
-        if len(self._node2tgt_edges) < n_nodes:
-            self._node2tgt_edges = np.full(
-                n_nodes, fill_value=_EDGE_EMPTY_PTR, dtype=np.int64
-            )
-        else:
-            self._node2tgt_edges.fill(_EDGE_EMPTY_PTR)
-
     def _realloc_nodes_buffers(self, size: int) -> None:
         diff_size = size - self.n_allocated_nodes
         super()._realloc_nodes_buffers(size)
         self._node2tgt_edges = np.append(
             self._node2tgt_edges,
             np.full(diff_size, fill_value=_NODE_EMPTY_PTR, dtype=np.int64),
         )
```

### Comparing `napari-graph-0.1.0/src/napari_graph/undirected_graph.py` & `napari-graph-0.1.1/src/napari_graph/undirected_graph.py`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.0/src/napari_graph.egg-info/PKG-INFO` & `napari-graph-0.1.1/src/napari_graph.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-graph
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fast editable graphs in Python and numba
 Home-page: https://github.com/napari/napari-graph
 Author: Jordão Bragantini, Jonas Windhager & Juan Nunez-Iglesias
 Author-email: jordao.bragantini@czbiohub.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-graph-0.1.0/src/napari_graph.egg-info/SOURCES.txt` & `napari-graph-0.1.1/src/napari_graph.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 docs/index.md
 docs/make.bat
 docs/api/api.md
 src/napari_graph/__init__.py
 src/napari_graph/_version.py
 src/napari_graph/base_graph.py
 src/napari_graph/directed_graph.py
+src/napari_graph/interops.py
 src/napari_graph/undirected_graph.py
 src/napari_graph.egg-info/PKG-INFO
 src/napari_graph.egg-info/SOURCES.txt
 src/napari_graph.egg-info/dependency_links.txt
 src/napari_graph.egg-info/requires.txt
 src/napari_graph.egg-info/top_level.txt
-src/napari_graph/_tests/test_graph.py
+src/napari_graph/_tests/test_graph.py
+src/napari_graph/_tests/test_interops.py
```

### Comparing `napari-graph-0.1.0/tox.ini` & `napari-graph-0.1.1/tox.ini`

 * *Files identical despite different names*

