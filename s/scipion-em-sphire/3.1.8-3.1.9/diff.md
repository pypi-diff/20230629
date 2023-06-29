# Comparing `tmp/scipion-em-sphire-3.1.8.tar.gz` & `tmp/scipion-em-sphire-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-sphire-3.1.8.tar", last modified: Thu May 11 07:57:01 2023, max compression
+gzip compressed data, was "scipion-em-sphire-3.1.9.tar", last modified: Mon May 15 08:53:14 2023, max compression
```

## Comparing `scipion-em-sphire-3.1.8.tar` & `scipion-em-sphire-3.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.161172 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 07:57:01.000000 scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.161172 scipion-em-sphire-3.1.8/sphire/
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.161172 scipion-em-sphire-3.1.8/sphire/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_napari_tomo_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_tomo_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_tomo_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols/protocol_janni_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/sphire_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/sphire/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/tests/test_protocol_cryolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/tests/test_protocol_janni.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:57:01.165172 scipion-em-sphire-3.1.8/sphire/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/viewers/viewer_napari.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-11 07:54:45.000000 scipion-em-sphire-3.1.8/sphire/viewers/views_tkinter_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:53:14.945712 scipion-em-sphire-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-15 08:53:14.941712 scipion-em-sphire-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:53:14.941712 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-15 08:53:14.000000 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-15 08:53:14.000000 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:53:14.000000 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 08:53:14.000000 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 08:53:14.000000 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 08:53:14.000000 scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 08:53:14.945712 scipion-em-sphire-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:53:14.941712 scipion-em-sphire-3.1.9/sphire/
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:53:14.941712 scipion-em-sphire-3.1.9/sphire/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_napari_tomo_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_tomo_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_tomo_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols/protocol_janni_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/sphire_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:53:14.941712 scipion-em-sphire-3.1.9/sphire/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/tests/test_protocol_cryolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/tests/test_protocol_janni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:53:14.941712 scipion-em-sphire-3.1.9/sphire/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/viewers/viewer_napari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-15 08:51:25.000000 scipion-em-sphire-3.1.9/sphire/viewers/views_tkinter_tree.py
```

### Comparing `scipion-em-sphire-3.1.8/CHANGES.txt` & `scipion-em-sphire-3.1.9/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.1.9: ftp links are not working, replaced by https
 3.1.8: Fix: coordinates 3d sent to napari are not flipped on Y axis.
 3.1.7:
      - Creating a manual picking protocol using napari-boxmanager
      - Creating a tomogram training protocol
      - Adding the filaments options to cryolo tomogram picking protocol
 3.1.6: fix pretrained_weights param
 3.1.5: fix auto picking streaming
```

### Comparing `scipion-em-sphire-3.1.8/LICENSE` & `scipion-em-sphire-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/PKG-INFO` & `scipion-em-sphire-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-sphire
-Version: 3.1.8
+Version: 3.1.9
 Summary: Plugin to use Sphire programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-sphire
 Author: I2PC, Jose Miguel de La Rosa Trevin, Jorge Jiménez
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-sphire/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-sphire/
```

### Comparing `scipion-em-sphire-3.1.8/README.rst` & `scipion-em-sphire-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/PKG-INFO` & `scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-sphire
-Version: 3.1.8
+Version: 3.1.9
 Summary: Plugin to use Sphire programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-sphire
 Author: I2PC, Jose Miguel de La Rosa Trevin, Jorge Jiménez
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-sphire/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-sphire/
```

### Comparing `scipion-em-sphire-3.1.8/scipion_em_sphire.egg-info/SOURCES.txt` & `scipion-em-sphire-3.1.9/scipion_em_sphire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/setup.py` & `scipion-em-sphire-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/__init__.py` & `scipion-em-sphire-3.1.9/sphire/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import pwem
 import pyworkflow.utils as pwutils
 from pyworkflow.utils import runJob, weakImport
 
 from .constants import *
 
 
-__version__ = '3.1.8'
+__version__ = '3.1.9'
 _logo = "sphire_logo.png"
 _references = ['Wagner2019']
 
 
 class Plugin(pwem.Plugin):
     _pathVars = [CRYOLO_CUDA_LIB]
     _url = 'https://github.com/scipion-em/scipion-em-sphire'
