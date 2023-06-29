# Comparing `tmp/zope.deferredimport-4.4.tar.gz` & `tmp/zope.deferredimport-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.deferredimport-4.4.tar", last modified: Fri Dec 10 08:16:06 2021, max compression
+gzip compressed data, was "zope.deferredimport-5.0.tar", last modified: Thu Jun 29 06:19:27 2023, max compression
```

## Comparing `zope.deferredimport-4.4.tar` & `zope.deferredimport-5.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.752334 zope.deferredimport-4.4/
--rw-r--r--   0 mac        (513) staff       (20)     1917 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)       32 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      331 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4915 2021-12-10 08:16:06.752614 zope.deferredimport-4.4/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1388 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      191 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.733807 zope.deferredimport-4.4/docs/
--rw-r--r--   0 mac        (513) staff       (20)     6778 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      148 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)     8615 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      210 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     6709 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)     9887 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/docs/narrative.rst
--rw-r--r--   0 mac        (513) staff       (20)      197 2021-12-10 08:16:06.754081 zope.deferredimport-4.4/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3341 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.718744 zope.deferredimport-4.4/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.734604 zope.deferredimport-4.4/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.744991 zope.deferredimport-4.4/src/zope/deferredimport/
--rw-r--r--   0 mac        (513) staff       (20)      304 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     5519 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/deferredmodule.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.751747 zope.deferredimport-4.4/src/zope/deferredimport/samples/
--rw-r--r--   0 mac        (513) staff       (20)       18 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       70 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample1.py
--rw-r--r--   0 mac        (513) staff       (20)      234 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample2.py
--rw-r--r--   0 mac        (513) staff       (20)      298 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample5.py
--rw-r--r--   0 mac        (513) staff       (20)       95 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample6.py
--rw-r--r--   0 mac        (513) staff       (20)      254 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample7.py
--rw-r--r--   0 mac        (513) staff       (20)      245 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample8.py
--rw-r--r--   0 mac        (513) staff       (20)       52 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/samples/sample9.py
--rw-r--r--   0 mac        (513) staff       (20)     2470 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/src/zope/deferredimport/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-10 08:16:06.742666 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4915 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1001 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       89 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2021-12-10 08:16:06.000000 zope.deferredimport-4.4/src/zope.deferredimport.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1655 2021-12-10 08:16:04.000000 zope.deferredimport-4.4/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.390509 zope.deferredimport-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2027 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      344 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4860 2023-06-29 06:19:27.390567 zope.deferredimport-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1430 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      191 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.387765 zope.deferredimport-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6778 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      148 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8615 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      210 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6709 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9887 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/docs/narrative.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-06-29 06:19:27.390802 zope.deferredimport-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3183 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.385412 zope.deferredimport-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.387895 zope.deferredimport-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.389252 zope.deferredimport-5.0/src/zope/deferredimport/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      396 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5441 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/deferredmodule.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.390365 zope.deferredimport-5.0/src/zope/deferredimport/samples/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       70 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      235 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample2.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      301 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample5.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       95 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample6.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      256 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample7.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      246 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample8.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       52 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/samples/sample9.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2470 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope/deferredimport/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:19:27.388842 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4860 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1017 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       89 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/src/zope.deferredimport.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1832 2023-06-29 06:19:27.000000 zope.deferredimport-5.0/tox.ini
```

### Comparing `zope.deferredimport-4.4/CHANGES.rst` & `zope.deferredimport-5.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2021-12-10)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.deferredimport-4.4/LICENSE.txt` & `zope.deferredimport-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.deferredimport-4.4/PKG-INFO` & `zope.deferredimport-5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.deferredimport
-Version: 4.4
+Version: 5.0
 Summary: zope.deferredimport allows you to perform imports names that will only be resolved when used in the code.
 Home-page: http://github.com/zopefoundation/zope.deferredimport
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.deferredimport/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.deferredimport
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =========================
  ``zope.deferredimport``
 =========================
@@ -41,16 +37,16 @@
         :target: https://pypi.python.org/pypi/zope.deferredimport/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.deferredimport.svg
         :target: https://pypi.org/project/zope.deferredimport/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/zope.deferredimport.svg?branch=master
-        :target: https://travis-ci.com/zopefoundation/zope.deferredimport
+.. image:: https://github.com/zopefoundation/zope.deferredimport/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.deferredimport/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.deferredimport/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.deferredimport?branch=master
 
 .. image:: https://readthedocs.org/projects/zopedeferredimport/badge/?version=latest
         :target: http://zopedeferredimport.readthedocs.io/en/latest/
         :alt: Documentation Status
@@ -65,14 +61,22 @@
 Documentation is hosted at https://zopedeferredimport.readthedocs.io/
 
 
 =========
  Changes
 =========
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2021-12-10)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -163,9 +167,7 @@
 
 
 3.4.0b1 (2007-07-09)
 ====================
 
 - Initial release as a separate project, corresponding to the
   ``zope.deferredimport`` from Zope 3.4.0b1.
-
-
```

### Comparing `zope.deferredimport-4.4/README.rst` & `zope.deferredimport-5.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,16 @@
         :target: https://pypi.python.org/pypi/zope.deferredimport/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.deferredimport.svg
         :target: https://pypi.org/project/zope.deferredimport/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/zope.deferredimport.svg?branch=master
