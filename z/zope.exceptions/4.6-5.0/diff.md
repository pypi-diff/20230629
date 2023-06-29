# Comparing `tmp/zope.exceptions-4.6.tar.gz` & `tmp/zope.exceptions-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.exceptions-4.6.tar", last modified: Thu Nov 10 07:28:48 2022, max compression
+gzip compressed data, was "zope.exceptions-5.0.tar", last modified: Thu Jun 29 06:08:19 2023, max compression
```

## Comparing `zope.exceptions-4.6.tar` & `zope.exceptions-5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.155330 zope.exceptions-4.6/
--rw-r--r--   0 mac        (513) staff       (20)     5421 2022-11-10 07:28:46.000000 zope.exceptions-4.6/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-11-10 07:28:46.000000 zope.exceptions-4.6/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-11-10 07:28:46.000000 zope.exceptions-4.6/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-11-10 07:28:46.000000 zope.exceptions-4.6/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      344 2022-11-10 07:28:46.000000 zope.exceptions-4.6/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     8214 2022-11-10 07:28:48.155491 zope.exceptions-4.6/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1175 2022-11-10 07:28:46.000000 zope.exceptions-4.6/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       97 2022-11-10 07:28:46.000000 zope.exceptions-4.6/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.149582 zope.exceptions-4.6/docs/
--rw-r--r--   0 mac        (513) staff       (20)     5596 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)     1166 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)     8197 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     9152 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)      236 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     5112 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)     5970 2022-11-10 07:28:46.000000 zope.exceptions-4.6/docs/narr.rst
--rw-r--r--   0 mac        (513) staff       (20)       43 2022-11-10 07:28:46.000000 zope.exceptions-4.6/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      469 2022-11-10 07:28:48.156146 zope.exceptions-4.6/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3246 2022-11-10 07:28:46.000000 zope.exceptions-4.6/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.142297 zope.exceptions-4.6/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.149933 zope.exceptions-4.6/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.153976 zope.exceptions-4.6/src/zope/exceptions/
--rw-r--r--   0 mac        (513) staff       (20)     2122 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    11973 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/exceptionformatter.py
--rw-r--r--   0 mac        (513) staff       (20)     3439 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1303 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/log.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.155076 zope.exceptions-4.6/src/zope/exceptions/tests/
--rw-r--r--   0 mac        (513) staff       (20)        2 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    35803 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/tests/test_exceptionformatter.py
--rw-r--r--   0 mac        (513) staff       (20)     3000 2022-11-10 07:28:46.000000 zope.exceptions-4.6/src/zope/exceptions/tests/test_log.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-10 07:28:48.152620 zope.exceptions-4.6/src/zope.exceptions.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     8214 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      817 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       93 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-11-10 07:28:47.000000 zope.exceptions-4.6/src/zope.exceptions.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1876 2022-11-10 07:28:46.000000 zope.exceptions-4.6/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.439715 zope.exceptions-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5499 2023-06-29 06:08:19.000000 zope.exceptions-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-06-29 06:08:19.000000 zope.exceptions-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-06-29 06:08:19.000000 zope.exceptions-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-06-29 06:08:19.000000 zope.exceptions-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      344 2023-06-29 06:08:19.000000 zope.exceptions-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8034 2023-06-29 06:08:19.439772 zope.exceptions-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1175 2023-06-29 06:08:19.000000 zope.exceptions-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       97 2023-06-29 06:08:19.000000 zope.exceptions-5.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.437454 zope.exceptions-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5596 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1166 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8197 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9152 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      236 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5112 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5970 2023-06-29 06:08:19.000000 zope.exceptions-5.0/docs/narr.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-06-29 06:08:19.000000 zope.exceptions-5.0/rtd.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-06-29 06:08:19.439997 zope.exceptions-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2023-06-29 06:08:19.000000 zope.exceptions-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.434629 zope.exceptions-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.437587 zope.exceptions-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.439141 zope.exceptions-5.0/src/zope/exceptions/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2122 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11235 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/exceptionformatter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3439 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1236 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/log.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.439582 zope.exceptions-5.0/src/zope/exceptions/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        2 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    35450 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/tests/test_exceptionformatter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2858 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope/exceptions/tests/test_log.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-29 06:08:19.438573 zope.exceptions-5.0/src/zope.exceptions.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8034 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      817 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       93 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-29 06:08:19.000000 zope.exceptions-5.0/src/zope.exceptions.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1828 2023-06-29 06:08:19.000000 zope.exceptions-5.0/tox.ini
```

### Comparing `zope.exceptions-4.6/CHANGES.rst` & `zope.exceptions-5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ===========================
  zope.exceptions Changelog
 ===========================
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.6 (2022-11-10)
 ================
 
 - Catch exceptions in ``formatExceptionOnly``.
   Getting an exception when reporting about a different exception is not helpful.
   On Python 3.11 this is needed for some HTTPErrors.
