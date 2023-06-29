# Comparing `tmp/pimms-0.3.8.tar.gz` & `tmp/pimms-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pimms-0.3.8.tar", last modified: Sat Jun 29 03:51:35 2019, max compression
+gzip compressed data, was "dist/pimms-0.3.9.tar", last modified: Mon Jul  1 18:07:51 2019, max compression
```

## Comparing `pimms-0.3.8.tar` & `pimms-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 nben       (501) staff       (20)        0 2019-06-29 03:51:35.000000 pimms-0.3.8/
--rw-r--r--   0 nben       (501) staff       (20)      293 2019-06-29 03:51:35.000000 pimms-0.3.8/PKG-INFO
--rw-r--r--   0 nben       (501) staff       (20)    20456 2019-05-12 02:53:53.000000 pimms-0.3.8/README.md
--rw-r--r--   0 nben       (501) staff       (20)      777 2019-06-29 03:50:39.000000 pimms-0.3.8/setup.py
-drwxr-xr-x   0 nben       (501) staff       (20)        0 2019-06-29 03:51:35.000000 pimms-0.3.8/pimms/
--rw-r--r--   0 nben       (501) staff       (20)    33770 2019-06-28 11:49:15.000000 pimms-0.3.8/pimms/immutable.py
-drwxr-xr-x   0 nben       (501) staff       (20)        0 2019-06-29 03:51:35.000000 pimms-0.3.8/pimms/test/
--rw-r--r--   0 nben       (501) staff       (20)     1498 2019-05-12 02:53:53.000000 pimms-0.3.8/pimms/test/lazy_complex.py
--rw-r--r--   0 nben       (501) staff       (20)    20863 2019-06-29 01:30:02.000000 pimms-0.3.8/pimms/test/__init__.py
--rw-r--r--   0 nben       (501) staff       (20)     1387 2019-05-12 02:53:53.000000 pimms-0.3.8/pimms/test/tri_calc.py
--rw-r--r--   0 nben       (501) staff       (20)     2077 2019-05-12 02:53:53.000000 pimms-0.3.8/pimms/test/normal_calc.py
--rw-r--r--   0 nben       (501) staff       (20)    58574 2019-06-29 01:16:44.000000 pimms-0.3.8/pimms/util.py
--rw-r--r--   0 nben       (501) staff       (20)    24705 2019-06-28 11:52:16.000000 pimms-0.3.8/pimms/cmdline.py
--rw-r--r--   0 nben       (501) staff       (20)    39449 2019-06-29 03:49:25.000000 pimms-0.3.8/pimms/calculation.py
--rw-r--r--   0 nben       (501) staff       (20)    11284 2019-06-29 03:50:52.000000 pimms-0.3.8/pimms/__init__.py
--rw-r--r--   0 nben       (501) staff       (20)    19575 2019-06-28 11:51:45.000000 pimms-0.3.8/pimms/table.py
--rw-r--r--   0 nben       (501) staff       (20)       79 2019-06-29 03:51:35.000000 pimms-0.3.8/setup.cfg
-drwxr-xr-x   0 nben       (501) staff       (20)        0 2019-06-29 03:51:35.000000 pimms-0.3.8/pimms.egg-info/
--rw-r--r--   0 nben       (501) staff       (20)      293 2019-06-29 03:51:34.000000 pimms-0.3.8/pimms.egg-info/PKG-INFO
--rw-r--r--   0 nben       (501) staff       (20)      375 2019-06-29 03:51:34.000000 pimms-0.3.8/pimms.egg-info/SOURCES.txt
--rw-r--r--   0 nben       (501) staff       (20)       48 2019-06-29 03:51:34.000000 pimms-0.3.8/pimms.egg-info/requires.txt
--rw-r--r--   0 nben       (501) staff       (20)        6 2019-06-29 03:51:34.000000 pimms-0.3.8/pimms.egg-info/top_level.txt
--rw-r--r--   0 nben       (501) staff       (20)        1 2019-06-29 03:51:34.000000 pimms-0.3.8/pimms.egg-info/dependency_links.txt
+drwxr-xr-x   0 nben       (504) staff       (20)        0 2019-07-01 18:07:51.000000 pimms-0.3.9/
+-rw-r--r--   0 nben       (504) staff       (20)      293 2019-07-01 18:07:51.000000 pimms-0.3.9/PKG-INFO
+-rw-r--r--   0 nben       (504) staff       (20)    20456 2019-04-12 20:32:53.000000 pimms-0.3.9/README.md
+-rw-r--r--   0 nben       (504) staff       (20)      777 2019-07-01 18:05:22.000000 pimms-0.3.9/setup.py
+drwxr-xr-x   0 nben       (504) staff       (20)        0 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms/
+-rw-r--r--   0 nben       (504) staff       (20)    33770 2019-07-01 17:57:57.000000 pimms-0.3.9/pimms/immutable.py
+drwxr-xr-x   0 nben       (504) staff       (20)        0 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms/test/
+-rw-r--r--   0 nben       (504) staff       (20)     2122 2016-12-08 15:12:17.000000 pimms-0.3.9/pimms/test/normal.py
+-rw-r--r--   0 nben       (504) staff       (20)     1498 2018-09-13 01:56:51.000000 pimms-0.3.9/pimms/test/lazy_complex.py
+-rw-r--r--   0 nben       (504) staff       (20)    20863 2019-07-01 17:57:57.000000 pimms-0.3.9/pimms/test/__init__.py
+-rw-r--r--   0 nben       (504) staff       (20)     1387 2017-06-01 19:02:06.000000 pimms-0.3.9/pimms/test/tri_calc.py
+-rw-r--r--   0 nben       (504) staff       (20)     2077 2017-03-11 16:06:34.000000 pimms-0.3.9/pimms/test/normal_calc.py
+-rw-r--r--   0 nben       (504) staff       (20)    58574 2019-07-01 17:57:57.000000 pimms-0.3.9/pimms/util.py
+-rw-r--r--   0 nben       (504) staff       (20)    24705 2019-07-01 17:57:57.000000 pimms-0.3.9/pimms/cmdline.py
+-rw-r--r--   0 nben       (504) staff       (20)    39515 2019-07-01 18:04:46.000000 pimms-0.3.9/pimms/calculation.py
+-rw-r--r--   0 nben       (504) staff       (20)    11284 2019-07-01 18:05:28.000000 pimms-0.3.9/pimms/__init__.py
+-rw-r--r--   0 nben       (504) staff       (20)    19575 2019-07-01 17:57:57.000000 pimms-0.3.9/pimms/table.py
+-rw-r--r--   0 nben       (504) staff       (20)       79 2019-07-01 18:07:51.000000 pimms-0.3.9/setup.cfg
+drwxr-xr-x   0 nben       (504) staff       (20)        0 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms.egg-info/
+-rw-r--r--   0 nben       (504) staff       (20)      293 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms.egg-info/PKG-INFO
+-rw-r--r--   0 nben       (504) staff       (20)      396 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms.egg-info/SOURCES.txt
+-rw-r--r--   0 nben       (504) staff       (20)       48 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms.egg-info/requires.txt
+-rw-r--r--   0 nben       (504) staff       (20)        6 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms.egg-info/top_level.txt
+-rw-r--r--   0 nben       (504) staff       (20)        1 2019-07-01 18:07:51.000000 pimms-0.3.9/pimms.egg-info/dependency_links.txt
```

### Comparing `pimms-0.3.8/README.md` & `pimms-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/setup.py` & `pimms-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 ####################################################################################################
 
 from setuptools import (setup, Extension)
 
 setup(
     name='pimms',
-    version='0.3.8',
+    version='0.3.9',
     description='Python immutable data structures library',
     keywords='persistent immutable functional',
     author='Noah C. Benson',
     author_email='nben@nyu.edu',
     url='https://github.com/noahbenson/pimms/',
     license='GPLv3',
     packages=['pimms', 'pimms.test'],
```

### Comparing `pimms-0.3.8/pimms/immutable.py` & `pimms-0.3.9/pimms/immutable.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/test/lazy_complex.py` & `pimms-0.3.9/pimms/test/lazy_complex.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/test/__init__.py` & `pimms-0.3.9/pimms/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/test/tri_calc.py` & `pimms-0.3.9/pimms/test/tri_calc.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/test/normal_calc.py` & `pimms-0.3.9/pimms/test/normal_calc.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/util.py` & `pimms-0.3.9/pimms/util.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/cmdline.py` & `pimms-0.3.9/pimms/cmdline.py`

 * *Files identical despite different names*

### Comparing `pimms-0.3.8/pimms/calculation.py` & `pimms-0.3.9/pimms/calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # By Noah C. Benson
 
 import copy, types, os, sys, re, warnings, pickle, pint, six
 import pyrsistent as ps, numpy as np, collections as colls
 from functools import reduce
 from .util  import (merge, is_pmap, is_str, is_map, is_lazy_map, is_vector, is_quantity, quant, mag,
                     units, qhash, save, load, is_nparray, getargspec_py27like, cache_filename,
-                    cache_lmap)
+                    cache_lmap, qhashform)
 from .table import (itable, is_itable)
 
 if six.PY2: tuple_type = types.TupleType
 else:       tuple_type = tuple
 
 ####################################################################################################
 # The Calc, Plan, and IMap classes
