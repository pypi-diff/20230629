# Comparing `tmp/pywhen-0.11.1.tar.gz` & `tmp/pywhen-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywhen-0.11.1.tar", last modified: Sun Feb 20 19:04:45 2022, max compression
+gzip compressed data, was "pywhen-0.11.2.tar", last modified: Thu Jun 29 21:00:21 2023, max compression
```

## Comparing `pywhen-0.11.1.tar` & `pywhen-0.11.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2022-02-20 19:04:45.569499 pywhen-0.11.1/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1679 2022-02-20 19:04:45.569223 pywhen-0.11.1/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      596 2022-02-20 19:02:47.000000 pywhen-0.11.1/README.rst
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2022-02-20 19:04:45.568796 pywhen-0.11.1/pywhen.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1679 2022-02-20 19:04:45.000000 pywhen-0.11.1/pywhen.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      147 2022-02-20 19:04:45.000000 pywhen-0.11.1/pywhen.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2022-02-20 19:04:45.000000 pywhen-0.11.1/pywhen.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        5 2022-02-20 19:04:45.000000 pywhen-0.11.1/pywhen.egg-info/top_level.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2022-02-20 19:04:45.569593 pywhen-0.11.1/setup.cfg
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1350 2021-04-08 13:25:38.000000 pywhen-0.11.1/setup.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     8462 2022-02-20 19:03:05.000000 pywhen-0.11.1/when.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 21:00:21.807320 pywhen-0.11.2/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2021-04-08 13:22:20.000000 pywhen-0.11.2/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1445 2023-06-29 21:00:21.806990 pywhen-0.11.2/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      585 2023-06-29 20:59:56.000000 pywhen-0.11.2/README.rst
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 21:00:21.806553 pywhen-0.11.2/pywhen.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1445 2023-06-29 21:00:21.000000 pywhen-0.11.2/pywhen.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      155 2023-06-29 21:00:21.000000 pywhen-0.11.2/pywhen.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-06-29 21:00:21.000000 pywhen-0.11.2/pywhen.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        5 2023-06-29 21:00:21.000000 pywhen-0.11.2/pywhen.egg-info/top_level.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-06-29 21:00:21.807419 pywhen-0.11.2/setup.cfg
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1352 2023-06-29 20:59:12.000000 pywhen-0.11.2/setup.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     8462 2023-06-29 20:58:23.000000 pywhen-0.11.2/when.py
```

### Comparing `pywhen-0.11.1/PKG-INFO` & `pywhen-0.11.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pywhen
-Version: 0.11.1
+Version: 0.11.2
 Summary: Collection of random python tools and utilities 
 Home-page: https://github.com/cltrudeau/wrench
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
-Description: when
-        ****
-        
-        A wrapper library for date/time conversion.  Takes many of the standard ISO
-        date formats as strings and creates an internally consistent datetime object.
-        
-        Installation
-        ============
-        
-        .. code-block:: bash
-        
-            $ pip install pywhen
-        
-        Supports
-        ========
-        
-        pywhen has been tested with Python 3.6, 3.7, 3.8, 3.9, and 3.10
-        
-        Previously it was tested with Python 2.7, not much has changed since then and
-        it should still work, but it isn't part of the automatic tests anymore.
-        
-        Docs & Source
-        =============
-        
-        Docs: http://pywhen.readthedocs.io/en/latest/
-        
-        Source: https://github.com/cltrudeau/pywhen
-        
 Keywords: tools
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+when
+****
+
+A wrapper library for date/time conversion.  Takes many of the standard ISO
+date formats as strings and creates an internally consistent datetime object.
+
+Installation
+============
+
+.. code-block:: bash
+
+    $ pip install pywhen
+
+Supports
+========
+
+pywhen has been tested with Python 3.8-3.11
+
+Previously it was tested with Python 2.7, 3.6-3.7. Not much has changed since
+then and it should still work, but it isn't part of the automatic tests
+anymore.
+
+Docs & Source
+=============
+
+Docs: http://pywhen.readthedocs.io/en/latest/
+
+Source: https://github.com/cltrudeau/pywhen
```

### Comparing `pywhen-0.11.1/README.rst` & `pywhen-0.11.2/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 .. code-block:: bash
 
     $ pip install pywhen
 
 Supports
 ========
 
-pywhen has been tested with Python 3.6, 3.7, 3.8, 3.9, and 3.10
+pywhen has been tested with Python 3.8-3.11
 
-Previously it was tested with Python 2.7, not much has changed since then and
-it should still work, but it isn't part of the automatic tests anymore.
+Previously it was tested with Python 2.7, 3.6-3.7. Not much has changed since
+then and it should still work, but it isn't part of the automatic tests
+anymore.
 
 Docs & Source
 =============
 
 Docs: http://pywhen.readthedocs.io/en/latest/
 
 Source: https://github.com/cltrudeau/pywhen
```

### Comparing `pywhen-0.11.1/pywhen.egg-info/PKG-INFO` & `pywhen-0.11.2/pywhen.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pywhen
-Version: 0.11.1
+Version: 0.11.2
 Summary: Collection of random python tools and utilities 
 Home-page: https://github.com/cltrudeau/wrench
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
-Description: when
-        ****
-        
-        A wrapper library for date/time conversion.  Takes many of the standard ISO
-        date formats as strings and creates an internally consistent datetime object.
-        
-        Installation
-        ============
-        
-        .. code-block:: bash
-        
-            $ pip install pywhen
-        
-        Supports
-        ========
-        
-        pywhen has been tested with Python 3.6, 3.7, 3.8, 3.9, and 3.10
-        
-        Previously it was tested with Python 2.7, not much has changed since then and
-        it should still work, but it isn't part of the automatic tests anymore.
-        
-        Docs & Source
-        =============
-        
-        Docs: http://pywhen.readthedocs.io/en/latest/
-        
-        Source: https://github.com/cltrudeau/pywhen
-        
 Keywords: tools
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+when
+****
+
+A wrapper library for date/time conversion.  Takes many of the standard ISO
+date formats as strings and creates an internally consistent datetime object.
+
+Installation
+============
+
+.. code-block:: bash
+
+    $ pip install pywhen
+
+Supports
+========
+
+pywhen has been tested with Python 3.8-3.11
+
+Previously it was tested with Python 2.7, 3.6-3.7. Not much has changed since
+then and it should still work, but it isn't part of the automatic tests
+anymore.
+
+Docs & Source
+=============
+
+Docs: http://pywhen.readthedocs.io/en/latest/
+
+Source: https://github.com/cltrudeau/pywhen
```

### Comparing `pywhen-0.11.1/setup.py` & `pywhen-0.11.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords='tools',
     test_suite='load_tests.get_suite',
     py_modules = ['when',],
     install_requires=[],
```

### Comparing `pywhen-0.11.1/when.py` & `pywhen-0.11.2/when.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.11.1'
+__version__ = '0.11.2'
 
 import sys
 from datetime import datetime, time
 import time as time_mod
 
 # =============================================================================
```