```

### Comparing `zope.exceptions-4.6/CONTRIBUTING.md` & `zope.exceptions-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/LICENSE.txt` & `zope.exceptions-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/PKG-INFO` & `zope.exceptions-5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 Metadata-Version: 2.1
 Name: zope.exceptions
-Version: 4.6
+Version: 5.0
 Summary: Zope Exceptions
 Home-page: https://github.com/zopefoundation/zope.exceptions
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.exceptions/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.exceptions
 Keywords: zope exceptions
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =================
  zope.exceptions
 =================
@@ -64,14 +59,20 @@
 Please see https://zopeexceptions.readthedocs.io/ for the documentation.
 
 
 ===========================
  zope.exceptions Changelog
 ===========================
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.6 (2022-11-10)
 ================
 
 - Catch exceptions in ``formatExceptionOnly``.
   Getting an exception when reporting about a different exception is not helpful.
   On Python 3.11 this is needed for some HTTPErrors.
 
@@ -306,9 +307,7 @@
 
 
 3.0.0 (2004-11-07)
 ==================
 
 - Corresponds to the version of the zope.exceptions package shipped as part of
   the Zope X3.0.0 release.
-
-
```

### Comparing `zope.exceptions-4.6/README.rst` & `zope.exceptions-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/docs/Makefile` & `zope.exceptions-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/docs/api.rst` & `zope.exceptions-5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/docs/conf.py` & `zope.exceptions-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/docs/hacking.rst` & `zope.exceptions-5.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/docs/make.bat` & `zope.exceptions-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/docs/narr.rst` & `zope.exceptions-5.0/docs/narr.rst`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/setup.py` & `zope.exceptions-5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
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
 """Setup for zope.exceptions package
 """
 import os
 
@@ -26,32 +26,28 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name='zope.exceptions',
-    version='4.6',
+    version='5.0',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     description='Zope Exceptions',
     long_description=(read('README.rst') + '\n\n' +
                       read('CHANGES.rst')),
     keywords='zope exceptions',
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
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
@@ -66,15 +62,15 @@
                           'zope.exceptions/issues'),
         'Sources': 'https://github.com/zopefoundation/zope.exceptions',
     },
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.interface',
     ],
     include_package_data=True,
     zip_safe=False,
     extras_require={
```

