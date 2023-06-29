# Comparing `tmp/zope.principalannotation-4.4.tar.gz` & `tmp/zope.principalannotation-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.principalannotation-4.4.tar", last modified: Thu Mar 17 07:01:06 2022, max compression
+gzip compressed data, was "zope.principalannotation-5.0.tar", last modified: Thu Jun 29 06:21:34 2023, max compression
```

## Comparing `zope.principalannotation-4.4.tar` & `zope.principalannotation-5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-17 07:01:06.891395 zope.principalannotation-4.4/
--rw-r--r--   0 mac        (513) staff       (20)     1740 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      372 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4473 2022-03-17 07:01:06.891520 zope.principalannotation-4.4/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1333 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      582 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-17 07:01:06.885920 zope.principalannotation-4.4/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      186 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    11064 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      491 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       56 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs/narr.rst
--rw-r--r--   0 mac        (513) staff       (20)        8 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/docs-requirements.txt
--rw-r--r--   0 mac        (513) staff       (20)      174 2022-03-17 07:01:06.892103 zope.principalannotation-4.4/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3098 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-17 07:01:06.879506 zope.principalannotation-4.4/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-17 07:01:06.886387 zope.principalannotation-4.4/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)      200 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-17 07:01:06.891152 zope.principalannotation-4.4/src/zope/principalannotation/
--rw-r--r--   0 mac        (513) staff       (20)     6764 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/principalannotation/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       16 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/principalannotation/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      673 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/principalannotation/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1526 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/principalannotation/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1216 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/principalannotation/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     4802 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/src/zope/principalannotation/utility.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-17 07:01:06.889013 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4473 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      864 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      259 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-03-17 07:01:06.000000 zope.principalannotation-4.4/src/zope.principalannotation.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1396 2022-03-17 07:01:05.000000 zope.principalannotation-4.4/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:21:34.139891 zope.principalannotation-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1907 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      372 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4528 2023-06-29 06:21:34.140104 zope.principalannotation-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1365 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      582 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:21:34.136100 zope.principalannotation-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      186 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11064 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      491 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs/narr.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)        8 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/docs-requirements.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      447 2023-06-29 06:21:34.140614 zope.principalannotation-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2913 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:21:34.133193 zope.principalannotation-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:21:34.136274 zope.principalannotation-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:21:34.139343 zope.principalannotation-5.0/src/zope/principalannotation/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6764 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/principalannotation/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       16 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/principalannotation/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      673 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/principalannotation/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1526 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/principalannotation/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1243 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/principalannotation/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4819 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/src/zope/principalannotation/utility.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:21:34.138118 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4528 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      864 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      259 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:21:34.000000 zope.principalannotation-5.0/src/zope.principalannotation.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1586 2023-06-29 06:21:33.000000 zope.principalannotation-5.0/tox.ini
```

### Comparing `zope.principalannotation-4.4/CHANGES.rst` & `zope.principalannotation-5.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
  Changes
 =========
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-03-17)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.principalannotation-4.4/CONTRIBUTING.md` & `zope.principalannotation-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/LICENSE.txt` & `zope.principalannotation-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/PKG-INFO` & `zope.principalannotation-5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.principalannotation
-Version: 4.4
+Version: 5.0
 Summary: Annotations for Zope Principals
 Home-page: https://github.com/zopefoundation/zope.principalannotation
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope security principal annotation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
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
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ==============================
  ``zope.principalannotation``
 ==============================
@@ -40,35 +37,45 @@
         :target: https://pypi.python.org/pypi/zope.principalannotation/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.principalannotation.svg
         :target: https://pypi.org/project/zope.principalannotation/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/zope.principalannotation.svg?branch=master
