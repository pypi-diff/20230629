# Comparing `tmp/piper-0.9.3.tar.gz` & `tmp/piper-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/piper-0.9.3.tar", last modified: Thu Jan 31 15:49:24 2019, max compression
+gzip compressed data, was "dist/piper-0.9.4.tar", last modified: Thu Jan 31 16:13:53 2019, max compression
```

## Comparing `piper-0.9.3.tar` & `piper-0.9.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 15:49:24.000000 piper-0.9.3/
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     7513 2019-01-22 15:41:03.000000 piper-0.9.3/logo_pypiper.svg
-drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 15:49:24.000000 piper-0.9.3/requirements/
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       25 2019-01-22 15:41:03.000000 piper-0.9.3/requirements/reqs-plot.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       26 2019-01-22 15:41:03.000000 piper-0.9.3/requirements/reqs-ngstk.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       26 2019-01-22 15:41:03.000000 piper-0.9.3/requirements/reqs-test.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       14 2019-01-22 15:41:03.000000 piper-0.9.3/requirements/reqs-pypiper.txt
-drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 15:49:24.000000 piper-0.9.3/pypiper/
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     1051 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/folder_context.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)    18977 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/pipeline.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)    84245 2019-01-29 22:58:13.000000 piper-0.9.3/pypiper/manager.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)    27842 2019-01-29 22:58:13.000000 piper-0.9.3/pypiper/utils.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     2663 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/stage.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      355 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/flags.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      137 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/const.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     3307 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/exceptions.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      199 2019-01-22 15:41:03.000000 piper-0.9.3/pypiper/__init__.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     2231 2019-01-30 22:45:40.000000 piper-0.9.3/pypiper/AttributeDict.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       23 2019-01-31 15:42:31.000000 piper-0.9.3/pypiper/_version.py
--rwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)    76093 2019-01-29 22:59:01.000000 piper-0.9.3/pypiper/ngstk.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      553 2019-01-22 15:41:03.000000 piper-0.9.3/README.md
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     2651 2019-01-22 15:41:03.000000 piper-0.9.3/setup.py
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       38 2019-01-31 15:49:24.000000 piper-0.9.3/setup.cfg
-drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 15:49:24.000000 piper-0.9.3/piper.egg-info/
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)        1 2019-01-31 15:49:24.000000 piper-0.9.3/piper.egg-info/dependency_links.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)        8 2019-01-31 15:49:24.000000 piper-0.9.3/piper.egg-info/top_level.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      540 2019-01-31 15:49:24.000000 piper-0.9.3/piper.egg-info/SOURCES.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      224 2019-01-31 15:49:24.000000 piper-0.9.3/piper.egg-info/requires.txt
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     1305 2019-01-31 15:49:24.000000 piper-0.9.3/piper.egg-info/PKG-INFO
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       65 2019-01-22 15:41:03.000000 piper-0.9.3/MANIFEST.in
--rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     1305 2019-01-31 15:49:24.000000 piper-0.9.3/PKG-INFO
+drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 16:13:53.000000 piper-0.9.4/
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     7513 2019-01-22 15:41:03.000000 piper-0.9.4/logo_pypiper.svg
+drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 16:13:53.000000 piper-0.9.4/requirements/
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       25 2019-01-22 15:41:03.000000 piper-0.9.4/requirements/reqs-plot.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       26 2019-01-22 15:41:03.000000 piper-0.9.4/requirements/reqs-ngstk.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       26 2019-01-22 15:41:03.000000 piper-0.9.4/requirements/reqs-test.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       33 2019-01-31 16:02:07.000000 piper-0.9.4/requirements/reqs-build-release.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       14 2019-01-22 15:41:03.000000 piper-0.9.4/requirements/reqs-pypiper.txt
+drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 16:13:53.000000 piper-0.9.4/pypiper/
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     1051 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/folder_context.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)    18977 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/pipeline.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)    84245 2019-01-29 22:58:13.000000 piper-0.9.4/pypiper/manager.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)    27842 2019-01-29 22:58:13.000000 piper-0.9.4/pypiper/utils.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     2663 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/stage.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      355 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/flags.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      137 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/const.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     3307 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/exceptions.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      199 2019-01-22 15:41:03.000000 piper-0.9.4/pypiper/__init__.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     2231 2019-01-30 22:45:40.000000 piper-0.9.4/pypiper/AttributeDict.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       23 2019-01-31 15:56:39.000000 piper-0.9.4/pypiper/_version.py
+-rwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)    76093 2019-01-29 22:59:01.000000 piper-0.9.4/pypiper/ngstk.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      553 2019-01-22 15:41:03.000000 piper-0.9.4/README.md
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     2702 2019-01-31 15:55:52.000000 piper-0.9.4/setup.py
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       38 2019-01-31 16:13:53.000000 piper-0.9.4/setup.cfg
+drwxr-xr-x   0 vpr9v     (1000) vpr9v     (1000)        0 2019-01-31 16:13:53.000000 piper-0.9.4/piper.egg-info/
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)        1 2019-01-31 16:13:53.000000 piper-0.9.4/piper.egg-info/dependency_links.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)        8 2019-01-31 16:13:53.000000 piper-0.9.4/piper.egg-info/top_level.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      576 2019-01-31 16:13:53.000000 piper-0.9.4/piper.egg-info/SOURCES.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)      224 2019-01-31 16:13:53.000000 piper-0.9.4/piper.egg-info/requires.txt
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     1345 2019-01-31 16:13:53.000000 piper-0.9.4/piper.egg-info/PKG-INFO
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)       65 2019-01-22 15:41:03.000000 piper-0.9.4/MANIFEST.in
+-rw-r--r--   0 vpr9v     (1000) vpr9v     (1000)     1345 2019-01-31 16:13:53.000000 piper-0.9.4/PKG-INFO
```

### Comparing `piper-0.9.3/logo_pypiper.svg` & `piper-0.9.4/logo_pypiper.svg`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/folder_context.py` & `piper-0.9.4/pypiper/folder_context.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/pipeline.py` & `piper-0.9.4/pypiper/pipeline.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/manager.py` & `piper-0.9.4/pypiper/manager.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/utils.py` & `piper-0.9.4/pypiper/utils.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/stage.py` & `piper-0.9.4/pypiper/stage.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/exceptions.py` & `piper-0.9.4/pypiper/exceptions.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/AttributeDict.py` & `piper-0.9.4/pypiper/AttributeDict.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/pypiper/ngstk.py` & `piper-0.9.4/pypiper/ngstk.py`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/README.md` & `piper-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `piper-0.9.3/setup.py` & `piper-0.9.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 setup(
     name='piper',
     packages=['pypiper'],
     install_requires=basic_reqs,
     version=version,
     description='A lightweight python toolkit for gluing together restartable, robust command line pipelines',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 2.7",
         "Topic :: Scientific/Engineering :: Bio-Informatics"
     ],    
     author='Nathan Sheffield, Johanna Klughammer, Andre Rendeiro',
```