### Comparing `zope.exceptions-4.6/src/zope/exceptions/__init__.py` & `zope.exceptions-5.0/src/zope/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/src/zope/exceptions/exceptionformatter.py` & `zope.exceptions-5.0/src/zope/exceptions/exceptionformatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,24 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """An exception formatter that shows traceback supplements and traceback info,
 optionally in HTML.
 """
-import sys
-
-
-try:
-    from html import escape
-except ImportError:  # pragma: PY2
-    from cgi import escape
-
 import linecache
+import sys
 import traceback
+from html import escape
 
 
 DEBUG_EXCEPTION_FORMATTER = 1
 
 
-class TextExceptionFormatter(object):
+class TextExceptionFormatter:
 
     line_sep = '\n'
 
     def __init__(self, limit=None, with_filenames=False):
         self.limit = limit
         self.with_filenames = with_filenames
 
@@ -46,20 +40,15 @@
     def getLimit(self):
         limit = self.limit
         if limit is None:
             limit = getattr(sys, 'tracebacklimit', 200)
         return limit
 
     def formatSupplementLine(self, line):
-        result = '   - %s' % line
-        if not isinstance(result, str):  # pragma: PY2
-            # Must be an Python 2, and must be a unicode `line`
-            # and we upconverted the result to a unicode
-            result = result.encode('utf-8')
-        return result
+        return f'   - {line}'
 
     def formatSourceURL(self, url):
         return [self.formatSupplementLine(url)]
 
     def formatSupplement(self, supplement, tb):
         result = []
         fmtLine = self.formatSupplementLine
@@ -70,15 +59,15 @@
 
         line = getattr(supplement, 'line', 0)
         if line == -1:
             line = tb.tb_lineno
         col = getattr(supplement, 'column', -1)
         if line:
             if col is not None and col >= 0:
-                result.append(fmtLine('Line %s, Column %s' % (
+                result.append(fmtLine('Line {}, Column {}'.format(
                     line, col)))
             else:
                 result.append(fmtLine('Line %s' % line))
         elif col is not None and col >= 0:
             result.append(fmtLine('Column %s' % col))
 
         expr = getattr(supplement, 'expression', None)
@@ -102,15 +91,15 @@
                 # else just swallow the exception.
         return result
 
     def formatSupplementInfo(self, info):
         return self.escape(info)
 
     def formatTracebackInfo(self, tbi):
-        return self.formatSupplementLine('__traceback_info__: %s' % (tbi, ))
+        return self.formatSupplementLine('__traceback_info__: {}'.format(tbi))
 
     def formatLine(self, tb=None, f=None):
         if tb and not f:
             f = tb.tb_frame
             lineno = tb.tb_lineno
         elif not tb and f:
             lineno = f.f_lineno
@@ -174,15 +163,15 @@
         # We don't want to get an error when we format an error, so we
         # compensate in our code.  For example, on Python 3.11.0 HTTPError
         # gives an unhelpful KeyError in tempfile when Python formats it.
         # See https://github.com/python/cpython/issues/90113
         try:
             result = ''.join(traceback.format_exception_only(etype, value))
         except Exception:  # pragma: no cover
-            # This code branch is only covered on Python 3.11.
+            # This code branch is only covered on Python 3.11+.
             result = str(value)
         return result
 
     def formatLastLine(self, exc_line):
         return self.escape(exc_line)
 
     def formatException(self, etype, value, tb):
@@ -255,23 +244,14 @@
 
 
 class HTMLExceptionFormatter(TextExceptionFormatter):
 
     line_sep = '<br />\r\n'
 
     def escape(self, s):
-        if not isinstance(s, str):
-            try:  # pragma: PY2
-                s = str(s)
-            except UnicodeError:  # pragma: PY2
-                if hasattr(s, 'encode'):
-                    # We probably got a unicode string on Python 2.
-                    s = s.encode('utf-8')
-                else:  # pragma: no cover
-                    raise
         return escape(s, quote=False)
 
     def getPrefix(self):
         return '<p>Traceback (most recent call last):</p>\r\n<ul>'
 
     def formatSupplementLine(self, line):
         return '<b>%s</b>' % self.escape(line)
@@ -281,15 +261,15 @@
         info = info.replace(" ", "&nbsp;")
         info = info.replace("\n", self.line_sep)
         return info
 
     def formatTracebackInfo(self, tbi):
         s = self.escape(tbi)
         s = s.replace('\n', self.line_sep)
-        return '__traceback_info__: %s' % (s, )
+        return '__traceback_info__: {}'.format(s)
 
     def formatLine(self, tb=None, f=None):
         line = TextExceptionFormatter.formatLine(self, tb, f)
         return '<li>%s</li>' % line
 
     def formatLastLine(self, exc_line):
         line = '</ul><p>%s</p>' % self.escape(exc_line)
@@ -300,16 +280,15 @@
                      with_filenames=False):
     """Format a stack trace and the exception information.
 
     Similar to 'traceback.format_exception', but adds supplemental
     information to the traceback and accepts two options, 'as_html'
     and 'with_filenames'.
 
