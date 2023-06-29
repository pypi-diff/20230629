# Comparing `tmp/enstat-0.9.2.tar.gz` & `tmp/enstat-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.9.2.tar", last modified: Tue May  2 10:19:22 2023, max compression
+gzip compressed data, was "enstat-0.9.3.tar", last modified: Thu Jun 29 13:13:44 2023, max compression
```

## Comparing `enstat-0.9.2.tar` & `enstat-0.9.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.796221 enstat-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 10:19:14.000000 enstat-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-02 10:19:14.000000 enstat-0.9.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 10:19:14.000000 enstat-0.9.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-02 10:19:14.000000 enstat-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-02 10:19:14.000000 enstat-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 10:19:14.000000 enstat-0.9.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 10:19:14.000000 enstat-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-02 10:19:22.800221 enstat-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-02 10:19:14.000000 enstat-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    27159 2023-05-02 10:19:14.000000 enstat-0.9.2/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 10:19:14.000000 enstat-0.9.2/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-02 10:19:14.000000 enstat-0.9.2/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 10:19:14.000000 enstat-0.9.2/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 10:19:14.000000 enstat-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:19:22.800221 enstat-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.750699 enstat-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.738699 enstat-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.742699 enstat-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 13:13:35.000000 enstat-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 13:13:35.000000 enstat-0.9.3/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 13:13:35.000000 enstat-0.9.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-29 13:13:35.000000 enstat-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-29 13:13:35.000000 enstat-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 13:13:35.000000 enstat-0.9.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 13:13:35.000000 enstat-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 13:13:44.750699 enstat-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-29 13:13:35.000000 enstat-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.746699 enstat-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.746699 enstat-0.9.3/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    30597 2023-06-29 13:13:35.000000 enstat-0.9.3/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-29 13:13:35.000000 enstat-0.9.3/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-29 13:13:35.000000 enstat-0.9.3/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.750699 enstat-0.9.3/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 13:13:35.000000 enstat-0.9.3/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 13:13:35.000000 enstat-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:13:44.750699 enstat-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.750699 enstat-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/test_main.py
```

### Comparing `enstat-0.9.2/.github/workflows/ci.yml` & `enstat-0.9.3/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 name: CI
 
 on:
   workflow_dispatch:
   pull_request:
   push:
-    branches:
-    - main
+    branches: [main]
 
 jobs:
 
   default-shell:
 
     strategy:
       fail-fast: false
@@ -29,21 +28,25 @@
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Checkout latest release tag
       run: |
         LATEST_TAG=$(git describe --tags `git rev-list --tags --max-count=1`)
-        git checkout $LATEST_TAG
         echo "SETUPTOOLS_SCM_PRETEND_VERSION=$LATEST_TAG" >> $GITHUB_ENV
 
     - name: Set conda environment
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-file: environment.yaml
         environment-name: myenv
+        cache-env: true
 
     - name: Install library
-      run: python -m pip install .
+      run: python -m pip install . -v
 
     - name: Run tests
       run: python -m unittest discover tests -v
+
+    - name: Build docs
+      working-directory: docs
+      run: make html
```

### Comparing `enstat-0.9.2/.github/workflows/python-publish.yml` & `enstat-0.9.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/.gitignore` & `enstat-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/.pre-commit-config.yaml` & `enstat-0.9.3/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-yaml
   - id: check-toml
   - id: debug-statements
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.8.0
+  rev: v2.9.0
   hooks:
   - id: pretty-format-yaml
     args: [--preserve-quotes, --autofix, --indent, '2']
   - id: pretty-format-toml
     args: [--autofix]
 - repo: https://github.com/psf/black
   rev: 23.3.0
@@ -21,29 +21,29 @@
     args: [--safe, --quiet, --line-length=100]
 - repo: https://github.com/humitos/mirrors-autoflake.git
   rev: v1.1
   hooks:
   - id: autoflake
     args: [--in-place, --remove-unused-variable, --remove-all-unused-imports]
 - repo: https://github.com/asottile/reorder_python_imports