-        :target: https://travis-ci.com/zopefoundation/zope.deferredimport
+.. image:: https://github.com/zopefoundation/zope.deferredimport/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.deferredimport/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.deferredimport/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.deferredimport?branch=master
 
 .. image:: https://readthedocs.org/projects/zopedeferredimport/badge/?version=latest
         :target: http://zopedeferredimport.readthedocs.io/en/latest/
         :alt: Documentation Status
```

### Comparing `zope.deferredimport-4.4/docs/Makefile` & `zope.deferredimport-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.deferredimport-4.4/docs/conf.py` & `zope.deferredimport-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.deferredimport-4.4/docs/make.bat` & `zope.deferredimport-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.deferredimport-4.4/docs/narrative.rst` & `zope.deferredimport-5.0/docs/narrative.rst`

 * *Files identical despite different names*

### Comparing `zope.deferredimport-4.4/setup.py` & `zope.deferredimport-5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.deferredimport package
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -34,57 +36,54 @@
 DOCS_REQUIRE = [
     'Sphinx',
     'repoze.sphinx.autointerface',
 ]
 
 setup(
     name='zope.deferredimport',
-    version='4.4',
+    version='5.0',
     url='http://github.com/zopefoundation/zope.deferredimport',
     license='ZPL 2.1',
     description=('zope.deferredimport allows you to perform imports names '
                  'that will only be resolved when used in the code.'),
     project_urls={
         'Issue Tracker': ('https://github.com/zopefoundation/'
                           'zope.deferredimport/issues'),
         'Sources': 'https://github.com/zopefoundation/zope.deferredimport',
     },
 
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
     ),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development',
     ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.proxy',
     ],
     extras_require={
         'test': TESTS_REQUIRE,
         'docs': DOCS_REQUIRE,
```

### Comparing `zope.deferredimport-4.4/src/zope/deferredimport/deferredmodule.py` & `zope.deferredimport-5.0/src/zope/deferredimport/deferredmodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Modules with defered attributes
 """
 import sys
 import warnings
+
 import zope.proxy
 
 
-class Deferred(object):
+class Deferred:
 
     def __init__(self, name, specifier):
         self.__name__ = name
         self.specifier = specifier
 
     _import_chicken = {}, {}, ['*']
 
@@ -40,30 +41,30 @@
                 v = getattr(v, n)
         return v
 
 
 class DeferredAndDeprecated(Deferred):
 
     def __init__(self, name, specifier, message):
-        super(DeferredAndDeprecated, self).__init__(name, specifier)
+        super().__init__(name, specifier)
         self.message = message
 
     def get(self):
         warnings.warn(
             self.__name__ + " is deprecated. " + self.message,
             DeprecationWarning, stacklevel=3)
 
-        return super(DeferredAndDeprecated, self).get()
+        return super().get()
 
 
 class ModuleProxy(zope.proxy.ProxyBase):
     __slots__ = ('__deferred_definitions__', '__doc__')
 
     def __init__(self, module):
-        super(ModuleProxy, self).__init__(module)
+        super().__init__(module)
         self.__deferred_definitions__ = {}
         self.__doc__ = module.__doc__
 
     def __getattr__(self, name):
         try:
             get = self.__deferred_definitions__[name]
         except KeyError:
```

### Comparing `zope.deferredimport-4.4/src/zope/deferredimport/tests.py` & `zope.deferredimport-5.0/src/zope/deferredimport/tests.py`

 * *Files identical despite different names*

### Comparing `zope.deferredimport-4.4/src/zope.deferredimport.egg-info/PKG-INFO` & `zope.deferredimport-5.0/src/zope.deferredimport.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.deferredimport
-Version: 4.4
+Version: 5.0
 Summary: zope.deferredimport allows you to perform imports names that will only be resolved when used in the code.
 Home-page: http://github.com/zopefoundation/zope.deferredimport
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.deferredimport/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.deferredimport
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =========================
  ``zope.deferredimport``
 =========================
@@ -41,16 +37,16 @@
         :target: https://pypi.python.org/pypi/zope.deferredimport/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.deferredimport.svg
         :target: https://pypi.org/project/zope.deferredimport/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/zope.deferredimport.svg?branch=master
-        :target: https://travis-ci.com/zopefoundation/zope.deferredimport
+.. image:: https://github.com/zopefoundation/zope.deferredimport/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.deferredimport/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.deferredimport/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.deferredimport?branch=master
 
 .. image:: https://readthedocs.org/projects/zopedeferredimport/badge/?version=latest
         :target: http://zopedeferredimport.readthedocs.io/en/latest/
         :alt: Documentation Status
@@ -65,14 +61,22 @@
 Documentation is hosted at https://zopedeferredimport.readthedocs.io/
 
 
 =========
  Changes
 =========
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2021-12-10)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -163,9 +167,7 @@
 
 
 3.4.0b1 (2007-07-09)
 ====================
 
 - Initial release as a separate project, corresponding to the
   ``zope.deferredimport`` from Zope 3.4.0b1.
-
-
```

### Comparing `zope.deferredimport-4.4/src/zope.deferredimport.egg-info/SOURCES.txt` & `zope.deferredimport-5.0/src/zope.deferredimport.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 setup.cfg
 setup.py
```

### Comparing `zope.deferredimport-4.4/tox.ini` & `zope.deferredimport-5.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
-    !py27-!pypy: sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+    sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 commands_pre =
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
@@ -49,25 +57,23 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
-    coverage html
-    coverage report -m --fail-under=100
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.deferredimport
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