-    The result is a list of native strings; on Python 2 they are UTF-8
-    encoded if need be.
+    The result is a list of strings.
     """
     if as_html:
         fmt = HTMLExceptionFormatter(limit, with_filenames)
     else:
         fmt = TextExceptionFormatter(limit, with_filenames)
     return fmt.formatException(t, v, tb)
```

### Comparing `zope.exceptions-4.6/src/zope/exceptions/interfaces.py` & `zope.exceptions-5.0/src/zope/exceptions/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/src/zope/exceptions/log.py` & `zope.exceptions-5.0/src/zope/exceptions/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,19 @@
 
 import io
 import logging
 
 from zope.exceptions.exceptionformatter import print_exception
 
 
-Buffer = io.StringIO if bytes is not str else io.BytesIO  # PY2
-
-
 class Formatter(logging.Formatter):
 
     def formatException(self, ei):
         """Format and return the specified exception information as a string.
 
         Uses zope.exceptions.exceptionformatter to generate the traceback.
         """
-        sio = Buffer()
+        sio = io.StringIO()
         print_exception(ei[0], ei[1], ei[2], file=sio, with_filenames=True)
         s = sio.getvalue()
-        if s.endswith("\n"):
-            s = s[:-1]
+        s = s[:-1] if s.endswith("\n") else s
         return s
```

### Comparing `zope.exceptions-4.6/src/zope/exceptions/tests/test_exceptionformatter.py` & `zope.exceptions-5.0/src/zope/exceptions/tests/test_exceptionformatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ExceptionFormatter tests.
 """
 import sys
 import unittest
-
-
-try:
-    from urllib.error import HTTPError
-except ImportError:
-    # BBB for Python 2.7
-    from urllib2 import HTTPError
+from urllib.error import HTTPError
 
 
 IS_PY39_OR_GREATER = sys.version_info >= (3, 9)
 
 
 class TextExceptionFormatterTests(unittest.TestCase):
 
@@ -160,21 +154,19 @@
 
     def test_formatTracebackInfo(self):
         fmt = self._makeOne()
         self.assertEqual(fmt.formatTracebackInfo('XYZZY'),
                          '   - __traceback_info__: XYZZY')
 
     def test_formatTracebackInfo_unicode(self):
-        __traceback_info__ = u"Have a Snowman: \u2603"
+        __traceback_info__ = "Have a Snowman: \u2603"
         fmt = self._makeOne()
 
         result = fmt.formatTracebackInfo(__traceback_info__)
-        expected = '   - __traceback_info__: Have a Snowman: '
-        # utf-8 encoded on Python 2, unicode on Python 3
-        expected += '\xe2\x98\x83' if bytes is str else u'\u2603'
+        expected = '   - __traceback_info__: Have a Snowman: \u2603'
         self.assertIsInstance(result, str)
         self.assertEqual(result, expected)
 
     def test_formatLine_no_tb_no_f(self):
         fmt = self._makeOne()
         self.assertRaises(ValueError, fmt.formatLine, None, None)
 
@@ -684,15 +676,15 @@
             f(HOW_MANY)
         except ExceptionForTesting:
             s = self._callFUT(False)
         for n in range(HOW_MANY+1):
             self.assertTrue(s.find('level%d' % n) >= 0, s)
 
     def test_quote_last_line(self):
-        class C(object):
+        class C:
             pass
         try:
             raise TypeError(C())
         except TypeError:
             s = self._callFUT(True)
         self.assertIn('&lt;', s)
         self.assertIn('&gt;', s)
