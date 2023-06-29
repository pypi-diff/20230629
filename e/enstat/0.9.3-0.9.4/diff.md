# Comparing `tmp/enstat-0.9.3.tar.gz` & `tmp/enstat-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.9.3.tar", last modified: Thu Jun 29 13:13:44 2023, max compression
+gzip compressed data, was "enstat-0.9.4.tar", last modified: Thu Jun 29 18:11:57 2023, max compression
```

## Comparing `enstat-0.9.3.tar` & `enstat-0.9.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.750699 enstat-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.738699 enstat-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.742699 enstat-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 13:13:35.000000 enstat-0.9.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 13:13:35.000000 enstat-0.9.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 13:13:35.000000 enstat-0.9.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-29 13:13:35.000000 enstat-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-29 13:13:35.000000 enstat-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 13:13:35.000000 enstat-0.9.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 13:13:35.000000 enstat-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 13:13:44.750699 enstat-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-29 13:13:35.000000 enstat-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.746699 enstat-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-29 13:13:35.000000 enstat-0.9.3/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.746699 enstat-0.9.3/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    30597 2023-06-29 13:13:35.000000 enstat-0.9.3/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-29 13:13:35.000000 enstat-0.9.3/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-29 13:13:35.000000 enstat-0.9.3/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.750699 enstat-0.9.3/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 13:13:44.000000 enstat-0.9.3/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 13:13:35.000000 enstat-0.9.3/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 13:13:35.000000 enstat-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:13:44.750699 enstat-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:44.750699 enstat-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-06-29 13:13:35.000000 enstat-0.9.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.558464 enstat-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 18:11:48.000000 enstat-0.9.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 18:11:48.000000 enstat-0.9.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 18:11:48.000000 enstat-0.9.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-29 18:11:48.000000 enstat-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-29 18:11:48.000000 enstat-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 18:11:48.000000 enstat-0.9.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 18:11:48.000000 enstat-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 18:11:57.562464 enstat-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-29 18:11:48.000000 enstat-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    30649 2023-06-29 18:11:48.000000 enstat-0.9.4/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-29 18:11:48.000000 enstat-0.9.4/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-29 18:11:48.000000 enstat-0.9.4/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 18:11:48.000000 enstat-0.9.4/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 18:11:48.000000 enstat-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:11:57.562464 enstat-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/test_main.py
```

### Comparing `enstat-0.9.3/.github/workflows/ci.yml` & `enstat-0.9.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/.github/workflows/python-publish.yml` & `enstat-0.9.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/.gitignore` & `enstat-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/.pre-commit-config.yaml` & `enstat-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/LICENSE` & `enstat-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/PKG-INFO` & `enstat-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.3
+Version: 0.9.4
 Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enstat-0.9.3/README.md` & `enstat-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/docs/Makefile` & `enstat-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/docs/make.bat` & `enstat-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/docs/module.rst` & `enstat-0.9.4/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/enstat/__init__.py` & `enstat-0.9.4/enstat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,14 +994,17 @@
         kwargs = {name: np.asarray(arg)[keep] for name, arg in kwargs.items()}
         sqr = {name: arg * arg for name, arg in kwargs.items()}
 
         for name, arg in kwargs.items():
             if arg.shape != kwargs[self.names[0]].shape:
                 raise ValueError("All arguments must have the same shape")
 
+        if ibin.size == 0:
+            return self
+
         # see https://stackoverflow.com/q/76574134/2646505
         sorter = np.argsort(ibin)
         ibin = ibin[sorter]
         norm = np.argwhere(np.diff(ibin, prepend=ibin[0], append=1)).flatten()
         split = norm - 1
         norm = np.diff(norm, prepend=0)
         store = ibin[split]
```

### Comparing `enstat-0.9.3/enstat/detail.py` & `enstat-0.9.4/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/enstat/mean.py` & `enstat-0.9.4/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/enstat.egg-info/PKG-INFO` & `enstat-0.9.4/enstat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.3
+Version: 0.9.4
 Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enstat-0.9.3/enstat.egg-info/SOURCES.txt` & `enstat-0.9.4/enstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/tests/test_binned.py` & `enstat-0.9.4/tests/test_binned.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 
         x = np.array([2.5, 4.5])
         y = np.array([1, 2])
         bin_edges = np.array([0, 1, 2, 3, 4, 5])
         notnan = np.array([False, False, True, False, True])
         binned = enstat.binned.from_data(x, y, bin_edges=bin_edges)
 
+    def test_bounds(self):
+        x = np.array([0.5, 1.5, 2.5, 4, 5, 6])
+        y = np.array([1, 2, 3, 1, 2, 3])
+        bin_edges = np.array([0, 1, 2, 3])
+        binned = enstat.binned.from_data(x, y, bin_edges=bin_edges, bound_error="ignore")
+        self.assertTrue(np.allclose(binned[0].mean(), np.array([0.5, 1.5, 2.5])))
+        self.assertTrue(np.allclose(binned[1].mean(), np.array([1, 2, 3])))
+
     def test_simple(self):
         """
         Plain data, one variables.
         """
         x = np.random.random(1234)
         bin_edges = np.linspace(0, 1, 13)
         binned = enstat.binned.from_data(x, bin_edges=bin_edges)
```

### Comparing `enstat-0.9.3/tests/test_histogram.py` & `enstat-0.9.4/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.3/tests/test_main.py` & `enstat-0.9.4/tests/test_main.py`

 * *Files identical despite different names*