-        :target: https://travis-ci.com/zopefoundation/zope.principalannotation
+.. image:: https://github.com/zopefoundation/zope.principalannotation/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.principalannotation/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.principalannotation/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.principalannotation?branch=master
 
 .. image:: https://readthedocs.org/projects/zopeprincipalannotation/badge/?version=latest
         :target: https://zopeprincipalannotation.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 This package implements annotations for zope.security principals. Common
 annotation techniques, like ``AttributeAnnotations`` cannot be applied to
 principals, since they are created on the fly for every request.
 
-Documentation is hosted at https://zopeprincipalannotation.readthedocs.io/en/latest/.
+Documentation is hosted at https://zopeprincipalannotation.readthedocs.io/.
 
 
 =========
  Changes
 =========
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-03-17)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -145,9 +152,7 @@
  - The IAnnotations implementation was fixed to look in the higher-level
    utility not only on ``__getitem__``, but also on ``get`` and ``__nonzero``.
 
  - Tests was reworked into the README.txt doctest.
 
  - Added a buildout part that generates Sphinx documentation from the
    README.txt
-
-
```

### Comparing `zope.principalannotation-4.4/README.rst` & `zope.principalannotation-5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         :target: https://pypi.python.org/pypi/zope.principalannotation/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.principalannotation.svg
         :target: https://pypi.org/project/zope.principalannotation/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/zope.principalannotation.svg?branch=master
-        :target: https://travis-ci.com/zopefoundation/zope.principalannotation
+.. image:: https://github.com/zopefoundation/zope.principalannotation/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.principalannotation/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.principalannotation/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.principalannotation?branch=master
 
 .. image:: https://readthedocs.org/projects/zopeprincipalannotation/badge/?version=latest
         :target: https://zopeprincipalannotation.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 This package implements annotations for zope.security principals. Common
 annotation techniques, like ``AttributeAnnotations`` cannot be applied to
 principals, since they are created on the fly for every request.
 
-Documentation is hosted at https://zopeprincipalannotation.readthedocs.io/en/latest/.
+Documentation is hosted at https://zopeprincipalannotation.readthedocs.io/.
```

### Comparing `zope.principalannotation-4.4/buildout.cfg` & `zope.principalannotation-5.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/docs/Makefile` & `zope.principalannotation-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/docs/conf.py` & `zope.principalannotation-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/setup.py` & `zope.principalannotation-5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Setup for zope.principalannotation package
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -27,51 +29,49 @@
     'zope.testing',
     'zope.site[test]',
     'zope.testrunner',
 ]
 
 setup(
     name='zope.principalannotation',
-    version='4.4',
+    version='5.0',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     description='Annotations for Zope Principals',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
     ),
     keywords="zope security principal annotation",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
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
         'Framework :: Zope :: 3',
     ],
     url='https://github.com/zopefoundation/zope.principalannotation',
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
+    python_requires='>=3.7',
     extras_require={
         'test': TESTS_REQUIRE,
         'docs': [
             'Sphinx',
             'repoze.sphinx.autointerface',
             'sphinx_rtd_theme',
         ],
@@ -82,12 +82,10 @@
         'zope.annotation',
         'zope.component >= 4.5.0',
         'zope.interface >= 4.5.0',
         'zope.location',
         'zope.security',
         'zope.site',
     ],
-    tests_require=TESTS_REQUIRE,
-    test_suite='zope.principalannotation.tests.test_suite',
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `zope.principalannotation-4.4/src/zope/principalannotation/README.rst` & `zope.principalannotation-5.0/src/zope/principalannotation/README.rst`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/src/zope/principalannotation/configure.zcml` & `zope.principalannotation-5.0/src/zope/principalannotation/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/src/zope/principalannotation/interfaces.py` & `zope.principalannotation-5.0/src/zope/principalannotation/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/src/zope/principalannotation/tests.py` & `zope.principalannotation-5.0/src/zope/principalannotation/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 #
 ##############################################################################
 """Principal Annotation Tests
 """
 import doctest
 import unittest
 
-from zope.site.testing import siteSetUp, siteTearDown
 from zope.configuration import xmlconfig
