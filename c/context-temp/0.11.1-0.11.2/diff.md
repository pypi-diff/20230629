# Comparing `tmp/context_temp-0.11.1.tar.gz` & `tmp/context_temp-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/context_temp-0.11.1.tar", last modified: Fri Jul 26 18:54:07 2019, max compression
+gzip compressed data, was "context_temp-0.11.2.tar", last modified: Thu Jun 29 18:49:57 2023, max compression
```

## Comparing `context_temp-0.11.1.tar` & `context_temp-0.11.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2019-07-26 18:54:07.000000 context_temp-0.11.1/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1526 2019-07-26 18:54:07.000000 context_temp-0.11.1/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      449 2019-07-26 18:52:53.000000 context_temp-0.11.1/README.rst
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2019-07-26 18:54:07.000000 context_temp-0.11.1/context_temp.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1526 2019-07-26 18:54:07.000000 context_temp-0.11.1/context_temp.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      179 2019-07-26 18:54:07.000000 context_temp-0.11.1/context_temp.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2019-07-26 18:54:07.000000 context_temp-0.11.1/context_temp.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       13 2019-07-26 18:54:07.000000 context_temp-0.11.1/context_temp.egg-info/top_level.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1699 2019-07-26 18:53:43.000000 context_temp-0.11.1/context_temp.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2019-07-26 18:54:07.000000 context_temp-0.11.1/setup.cfg
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1439 2019-07-26 18:45:13.000000 context_temp-0.11.1/setup.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 18:49:57.143714 context_temp-0.11.2/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2019-07-26 18:16:52.000000 context_temp-0.11.2/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1312 2023-06-29 18:49:57.143376 context_temp-0.11.2/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      444 2023-06-29 18:48:09.000000 context_temp-0.11.2/README.rst
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 18:49:57.142842 context_temp-0.11.2/context_temp.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1312 2023-06-29 18:49:57.000000 context_temp-0.11.2/context_temp.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      187 2023-06-29 18:49:57.000000 context_temp-0.11.2/context_temp.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-06-29 18:49:57.000000 context_temp-0.11.2/context_temp.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       13 2023-06-29 18:49:57.000000 context_temp-0.11.2/context_temp.egg-info/top_level.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1699 2023-06-29 18:46:43.000000 context_temp-0.11.2/context_temp.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-06-29 18:49:57.143842 context_temp-0.11.2/setup.cfg
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1439 2023-06-29 18:46:29.000000 context_temp-0.11.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `context_temp-0.11.1/PKG-INFO` & `context_temp-0.11.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: context_temp
-Version: 0.11.1
+Version: 0.11.2
 Summary: Context Manager wrappers for temp files and directories
 Home-page: https://github.com/cltrudeau/context_temp
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
-Description: context_temp
-        ************
-        
-        Context Manager wrappers for temp files and directories which remove the file
-        or directory when when the manager goes out of scope.
-        
-        
-        Installation
-        ============
-        
-        .. code-block:: bash
-        
-            $ pip install context_temp
-        
-        Supports
-        ========
-        
-        context_temp has been tested with Python 2.7, 3.6, 3.7
-        
-        Docs & Source
-        =============
-        
-        Docs: http://context_temp.readthedocs.io/en/latest/
-        
-        Source: https://github.com/cltrudeau/context_temp
-        
 Keywords: context manager,tools,temp file,temp directory
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+context_temp
+************
+
+Context Manager wrappers for temp files and directories which remove the file
+or directory when when the manager goes out of scope.
+
+
+Installation
+============
+
+.. code-block:: bash
+
+    $ pip install context_temp
+
+Supports
+========
+
+context_temp has been tested with Python 3.8-3.11
+
+Docs & Source
+=============
+
+Docs: http://context_temp.readthedocs.io/en/latest/
+
+Source: https://github.com/cltrudeau/context_temp
```

### Comparing `context_temp-0.11.1/context_temp.egg-info/PKG-INFO` & `context_temp-0.11.2/context_temp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: context-temp
-Version: 0.11.1
+Version: 0.11.2
 Summary: Context Manager wrappers for temp files and directories
 Home-page: https://github.com/cltrudeau/context_temp
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
-Description: context_temp
-        ************
-        
-        Context Manager wrappers for temp files and directories which remove the file
-        or directory when when the manager goes out of scope.
-        
-        
-        Installation
-        ============
-        
-        .. code-block:: bash
-        
-            $ pip install context_temp
-        
-        Supports
-        ========
-        
-        context_temp has been tested with Python 2.7, 3.6, 3.7
-        
-        Docs & Source
-        =============
-        
-        Docs: http://context_temp.readthedocs.io/en/latest/
-        
-        Source: https://github.com/cltrudeau/context_temp
-        
 Keywords: context manager,tools,temp file,temp directory
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+context_temp
+************
+
+Context Manager wrappers for temp files and directories which remove the file
+or directory when when the manager goes out of scope.
+
+
+Installation
+============
+
+.. code-block:: bash
+
+    $ pip install context_temp
+
+Supports
+========
+
+context_temp has been tested with Python 3.8-3.11
+
+Docs & Source
+=============
+
+Docs: http://context_temp.readthedocs.io/en/latest/
+
+Source: https://github.com/cltrudeau/context_temp
```

### Comparing `context_temp-0.11.1/context_temp.py` & `context_temp-0.11.2/context_temp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.11.1'
+__version__ = '0.11.2'
 
 import contextlib, os, shutil, tempfile
 
 # =============================================================================
 # Context Managers
 # =============================================================================
```

### Comparing `context_temp-0.11.1/setup.py` & `context_temp-0.11.2/setup.py`

 * *Files identical despite different names*

