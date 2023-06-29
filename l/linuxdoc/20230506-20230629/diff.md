# Comparing `tmp/linuxdoc-20230506.tar.gz` & `tmp/linuxdoc-20230629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxdoc-20230506.tar", last modified: Sat May  6 08:55:08 2023, max compression
+gzip compressed data, was "linuxdoc-20230629.tar", last modified: Thu Jun 29 20:10:30 2023, max compression
```

## Comparing `linuxdoc-20230506.tar` & `linuxdoc-20230629.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/
--rw-rw-r--   0 markus    (1001) markus    (1001)    34520 2023-03-25 08:10:56.000000 linuxdoc-20230506/LICENSE
--rw-rw-r--   0 markus    (1001) markus    (1001)     2211 2023-05-06 08:55:08.801174 linuxdoc-20230506/PKG-INFO
--rw-rw-r--   0 markus    (1001) markus    (1001)     1002 2023-05-06 08:50:39.000000 linuxdoc-20230506/README.rst
-drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/linuxdoc/
--rw-rw-r--   0 markus    (1001) markus    (1001)      777 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/__init__.py
--rw-rw-r--   0 markus    (1001) markus    (1001)     5829 2023-05-06 08:39:00.000000 linuxdoc-20230506/linuxdoc/__pkginfo__.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)     7200 2023-03-26 12:51:46.000000 linuxdoc-20230506/linuxdoc/autodoc.py
--rw-rw-r--   0 markus    (1001) markus    (1001)      560 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/cdomain.py
--rw-rw-r--   0 markus    (1001) markus    (1001)     5085 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/cdomainv2.py
--rw-rw-r--   0 markus    (1001) markus    (1001)      754 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/cdomainv3.py
--rw-rw-r--   0 markus    (1001) markus    (1001)     1734 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/compat.py
--rw-rw-r--   0 markus    (1001) markus    (1001)     1701 2023-05-06 08:23:40.000000 linuxdoc-20230506/linuxdoc/deprecated.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)     2016 2023-03-26 12:51:46.000000 linuxdoc-20230506/linuxdoc/grepdoc.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)   110357 2023-05-06 07:53:06.000000 linuxdoc-20230506/linuxdoc/kernel_doc.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)     7949 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/kernel_include.py
--rw-rw-r--   0 markus    (1001) markus    (1001)    17224 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/kfigure.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)     3321 2023-03-26 12:51:46.000000 linuxdoc-20230506/linuxdoc/lint.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)    13347 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/manKernelDoc.py
--rw-rw-r--   0 markus    (1001) markus    (1001)     6418 2023-05-06 07:47:06.000000 linuxdoc-20230506/linuxdoc/rest.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)    12757 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/rstFlatTable.py
--rwxrwxr-x   0 markus    (1001) markus    (1001)    18769 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/rstKernelDoc.py
-drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/linuxdoc.egg-info/
--rw-rw-r--   0 markus    (1001) markus    (1001)     2211 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1001) markus    (1001)      619 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1001) markus    (1001)        1 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1001) markus    (1001)      389 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/entry_points.txt
--rw-rw-r--   0 markus    (1001) markus    (1001)       34 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/requires.txt
--rw-rw-r--   0 markus    (1001) markus    (1001)       15 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1001) markus    (1001)       61 2023-05-06 08:55:08.805174 linuxdoc-20230506/setup.cfg
--rwxrwxr-x   0 markus    (1001) markus    (1001)     1191 2023-05-06 08:15:34.000000 linuxdoc-20230506/setup.py
-drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/tests/
--rwxrwxr-x   0 markus    (1001) markus    (1001)      392 2023-03-25 08:10:56.000000 linuxdoc-20230506/tests/__init__.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-06-29 20:10:30.695704 linuxdoc-20230629/
+-rw-rw-r--   0 markus    (1001) markus    (1001)    34520 2023-03-25 08:10:56.000000 linuxdoc-20230629/LICENSE
+-rw-rw-r--   0 markus    (1001) markus    (1001)     2211 2023-06-29 20:10:30.695704 linuxdoc-20230629/PKG-INFO
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1002 2023-06-29 19:59:04.000000 linuxdoc-20230629/README.rst
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-06-29 20:10:30.695704 linuxdoc-20230629/linuxdoc/
+-rw-rw-r--   0 markus    (1001) markus    (1001)      777 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/__init__.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     5829 2023-06-29 19:58:55.000000 linuxdoc-20230629/linuxdoc/__pkginfo__.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     7200 2023-03-26 12:51:46.000000 linuxdoc-20230629/linuxdoc/autodoc.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)      560 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/cdomain.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     5085 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/cdomainv2.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)      754 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/cdomainv3.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1734 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/compat.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1701 2023-05-06 08:23:40.000000 linuxdoc-20230629/linuxdoc/deprecated.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     2016 2023-03-26 12:51:46.000000 linuxdoc-20230629/linuxdoc/grepdoc.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)   110357 2023-05-06 07:53:06.000000 linuxdoc-20230629/linuxdoc/kernel_doc.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     7949 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/kernel_include.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)    17224 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/kfigure.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     3321 2023-03-26 12:51:46.000000 linuxdoc-20230629/linuxdoc/lint.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    13347 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/manKernelDoc.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     6418 2023-05-06 07:47:06.000000 linuxdoc-20230629/linuxdoc/rest.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    12757 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/rstFlatTable.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    18769 2023-03-25 08:10:56.000000 linuxdoc-20230629/linuxdoc/rstKernelDoc.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-06-29 20:10:30.695704 linuxdoc-20230629/linuxdoc.egg-info/
+-rw-rw-r--   0 markus    (1001) markus    (1001)     2211 2023-06-29 20:10:30.000000 linuxdoc-20230629/linuxdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1001) markus    (1001)      619 2023-06-29 20:10:30.000000 linuxdoc-20230629/linuxdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)        1 2023-06-29 20:10:30.000000 linuxdoc-20230629/linuxdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)      389 2023-06-29 20:10:30.000000 linuxdoc-20230629/linuxdoc.egg-info/entry_points.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       34 2023-06-29 20:10:30.000000 linuxdoc-20230629/linuxdoc.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       15 2023-06-29 20:10:30.000000 linuxdoc-20230629/linuxdoc.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       61 2023-06-29 20:10:30.695704 linuxdoc-20230629/setup.cfg
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     1542 2023-06-29 17:39:37.000000 linuxdoc-20230629/setup.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-06-29 20:10:30.695704 linuxdoc-20230629/tests/
+-rwxrwxr-x   0 markus    (1001) markus    (1001)      392 2023-03-25 08:10:56.000000 linuxdoc-20230629/tests/__init__.py
```

### Comparing `linuxdoc-20230506/LICENSE` & `linuxdoc-20230629/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/PKG-INFO` & `linuxdoc-20230629/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxdoc
-Version: 20230506
+Version: 20230629
 Summary: Sphinx-doc extensions & tools to extract documentation from C/C++ source file comments.
 Home-page: https://github.com/return42/linuxdoc
 Author: Markus Heiser
 Author-email: markus.heiser@darmarIT.de
 License: AGPLv3+
 Project-URL: Documentation, https://return42.github.io/linuxdoc
 Project-URL: Code, https://github.com/return42/linuxdoc