+from zope.site.testing import siteSetUp
+from zope.site.testing import siteTearDown
 
 import zope.principalannotation
 
 
 def setUp(test):
     site = siteSetUp(site=True)
     test.globs['root'] = site
@@ -29,13 +30,13 @@
 
 
 def tearDown(test):
     siteTearDown()
 
 
 def test_suite():
-    return unittest.TestSuite((
+    return unittest.TestSuite(
         doctest.DocFileSuite(
             'README.rst',
             setUp=setUp, tearDown=tearDown,
             optionflags=doctest.ELLIPSIS)
-    ))
+    )
```

### Comparing `zope.principalannotation-4.4/src/zope/principalannotation/utility.py` & `zope.principalannotation-5.0/src/zope/principalannotation/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 ##############################################################################
 """Implementation of IPrincipalAnnotationUtility
 """
 __docformat__ = 'restructuredtext'
 from BTrees.OOBTree import OOBTree
 from persistent import Persistent
 from persistent.dict import PersistentDict
-from zope import interface, component
 from zope.annotation.interfaces import IAnnotations
+from zope.component import queryNextUtility
 from zope.location import Location
 from zope.location.interfaces import IContained
 from zope.security.interfaces import IPrincipal
-from zope.component import queryNextUtility
 
+from zope import component
+from zope import interface
 from zope.principalannotation.interfaces import IPrincipalAnnotationUtility
 
+
 # TODO: register utility as adapter for IAnnotations on utility activation.
 
 
 @interface.implementer(IPrincipalAnnotationUtility, IContained)
 class PrincipalAnnotationUtility(Persistent):
     """
     Stores :class:`zope.annotation.interfaces.IAnnotations` for
```

### Comparing `zope.principalannotation-4.4/src/zope.principalannotation.egg-info/PKG-INFO` & `zope.principalannotation-5.0/src/zope.principalannotation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.principalannotation
-Version: 4.4
+Version: 5.0
 Summary: Annotations for Zope Principals
 Home-page: https://github.com/zopefoundation/zope.principalannotation
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope security principal annotation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
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
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ==============================
  ``zope.principalannotation``
 ==============================
@@ -40,35 +37,45 @@
         :target: https://pypi.python.org/pypi/zope.principalannotation/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.principalannotation.svg
         :target: https://pypi.org/project/zope.principalannotation/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/zope.principalannotation.svg?branch=master
-        :target: https://travis-ci.com/zopefoundation/zope.principalannotation
+.. image:: https://github.com/zopefoundation/zope.principalannotation/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.principalannotation/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.principalannotation/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.principalannotation?branch=master
 
 .. image:: https://readthedocs.org/projects/zopeprincipalannotation/badge/?version=latest
         :target: https://zopeprincipalannotation.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 This package implements annotations for zope.security principals. Common
 annotation techniques, like ``AttributeAnnotations`` cannot be applied to
 principals, since they are created on the fly for every request.
 
-Documentation is hosted at https://zopeprincipalannotation.readthedocs.io/en/latest/.
+Documentation is hosted at https://zopeprincipalannotation.readthedocs.io/.
 
 
 =========
  Changes
 =========
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-03-17)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -145,9 +152,7 @@
  - The IAnnotations implementation was fixed to look in the higher-level
    utility not only on ``__getitem__``, but also on ``get`` and ``__nonzero``.
 
  - Tests was reworked into the README.txt doctest.
 
  - Added a buildout part that generates Sphinx documentation from the
    README.txt
-
-
```

### Comparing `zope.principalannotation-4.4/src/zope.principalannotation.egg-info/SOURCES.txt` & `zope.principalannotation-5.0/src/zope.principalannotation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.principalannotation-4.4/tox.ini` & `zope.principalannotation-5.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
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
@@ -23,23 +20,34 @@
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
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
 extras =
     docs
 commands_pre =
@@ -48,24 +56,22 @@
 
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
-    coverage html
-    coverage report -m --fail-under=100
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.principalannotation
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