@@ -504,27 +504,28 @@
         #
         # We need to pause here and handle caching, if needed.
         (res, h, found) = (None, None, False)
         if ('memoize' in self.afferents and self.afferents['memoize']) and node.memoize:
             memdat = self.plan._memoized_data
             try:
                 h = {k:self.afferents[k] for k in self.plan.afferent_dependencies[node.name]}
-                h = (node.name, ps.pmap(h))
+                h = qhashform((node.name, ps.pmap(h)))
                 if h in memdat:
                     # memoization success; set h to None so we don't re-memoize the value
                     (res, h, found) = (memdat[h], None, True)
                 elif node.cache:
                     cpath = self.afferents.get('cache_directory', None)
                     if cpath is not None:
                         ureg = self.afferents.get('unit_registry', 'pimms')
-                        cpath = cache_filename(cpath, h)
-                        if os.path.isfile(cpath):
-                            # set cpath to None to signal we don't need to cache the value out
-                            try: (res, cpath, found) = (load(cpath, ureg), None, True)
-                            except Exception: pass
+                        try:
+                            cpath = cache_filename(cpath, h)
+                            if os.path.isfile(cpath):
+                                # set cpath to None to signal we don't need to cache the value out
+                                (res, cpath, found) = (load(cpath, ureg), None, True)
+                        except Exception: cpath = None
                 else: cpath = None
             except Exception: raise#b(h, found) = (None, False)
         # ensure we have a result
         if not found: res = node(self)
         # process the result:
         effs = reduce(lambda m,v: m.set(v[0],v[1]), six.iteritems(res), self.efferents)
         object.__setattr__(self, 'efferents', effs)
```

### Comparing `pimms-0.3.8/pimms/__init__.py` & `pimms-0.3.9/pimms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,9 +152,9 @@
     reload(sys.modules['pimms.table'])
     reload(sys.modules['pimms.immutable'])
     reload(sys.modules['pimms.calculation'])
     reload(sys.modules['pimms.cmdline'])
     reload(sys.modules['pimms'])
     return sys.modules['pimms']
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 description = 'Lazy immutable library for Python built on top of pyrsistent'
```

### Comparing `pimms-0.3.8/pimms/table.py` & `pimms-0.3.9/pimms/table.py`

 * *Files identical despite different names*

