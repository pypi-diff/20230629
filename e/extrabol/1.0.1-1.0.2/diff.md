# Comparing `tmp/extrabol-1.0.1.tar.gz` & `tmp/extrabol-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrabol-1.0.1.tar", last modified: Thu Jun 29 17:17:41 2023, max compression
+gzip compressed data, was "extrabol-1.0.2.tar", last modified: Thu Jun 29 19:51:07 2023, max compression
```

## Comparing `extrabol-1.0.1.tar` & `extrabol-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:41.835362 extrabol-1.0.1/
--rw-r--r--   0 ian       (1000) ian       (1000)     1058 2023-06-29 17:17:27.000000 extrabol-1.0.1/LICENSE
--rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 17:17:41.835362 extrabol-1.0.1/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)     3411 2023-06-29 17:17:27.000000 extrabol-1.0.1/README.md
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:41.825362 extrabol-1.0.1/extrabol/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:27.000000 extrabol-1.0.1/extrabol/__init__.py
--rw-r--r--   0 ian       (1000) ian       (1000)    36969 2023-06-29 17:17:27.000000 extrabol-1.0.1/extrabol/extrabol.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 17:17:41.835362 extrabol-1.0.1/extrabol.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)      268 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       52 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       74 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-06-29 17:17:41.000000 extrabol-1.0.1/extrabol.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)      928 2023-06-29 17:17:27.000000 extrabol-1.0.1/pyproject.toml
--rw-r--r--   0 ian       (1000) ian       (1000)       38 2023-06-29 17:17:41.835362 extrabol-1.0.1/setup.cfg
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.363808 extrabol-1.0.2/
+-rw-r--r--   0 ian       (1000) ian       (1000)     1058 2023-06-29 19:50:56.000000 extrabol-1.0.2/LICENSE
+-rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 19:51:07.363808 extrabol-1.0.2/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)     3411 2023-06-29 19:50:56.000000 extrabol-1.0.2/README.md
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.353808 extrabol-1.0.2/extrabol/
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/__init__.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.353808 extrabol-1.0.2/extrabol/example/
+-rw-r--r--   0 ian       (1000) ian       (1000)    17503 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/example/SN2010bc.dat
+-rw-r--r--   0 ian       (1000) ian       (1000)    36965 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/extrabol.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.363808 extrabol-1.0.2/extrabol/template_bank/
+-rw-r--r--   0 ian       (1000) ian       (1000)  5244546 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn1a.npz
+-rw-r--r--   0 ian       (1000) ian       (1000)  4956426 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn1bc.npz
+-rw-r--r--   0 ian       (1000) ian       (1000)   692250 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn2l.npz
+-rw-r--r--   0 ian       (1000) ian       (1000)   692250 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn2p.npz
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.353808 extrabol-1.0.2/extrabol.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)      463 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       52 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/entry_points.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       94 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/top_level.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)     1030 2023-06-29 19:50:56.000000 extrabol-1.0.2/pyproject.toml
+-rw-r--r--   0 ian       (1000) ian       (1000)       38 2023-06-29 19:51:07.363808 extrabol-1.0.2/setup.cfg
```

### Comparing `extrabol-1.0.1/LICENSE` & `extrabol-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.1/PKG-INFO` & `extrabol-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrabol
-Version: 1.0.1
+Version: 1.0.2
 Summary: Estimate SN bolometric light curves
 Author-email: "Ian M. Thornton" <iot5037@psu.edu>
 Project-URL: Repository, https://github.com/villrv/extrabol
 Project-URL: Documentation, https://extrabol.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extrabol-1.0.1/README.md` & `extrabol-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.1/extrabol/extrabol.py` & `extrabol-1.0.2/extrabol/extrabol.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from astropy.io import ascii
 import matplotlib.cm as cm
 import sys
 from scipy import interpolate as interp
 from george.modeling import Model
 import extinction
 import emcee
-import pkg_resources
+import importlib_resources
 
 # Define a few important constants that will be used later
 epsilon = 0.001
 c = 2.99792458E10  # cm / s
 sigsb = 5.6704e-5  # erg / cm^2 / s / K^4
 h = 6.62607E-27
 ang_to_cm = 1e-8
@@ -915,19 +915,16 @@
     ascii.write(table, outdir + snname + '_' + str(sn_type) + '.txt',
                 formats=format_dict, overwrite=True)
 
     return 1
 
 
 def main():
-
-    default_data = pkg_resources.resource_filename(
-                   'extrabol.example', 'SN2010bc.dat'
-                   )
-
+    default_data = importlib_resources.files('extrabol.example') / 'SN2010bc.dat'
+    default_data = str(default_data)
     # Define all arguments
     parser = argparse.ArgumentParser(description='extrabol helpers')
     parser.add_argument('snfile', nargs='?',
                         default=default_data,
                         type=str, help='Give name of SN file')
     parser.add_argument('-m', '--mean', dest='mean', type=str, default='0',
                         help="Template function for gp.\
```

### Comparing `extrabol-1.0.1/extrabol.egg-info/PKG-INFO` & `extrabol-1.0.2/extrabol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrabol
-Version: 1.0.1
+Version: 1.0.2
 Summary: Estimate SN bolometric light curves
 Author-email: "Ian M. Thornton" <iot5037@psu.edu>
 Project-URL: Repository, https://github.com/villrv/extrabol
 Project-URL: Documentation, https://extrabol.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extrabol-1.0.1/pyproject.toml` & `extrabol-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="extrabol"
-version="1.0.1"
+version="1.0.2"
 readme = "README.md"
 authors = [
     {name = "Ian M. Thornton", email = "iot5037@psu.edu"},
 ]
 description="Estimate SN bolometric light curves"
 dependencies=[
     "numpy",
     "astropy",
     "astroquery",
     "matplotlib",
     "george",
     "extinction",
     "emcee",
     "mkdocs >= 1.2.2",
+    "importlib_resources"
 ]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python='>=3.6'
@@ -32,15 +33,18 @@
 
 [project.urls]
 Repository = "https://github.com/villrv/extrabol"
 Documentation = "https://extrabol.readthedocs.io/en/latest/"
 
 
 [tool.setuptools]
-packages=["extrabol"]
+packages=["extrabol",
+          "extrabol.template_bank",
+          "extrabol.example"
+         ]
 
 [tool.setuptools.package-data]
 "extrabol.example" = ["SN2010bc.dat"]
 "extrabol.template_bank" = ["*.npz"]
```