@@ -705,15 +697,15 @@
         lines = s.splitlines()[-3:]
         self.assertEqual(lines[0], '    syntax error')
         self.assertIn('    ^', lines[1])
         self.assertTrue(lines[2].startswith('SyntaxError: invalid syntax'),
                         lines[2])
 
     def test_traceback_info_non_ascii(self):
-        __traceback_info__ = u"Have a Snowman: \u2603"
+        __traceback_info__ = "Have a Snowman: \u2603"
         try:
             raise TypeError()
         except TypeError:
             s = self._callFUT(True)
 
         self.assertIsInstance(s, str)
         self.assertIn('Have a Snowman', s)
@@ -846,24 +838,24 @@
             raise ExceptionForTesting
         except ExceptionForTesting:
             s = self._callFUT(False)
         self.assertTrue(s.find('Adam & Eve') >= 0, s)
 
     def test_traceback_info_html(self):
         try:
-            __traceback_info__ = u"Adam & Eve"
+            __traceback_info__ = "Adam & Eve"
             raise ExceptionForTesting
         except ExceptionForTesting:
             s = self._callFUT(True)
         self.assertTrue(s.find('Adam &amp; Eve') >= 0, s)
 
     def test_traceback_supplement_text(self):
         try:
             __traceback_supplement__ = (TestingTracebackSupplement,
-                                        u"You're one in a million")
+                                        "You're one in a million")
             raise ExceptionForTesting
         except ExceptionForTesting:
             s = self._callFUT(False)
         # The source URL
         self.assertTrue(s.find('/somepath') >= 0, s)
         # The line number
         self.assertTrue(s.find('634') >= 0, s)
@@ -901,51 +893,51 @@
             self.assertTrue(s.find('test_noinput') >= 0)
 
 
 class ExceptionForTesting(Exception):
     pass
 
 
-class TestingTracebackSupplement(object):
+class TestingTracebackSupplement:
     source_url = '/somepath'
     line = 634
     column = 57
     warnings = ['Repent, for the end is nigh']
 
     def __init__(self, expression):
         self.expression = expression
 
 
-class DummySupplement(object):
+class DummySupplement:
     def __init__(self, info=''):
         self._info = info
 
     def getInfo(self):
         return self._info
 
 
-class DummyTB(object):
+class DummyTB:
     # https://docs.python.org/3/reference/datamodel.html#traceback-objects
     tb_frame = None
     tb_lineno = 14
     tb_next = None
     tb_lasti = 1
 
 
-class DummyFrame(object):
+class DummyFrame:
     f_lineno = 137
     f_back = None
 
     def __init__(self):
         self.f_locals = {}
         self.f_globals = {}
         self.f_code = DummyCode()
 
 
-class DummyCode(object):
+class DummyCode:
     co_filename = 'dummy/filename.py'
     co_name = 'dummy_function'
 
     def co_positions(self):
         # New in Python 3.11.
         # https://docs.python.org/3/reference/datamodel.html#codeobject.co_positions
         # Note that this is not called for DummyTB if you have tb_lasti=-1.
@@ -953,15 +945,15 @@
         # in test_formatException_recursion_in_tb_stack in this file.
         # The rest is random.
         # Note that this code is only called on Python 3.11+, so we mark it for
         # the coverage tool.
         return [(27, 2, 3, 4)]  # pragma: no cover
 
 
-class _Monkey(object):
+class _Monkey:
     # context-manager for replacing module names in the scope of a test.
     def __init__(self, module, **kw):
         self.module = module
         self.to_restore = {key: getattr(module, key, self)
                            for key in kw}
         for key, value in kw.items():
             setattr(module, key, value)
@@ -971,11 +963,7 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for key, value in self.to_restore.items():
             if value is not self:  # pragma: no cover
                 setattr(self.module, key, value)
             else:
                 delattr(self.module, key)