-  rev: v3.9.0
+  rev: v3.10.0
   hooks:
   - id: reorder-python-imports
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.2
+  rev: v3.7.0
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
-    args: [--max-line-length=100, "--ignore=F811", "--per-file-ignores=*/mean.py:W503"]
+    args: [--max-line-length=100, "--ignore=F811,W503"]
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v2.2.0
+  rev: v2.3.0
   hooks:
   - id: setup-cfg-fmt
 - repo: https://github.com/tdegeus/conda_envfile
   rev: v0.4.2
   hooks:
   - id: conda_envfile_parse
     files: environment.yaml
```

### Comparing `enstat-0.9.2/LICENSE` & `enstat-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/PKG-INFO` & `enstat-0.9.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,86 @@
-Metadata-Version: 2.1
-Name: enstat
-Version: 0.9.2
-Summary: Ensemble averages
-Author-email: Tom de Geus <tom@geus.me>
-Project-URL: Source, https://github.com/tdegeus/enstat
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # enstat
 
 [![CI](https://github.com/tdegeus/enstat/workflows/CI/badge.svg)](https://github.com/tdegeus/enstat/actions)
 [![Documentation Status](https://readthedocs.org/projects/enstat/badge/?version=latest)](https://enstat.readthedocs.io)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/enstat.svg)](https://anaconda.org/conda-forge/enstat)
 [![PyPi release](https://img.shields.io/pypi/v/enstat.svg)](https://pypi.org/project/enstat/)
 
 Documentation: [enstat.readthedocs.io](https://enstat.readthedocs.io)
 
-## Overview
+## Hallmark feature
+
+*enstat* is a library to facilitate the computation of
+
+*   [Ensemble averages (and their variance)](#readme-average);
+*   [Ensemble averages (and their variance) based on a certain binning of a quantity](#readme-binned);
+*   [Histograms of an ensemble](#readme-histogram).
 
-*enstat* is a library to facilitate the computation of ensemble averages (and their variances) or histograms.
+**without storing the entire ensemble in memory**.
 
-The key feature is that a class stores the sum of the first and second statistical moments and the number of samples.
-This gives access to the mean (and variance) at all times, while you can keep adding samples.
+> Below you find a quick-start.
+> For more information, see the [documentation](https://enstat.readthedocs.io).
 
-For the histogram something similar holds, but this time the count per bin is stored.
+<div id="readme-average"></div>
 
-### Ensemble average
+## Ensemble average
+
+> The key feature is to store the sum of the first and second statistical moments and the number of samples.
+> This gives access to the mean (and variance) at all times, while you can keep adding samples.
 
 Suppose that we have 100 realisations, each with 1000 'blocks', and we want to know the ensemble average of each block:
 
 ```python
 import enstat
 import numpy as np
 
 ensemble = enstat.static()
 
 for realisation in range(100):
-
     sample = np.random.random(1000)
     ensemble += sample
 
 print(ensemble.mean())
 ```
 
 which will print a list of 1000 values, each around `0.5`.
+
 This is the equivalent of
 
 ```python
 import numpy as np
 
 container = np.empty((100, 1000))
 
-for realisation in range(100):
 
     sample = np.random.random(1000)
     container[realisation, :] = sample
 
 print(np.mean(container, axis=0))
 ```
 
 The key difference is that *enstat* only requires you to have `4 * N` values in memory for a sample of size `N`: the sample itself, the sums of the first and second moment, and the normalisation.
 Instead the solution with the container uses much more memory.
 
 A nice feature is also that you can keep adding samples to `ensemble`.
 You can even store it and continue later.
 
-### Ensemble histogram
+<div id="readme-histogram"></div>
+
+## Ensemble histogram
 
 Same example, but now we want the histogram for predefined bins:
 ```python
 import enstat
 import numpy as np
 
 bin_edges = np.linspace(0, 1, 11)
 hist = enstat.histogram(bin_edges=bin_edges)
 
 for realisation in range(100):
-
     sample = np.random.random(1000)
     hist += sample
 
 print(hist.p)
 ```
 
 which prints the probability density of each bin (so list of values around `0.1` for these bins).
@@ -104,14 +102,34 @@
     fig, ax = plt.subplots()
     ax.plot(hist.x, hist.p)
     plt.show()
     ```
 
     You can even use `ax.plot(*hist.plot)`.
 
+<div id="readme-binned"></div>
+
+## Average per bin
+
+Suppose you have some time series (`t`) with multiple observables (`a` and `b`); e.g.;
+```python
+import enstat
+import numpy as np
+
+t = np.linspace(0, 10, 100)
+a = np.random.normal(loc=5, scale=0.1, size=t.size)
+b = np.random.normal(loc=1, scale=0.5, size=t.size)
+```
+Now suppose that you want to compute the average `a`, `b`, and `t` based on a certain binning of `t`:
+```python
+bin_edges = np.linspace(0, 12, 12)
+binned = enstat.binned.from_data(t, a, b, names=["t", "a", "b"]m bin_edges=bin_edges)
+print(binned["a"].mean())
+```
+
 ## Installation
 
 -   Using conda
 
     ```bash
     conda install -c conda-forge enstat
     ```
```

### Comparing `enstat-0.9.2/docs/Makefile` & `enstat-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/docs/make.bat` & `enstat-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/docs/module.rst` & `enstat-0.9.3/docs/module.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 .. autosummary::
 
     enstat.scalar
     enstat.static
     enstat.dynamic1d
     enstat.histogram
+    enstat.binned
 
 scalar
 ------
 
 .. autoclass:: enstat.scalar
    :members:
    :undoc-members:
@@ -44,7 +45,16 @@
 ---------
 
 .. autoclass:: enstat.histogram
    :members:
    :undoc-members:
    :show-inheritance:
    :inherited-members:
+
+binned
+------
+
+.. autoclass:: enstat.binned
+   :members:
+   :undoc-members:
+   :show-inheritance:
+   :inherited-members:
```

### Comparing `enstat-0.9.2/enstat/__init__.py` & `enstat-0.9.3/enstat/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,36 @@
 from ._version import version  # noqa: F401
 from ._version import version_tuple  # noqa: F401
 
 
 class scalar:
     r"""
     Ensemble average of a scalar.
-    Add samples to it using :py:func:`scalar.add_sample`.
+    Example:
+
+    .. code-block:: python
+
+        import enstat
+
+        average = enstat.scalar()
+        average += 1.0
+        average += 2.0
+        average += 3.0
+        print(average.mean())  # 2.0
+
+    Add samples to it using :py:func:`scalar.add_sample`, or simply `average += datum`.
     The mean, variance, and standard deviation can be obtained at any time.
     They are derived from the following members:
 
     *   :py:attr:`scalar.first`: Sum of the first statistical moment.
     *   :py:attr:`scalar.second`: Sum of the second statistical moment.
     *   :py:attr:`scalar.norm`: Number of samples.
+
+    To restore data: use :py:func:`scalar.restore`.
+    In short: `restored = enstat.scalar.restore(**dict(average))`.
     """
 
     def __init__(self):
         self.first = 0.0
         self.second = 0.0
         self.norm = 0.0
 
@@ -116,23 +131,38 @@
 
         return np.sqrt(self.variance())
 
 
 class static:
     r"""
     Ensemble average of an nd-array (of same size for all samples).
-    Add samples to it using :py:func:`static.add_sample`.
+    .. code-block:: python
+
+        import enstat
+        import numpy as np
+
+        data = np.random.random(35 * 50).reshape(35, 50)
+
+        average = enstat.static()
+        for datum in data:
+            average += datum
+        print(average.mean())  # approximately [0.5, 0.5, ...]
+
+    Add samples to it using :py:func:`static.add_sample`, or simply `average += datum`.
     The mean, variance, and standard deviation can be obtained at any time.
     They are derived from the following members:
 
     *   :py:attr:`static.first`: Sum of the first statistical moment.
     *   :py:attr:`static.second`: Sum of the second statistical moment.
     *   :py:attr:`static.norm`: Number of samples.
 
-    Furthermore, the following members are available:
+    To restore data: use :py:func:`static.restore`.
+    In short: `restored = enstat.static.restore(**dict(average))`.
+
+    For convenience, the following members are available:
 
     *   :py:attr:`static.shape`: Shape of the data.
     *   :py:attr:`static.size`: Size of the data (= prod(shape)).
 
     :param compute_variance:
         If set ``False`` no second moment will be computed (making things slightly faster).
         In that case, the variance an standard deviation will not be available.
@@ -354,30 +384,63 @@
         """
 
         if self.norm is None:
             return None
 
         return np.sqrt(self.variance(min_norm))
 
+    def squash(self, n: int | list[int]):
+        """
+        Squash the data to a smaller size by summing over blocks of size ``n``.
+        For example, suppose that::
+
+            >>> avg.norm
+            [[2, 2, 3, 1, 1],
+             [2, 2, 1, 1, 3],
+             [1, 1, 2, 2, 1],
+             [2, 1, 2, 2, 2]]
+
+        Then calling::
+
+            >>> avg.squash(2)
+            >>> avg.norm
+            [[8, 6, 4],
+             [5, 8, 3]]
+        """
+        assert self.norm is not None, "no data yet"
+
+        if not hasattr(n, "__len__"):
+            n = [n]
+
+        assert self.norm.ndim == len(n)
+
+        for i in range(len(n)):
+            iter = np.arange(0, self.norm.shape[i], n[i])
+            self.norm = np.add.reduceat(self.norm, iter, axis=i)
+            self.first = np.add.reduceat(self.first, iter, axis=i)
+            if self.compute_variance:
+                self.second = np.add.reduceat(self.second, iter, axis=i)
+
 
 def _expand_array1d(data, size):
     tmp = np.zeros((size), data.dtype)
     tmp[: data.size] = data
     return tmp
 
 
 class dynamic1d(static):
     r"""
     Ensemble average of an 1d-array (which grows depending of the size of the samples).
-    Add samples to it using :py:func:`dynamic1d.add_sample`.
+    Add samples to it using :py:func:`dynamic1d.add_sample`, or simply `average += datum`.
     The mean, variance, and standard deviation can be obtained at any time.
     Also the sums of the first and statistical moments, as well as the number of samples can be
     obtained at any time.
 
-    Continue an old average by specifying:
+    To restore data: use :py:func:`dynamic1d.restore`.
+    In short: `restored = enstat.dynamic1d.restore(**dict(average))`.
 
     :param compute_variance:
         If set ``False`` no second moment will be computed.
         In that case, the variance an standard deviation will not be available.
 
     :param size:
         The initial size of the data.
@@ -436,15 +499,48 @@
 
         return super().add_point(datum, index)
 
 
 class histogram:
     """
     Histogram.
-    One can add samples to it using :py:func:`Histogram.add_sample`.
+    Example single dataset:
+
+    .. code-block:: python
+
+        data = [0, 0, 0, 1, 1, 2]
+        bin_edges = [-0.5, 0.5, 1.5, 2.5]
+        hist = enstat.histogram.from_data(data, bin_edges)
+        print(hist.count)
+
+    Example ensemble:
+
+    .. code-block:: python
+
+        data = np.random.random(35 * 50).reshape(35, 50)
+        bin_edges = np.linspace(0, 1, 11)
+        hist = enstat.histogram(bin_edges)
+
+        for datum in data:
+            hist += datum
+
+        print(hist.count)
+
+    One can add samples to it using :py:func:`Histogram.add_sample`, or simply `hist += datum`.
+
+    Members:
+
+    *   :py:attr:`scalar.count`: The number of samples in each bin.
+    *   :py:attr:`scalar.bin_edges`: See option ``bin_edges``.
+    *   :py:attr:`scalar.x`: Midpoint of each bin.
+    *   :py:attr:`scalar.p`: Probability density of each bin.
+    *   :py:attr:`scalar.right`: See option ``right``.
+    *   :py:attr:`scalar.bound_error`: See option ``bound_error``
+    *   :py:attr:`scalar.count_left`: Number of samples that fall below the leftmost bin.
+    *   :py:attr:`scalar.count_right`: Number of samples that fall above the rightmost bin.
 
     :param bin_edges: The bin-edges.
     :param right: Whether the bin includes the right edge (or the left edge) see numpy.digitize.
     :param bound_error: What to do if a sample falls out of the bin range:
 
         - ``"raise"``: raise an error
         - ``"ignore"``: ignore the data that are out of range
@@ -589,16 +685,17 @@
 
         if min_width is not None:
             bin_edges = detail.histogram_bin_edges_minwidth(bin_edges, min_width)
 
         if integer:
             bin_edges = detail.histogram_bin_edges_integer(bin_edges)
 
-        bin_edges[0] = np.nextafter(bin_edges[0], data.min() - (data.max() - data.min()))
-        bin_edges[-1] = np.nextafter(bin_edges[-1], data.max() + (data.max() - data.min()))
+        d = bin_edges[-1] - bin_edges[0]
+        bin_edges[0] = np.nextafter(bin_edges[0], bin_edges[0] - d)
+        bin_edges[-1] = np.nextafter(bin_edges[-1], bin_edges[-1] + d)
         return cls(bin_edges, right=True, bound_error=bound_error).add_sample(data)
 
     def strip(self, min_count: int = 0):
         """
         Strip the histogram of empty bins to the left and the right.
 
         :param min_count: The minimum count for a bin to be considered non-empty.
@@ -767,51 +864,59 @@
         return self
 
     @property
     def x(self) -> ArrayLike:
         """
         The bin centers.
         """
-
         return 0.5 * (self.bin_edges[:-1] + self.bin_edges[1:])
 
     @property
     def density(self) -> ArrayLike:
         """
         The probability density function at the bin.
         """
-
         count = self.count.astype(np.float64)
         norm = np.sum(count)
 
         if self.bound_error == "norm":
             norm += self.count_left + self.count_right
 
         return count / (np.diff(self.bin_edges) * norm)
 
     @property
     def p(self) -> ArrayLike:
         """
         The probability density function at the bin.
         """
-
         return self.density
 
     @property
     def plot(self) -> tuple[ArrayLike, ArrayLike]:
         """
         Alias for ``(x, density)``.
         """
-
         return (self.x, self.density)
 
 
 class binned:
     """
     Ensemble average after binning.
+    Example:
+
+    .. code-block:: python
+
+        import numpy as np
+        import enstat
+
+        x = np.array([0.5, 1.5, 2.5])
+        y = np.array([1, 2, 3])
+        bin_edges = np.array([0, 1, 2, 3])
+        binned = enstat.binned.from_data(x, y, bin_edges=bin_edges)
+        print(binned[0].mean())
 
     :param bin_edges: The bin-edges.
     :param right: Whether the bin includes the right edge (or the left edge) see numpy.digitize.
     :param bound_error: What to do if a sample falls out of the bin range:
 
         - ``"raise"``: raise an error
         - ``"ignore"``: ignore the data that are out of range
@@ -881,29 +986,33 @@
             if name in kwargs:
                 raise ValueError(f"Duplicate argument: {name}")
             kwargs[name] = args[i]
 
         if len(kwargs) != len(self.names):
             raise ValueError("Incorrect number of arguments")
 
-        bin, keep = self.hist._get_bins(kwargs[self.names[0]], return_selector=True)
+        ibin, keep = self.hist._get_bins(kwargs[self.names[0]], return_selector=True)
         kwargs = {name: np.asarray(arg)[keep] for name, arg in kwargs.items()}
         sqr = {name: arg * arg for name, arg in kwargs.items()}
 
         for name, arg in kwargs.items():
             if arg.shape != kwargs[self.names[0]].shape:
                 raise ValueError("All arguments must have the same shape")
 
-        for ibin in range(np.max(bin) + 1):
-            sel = bin == ibin
-            if not np.any(sel):
-                continue
-            for name, arg in kwargs.items():
-                self.data[name].first[ibin] += np.sum(kwargs[name][sel])
-                self.data[name].second[ibin] += np.sum(sqr[name][sel])
-                self.data[name].norm[ibin] += np.sum(sel)
+        # see https://stackoverflow.com/q/76574134/2646505
+        sorter = np.argsort(ibin)
+        ibin = ibin[sorter]
+        norm = np.argwhere(np.diff(ibin, prepend=ibin[0], append=1)).flatten()
+        split = norm - 1
+        norm = np.diff(norm, prepend=0)
+        store = ibin[split]
+
+        for name, arg in kwargs.items():
+            self.data[name].first[store] += np.diff(np.cumsum(arg[sorter])[split], prepend=0)
+            self.data[name].second[store] += np.diff(np.cumsum(sqr[name][sorter])[split], prepend=0)
+            self.data[name].norm[store] += norm
 
         return self
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `enstat-0.9.2/enstat/detail.py` & `enstat-0.9.3/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/enstat/mean.py` & `enstat-0.9.3/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/enstat.egg-info/PKG-INFO` & `enstat-0.9.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.2
+Version: 0.9.3
 Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,75 +14,84 @@
 [![CI](https://github.com/tdegeus/enstat/workflows/CI/badge.svg)](https://github.com/tdegeus/enstat/actions)
 [![Documentation Status](https://readthedocs.org/projects/enstat/badge/?version=latest)](https://enstat.readthedocs.io)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/enstat.svg)](https://anaconda.org/conda-forge/enstat)
 [![PyPi release](https://img.shields.io/pypi/v/enstat.svg)](https://pypi.org/project/enstat/)
 
 Documentation: [enstat.readthedocs.io](https://enstat.readthedocs.io)
 
-## Overview
+## Hallmark feature
 
-*enstat* is a library to facilitate the computation of ensemble averages (and their variances) or histograms.
+*enstat* is a library to facilitate the computation of
 
-The key feature is that a class stores the sum of the first and second statistical moments and the number of samples.
-This gives access to the mean (and variance) at all times, while you can keep adding samples.
+*   [Ensemble averages (and their variance)](#readme-average);
+*   [Ensemble averages (and their variance) based on a certain binning of a quantity](#readme-binned);
+*   [Histograms of an ensemble](#readme-histogram).
 
-For the histogram something similar holds, but this time the count per bin is stored.
+**without storing the entire ensemble in memory**.
 
-### Ensemble average
+> Below you find a quick-start.
+> For more information, see the [documentation](https://enstat.readthedocs.io).
+
+<div id="readme-average"></div>
+
+## Ensemble average
+
+> The key feature is to store the sum of the first and second statistical moments and the number of samples.
+> This gives access to the mean (and variance) at all times, while you can keep adding samples.
 
 Suppose that we have 100 realisations, each with 1000 'blocks', and we want to know the ensemble average of each block:
 
 ```python
 import enstat
 import numpy as np
 
 ensemble = enstat.static()
 
 for realisation in range(100):
-
     sample = np.random.random(1000)
     ensemble += sample
 
 print(ensemble.mean())
 ```
 
 which will print a list of 1000 values, each around `0.5`.
+
 This is the equivalent of
 
 ```python
 import numpy as np
 
 container = np.empty((100, 1000))
 
-for realisation in range(100):
 
     sample = np.random.random(1000)
     container[realisation, :] = sample
 
 print(np.mean(container, axis=0))
 ```
 
 The key difference is that *enstat* only requires you to have `4 * N` values in memory for a sample of size `N`: the sample itself, the sums of the first and second moment, and the normalisation.
 Instead the solution with the container uses much more memory.
 
 A nice feature is also that you can keep adding samples to `ensemble`.
 You can even store it and continue later.
 
-### Ensemble histogram
+<div id="readme-histogram"></div>
+
+## Ensemble histogram
 
 Same example, but now we want the histogram for predefined bins:
 ```python
 import enstat
 import numpy as np
 
 bin_edges = np.linspace(0, 1, 11)
 hist = enstat.histogram(bin_edges=bin_edges)
 
 for realisation in range(100):
-
     sample = np.random.random(1000)
     hist += sample
 
 print(hist.p)
 ```
 
 which prints the probability density of each bin (so list of values around `0.1` for these bins).
@@ -104,14 +113,34 @@
     fig, ax = plt.subplots()
     ax.plot(hist.x, hist.p)
     plt.show()
     ```
 
     You can even use `ax.plot(*hist.plot)`.
 
+<div id="readme-binned"></div>
+
+## Average per bin
+
+Suppose you have some time series (`t`) with multiple observables (`a` and `b`); e.g.;
+```python
+import enstat
+import numpy as np
+
+t = np.linspace(0, 10, 100)
+a = np.random.normal(loc=5, scale=0.1, size=t.size)
+b = np.random.normal(loc=1, scale=0.5, size=t.size)
+```
+Now suppose that you want to compute the average `a`, `b`, and `t` based on a certain binning of `t`:
+```python
+bin_edges = np.linspace(0, 12, 12)
+binned = enstat.binned.from_data(t, a, b, names=["t", "a", "b"]m bin_edges=bin_edges)
+print(binned["a"].mean())
+```
+
 ## Installation
 
 -   Using conda
 
     ```bash
     conda install -c conda-forge enstat
     ```
```

### Comparing `enstat-0.9.2/enstat.egg-info/SOURCES.txt` & `enstat-0.9.3/enstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstat-0.9.2/tests/test_histogram.py` & `enstat-0.9.3/tests/test_histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,15 @@
 
         self.assertTrue(np.all(hist.count == hist_full.count[1:-1]))
         self.assertTrue(np.allclose(hist.p, hist_full.p[1:-1]))
 
     def test_mid(self):
         bin_edges = [-0.5, 0.5, 1.5, 2.5]
         mid = [0, 1, 2]
-
         hist = enstat.histogram(bin_edges=bin_edges)
-
         self.assertEqual(mid, hist.x.tolist())
 
 
 class Test_accumulate(unittest.TestCase):
     """
     Histogram accumulation.
     """
```

### Comparing `enstat-0.9.2/tests/test_main.py` & `enstat-0.9.3/tests/test_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 
     def test_scalar(self):
         """
         Basic test of "mean" and "std" using a random sample.
         """
 
         average = enstat.scalar()
-
-        average += np.array(1.0)
+        average += 1.0
 
         self.assertFalse(np.isnan(average.mean()))
         self.assertTrue(np.isnan(average.std()))
+        self.assertAlmostEqual(average.mean(), 1.0)
 
         average += np.array(1.0)
 
         self.assertFalse(np.isnan(average.mean()))
         self.assertFalse(np.isnan(average.std()))
+        self.assertAlmostEqual(average.mean(), 1.0)
+        self.assertAlmostEqual(average.std(), 0.0)
 
     def test_scalar_zero_division(self):
         """
         Check for zero division.
         """
 
         average = enstat.scalar()
@@ -230,14 +232,122 @@
                 np.sum(average.first) / np.sum(average.norm),
                 np.mean(a[np.logical_not(m)]),
             )
         )
 
         self.assertTrue(np.all(np.equal(average.norm, np.sum(np.logical_not(m), axis=0))))
 
+    def test_static_squash_example(self):
+        norm = np.array([[2, 2, 3, 1, 1], [2, 2, 1, 1, 3], [1, 1, 2, 2, 1], [2, 1, 2, 2, 2]])
+        average = enstat.static(shape=norm.shape)
+        average.norm = norm
+        average.squash([2, 2])
+        expect = np.array([[8, 6, 4], [5, 8, 3]])
+        self.assertTrue(np.all(np.equal(average.norm, expect)))
+
+    def test_static_squash_1d_a(self):
+        a = np.random.random(13 * 2).reshape(13, 2)
+        average = enstat.static(shape=[a.size])
+        average += a.ravel()
+        average.squash(2)
+        self.assertTrue(np.allclose(average.mean(), np.mean(a, axis=1)))
+
+        e = np.random.random(1)
+        average = enstat.static(shape=[a.size + 1])
+        average += np.concatenate((a.ravel(), e))
+        average.squash(2)
+        self.assertTrue(np.allclose(average.mean(), np.concatenate((np.mean(a, axis=1), e))))
+
+    def test_static_squash_1d_b(self):
+        a = np.random.random(13 * 3).reshape(13, 3)
+        average = enstat.static(shape=[a.size])
+        average += a.ravel()
+        average.squash(3)
+        self.assertTrue(np.allclose(average.mean(), np.mean(a, axis=1)))
+
+        e = np.random.random(2)
+        average = enstat.static(shape=[a.size + 2])
+        average += np.concatenate((a.ravel(), e))
+        average.squash(3)
+        self.assertTrue(
+            np.allclose(
+                average.mean(), np.concatenate((np.mean(a, axis=1), np.array([np.mean(e)])))
+            )
+        )
+
+    def test_static_squash_2d_a(self):
+        a = np.random.random(12 * 8).reshape(12, 8)
+        b = 0.25 * (a[::2, ::2] + a[1::2, ::2] + a[::2, 1::2] + a[1::2, 1::2])
+        average = enstat.static(shape=a.shape)
+        average += a
+        average.squash([2, 2])
+        self.assertTrue(np.allclose(average.mean(), b))
+
+        a = np.random.random(12 * 8).reshape(12, 8)[:-1, :]
+        n = np.ones_like(a)
+        z = np.zeros((1, 4))
+        b = (
+            a[::2, ::2]
+            + np.vstack((a[1::2, ::2], z))
+            + a[::2, 1::2]
+            + np.vstack((a[1::2, 1::2], z))
+        )
+        n = (
+            n[::2, ::2]
+            + np.vstack((n[1::2, ::2], z))
+            + n[::2, 1::2]
+            + np.vstack((n[1::2, 1::2], z))
+        )
+        average = enstat.static(shape=a.shape)
+        average += a
+        average.squash([2, 2])
+        self.assertTrue(np.allclose(average.mean(), b / n))
+
+        a = np.random.random(12 * 8).reshape(12, 8)[:, :-1]
+        n = np.ones_like(a)
+        z = np.zeros((6, 1))
+        b = (
+            a[::2, ::2]
+            + a[1::2, ::2]
+            + np.hstack((a[::2, 1::2], z))
+            + np.hstack((a[1::2, 1::2], z))
+        )
+        n = (
+            n[::2, ::2]
+            + n[1::2, ::2]
+            + np.hstack((n[::2, 1::2], z))
+            + np.hstack((n[1::2, 1::2], z))
+        )
+        average = enstat.static(shape=a.shape)
+        average += a
+        average.squash([2, 2])
+        self.assertTrue(np.allclose(average.mean(), b / n))
+
+        a = np.random.random(12 * 8).reshape(12, 8)[:-1, :-1]
+        n = np.ones_like(a)
+        zr = np.zeros((1, 4))
+        zc = np.zeros((6, 1))
+        zc1 = np.zeros((5, 1))
+        b = (
+            a[::2, ::2]
+            + np.vstack((a[1::2, ::2], zr))
+            + np.hstack((a[::2, 1::2], zc))
+            + np.vstack((np.hstack((a[1::2, 1::2], zc1)), zr))
+        )
+        n = (
+            n[::2, ::2]
+            + np.vstack((n[1::2, ::2], zr))
+            + np.hstack((n[::2, 1::2], zc))
+            + np.vstack((np.hstack((n[1::2, 1::2], zc1)), zr))
+        )
+        average = enstat.static(shape=a.shape)
+        average += a
+        average.squash([2, 2])
+        self.assertTrue(np.allclose(average.mean(), b / n))
+
     def test_dynamic1d(self):
         """
         Dynamically grow shape.
         """
 
         average = enstat.dynamic1d()
```

