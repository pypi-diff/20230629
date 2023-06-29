# Comparing `tmp/dkist_data_simulator-3.2.0.tar.gz` & `tmp/dkist_data_simulator-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_data_simulator-3.2.0.tar", last modified: Thu Jun 29 19:18:51 2023, max compression
+gzip compressed data, was "dkist_data_simulator-3.2.0rc1.tar", last modified: Tue Jun 27 17:09:39 2023, max compression
```

## Comparing `dkist_data_simulator-3.2.0.tar` & `dkist_data_simulator-3.2.0rc1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.685298 dkist_data_simulator-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     3308 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-06-29 19:18:51.685298 dkist_data_simulator-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1252 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/dkist_data_simulator/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/dkist_data_simulator/data/
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/data/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    16824 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10932 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     7180 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec122.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27073 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/core.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/cryo.py
--rw-rw-rw-   0 root         (0) root         (0)     3446 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/dlnirsp.py
--rw-rw-rw-   0 root         (0) root         (0)     7623 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/vbi.py
--rw-rw-rw-   0 root         (0) root         (0)     6602 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/visp.py
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/vtf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     8380 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     4339 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_214_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/util.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-29 19:18:51.000000 dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.677298 dkist_data_simulator-3.2.0/examples/
--rwxrwxrwx   0 root         (0) root         (0)     4098 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/examples/vtf_crisp_5d.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 19:18:51.685298 dkist_data_simulator-3.2.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2634 2023-06-29 19:18:51.685298 dkist_data_simulator-3.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      607 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-29 19:18:28.000000 dkist_data_simulator-3.2.0/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.812946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.812946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/data/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/data/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16824 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10932 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7180 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec122.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27073 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/cryo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3446 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/dlnirsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7623 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vbi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6602 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/visp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vtf.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     8380 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     4339 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.812946 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 17:09:39.000000 dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     4098 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/examples/vtf_crisp_5d.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 17:09:39.816946 dkist_data_simulator-3.2.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2634 2023-06-27 17:09:39.820946 dkist_data_simulator-3.2.0rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      607 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-27 17:09:16.000000 dkist_data_simulator-3.2.0rc1/tox.ini
```

### Comparing `dkist_data_simulator-3.2.0/.gitignore` & `dkist_data_simulator-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/.pre-commit-config.yaml` & `dkist_data_simulator-3.2.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/PKG-INFO` & `dkist_data_simulator-3.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_data_simulator
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.2.0/README.rst` & `dkist_data_simulator-3.2.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/bitbucket-pipelines.yml` & `dkist_data_simulator-3.2.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/dataset.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/expansions.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/schemas.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/schemas.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec122.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/core.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/core.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/cryo.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/cryo.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/dlnirsp.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/dlnirsp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/vbi.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vbi.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/visp.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/visp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/spec214/vtf.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/spec214/vtf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/tests/conftest.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_122.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_214.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_214_inventory.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_214_inventory.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/tests/test_dataset.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator/util.py` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator/util.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/PKG-INFO` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-data-simulator
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.2.0/dkist_data_simulator.egg-info/SOURCES.txt` & `dkist_data_simulator-3.2.0rc1/dkist_data_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/docs/Makefile` & `dkist_data_simulator-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/docs/conf.py` & `dkist_data_simulator-3.2.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/docs/make.bat` & `dkist_data_simulator-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/examples/vtf_crisp_5d.py` & `dkist_data_simulator-3.2.0rc1/examples/vtf_crisp_5d.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/licenses/LICENSE.rst` & `dkist_data_simulator-3.2.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/licenses/TEMPLATE_LICENSE.rst` & `dkist_data_simulator-3.2.0rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/setup.cfg` & `dkist_data_simulator-3.2.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/setup.py` & `dkist_data_simulator-3.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.2.0/tox.ini` & `dkist_data_simulator-3.2.0rc1/tox.ini`

 * *Files identical despite different names*

