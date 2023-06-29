# Comparing `tmp/extrabol-1.0.2.tar.gz` & `tmp/extrabol-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrabol-1.0.2.tar", last modified: Thu Jun 29 19:51:07 2023, max compression
+gzip compressed data, was "extrabol-1.0.3.tar", last modified: Thu Jun 29 20:57:49 2023, max compression
```

## Comparing `extrabol-1.0.2.tar` & `extrabol-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.363808 extrabol-1.0.2/
--rw-r--r--   0 ian       (1000) ian       (1000)     1058 2023-06-29 19:50:56.000000 extrabol-1.0.2/LICENSE
--rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 19:51:07.363808 extrabol-1.0.2/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)     3411 2023-06-29 19:50:56.000000 extrabol-1.0.2/README.md
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.353808 extrabol-1.0.2/extrabol/
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/__init__.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.353808 extrabol-1.0.2/extrabol/example/
--rw-r--r--   0 ian       (1000) ian       (1000)    17503 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/example/SN2010bc.dat
--rw-r--r--   0 ian       (1000) ian       (1000)    36965 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/extrabol.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.363808 extrabol-1.0.2/extrabol/template_bank/
--rw-r--r--   0 ian       (1000) ian       (1000)  5244546 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn1a.npz
--rw-r--r--   0 ian       (1000) ian       (1000)  4956426 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn1bc.npz
--rw-r--r--   0 ian       (1000) ian       (1000)   692250 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn2l.npz
--rw-r--r--   0 ian       (1000) ian       (1000)   692250 2023-06-29 19:50:56.000000 extrabol-1.0.2/extrabol/template_bank/smoothed_sn2p.npz
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 19:51:07.353808 extrabol-1.0.2/extrabol.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)      463 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       52 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       94 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-06-29 19:51:07.000000 extrabol-1.0.2/extrabol.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)     1030 2023-06-29 19:50:56.000000 extrabol-1.0.2/pyproject.toml
--rw-r--r--   0 ian       (1000) ian       (1000)       38 2023-06-29 19:51:07.363808 extrabol-1.0.2/setup.cfg
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 20:57:49.639466 extrabol-1.0.3/
+-rw-r--r--   0 ian       (1000) ian       (1000)     1058 2023-06-29 20:57:38.000000 extrabol-1.0.3/LICENSE
+-rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 20:57:49.639466 extrabol-1.0.3/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)     3411 2023-06-29 20:57:38.000000 extrabol-1.0.3/README.md
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 20:57:49.619466 extrabol-1.0.3/extrabol/
+-rw-r--r--   0 ian       (1000) ian       (1000)        0 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/__init__.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 20:57:49.629466 extrabol-1.0.3/extrabol/example/
+-rw-r--r--   0 ian       (1000) ian       (1000)    17503 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/example/SN2010bc.dat
+-rw-r--r--   0 ian       (1000) ian       (1000)    36893 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/extrabol.py
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 20:57:49.639466 extrabol-1.0.3/extrabol/template_bank/
+-rw-r--r--   0 ian       (1000) ian       (1000)  5244546 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/template_bank/smoothed_sn1a.npz
+-rw-r--r--   0 ian       (1000) ian       (1000)  4956426 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/template_bank/smoothed_sn1bc.npz
+-rw-r--r--   0 ian       (1000) ian       (1000)   692250 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/template_bank/smoothed_sn2l.npz
+-rw-r--r--   0 ian       (1000) ian       (1000)   692250 2023-06-29 20:57:38.000000 extrabol-1.0.3/extrabol/template_bank/smoothed_sn2p.npz
+drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-06-29 20:57:49.619466 extrabol-1.0.3/extrabol.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3921 2023-06-29 20:57:49.000000 extrabol-1.0.3/extrabol.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)      463 2023-06-29 20:57:49.000000 extrabol-1.0.3/extrabol.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-06-29 20:57:49.000000 extrabol-1.0.3/extrabol.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       52 2023-06-29 20:57:49.000000 extrabol-1.0.3/extrabol.egg-info/entry_points.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)       94 2023-06-29 20:57:49.000000 extrabol-1.0.3/extrabol.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-06-29 20:57:49.000000 extrabol-1.0.3/extrabol.egg-info/top_level.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)     1030 2023-06-29 20:57:38.000000 extrabol-1.0.3/pyproject.toml
+-rw-r--r--   0 ian       (1000) ian       (1000)       38 2023-06-29 20:57:49.639466 extrabol-1.0.3/setup.cfg
```

### Comparing `extrabol-1.0.2/LICENSE` & `extrabol-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/PKG-INFO` & `extrabol-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrabol
-Version: 1.0.2
+Version: 1.0.3
 Summary: Estimate SN bolometric light curves
 Author-email: "Ian M. Thornton" <iot5037@psu.edu>
 Project-URL: Repository, https://github.com/villrv/extrabol
 Project-URL: Documentation, https://extrabol.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extrabol-1.0.2/README.md` & `extrabol-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/extrabol/example/SN2010bc.dat` & `extrabol-1.0.3/extrabol/example/SN2010bc.dat`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/extrabol/extrabol.py` & `extrabol-1.0.3/extrabol/extrabol.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,18 +239,17 @@
 
     Output
     ------
     temp_interped : RectBivariateSpline object
         interpolated template
     '''
 
-    my_template_file = pkg_resources.resource_filename(
-                       'extrabol.template_bank', 'smoothed_sn' +
-                       sn_type + '.npz'
-                       )
+
+
+    my_template_file = importlib_resources.files('extrabol.template_bank') / ('smoothed_sn' + sn_type + '.npz')
     template = np.load(my_template_file)
     temp_times = template['time']
     temp_wavelength = template['wavelength']
     temp_f_lambda = template['f_lambda']
 
     # The template is too large, so we thin it out
     # First chop off unnecessary ends
```

### Comparing `extrabol-1.0.2/extrabol/template_bank/smoothed_sn1a.npz` & `extrabol-1.0.3/extrabol/template_bank/smoothed_sn1a.npz`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/extrabol/template_bank/smoothed_sn1bc.npz` & `extrabol-1.0.3/extrabol/template_bank/smoothed_sn1bc.npz`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/extrabol/template_bank/smoothed_sn2l.npz` & `extrabol-1.0.3/extrabol/template_bank/smoothed_sn2l.npz`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/extrabol/template_bank/smoothed_sn2p.npz` & `extrabol-1.0.3/extrabol/template_bank/smoothed_sn2p.npz`

 * *Files identical despite different names*

### Comparing `extrabol-1.0.2/extrabol.egg-info/PKG-INFO` & `extrabol-1.0.3/extrabol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrabol
-Version: 1.0.2
+Version: 1.0.3
 Summary: Estimate SN bolometric light curves
 Author-email: "Ian M. Thornton" <iot5037@psu.edu>
 Project-URL: Repository, https://github.com/villrv/extrabol
 Project-URL: Documentation, https://extrabol.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extrabol-1.0.2/pyproject.toml` & `extrabol-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="extrabol"
-version="1.0.2"
+version="1.0.3"
 readme = "README.md"
 authors = [
     {name = "Ian M. Thornton", email = "iot5037@psu.edu"},
 ]
 description="Estimate SN bolometric light curves"
 dependencies=[
     "numpy",
```