@@ -51,13 +51,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20230506)
+package:     linuxdoc (20230629)
 copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20230506/README.rst` & `linuxdoc-20230629/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20230506)
+package:     linuxdoc (20230629)
 copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20230506/linuxdoc/__init__.py` & `linuxdoc-20230629/linuxdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/__pkginfo__.py` & `linuxdoc-20230629/linuxdoc/__pkginfo__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=line-too-long, invalid-name, consider-using-f-string
 """Python package meta informations used by setup.py and other project files.
 """
 
 from setuptools import find_packages
 
 package = 'linuxdoc'
-version = '20230506'
+version = '20230629'
 
 copyright = '2023 Markus Heiser'  # pylint: disable=redefined-builtin
 description = (
     'Sphinx-doc extensions & tools to extract documentation'
     ' from C/C++ source file comments.'
 )
 license   = 'AGPLv3+'  # pylint: disable=redefined-builtin
```

### Comparing `linuxdoc-20230506/linuxdoc/autodoc.py` & `linuxdoc-20230629/linuxdoc/autodoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/cdomain.py` & `linuxdoc-20230629/linuxdoc/cdomain.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/cdomainv2.py` & `linuxdoc-20230629/linuxdoc/cdomainv2.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/cdomainv3.py` & `linuxdoc-20230629/linuxdoc/cdomainv3.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/compat.py` & `linuxdoc-20230629/linuxdoc/compat.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/deprecated.py` & `linuxdoc-20230629/linuxdoc/deprecated.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/grepdoc.py` & `linuxdoc-20230629/linuxdoc/grepdoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/kernel_doc.py` & `linuxdoc-20230629/linuxdoc/kernel_doc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/kernel_include.py` & `linuxdoc-20230629/linuxdoc/kernel_include.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/kfigure.py` & `linuxdoc-20230629/linuxdoc/kfigure.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/lint.py` & `linuxdoc-20230629/linuxdoc/lint.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/manKernelDoc.py` & `linuxdoc-20230629/linuxdoc/manKernelDoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/rest.py` & `linuxdoc-20230629/linuxdoc/rest.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/rstFlatTable.py` & `linuxdoc-20230629/linuxdoc/rstFlatTable.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc/rstKernelDoc.py` & `linuxdoc-20230629/linuxdoc/rstKernelDoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230506/linuxdoc.egg-info/PKG-INFO` & `linuxdoc-20230629/linuxdoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxdoc
-Version: 20230506
+Version: 20230629
 Summary: Sphinx-doc extensions & tools to extract documentation from C/C++ source file comments.
 Home-page: https://github.com/return42/linuxdoc
 Author: Markus Heiser
 Author-email: markus.heiser@darmarIT.de
 License: AGPLv3+
 Project-URL: Documentation, https://return42.github.io/linuxdoc
 Project-URL: Code, https://github.com/return42/linuxdoc
@@ -51,13 +51,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20230506)
+package:     linuxdoc (20230629)
 copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20230506/linuxdoc.egg-info/SOURCES.txt` & `linuxdoc-20230629/linuxdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

