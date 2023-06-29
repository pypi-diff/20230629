# Comparing `tmp/nettoolkit-0.0.8.tar.gz` & `tmp/nettoolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettoolkit-0.0.8.tar", last modified: Sun Jul  4 13:02:37 2021, max compression
+gzip compressed data, was "nettoolkit-0.0.9.tar", last modified: Tue Jul  6 03:55:38 2021, max compression
```

## Comparing `nettoolkit-0.0.8.tar` & `nettoolkit-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-07-04 13:02:37.932687 nettoolkit-0.0.8/
--rw-rw-rw-   0        0        0     1091 2021-05-28 08:00:18.000000 nettoolkit-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1789 2021-07-04 13:02:37.932687 nettoolkit-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1301 2021-05-28 08:00:18.000000 nettoolkit-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-07-04 13:02:37.848037 nettoolkit-0.0.8/nettoolkit/
--rw-rw-rw-   0        0        0     2116 2021-07-04 12:52:06.000000 nettoolkit-0.0.8/nettoolkit/__init__.py
--rw-rw-rw-   0        0        0    28203 2021-05-31 03:56:22.000000 nettoolkit-0.0.8/nettoolkit/addressing.py
--rw-rw-rw-   0        0        0     3869 2021-07-04 12:50:22.000000 nettoolkit-0.0.8/nettoolkit/convertdict.py
--rw-rw-rw-   0        0        0    37348 2021-07-03 12:06:27.000000 nettoolkit-0.0.8/nettoolkit/gpl.py
--rw-rw-rw-   0        0        0    15330 2021-05-31 03:55:03.000000 nettoolkit-0.0.8/nettoolkit/hierarchy.py
--rw-rw-rw-   0        0        0     3917 2021-05-28 08:00:18.000000 nettoolkit-0.0.8/nettoolkit/hierarchy_rules.py
--rw-rw-rw-   0        0        0     3587 2021-05-30 04:58:38.000000 nettoolkit-0.0.8/nettoolkit/jset.py
--rw-rw-rw-   0        0        0     1476 2021-05-28 08:00:18.000000 nettoolkit-0.0.8/nettoolkit/juniper.py
-drwxrwxrwx   0        0        0        0 2021-07-04 13:02:37.932687 nettoolkit-0.0.8/nettoolkit.egg-info/
--rw-rw-rw-   0        0        0     1789 2021-07-04 13:02:37.000000 nettoolkit-0.0.8/nettoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2021-07-04 13:02:37.000000 nettoolkit-0.0.8/nettoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-04 13:02:37.000000 nettoolkit-0.0.8/nettoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2021-07-04 13:02:37.000000 nettoolkit-0.0.8/nettoolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-07-04 13:02:37.000000 nettoolkit-0.0.8/nettoolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-04 13:02:37.932687 nettoolkit-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      726 2021-05-31 03:58:46.000000 nettoolkit-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-06 03:55:38.637432 nettoolkit-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2021-05-28 08:00:18.000000 nettoolkit-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1789 2021-07-06 03:55:38.621809 nettoolkit-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1301 2021-05-28 08:00:18.000000 nettoolkit-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-07-06 03:55:38.543684 nettoolkit-0.0.9/nettoolkit/
+-rw-rw-rw-   0        0        0     2116 2021-07-04 13:06:20.000000 nettoolkit-0.0.9/nettoolkit/__init__.py
+-rw-rw-rw-   0        0        0    28203 2021-05-31 03:56:22.000000 nettoolkit-0.0.9/nettoolkit/addressing.py
+-rw-rw-rw-   0        0        0     6283 2021-07-06 03:44:24.000000 nettoolkit-0.0.9/nettoolkit/convertdict.py
+-rw-rw-rw-   0        0        0    37348 2021-07-03 12:06:27.000000 nettoolkit-0.0.9/nettoolkit/gpl.py
+-rw-rw-rw-   0        0        0    15330 2021-05-31 03:55:03.000000 nettoolkit-0.0.9/nettoolkit/hierarchy.py
+-rw-rw-rw-   0        0        0     3917 2021-05-28 08:00:18.000000 nettoolkit-0.0.9/nettoolkit/hierarchy_rules.py
+-rw-rw-rw-   0        0        0     3587 2021-05-30 04:58:38.000000 nettoolkit-0.0.9/nettoolkit/jset.py
+-rw-rw-rw-   0        0        0     1476 2021-05-28 08:00:18.000000 nettoolkit-0.0.9/nettoolkit/juniper.py
+drwxrwxrwx   0        0        0        0 2021-07-06 03:55:38.621809 nettoolkit-0.0.9/nettoolkit.egg-info/
+-rw-rw-rw-   0        0        0     1789 2021-07-06 03:55:38.000000 nettoolkit-0.0.9/nettoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2021-07-06 03:55:38.000000 nettoolkit-0.0.9/nettoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-06 03:55:38.000000 nettoolkit-0.0.9/nettoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2021-07-06 03:55:38.000000 nettoolkit-0.0.9/nettoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2021-07-06 03:55:38.000000 nettoolkit-0.0.9/nettoolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-06 03:55:38.637432 nettoolkit-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      726 2021-07-04 13:06:13.000000 nettoolkit-0.0.9/setup.py
```

### Comparing `nettoolkit-0.0.8/LICENSE` & `nettoolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/PKG-INFO` & `nettoolkit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettoolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool Set for Networking Geeks
 Home-page: https://github.com/alias1978/nettoolkit
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nettoolkit-0.0.8/README.md` & `nettoolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit/__init__.py` & `nettoolkit-0.0.9/nettoolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	'Default', 'Container', 'Numeric', 'DifferenceDict', 
 	'STR', 'IO', 'LST', 'DIC', 'LOG', 'DB', 'IP', 'XL_READ', 'XL_WRITE', 
 	'DictMethods', 'Multi_Execution',
 	# .convertdict
 	'ConvDict',
 	]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from .juniper import Juniper
 from .jset import JSet
 
 from .addressing import (
 	IPv4, IPv6, addressing, Validation, get_summaries, isSubset,
 	binsubnet, bin2dec, bin2decmask, to_dec_mask, bin_mask,
```

### Comparing `nettoolkit-0.0.8/nettoolkit/addressing.py` & `nettoolkit-0.0.9/nettoolkit/addressing.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit/gpl.py` & `nettoolkit-0.0.9/nettoolkit/gpl.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit/hierarchy.py` & `nettoolkit-0.0.9/nettoolkit/hierarchy.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit/hierarchy_rules.py` & `nettoolkit-0.0.9/nettoolkit/hierarchy_rules.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit/jset.py` & `nettoolkit-0.0.9/nettoolkit/jset.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit/juniper.py` & `nettoolkit-0.0.9/nettoolkit/juniper.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-0.0.8/nettoolkit.egg-info/PKG-INFO` & `nettoolkit-0.0.9/nettoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettoolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool Set for Networking Geeks
 Home-page: https://github.com/alias1978/nettoolkit
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nettoolkit-0.0.8/setup.py` & `nettoolkit-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nettoolkit",
-    version="0.0.8",
+    version="0.0.9",
     author="ALIASGAR - ALI",
     author_email="aholo2000@gmail.com",
     description="Tool Set for Networking Geeks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alias1978/nettoolkit",
     packages=setuptools.find_packages(),
```