### Comparing `piper-0.9.3/piper.egg-info/SOURCES.txt` & `piper-0.9.4/piper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 pypiper/flags.py
 pypiper/folder_context.py
 pypiper/manager.py
 pypiper/ngstk.py
 pypiper/pipeline.py
 pypiper/stage.py
 pypiper/utils.py
+requirements/reqs-build-release.txt
 requirements/reqs-ngstk.txt
 requirements/reqs-plot.txt
 requirements/reqs-pypiper.txt
 requirements/reqs-test.txt
```

### Comparing `piper-0.9.3/piper.egg-info/PKG-INFO` & `piper-0.9.4/piper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piper
-Version: 0.9.3
+Version: 0.9.4
 Summary: A lightweight python toolkit for gluing together restartable, robust command line pipelines
 Home-page: https://github.com/databio/pypiper/
 Author: Nathan Sheffield, Johanna Klughammer, Andre Rendeiro
 Author-email: nathan@code.databio.org, jklughammer@cemm.oeaw.ac.at, arendeiro@cemm.oeaw.ac.at
 License: BSD2
 Description: <img src="logo_pypiper.svg" alt="Pypiper logo" height="70" align="left"/>
         
@@ -16,11 +16,12 @@
         A lightweight python toolkit for gluing together restartable, robust command line pipelines. The best place to learn more is at the [documentation hosted at Read the Docs](http://pypiper.readthedocs.org/).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: all
 Provides-Extra: ngstk
 Provides-Extra: dev
```

### Comparing `piper-0.9.3/PKG-INFO` & `piper-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piper
-Version: 0.9.3
+Version: 0.9.4
 Summary: A lightweight python toolkit for gluing together restartable, robust command line pipelines
 Home-page: https://github.com/databio/pypiper/
 Author: Nathan Sheffield, Johanna Klughammer, Andre Rendeiro
 Author-email: nathan@code.databio.org, jklughammer@cemm.oeaw.ac.at, arendeiro@cemm.oeaw.ac.at
 License: BSD2
 Description: <img src="logo_pypiper.svg" alt="Pypiper logo" height="70" align="left"/>
         
@@ -16,11 +16,12 @@
         A lightweight python toolkit for gluing together restartable, robust command line pipelines. The best place to learn more is at the [documentation hosted at Read the Docs](http://pypiper.readthedocs.org/).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: all
 Provides-Extra: ngstk
 Provides-Extra: dev
```

