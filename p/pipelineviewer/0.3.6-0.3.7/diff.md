# Comparing `tmp/pipelineviewer-0.3.6.tar.gz` & `tmp/pipelineviewer-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelineviewer-0.3.6.tar", last modified: Tue May 25 16:57:05 2021, max compression
+gzip compressed data, was "pipelineviewer-0.3.7.tar", last modified: Thu Jun 29 12:36:15 2023, max compression
```

## Comparing `pipelineviewer-0.3.6.tar` & `pipelineviewer-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 16:57:05.479017 pipelineviewer-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 16:57:05.475016 pipelineviewer-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 16:57:05.475016 pipelineviewer-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-05-25 16:57:05.479017 pipelineviewer-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 16:57:05.475016 pipelineviewer-0.3.6/pipelineviewer/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/ariane.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/boom.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/ctf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/ibex.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8647 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/pipelineviewer/swerv.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 16:57:05.475016 pipelineviewer-0.3.6/pipelineviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      513 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-05-25 16:57:05.000000 pipelineviewer-0.3.6/pipelineviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-25 16:57:05.479017 pipelineviewer-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6625 2021-05-25 16:56:52.000000 pipelineviewer-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:36:15.579395 pipelineviewer-0.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:36:15.575395 pipelineviewer-0.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:36:15.575395 pipelineviewer-0.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 12:36:15.579395 pipelineviewer-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:36:15.579395 pipelineviewer-0.3.7/pipelineviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/ariane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/boom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/ibex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8647 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/pipelineviewer/swerv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:36:15.579395 pipelineviewer-0.3.7/pipelineviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 12:36:15.000000 pipelineviewer-0.3.7/pipelineviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:36:15.579395 pipelineviewer-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-29 12:35:59.000000 pipelineviewer-0.3.7/setup.py
```

### Comparing `pipelineviewer-0.3.6/.github/workflows/python-publish.yml` & `pipelineviewer-0.3.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/PKG-INFO` & `pipelineviewer-0.3.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pipelineviewer
-Version: 0.3.6
+Version: 0.3.7
 Summary: CPU Pipeline Viewer
 Home-page: https://github.com/wallento/pipeline-viewer
 Author: Stefan Wallentowitz
 Author-email: stefan@wallentowitz.de
-License: UNKNOWN
-Description: CPU Pipeline Viewer
-        ===================
-        
-        This is a CPU pipeline viewer, similar to gem5's o3-pipeview.
-        
 Keywords: cpu pipeline viewer
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+
+CPU Pipeline Viewer
+===================
+
+This is a CPU pipeline viewer, similar to gem5's o3-pipeview.
```

### Comparing `pipelineviewer-0.3.6/pipelineviewer/ariane.py` & `pipelineviewer-0.3.7/pipelineviewer/ariane.py`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/pipelineviewer/boom.py` & `pipelineviewer-0.3.7/pipelineviewer/boom.py`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/pipelineviewer/ctf.py` & `pipelineviewer-0.3.7/pipelineviewer/ctf.py`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/pipelineviewer/ibex.py` & `pipelineviewer-0.3.7/pipelineviewer/ibex.py`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/pipelineviewer/main.py` & `pipelineviewer-0.3.7/pipelineviewer/main.py`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/pipelineviewer/swerv.py` & `pipelineviewer-0.3.7/pipelineviewer/swerv.py`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/pipelineviewer.egg-info/PKG-INFO` & `pipelineviewer-0.3.7/pipelineviewer.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pipelineviewer
-Version: 0.3.6
+Version: 0.3.7
 Summary: CPU Pipeline Viewer
 Home-page: https://github.com/wallento/pipeline-viewer
 Author: Stefan Wallentowitz
 Author-email: stefan@wallentowitz.de
-License: UNKNOWN
-Description: CPU Pipeline Viewer
-        ===================
-        
-        This is a CPU pipeline viewer, similar to gem5's o3-pipeview.
-        
 Keywords: cpu pipeline viewer
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+
+CPU Pipeline Viewer
+===================
+
+This is a CPU pipeline viewer, similar to gem5's o3-pipeview.
```

### Comparing `pipelineviewer-0.3.6/pipelineviewer.egg-info/SOURCES.txt` & `pipelineviewer-0.3.7/pipelineviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipelineviewer-0.3.6/setup.py` & `pipelineviewer-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get the long description from the README file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
-requires = ["attrdict", "colorama", "pygments", "riscv-model>=0.6.6"]
+requires = ["attrdict3", "colorama", "pygments", "riscv-model>=0.6.6"]
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
```

