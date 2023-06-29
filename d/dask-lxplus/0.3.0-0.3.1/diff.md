# Comparing `tmp/dask_lxplus-0.3.0.tar.gz` & `tmp/dask_lxplus-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_lxplus-0.3.0.tar", last modified: Wed Jun 28 14:50:58 2023, max compression
+gzip compressed data, was "dask_lxplus-0.3.1.tar", last modified: Thu Jun 29 07:16:34 2023, max compression
```

## Comparing `dask_lxplus-0.3.0.tar` & `dask_lxplus-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-28 14:50:58.384212 dask_lxplus-0.3.0/
--rw-r--r--   0 ben        (501) staff       (20)      589 2022-08-10 12:35:46.000000 dask_lxplus-0.3.0/LICENSE.txt
--rw-r--r--   0 ben        (501) staff       (20)       27 2022-08-10 15:10:59.000000 dask_lxplus-0.3.0/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     2799 2023-06-28 14:50:58.384298 dask_lxplus-0.3.0/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     2064 2022-08-10 14:26:52.000000 dask_lxplus-0.3.0/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-28 14:50:58.382810 dask_lxplus-0.3.0/dask_lxplus/
--rw-r--r--   0 ben        (501) staff       (20)      286 2021-11-26 14:54:16.000000 dask_lxplus-0.3.0/dask_lxplus/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     8965 2023-06-28 14:50:15.000000 dask_lxplus-0.3.0/dask_lxplus/cluster.py
--rw-r--r--   0 ben        (501) staff       (20)      525 2021-11-26 14:54:16.000000 dask_lxplus-0.3.0/dask_lxplus/config.py
--rw-r--r--   0 ben        (501) staff       (20)      743 2023-06-28 14:50:15.000000 dask_lxplus-0.3.0/dask_lxplus/jobqueue-cern.yaml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-28 14:50:58.383785 dask_lxplus-0.3.0/dask_lxplus.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2799 2023-06-28 14:50:58.000000 dask_lxplus-0.3.0/dask_lxplus.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      348 2023-06-28 14:50:58.000000 dask_lxplus-0.3.0/dask_lxplus.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-06-28 14:50:58.000000 dask_lxplus-0.3.0/dask_lxplus.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)      166 2023-06-28 14:50:58.000000 dask_lxplus-0.3.0/dask_lxplus.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-06-28 14:50:58.000000 dask_lxplus-0.3.0/dask_lxplus.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     1010 2023-06-28 14:50:58.384640 dask_lxplus-0.3.0/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)       61 2021-11-26 14:54:16.000000 dask_lxplus-0.3.0/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-28 14:50:58.384010 dask_lxplus-0.3.0/tests/
--rw-r--r--   0 ben        (501) staff       (20)     4100 2023-06-28 14:50:15.000000 dask_lxplus-0.3.0/tests/test_cluster.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.983399 dask_lxplus-0.3.1/
+-rw-r--r--   0 ben        (501) staff       (20)      589 2022-08-10 12:35:46.000000 dask_lxplus-0.3.1/LICENSE.txt
+-rw-r--r--   0 ben        (501) staff       (20)       27 2022-08-10 15:10:59.000000 dask_lxplus-0.3.1/MANIFEST.in
+-rw-r--r--   0 ben        (501) staff       (20)     2799 2023-06-29 07:16:34.983469 dask_lxplus-0.3.1/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     2064 2022-08-10 14:26:52.000000 dask_lxplus-0.3.1/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.982274 dask_lxplus-0.3.1/dask_lxplus/
+-rw-r--r--   0 ben        (501) staff       (20)      286 2021-11-26 14:54:16.000000 dask_lxplus-0.3.1/dask_lxplus/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     8966 2023-06-29 07:14:25.000000 dask_lxplus-0.3.1/dask_lxplus/cluster.py
+-rw-r--r--   0 ben        (501) staff       (20)      525 2021-11-26 14:54:16.000000 dask_lxplus-0.3.1/dask_lxplus/config.py
+-rw-r--r--   0 ben        (501) staff       (20)      743 2023-06-28 14:50:15.000000 dask_lxplus-0.3.1/dask_lxplus/jobqueue-cern.yaml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.983099 dask_lxplus-0.3.1/dask_lxplus.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2799 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      348 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)      166 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)     1010 2023-06-29 07:16:34.984005 dask_lxplus-0.3.1/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)       61 2021-11-26 14:54:16.000000 dask_lxplus-0.3.1/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.983225 dask_lxplus-0.3.1/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     4100 2023-06-28 14:50:15.000000 dask_lxplus-0.3.1/tests/test_cluster.py
```

### Comparing `dask_lxplus-0.3.0/LICENSE.txt` & `dask_lxplus-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.0/PKG-INFO` & `dask_lxplus-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask_lxplus
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/cernops/dask-lxplus
 Author: Ben Jones
 Author-email: b.jones@cern.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `dask_lxplus-0.3.0/README.md` & `dask_lxplus-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.0/dask_lxplus/cluster.py` & `dask_lxplus-0.3.1/dask_lxplus/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 self.job_header_dict.pop("Stream_Output", None)
                 self.job_header_dict.pop("Stream_Error", None)
 
 
 class CernCluster(HTCondorCluster):
     __doc__ = (
         HTCondorCluster.__doc__
-    """
+    +"""
     A customized :class:`dask_jobqueue.HTCondorCluster` subclass for spawning Dask workers in the CERN HTCondor pool
 
     It provides the customizations and submit options required for the CERN pool.
     
     Additional CERN parameters:
     worker_image: The container to run the Dask workers inside. Defaults to: 
     ``"/cvmfs/unpacked.cern.ch/gitlab-registry.cern.ch/batch-team/dask-lxplus/lxdask-cc7:latest"``
```

### Comparing `dask_lxplus-0.3.0/dask_lxplus/config.py` & `dask_lxplus-0.3.1/dask_lxplus/config.py`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.0/dask_lxplus/jobqueue-cern.yaml` & `dask_lxplus-0.3.1/dask_lxplus/jobqueue-cern.yaml`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.0/dask_lxplus.egg-info/PKG-INFO` & `dask_lxplus-0.3.1/dask_lxplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-lxplus
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/cernops/dask-lxplus
 Author: Ben Jones
 Author-email: b.jones@cern.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `dask_lxplus-0.3.0/setup.cfg` & `dask_lxplus-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dask_lxplus
-version = 0.3.0
+version = 0.3.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.txt
 author = Ben Jones
 author_email = b.jones@cern.ch
 url = https://github.com/cernops/dask-lxplus
 classifiers =
```

### Comparing `dask_lxplus-0.3.0/tests/test_cluster.py` & `dask_lxplus-0.3.1/tests/test_cluster.py`

 * *Files identical despite different names*