@@ -175,28 +175,30 @@
 
         with weakImport('tomo'):
             _addNapari(defaultVersion, default=True)
 
         def _addModel(model, version, link, filename, default=False):
             env.addPackage(model, version=version,
                            tar='void.tgz',
-                           commands=[(f"wget {link}/{filename}", filename)],
+                           commands=[(f"wget {link} -O {filename}", filename)],
                            neededProgs=["wget"],
                            default=default)
 
-        url = "ftp://ftp.gwdg.de/pub/misc/sphire/crYOLO-GENERAL-MODELS"
-        _addModel(CRYOLO_GENMOD, CRYOLO_GENMOD_202005, url,
+        _addModel(CRYOLO_GENMOD, CRYOLO_GENMOD_202005,
+                  "https://owncloud.gwdg.de/index.php/s/AdVdYdcCg4XaNRw/download",
                   CRYOLO_GENMOD_202005_FN, True)
-        _addModel(CRYOLO_GENMOD, CRYOLO_GENMOD_NN_202005, url,
+        _addModel(CRYOLO_GENMOD, CRYOLO_GENMOD_NN_202005,
+                  "https://owncloud.gwdg.de/index.php/s/RVEnx1t0t7DTbgA/download",
                   CRYOLO_GENMOD_NN_202005_FN, True)
-        _addModel(CRYOLO_NS_GENMOD, CRYOLO_NS_GENMOD_20190226, url,
+        _addModel(CRYOLO_NS_GENMOD, CRYOLO_NS_GENMOD_20190226,
+                  "https://owncloud.gwdg.de/index.php/s/KpSw1gGIM3Q3KGa/download",
                   CRYOLO_NS_GENMOD_20190226_FN, False)
 
         url = "https://github.com/MPI-Dortmund/sphire-janni/raw/master/janni_general_models/"
-        _addModel(JANNI_GENMOD, JANNI_GENMOD_20190703, url,
+        _addModel(JANNI_GENMOD, JANNI_GENMOD_20190703, url + JANNI_GENMOD_20190703_FN,
                   JANNI_GENMOD_20190703_FN, True)
 
     @classmethod
     def versionGE(cls, version):
         """ Return True if current version of crYOLO is newer
          or equal than the input argument.
          Params:
```

### Comparing `scipion-em-sphire-3.1.8/sphire/bibtex.py` & `scipion-em-sphire-3.1.9/sphire/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/constants.py` & `scipion-em-sphire-3.1.9/sphire/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/convert.py` & `scipion-em-sphire-3.1.9/sphire/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/objects.py` & `scipion-em-sphire-3.1.9/sphire/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/__init__.py` & `scipion-em-sphire-3.1.9/sphire/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_base.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_import.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_napari_tomo_picking.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_napari_tomo_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_picking.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_tomo_picking.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_tomo_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_tomo_training.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_tomo_training.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_cryolo_training.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_cryolo_training.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols/protocol_janni_denoise.py` & `scipion-em-sphire-3.1.9/sphire/protocols/protocol_janni_denoise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/protocols.conf` & `scipion-em-sphire-3.1.9/sphire/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/sphire_logo.png` & `scipion-em-sphire-3.1.9/sphire/sphire_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/tests/__init__.py` & `scipion-em-sphire-3.1.9/sphire/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/tests/test_protocol_cryolo.py` & `scipion-em-sphire-3.1.9/sphire/tests/test_protocol_cryolo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/tests/test_protocol_janni.py` & `scipion-em-sphire-3.1.9/sphire/tests/test_protocol_janni.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/viewers/__init__.py` & `scipion-em-sphire-3.1.9/sphire/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/viewers/viewer_napari.py` & `scipion-em-sphire-3.1.9/sphire/viewers/viewer_napari.py`

 * *Files identical despite different names*

### Comparing `scipion-em-sphire-3.1.8/sphire/viewers/views_tkinter_tree.py` & `scipion-em-sphire-3.1.9/sphire/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