-
-
-def test_suite():
-    return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `zope.exceptions-4.6/src/zope/exceptions/tests/test_log.py` & `zope.exceptions-5.0/src/zope/exceptions/tests/test_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,50 +37,48 @@
         self.assertEqual(lines[1], '  File "dummy/filename.py", line 14, '
                                    'in dummy_function')
         emsg = traceback.format_exception_only(ValueError, exc)[0]
         self.assertEqual(lines[2], emsg[:-1])  # strip trailing \n from emsg
 
     def test_unicode_traceback_info(self):
         import traceback
-        __traceback_info__ = u"Have a Snowman: \u2603"
+        __traceback_info__ = "Have a Snowman: \u2603"
         tb = DummyTB()
         tb.tb_frame.f_locals['__traceback_info__'] = __traceback_info__
         exc = ValueError('testing')
         fmt = self._makeOne()
         result = fmt.formatException((ValueError, exc, tb))
         self.assertIsInstance(result, str)
         lines = result.splitlines()
         self.assertEqual(len(lines), 4)
         self.assertEqual(lines[0], 'Traceback (most recent call last):')
         self.assertEqual(lines[1], '  File "dummy/filename.py", line 14, '
                                    'in dummy_function')
-        expected = '   - __traceback_info__: Have a Snowman: '
-        # utf-8 encoded on Python 2, unicode on Python 3
-        expected += '\xe2\x98\x83' if bytes is str else u'\u2603'
+        expected = '   - __traceback_info__: Have a Snowman: \u2603'
 
         self.assertEqual(lines[2], expected)
 
         emsg = traceback.format_exception_only(ValueError, exc)[0]
         self.assertEqual(lines[3], emsg[:-1])  # strip trailing \n from emsg
 
 
-class DummyTB(object):
+class DummyTB:
     tb_lineno = 14
     tb_next = None
 
     def __init__(self):
         self.tb_frame = DummyFrame()
 
 
-class DummyFrame(object):
+class DummyFrame:
     f_lineno = 137
     f_back = None
 
     def __init__(self):
         self.f_locals = {}
         self.f_globals = {}
         self.f_code = DummyCode()
 
 
-class DummyCode(object):
+class DummyCode:
     co_filename = 'dummy/filename.py'
     co_name = 'dummy_function'
```

### Comparing `zope.exceptions-4.6/src/zope.exceptions.egg-info/PKG-INFO` & `zope.exceptions-5.0/src/zope.exceptions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 Metadata-Version: 2.1
 Name: zope.exceptions
-Version: 4.6
+Version: 5.0
 Summary: Zope Exceptions
 Home-page: https://github.com/zopefoundation/zope.exceptions
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.exceptions/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.exceptions
 Keywords: zope exceptions
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =================
  zope.exceptions
 =================
@@ -64,14 +59,20 @@
 Please see https://zopeexceptions.readthedocs.io/ for the documentation.
 
 
 ===========================
  zope.exceptions Changelog
 ===========================
 
+5.0 (2023-06-29)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.6 (2022-11-10)
 ================
 
 - Catch exceptions in ``formatExceptionOnly``.
   Getting an exception when reporting about a different exception is not helpful.
   On Python 3.11 this is needed for some HTTPErrors.
 
@@ -306,9 +307,7 @@
 
 
 3.0.0 (2004-11-07)
 ==================
 
 - Corresponds to the version of the zope.exceptions package shipped as part of
   the Zope X3.0.0 release.
-
-
```

### Comparing `zope.exceptions-4.6/src/zope.exceptions.egg-info/SOURCES.txt` & `zope.exceptions-5.0/src/zope.exceptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.exceptions-4.6/tox.ini` & `zope.exceptions-5.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,28 @@
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
     py311
-    pypy
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
@@ -40,14 +36,15 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
@@ -60,25 +57,23 @@
 
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
-    coverage report -m --fail-under=99.5
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.exceptions
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

