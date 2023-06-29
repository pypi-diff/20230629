# Comparing `tmp/chorde-1.0.6.tar.gz` & `tmp/chorde-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chorde-1.0.6.tar", last modified: Tue Jun 27 18:23:07 2023, max compression
+gzip compressed data, was "chorde-1.0.7.tar", last modified: Thu Jun 29 17:16:45 2023, max compression
```

## Comparing `chorde-1.0.6.tar` & `chorde-1.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     8379 2023-06-27 18:16:09.000000 chorde-1.0.6/CHANGELOG
--rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.6/MANIFEST.in
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 18:23:07.618338 chorde-1.0.6/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.6/README.rst
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.602338 chorde-1.0.6/lib/
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.606338 chorde-1.0.6/lib/chorde/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-06-27 18:21:58.000000 chorde-1.0.6/lib/chorde/_version.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/lib/chorde/clients/
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   664070 2023-06-27 13:47:53.000000 chorde-1.0.6/lib/chorde/clients/_async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/clients/_async.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    15794 2023-06-27 13:46:52.000000 chorde-1.0.6/lib/chorde/clients/_async.pyx
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.6/lib/chorde/clients/async.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.6/lib/chorde/clients/asyncache.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/asyncache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.6/lib/chorde/clients/base.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/coherent.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/elasticache.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/files.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.6/lib/chorde/clients/inproc.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/inproc.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.6/lib/chorde/clients/memcached.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.6/lib/chorde/clients/tiered.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/clients/tiered.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.6/lib/chorde/decorators.c
--rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.6/lib/chorde/decorators.pxd
--rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/decorators.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/dnsutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/external_integration.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/lib/chorde/mq/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/mq/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/mq/coherence.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/mq/compat.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.618338 chorde-1.0.6/lib/chorde/mq/ipsub/
--rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.6/lib/chorde/mq/ipsub/__init__.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/mq/ipsub/base.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/mq/ipsub/ipsub_zmq.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4668 2023-06-27 18:15:41.000000 chorde-1.0.6/lib/chorde/sPickle.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.6/lib/chorde/serialize.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/shmemutils.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/threadpool.py
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.6/lib/chorde/worker.py
-drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-27 18:23:07.606338 chorde-1.0.6/lib/chorde.egg-info/
--rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/PKG-INFO
--rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/SOURCES.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/dependency_links.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.6/lib/chorde.egg-info/not-zip-safe
--rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/requires.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-06-27 18:23:07.000000 chorde-1.0.6/lib/chorde.egg-info/top_level.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.6/requirements.txt
--rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-06-27 18:23:07.618338 chorde-1.0.6/setup.cfg
--rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-06-27 18:15:18.000000 chorde-1.0.6/setup.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:45.098691 chorde-1.0.7/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     8522 2023-06-29 15:47:34.000000 chorde-1.0.7/CHANGELOG
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      118 2020-11-19 21:31:23.000000 chorde-1.0.7/MANIFEST.in
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-29 17:16:45.098691 chorde-1.0.7/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     9696 2023-04-17 14:22:33.000000 chorde-1.0.7/README.rst
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:44.926690 chorde-1.0.7/lib/
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:44.978691 chorde-1.0.7/lib/chorde/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      341 2020-05-05 20:27:26.000000 chorde-1.0.7/lib/chorde/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       21 2023-06-29 15:47:14.000000 chorde-1.0.7/lib/chorde/_version.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:45.090691 chorde-1.0.7/lib/chorde/clients/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1091 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   669169 2023-06-29 16:59:59.000000 chorde-1.0.7/lib/chorde/clients/_async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      333 2020-05-05 20:27:26.000000 chorde-1.0.7/lib/chorde/clients/_async.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    16106 2023-06-29 15:47:14.000000 chorde-1.0.7/lib/chorde/clients/_async.pyx
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2646275 2022-12-26 12:49:23.000000 chorde-1.0.7/lib/chorde/clients/async.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  2731676 2023-04-17 14:22:41.000000 chorde-1.0.7/lib/chorde/clients/asyncache.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    65380 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/asyncache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1357604 2023-04-17 14:22:42.000000 chorde-1.0.7/lib/chorde/clients/base.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    20610 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    12458 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/coherent.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3869 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/elasticache.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    34220 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/files.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   546821 2023-04-17 14:22:42.000000 chorde-1.0.7/lib/chorde/clients/inproc.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     7711 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/inproc.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    90704 2023-04-21 13:34:45.000000 chorde-1.0.7/lib/chorde/clients/memcached.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)   738201 2023-04-17 14:22:42.000000 chorde-1.0.7/lib/chorde/clients/tiered.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    11788 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/clients/tiered.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)  1955228 2023-04-17 14:22:43.000000 chorde-1.0.7/lib/chorde/decorators.c
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      623 2021-03-18 18:58:29.000000 chorde-1.0.7/lib/chorde/decorators.pxd
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    62984 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/decorators.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10597 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/dnsutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      895 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/external_integration.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:45.094691 chorde-1.0.7/lib/chorde/mq/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      199 2020-05-05 20:27:26.000000 chorde-1.0.7/lib/chorde/mq/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    29620 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/mq/coherence.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      354 2020-05-05 20:27:26.000000 chorde-1.0.7/lib/chorde/mq/compat.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:45.098691 chorde-1.0.7/lib/chorde/mq/ipsub/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      113 2020-05-05 20:27:26.000000 chorde-1.0.7/lib/chorde/mq/ipsub/__init__.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    13792 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/mq/ipsub/base.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22514 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/mq/ipsub/ipsub_zmq.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4668 2023-06-27 18:15:41.000000 chorde-1.0.7/lib/chorde/sPickle.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     3568 2022-01-28 13:06:45.000000 chorde-1.0.7/lib/chorde/serialize.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    22430 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/shmemutils.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    21949 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/threadpool.py
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1619 2023-03-03 18:03:18.000000 chorde-1.0.7/lib/chorde/worker.py
+drwxr-xr-x   0 claudiofreire  (1000) users      (100)        0 2023-06-29 17:16:44.982691 chorde-1.0.7/lib/chorde.egg-info/
+-rw-r--r--   0 claudiofreire  (1000) users      (100)    10433 2023-06-29 17:16:44.000000 chorde-1.0.7/lib/chorde.egg-info/PKG-INFO
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     1237 2023-06-29 17:16:44.000000 chorde-1.0.7/lib/chorde.egg-info/SOURCES.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2023-06-29 17:16:44.000000 chorde-1.0.7/lib/chorde.egg-info/dependency_links.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        1 2020-05-05 20:40:40.000000 chorde-1.0.7/lib/chorde.egg-info/not-zip-safe
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      126 2023-06-29 17:16:44.000000 chorde-1.0.7/lib/chorde.egg-info/requires.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)        7 2023-06-29 17:16:44.000000 chorde-1.0.7/lib/chorde.egg-info/top_level.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)       74 2023-05-15 15:39:00.000000 chorde-1.0.7/requirements.txt
+-rw-r--r--   0 claudiofreire  (1000) users      (100)      151 2023-06-29 17:16:45.098691 chorde-1.0.7/setup.cfg
+-rw-r--r--   0 claudiofreire  (1000) users      (100)     4209 2023-06-29 15:47:14.000000 chorde-1.0.7/setup.py
```

### Comparing `chorde-1.0.6/CHANGELOG` & `chorde-1.0.7/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Change Log
 
 All notable changes to this project will be documented here.
 
+## [1.0.7] - 2023-06-29
+### Bugfixes
+- Prevent memory leaks by clearing non-running traceback
+  frames from exceptions set as future results.
+
 ## [1.0.6] - 2023-06-27
 ### Bugfixes
 - Allow sPickle unpicklers to accept strings as checksum keys
 
 ## [1.0.5] - 2023-06-27
 ### Bugfixes
 - Allow sPickle to accept strings as checksum keys, automatically
```

### Comparing `chorde-1.0.6/PKG-INFO` & `chorde-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.6
+Version: 1.0.7
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.6/README.rst` & `chorde-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/__init__.py` & `chorde-1.0.7/lib/chorde/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/_async.c` & `chorde-1.0.7/lib/chorde/clients/_async.c`

 * *Files 0% similar despite different names*

```diff
@@ -1027,86 +1027,86 @@
   PyObject_HEAD
   struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *__pyx_vtab;
   PyObject *value;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":83
+/* "chorde/clients/_async.pyx":92
  * 
  * @cython.freelist(100)
  * cdef class WeakCallback:             # <<<<<<<<<<<<<<
  *     cdef object me, callback, __weakref__
  * 
  */
 struct __pyx_obj_6chorde_7clients_6_async_WeakCallback {
   PyObject_HEAD
   PyObject *me;
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":97
+/* "chorde/clients/_async.pyx":106
  * 
  * @cython.freelist(100)
  * cdef class DeferExceptionCallback:             # <<<<<<<<<<<<<<
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):
  */
 struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback {
   PyObject_HEAD
   PyObject *defer;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":105
+/* "chorde/clients/_async.pyx":114
  * 
  * @cython.freelist(100)
  * cdef class ValueCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_ValueCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":114
+/* "chorde/clients/_async.pyx":123
  * 
  * @cython.freelist(100)
  * cdef class MissCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_MissCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":123
+/* "chorde/clients/_async.pyx":132
  * 
  * @cython.freelist(100)
  * cdef class ExceptionCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":132
+/* "chorde/clients/_async.pyx":141
  * 
  * @cython.freelist(100)
  * cdef class AnyCallback:             # <<<<<<<<<<<<<<
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):
  */
 struct __pyx_obj_6chorde_7clients_6_async_AnyCallback {
@@ -1114,42 +1114,42 @@
   PyObject *on_value;
   PyObject *on_miss;
   PyObject *on_exc;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":150
+/* "chorde/clients/_async.pyx":159
  * 
  * @cython.freelist(100)
  * cdef class DoneCallback:             # <<<<<<<<<<<<<<
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  */
 struct __pyx_obj_6chorde_7clients_6_async_DoneCallback {
   PyObject_HEAD
   PyObject *callback;
   PyObject *__weakref__;
 };
 
 
-/* "chorde/clients/_async.pyx":157
+/* "chorde/clients/_async.pyx":166
  *         return self.callback()
  * 
  * cdef class NONE:             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_6chorde_7clients_6_async_NONE {
   PyObject_HEAD
 };
 
 
 
-/* "chorde/clients/_async.pyx":161
+/* "chorde/clients/_async.pyx":170
  * 
  * @cython.freelist(100)
  * cdef class Future:             # <<<<<<<<<<<<<<
  *     def __cinit__(self, logger = None):
  *         self._cb = None
  */
 
@@ -1432,24 +1432,24 @@
 #define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
 #define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* GetAttr.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
-
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1668,14 +1668,15 @@
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_wait[] = "wait";
 static const char __pyx_k_Event[] = "Event";
+static const char __pyx_k_clear[] = "clear";
 static const char __pyx_k_defer[] = "defer";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_strip[] = "strip";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_Future[] = "Future";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_logger[] = "logger";
@@ -1685,23 +1686,25 @@
 static const char __pyx_k_reason[] = "reason";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_on_miss[] = "on_miss";
 static const char __pyx_k_partial[] = "partial";
 static const char __pyx_k_reraise[] = "reraise";
+static const char __pyx_k_tb_next[] = "tb_next";
 static const char __pyx_k_timeout[] = "timeout";
 static const char __pyx_k_weakref[] = "weakref";
 static const char __pyx_k_callback[] = "callback";
 static const char __pyx_k_exc_info[] = "exc_info";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_on_stuff[] = "_on_stuff";
 static const char __pyx_k_on_value[] = "on_value";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_tb_frame[] = "tb_frame";
 static const char __pyx_k_HTTPError[] = "HTTPError";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_functools[] = "functools";
 static const char __pyx_k_norecurse[] = "norecurse";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_threading[] = "threading";
@@ -1761,14 +1764,15 @@
 static PyObject *__pyx_n_s_ValueCallback;
 static PyObject *__pyx_n_s_WeakCallback;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_callback;
 static PyObject *__pyx_n_s_chorde_clients;
 static PyObject *__pyx_n_s_chorde_clients__async;
+static PyObject *__pyx_n_s_clear;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_defer;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_exc;
 static PyObject *__pyx_n_s_exc_info;
 static PyObject *__pyx_n_s_functools;
@@ -1808,14 +1812,16 @@
 static PyObject *__pyx_n_s_set_nothreads;
 static PyObject *__pyx_n_s_set_result;
 static PyObject *__pyx_n_s_set_strip_tracebacks;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_strip;
+static PyObject *__pyx_n_s_tb_frame;
+static PyObject *__pyx_n_s_tb_next;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_s_timeout;
 static PyObject *__pyx_n_s_tornado_web;
 static PyObject *__pyx_n_s_traceback;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_value;
@@ -2100,14 +2106,15 @@
 static PyObject *__pyx_f_6chorde_7clients_6_async_16ExceptionWrapper_reraise(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *__pyx_v_self, int __pyx_skip_dispatch, struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise *__pyx_optional_args) {
   int __pyx_v_strip = ((int)1);
   PyObject *__pyx_v_exc = NULL;
   PyObject *__pyx_v_exc_typ = NULL;
   PyObject *__pyx_v_exc_obj = NULL;
   PyObject *__pyx_v_exc_tb = NULL;
   PyObject *__pyx_v_kwargs = NULL;
+  PyObject *__pyx_v_tb = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -2428,15 +2435,15 @@
       }
 
       /* "chorde/clients/_async.pyx":66
  *                     # correctly without a reason, and reason is given only as kwarg
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj             # <<<<<<<<<<<<<<
  *             elif exc_tb is not None:
- *                 if exc_obj is not None:
+ *                 # clear any non-running traceback's frames to avoid leaking locals
  */
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_args); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L12_error)
@@ -2458,240 +2465,358 @@
  */
     }
 
     /* "chorde/clients/_async.pyx":67
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
- *                 if exc_obj is not None:
- *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
+ *                 # clear any non-running traceback's frames to avoid leaking locals
+ *                 tb = exc_tb
  */
     __pyx_t_6 = (__pyx_v_exc_tb != Py_None);
     __pyx_t_17 = (__pyx_t_6 != 0);
     if (__pyx_t_17) {
 
-      /* "chorde/clients/_async.pyx":68
- *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
+      /* "chorde/clients/_async.pyx":69
  *             elif exc_tb is not None:
+ *                 # clear any non-running traceback's frames to avoid leaking locals
+ *                 tb = exc_tb             # <<<<<<<<<<<<<<
+ *                 while tb is not None:
+ *                     try:
+ */
+      __Pyx_INCREF(__pyx_v_exc_tb);
+      __pyx_v_tb = __pyx_v_exc_tb;
+
+      /* "chorde/clients/_async.pyx":70
+ *                 # clear any non-running traceback's frames to avoid leaking locals
+ *                 tb = exc_tb
+ *                 while tb is not None:             # <<<<<<<<<<<<<<
+ *                     try:
+ *                         tb.tb_frame.clear()
+ */
+      while (1) {
+        __pyx_t_17 = (__pyx_v_tb != Py_None);
+        __pyx_t_6 = (__pyx_t_17 != 0);
+        if (!__pyx_t_6) break;
+
+        /* "chorde/clients/_async.pyx":71
+ *                 tb = exc_tb
+ *                 while tb is not None:
+ *                     try:             # <<<<<<<<<<<<<<
+ *                         tb.tb_frame.clear()
+ *                     except:
+ */
+        {
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __Pyx_ExceptionSave(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_14);
+          /*try:*/ {
+
+            /* "chorde/clients/_async.pyx":72
+ *                 while tb is not None:
+ *                     try:
+ *                         tb.tb_frame.clear()             # <<<<<<<<<<<<<<
+ *                     except:
+ *                         pass
+ */
+            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_tb, __pyx_n_s_tb_frame); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_4);
+            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            __pyx_t_4 = NULL;
+            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+              __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+              if (likely(__pyx_t_4)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+                __Pyx_INCREF(__pyx_t_4);
+                __Pyx_INCREF(function);
+                __Pyx_DECREF_SET(__pyx_t_2, function);
+              }
+            }
+            __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+            __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_1);
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+            /* "chorde/clients/_async.pyx":71
+ *                 tb = exc_tb
+ *                 while tb is not None:
+ *                     try:             # <<<<<<<<<<<<<<
+ *                         tb.tb_frame.clear()
+ *                     except:
+ */
+          }
+          __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+          __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+          goto __pyx_L27_try_end;
+          __pyx_L20_error:;
+          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+          /* "chorde/clients/_async.pyx":73
+ *                     try:
+ *                         tb.tb_frame.clear()
+ *                     except:             # <<<<<<<<<<<<<<
+ *                         pass
+ *                     tb = tb.tb_next
+ */
+          /*except:*/ {
+            __Pyx_ErrRestore(0,0,0);
+            goto __pyx_L21_exception_handled;
+          }
+          __pyx_L21_exception_handled:;
+          __Pyx_XGIVEREF(__pyx_t_16);
+          __Pyx_XGIVEREF(__pyx_t_15);
+          __Pyx_XGIVEREF(__pyx_t_14);
+          __Pyx_ExceptionReset(__pyx_t_16, __pyx_t_15, __pyx_t_14);
+          __pyx_L27_try_end:;
+        }
+
+        /* "chorde/clients/_async.pyx":75
+ *                     except:
+ *                         pass
+ *                     tb = tb.tb_next             # <<<<<<<<<<<<<<
+ * 
+ *                 if exc_obj is not None:
+ */
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_tb, __pyx_n_s_tb_next); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF_SET(__pyx_v_tb, __pyx_t_1);
+        __pyx_t_1 = 0;
+      }
+
+      /* "chorde/clients/_async.pyx":77
+ *                     tb = tb.tb_next
+ * 
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
-      __pyx_t_17 = (__pyx_v_exc_obj != Py_None);
-      __pyx_t_6 = (__pyx_t_17 != 0);
-      if (likely(__pyx_t_6)) {
+      __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
+      __pyx_t_17 = (__pyx_t_6 != 0);
+      if (likely(__pyx_t_17)) {
 
-        /* "chorde/clients/_async.pyx":69
- *             elif exc_tb is not None:
+        /* "chorde/clients/_async.pyx":78
+ * 
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
-        __pyx_t_1 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L12_error)
+        __pyx_t_1 = __Pyx_GetAttr(__pyx_v_exc_obj, __pyx_n_s_traceback); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = (__pyx_t_1 != __pyx_v_exc_tb);
+        __pyx_t_17 = (__pyx_t_1 != __pyx_v_exc_tb);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_17 = (__pyx_t_6 != 0);
-        if (__pyx_t_17) {
+        __pyx_t_6 = (__pyx_t_17 != 0);
+        if (__pyx_t_6) {
 
-          /* "chorde/clients/_async.pyx":70
+          /* "chorde/clients/_async.pyx":79
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *                     raise exc_obj
  *                 else:
  */
-          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L12_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-            __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-            if (likely(__pyx_t_2)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-              __Pyx_INCREF(__pyx_t_2);
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_exc_obj, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L12_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_4 = NULL;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+            __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+            if (likely(__pyx_t_4)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+              __Pyx_INCREF(__pyx_t_4);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_4, function);
+              __Pyx_DECREF_SET(__pyx_t_2, function);
             }
           }
-          __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_exc_tb);
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L12_error)
+          __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_exc_tb);
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF_SET(__pyx_v_exc_obj, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          /* "chorde/clients/_async.pyx":69
- *             elif exc_tb is not None:
+          /* "chorde/clients/_async.pyx":78
+ * 
  *                 if exc_obj is not None:
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:             # <<<<<<<<<<<<<<
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj
  */
         }
 
-        /* "chorde/clients/_async.pyx":71
+        /* "chorde/clients/_async.pyx":80
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  *                     raise exc_obj             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  */
         __Pyx_Raise(__pyx_v_exc_obj, 0, 0, 0);
-        __PYX_ERR(0, 71, __pyx_L12_error)
+        __PYX_ERR(0, 80, __pyx_L12_error)
 
-        /* "chorde/clients/_async.pyx":68
- *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
- *             elif exc_tb is not None:
+        /* "chorde/clients/_async.pyx":77
+ *                     tb = tb.tb_next
+ * 
  *                 if exc_obj is not None:             # <<<<<<<<<<<<<<
  *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
  *                         exc_obj = exc_obj.with_traceback(exc_tb)
  */
       }
 
-      /* "chorde/clients/_async.pyx":73
+      /* "chorde/clients/_async.pyx":82
  *                     raise exc_obj
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)             # <<<<<<<<<<<<<<
  *             elif exc_obj is not None:
  *                 raise exc_obj
  */
       /*else*/ {
         __Pyx_INCREF(__pyx_v_exc_typ);
-        __pyx_t_2 = __pyx_v_exc_typ; __pyx_t_3 = NULL;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+        __pyx_t_4 = __pyx_v_exc_typ; __pyx_t_3 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_2, function);
+            __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+        __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L12_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L12_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-          if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-            __Pyx_INCREF(__pyx_t_4);
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L12_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_2 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+          if (likely(__pyx_t_2)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+            __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_2, function);
+            __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_exc_tb);
-        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L12_error)
+        __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_v_exc_tb) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_exc_tb);
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __PYX_ERR(0, 73, __pyx_L12_error)
+        __PYX_ERR(0, 82, __pyx_L12_error)
       }
 
       /* "chorde/clients/_async.pyx":67
  *                     kwargs["reason"] = exc_obj.reason
  *                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
  *             elif exc_tb is not None:             # <<<<<<<<<<<<<<
- *                 if exc_obj is not None:
- *                     if getattr(exc_obj, '__traceback__') is not exc_tb:
+ *                 # clear any non-running traceback's frames to avoid leaking locals
+ *                 tb = exc_tb
  */
     }
 
-    /* "chorde/clients/_async.pyx":74
+    /* "chorde/clients/_async.pyx":83
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
-    __pyx_t_17 = (__pyx_v_exc_obj != Py_None);
-    __pyx_t_6 = (__pyx_t_17 != 0);
-    if (unlikely(__pyx_t_6)) {
+    __pyx_t_6 = (__pyx_v_exc_obj != Py_None);
+    __pyx_t_17 = (__pyx_t_6 != 0);
+    if (unlikely(__pyx_t_17)) {
 
-      /* "chorde/clients/_async.pyx":75
+      /* "chorde/clients/_async.pyx":84
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:
  *                 raise exc_obj             # <<<<<<<<<<<<<<
  *             else:
  *                 raise exc_typ()
  */
       __Pyx_Raise(__pyx_v_exc_obj, 0, 0, 0);
-      __PYX_ERR(0, 75, __pyx_L12_error)
+      __PYX_ERR(0, 84, __pyx_L12_error)
 
-      /* "chorde/clients/_async.pyx":74
+      /* "chorde/clients/_async.pyx":83
  *                 else:
  *                     raise exc_typ().with_traceback(exc_tb)
  *             elif exc_obj is not None:             # <<<<<<<<<<<<<<
  *                 raise exc_obj
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":77
+    /* "chorde/clients/_async.pyx":86
  *                 raise exc_obj
  *             else:
  *                 raise exc_typ()             # <<<<<<<<<<<<<<
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  */
     /*else*/ {
       __Pyx_INCREF(__pyx_v_exc_typ);
-      __pyx_t_2 = __pyx_v_exc_typ; __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_4);
+      __pyx_t_4 = __pyx_v_exc_typ; __pyx_t_2 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_2)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
-      __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L12_error)
+      __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 77, __pyx_L12_error)
+      __PYX_ERR(0, 86, __pyx_L12_error)
     }
   }
 
-  /* "chorde/clients/_async.pyx":80
+  /* "chorde/clients/_async.pyx":89
  *         finally:
  *             # Don't leave references to the exc/tb in the frame
  *             del exc_typ, exc_obj, exc_tb             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
   /*finally:*/ {
     __pyx_L12_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
-      __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
+      __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
-      if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14) < 0)) __Pyx_ErrFetch(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
-      __Pyx_XGOTREF(__pyx_t_16);
-      __Pyx_XGOTREF(__pyx_t_15);
+      if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16) < 0)) __Pyx_ErrFetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
       __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_16);
       __Pyx_XGOTREF(__pyx_t_13);
       __Pyx_XGOTREF(__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_11);
       __pyx_t_9 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_19 = __pyx_filename;
       {
         __Pyx_DECREF(__pyx_v_exc_typ);
         __pyx_v_exc_typ = NULL;
@@ -2702,19 +2827,19 @@
       }
       if (PY_MAJOR_VERSION >= 3) {
         __Pyx_XGIVEREF(__pyx_t_13);
         __Pyx_XGIVEREF(__pyx_t_12);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_12, __pyx_t_11);
       }
-      __Pyx_XGIVEREF(__pyx_t_16);
-      __Pyx_XGIVEREF(__pyx_t_15);
       __Pyx_XGIVEREF(__pyx_t_14);
-      __Pyx_ErrRestore(__pyx_t_16, __pyx_t_15, __pyx_t_14);
-      __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
+      __Pyx_XGIVEREF(__pyx_t_15);
+      __Pyx_XGIVEREF(__pyx_t_16);
+      __Pyx_ErrRestore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
+      __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0; __pyx_t_11 = 0;
       __pyx_lineno = __pyx_t_9; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_19;
       goto __pyx_L1_error;
     }
   }
 
   /* "chorde/clients/_async.pyx":50
  * 
@@ -2735,14 +2860,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_XDECREF(__pyx_v_exc_typ);
   __Pyx_XDECREF(__pyx_v_exc_obj);
   __Pyx_XDECREF(__pyx_v_exc_tb);
   __Pyx_XDECREF(__pyx_v_kwargs);
+  __Pyx_XDECREF(__pyx_v_tb);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6chorde_7clients_6_async_16ExceptionWrapper_3reraise(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -3039,15 +3165,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionWrapper.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":86
+/* "chorde/clients/_async.pyx":95
  *     cdef object me, callback, __weakref__
  * 
  *     def __cinit__(self, me, callback):             # <<<<<<<<<<<<<<
  *         self.me = wref(me)
  *         self.callback = callback
  */
 
@@ -3081,32 +3207,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_me)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 86, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 95, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 86, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 95, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_me = values[0];
     __pyx_v_callback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 86, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 95, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12WeakCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_WeakCallback *)__pyx_v_self), __pyx_v_me, __pyx_v_callback);
 
@@ -3122,15 +3248,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":87
+  /* "chorde/clients/_async.pyx":96
  * 
  *     def __cinit__(self, me, callback):
  *         self.me = wref(me)             # <<<<<<<<<<<<<<
  *         self.callback = callback
  * 
  */
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_wref);
@@ -3142,37 +3268,37 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_me) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_me);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->me);
   __Pyx_DECREF(__pyx_v_self->me);
   __pyx_v_self->me = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":88
+  /* "chorde/clients/_async.pyx":97
  *     def __cinit__(self, me, callback):
  *         self.me = wref(me)
  *         self.callback = callback             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, value):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":86
+  /* "chorde/clients/_async.pyx":95
  *     cdef object me, callback, __weakref__
  * 
  *     def __cinit__(self, me, callback):             # <<<<<<<<<<<<<<
  *         self.me = wref(me)
  *         self.callback = callback
  */
 
@@ -3186,15 +3312,15 @@
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":90
+/* "chorde/clients/_async.pyx":99
  *         self.callback = callback
  * 
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         cdef object me
  *         me = self.me()
  */
 
@@ -3223,26 +3349,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 99, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 99, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12WeakCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_WeakCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3261,15 +3387,15 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":92
+  /* "chorde/clients/_async.pyx":101
  *     def __call__(self, value):
  *         cdef object me
  *         me = self.me()             # <<<<<<<<<<<<<<
  *         if me is not None:
  *             return self.callback(me)
  */
   __Pyx_INCREF(__pyx_v_self->me);
@@ -3281,32 +3407,32 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_me = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":93
+  /* "chorde/clients/_async.pyx":102
  *         cdef object me
  *         me = self.me()
  *         if me is not None:             # <<<<<<<<<<<<<<
  *             return self.callback(me)
  * 
  */
   __pyx_t_4 = (__pyx_v_me != Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "chorde/clients/_async.pyx":94
+    /* "chorde/clients/_async.pyx":103
  *         me = self.me()
  *         if me is not None:
  *             return self.callback(me)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -3319,31 +3445,31 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_me) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_me);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":93
+    /* "chorde/clients/_async.pyx":102
  *         cdef object me
  *         me = self.me()
  *         if me is not None:             # <<<<<<<<<<<<<<
  *             return self.callback(me)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":90
+  /* "chorde/clients/_async.pyx":99
  *         self.callback = callback
  * 
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         cdef object me
  *         me = self.me()
  */
 
@@ -3472,15 +3598,15 @@
   __Pyx_AddTraceback("chorde.clients._async.WeakCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":99
+/* "chorde/clients/_async.pyx":108
  * cdef class DeferExceptionCallback:
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):             # <<<<<<<<<<<<<<
  *         self.defer = defer
  *     def __call__(self, value):
  */
 
@@ -3509,26 +3635,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defer)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 99, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 108, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_defer = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 99, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 108, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *)__pyx_v_self), __pyx_v_defer);
 
@@ -3538,42 +3664,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *__pyx_v_self, PyObject *__pyx_v_defer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":100
+  /* "chorde/clients/_async.pyx":109
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):
  *         self.defer = defer             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         self.defer.set_exception(value[1] or value[0])
  */
   __Pyx_INCREF(__pyx_v_defer);
   __Pyx_GIVEREF(__pyx_v_defer);
   __Pyx_GOTREF(__pyx_v_self->defer);
   __Pyx_DECREF(__pyx_v_self->defer);
   __pyx_v_self->defer = __pyx_v_defer;
 
-  /* "chorde/clients/_async.pyx":99
+  /* "chorde/clients/_async.pyx":108
  * cdef class DeferExceptionCallback:
  *     cdef object defer, __weakref__
  *     def __cinit__(self, defer):             # <<<<<<<<<<<<<<
  *         self.defer = defer
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":101
+/* "chorde/clients/_async.pyx":110
  *     def __cinit__(self, defer):
  *         self.defer = defer
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         self.defer.set_exception(value[1] or value[0])
  * 
  */
 
@@ -3602,26 +3728,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 101, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_22DeferExceptionCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3639,35 +3765,35 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":102
+  /* "chorde/clients/_async.pyx":111
  *         self.defer = defer
  *     def __call__(self, value):
  *         self.defer.set_exception(value[1] or value[0])             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
   if (!__pyx_t_5) {
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
@@ -3678,20 +3804,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":101
+  /* "chorde/clients/_async.pyx":110
  *     def __cinit__(self, defer):
  *         self.defer = defer
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         self.defer.set_exception(value[1] or value[0])
  * 
  */
 
@@ -3820,15 +3946,15 @@
   __Pyx_AddTraceback("chorde.clients._async.DeferExceptionCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":107
+/* "chorde/clients/_async.pyx":116
  * cdef class ValueCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -3857,26 +3983,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 107, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 107, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_13ValueCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -3886,42 +4012,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_13ValueCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":108
+  /* "chorde/clients/_async.pyx":117
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":107
+  /* "chorde/clients/_async.pyx":116
  * cdef class ValueCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":109
+/* "chorde/clients/_async.pyx":118
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -3950,26 +4076,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 109, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 109, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_13ValueCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_ValueCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -3988,15 +4114,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":110
+  /* "chorde/clients/_async.pyx":119
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_2 = (__pyx_v_value != __pyx_v_6chorde_7clients_6_async_CacheMissError);
@@ -4008,15 +4134,15 @@
   }
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":111
+    /* "chorde/clients/_async.pyx":120
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4029,31 +4155,31 @@
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":110
+    /* "chorde/clients/_async.pyx":119
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":109
+  /* "chorde/clients/_async.pyx":118
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is not CacheMissError and not isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4181,15 +4307,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ValueCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":116
+/* "chorde/clients/_async.pyx":125
  * cdef class MissCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4218,26 +4344,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 116, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12MissCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_MissCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4247,42 +4373,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_12MissCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_MissCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":117
+  /* "chorde/clients/_async.pyx":126
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is CacheMissError:
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":116
+  /* "chorde/clients/_async.pyx":125
  * cdef class MissCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":118
+/* "chorde/clients/_async.pyx":127
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             return self.callback(value)
  */
 
@@ -4311,26 +4437,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 127, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12MissCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_MissCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4348,26 +4474,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":119
+  /* "chorde/clients/_async.pyx":128
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":120
+    /* "chorde/clients/_async.pyx":129
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4380,31 +4506,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":119
+    /* "chorde/clients/_async.pyx":128
  *         self.callback = callback
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":118
+  /* "chorde/clients/_async.pyx":127
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             return self.callback(value)
  */
 
@@ -4532,15 +4658,15 @@
   __Pyx_AddTraceback("chorde.clients._async.MissCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":125
+/* "chorde/clients/_async.pyx":134
  * cdef class ExceptionCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -4569,26 +4695,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -4598,42 +4724,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":126
+  /* "chorde/clients/_async.pyx":135
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":125
+  /* "chorde/clients/_async.pyx":134
  * cdef class ExceptionCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":127
+/* "chorde/clients/_async.pyx":136
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4662,26 +4788,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 127, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 136, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_17ExceptionCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -4699,26 +4825,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":128
+  /* "chorde/clients/_async.pyx":137
  *         self.callback = callback
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":129
+    /* "chorde/clients/_async.pyx":138
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4731,31 +4857,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":128
+    /* "chorde/clients/_async.pyx":137
  *         self.callback = callback
  *     def __call__(self, value):
  *         if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             return self.callback(value)
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":127
+  /* "chorde/clients/_async.pyx":136
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, ExceptionWrapper):
  *             return self.callback(value)
  */
 
@@ -4883,15 +5009,15 @@
   __Pyx_AddTraceback("chorde.clients._async.ExceptionCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":134
+/* "chorde/clients/_async.pyx":143
  * cdef class AnyCallback:
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):             # <<<<<<<<<<<<<<
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  */
 
@@ -4928,40 +5054,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_miss)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 134, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 143, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 134, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 143, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 143, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 143, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_11AnyCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -4971,68 +5097,68 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_11AnyCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *__pyx_v_self, PyObject *__pyx_v_on_value, PyObject *__pyx_v_on_miss, PyObject *__pyx_v_on_exc) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":135
+  /* "chorde/clients/_async.pyx":144
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):
  *         self.on_value = on_value             # <<<<<<<<<<<<<<
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  */
   __Pyx_INCREF(__pyx_v_on_value);
   __Pyx_GIVEREF(__pyx_v_on_value);
   __Pyx_GOTREF(__pyx_v_self->on_value);
   __Pyx_DECREF(__pyx_v_self->on_value);
   __pyx_v_self->on_value = __pyx_v_on_value;
 
-  /* "chorde/clients/_async.pyx":136
+  /* "chorde/clients/_async.pyx":145
  *     def __cinit__(self, on_value, on_miss, on_exc):
  *         self.on_value = on_value
  *         self.on_miss = on_miss             # <<<<<<<<<<<<<<
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  */
   __Pyx_INCREF(__pyx_v_on_miss);
   __Pyx_GIVEREF(__pyx_v_on_miss);
   __Pyx_GOTREF(__pyx_v_self->on_miss);
   __Pyx_DECREF(__pyx_v_self->on_miss);
   __pyx_v_self->on_miss = __pyx_v_on_miss;
 
-  /* "chorde/clients/_async.pyx":137
+  /* "chorde/clients/_async.pyx":146
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         if value is CacheMissError:
  */
   __Pyx_INCREF(__pyx_v_on_exc);
   __Pyx_GIVEREF(__pyx_v_on_exc);
   __Pyx_GOTREF(__pyx_v_self->on_exc);
   __Pyx_DECREF(__pyx_v_self->on_exc);
   __pyx_v_self->on_exc = __pyx_v_on_exc;
 
-  /* "chorde/clients/_async.pyx":134
+  /* "chorde/clients/_async.pyx":143
  * cdef class AnyCallback:
  *     cdef object on_value, on_miss, on_exc, __weakref__
  *     def __cinit__(self, on_value, on_miss, on_exc):             # <<<<<<<<<<<<<<
  *         self.on_value = on_value
  *         self.on_miss = on_miss
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":138
+/* "chorde/clients/_async.pyx":147
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  */
 
@@ -5061,26 +5187,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 138, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 147, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 138, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 147, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_11AnyCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_AnyCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -5098,37 +5224,37 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":139
+  /* "chorde/clients/_async.pyx":148
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  */
   __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":140
+    /* "chorde/clients/_async.pyx":149
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             if self.on_miss is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  */
     __pyx_t_2 = (__pyx_v_self->on_miss != Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":141
+      /* "chorde/clients/_async.pyx":150
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  *                 return self.on_miss()             # <<<<<<<<<<<<<<
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5141,63 +5267,63 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":140
+      /* "chorde/clients/_async.pyx":149
  *     def __call__(self, value):
  *         if value is CacheMissError:
  *             if self.on_miss is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  */
     }
 
-    /* "chorde/clients/_async.pyx":139
+    /* "chorde/clients/_async.pyx":148
  *         self.on_exc = on_exc
  *     def __call__(self, value):
  *         if value is CacheMissError:             # <<<<<<<<<<<<<<
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":142
+  /* "chorde/clients/_async.pyx":151
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":143
+    /* "chorde/clients/_async.pyx":152
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  */
     __pyx_t_2 = (__pyx_v_self->on_exc != Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":144
+      /* "chorde/clients/_async.pyx":153
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)             # <<<<<<<<<<<<<<
  *         else:
  *             if self.on_value is not None:
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5210,53 +5336,53 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_value)->value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_value)->value);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":143
+      /* "chorde/clients/_async.pyx":152
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):
  *             if self.on_exc is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":142
+    /* "chorde/clients/_async.pyx":151
  *             if self.on_miss is not None:
  *                 return self.on_miss()
  *         elif isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *             if self.on_exc is not None:
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":146
+  /* "chorde/clients/_async.pyx":155
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  *             if self.on_value is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_value(value)
  * 
  */
   /*else*/ {
     __pyx_t_1 = (__pyx_v_self->on_value != Py_None);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "chorde/clients/_async.pyx":147
+      /* "chorde/clients/_async.pyx":156
  *         else:
  *             if self.on_value is not None:
  *                 return self.on_value(value)             # <<<<<<<<<<<<<<
  * 
  * @cython.freelist(100)
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5269,33 +5395,33 @@
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":146
+      /* "chorde/clients/_async.pyx":155
  *                 return self.on_exc((<ExceptionWrapper>value).value)
  *         else:
  *             if self.on_value is not None:             # <<<<<<<<<<<<<<
  *                 return self.on_value(value)
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":138
+  /* "chorde/clients/_async.pyx":147
  *         self.on_miss = on_miss
  *         self.on_exc = on_exc
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         if value is CacheMissError:
  *             if self.on_miss is not None:
  */
 
@@ -5423,15 +5549,15 @@
   __Pyx_AddTraceback("chorde.clients._async.AnyCallback.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":152
+/* "chorde/clients/_async.pyx":161
  * cdef class DoneCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
@@ -5460,26 +5586,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 152, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 152, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 161, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DoneCallback.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12DoneCallback___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *)__pyx_v_self), __pyx_v_callback);
 
@@ -5489,42 +5615,42 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_12DoneCallback___cinit__(struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *__pyx_v_self, PyObject *__pyx_v_callback) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":153
+  /* "chorde/clients/_async.pyx":162
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):
  *         self.callback = callback             # <<<<<<<<<<<<<<
  *     def __call__(self, value):
  *         return self.callback()
  */
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   __Pyx_GOTREF(__pyx_v_self->callback);
   __Pyx_DECREF(__pyx_v_self->callback);
   __pyx_v_self->callback = __pyx_v_callback;
 
-  /* "chorde/clients/_async.pyx":152
+  /* "chorde/clients/_async.pyx":161
  * cdef class DoneCallback:
  *     cdef object callback, __weakref__
  *     def __cinit__(self, callback):             # <<<<<<<<<<<<<<
  *         self.callback = callback
  *     def __call__(self, value):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":154
+/* "chorde/clients/_async.pyx":163
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         return self.callback()
  * 
  */
 
@@ -5553,26 +5679,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 154, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(0, 163, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 154, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 163, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.DoneCallback.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_12DoneCallback_2__call__(((struct __pyx_obj_6chorde_7clients_6_async_DoneCallback *)__pyx_v_self), __pyx_v_value);
 
@@ -5588,15 +5714,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "chorde/clients/_async.pyx":155
+  /* "chorde/clients/_async.pyx":164
  *         self.callback = callback
  *     def __call__(self, value):
  *         return self.callback()             # <<<<<<<<<<<<<<
  * 
  * cdef class NONE:
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5609,22 +5735,22 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":154
+  /* "chorde/clients/_async.pyx":163
  *     def __cinit__(self, callback):
  *         self.callback = callback
  *     def __call__(self, value):             # <<<<<<<<<<<<<<
  *         return self.callback()
  * 
  */
 
@@ -6037,15 +6163,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":162
+/* "chorde/clients/_async.pyx":171
  * @cython.freelist(100)
  * cdef class Future:
  *     def __cinit__(self, logger = None):             # <<<<<<<<<<<<<<
  *         self._cb = None
  *         self._value = NONE
  */
 
@@ -6077,29 +6203,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_logger);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 162, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 171, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_logger = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 162, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 171, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_logger);
 
@@ -6109,108 +6235,108 @@
 }
 
 static int __pyx_pf_6chorde_7clients_6_async_6Future___cinit__(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self, PyObject *__pyx_v_logger) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "chorde/clients/_async.pyx":163
+  /* "chorde/clients/_async.pyx":172
  * cdef class Future:
  *     def __cinit__(self, logger = None):
  *         self._cb = None             # <<<<<<<<<<<<<<
  *         self._value = NONE
  *         self._logger = logger
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_cb);
   __Pyx_DECREF(__pyx_v_self->_cb);
   __pyx_v_self->_cb = ((PyObject*)Py_None);
 
-  /* "chorde/clients/_async.pyx":164
+  /* "chorde/clients/_async.pyx":173
  *     def __cinit__(self, logger = None):
  *         self._cb = None
  *         self._value = NONE             # <<<<<<<<<<<<<<
  *         self._logger = logger
  *         self._done_event = None
  */
   __Pyx_INCREF(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __Pyx_GOTREF(__pyx_v_self->_value);
   __Pyx_DECREF(__pyx_v_self->_value);
   __pyx_v_self->_value = ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE);
 
-  /* "chorde/clients/_async.pyx":165
+  /* "chorde/clients/_async.pyx":174
  *         self._cb = None
  *         self._value = NONE
  *         self._logger = logger             # <<<<<<<<<<<<<<
  *         self._done_event = None
  *         self._running = 0
  */
   __Pyx_INCREF(__pyx_v_logger);
   __Pyx_GIVEREF(__pyx_v_logger);
   __Pyx_GOTREF(__pyx_v_self->_logger);
   __Pyx_DECREF(__pyx_v_self->_logger);
   __pyx_v_self->_logger = __pyx_v_logger;
 
-  /* "chorde/clients/_async.pyx":166
+  /* "chorde/clients/_async.pyx":175
  *         self._value = NONE
  *         self._logger = logger
  *         self._done_event = None             # <<<<<<<<<<<<<<
  *         self._running = 0
  *         self._cancel_pending = 0
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_done_event);
   __Pyx_DECREF(__pyx_v_self->_done_event);
   __pyx_v_self->_done_event = Py_None;
 
-  /* "chorde/clients/_async.pyx":167
+  /* "chorde/clients/_async.pyx":176
  *         self._logger = logger
  *         self._done_event = None
  *         self._running = 0             # <<<<<<<<<<<<<<
  *         self._cancel_pending = 0
  *         self._cancelled = 0
  */
   __pyx_v_self->_running = 0;
 
-  /* "chorde/clients/_async.pyx":168
+  /* "chorde/clients/_async.pyx":177
  *         self._done_event = None
  *         self._running = 0
  *         self._cancel_pending = 0             # <<<<<<<<<<<<<<
  *         self._cancelled = 0
  * 
  */
   __pyx_v_self->_cancel_pending = 0;
 
-  /* "chorde/clients/_async.pyx":169
+  /* "chorde/clients/_async.pyx":178
  *         self._running = 0
  *         self._cancel_pending = 0
  *         self._cancelled = 0             # <<<<<<<<<<<<<<
  * 
  *     cpdef _set_nothreads(self, value):
  */
   __pyx_v_self->_cancelled = 0;
 
-  /* "chorde/clients/_async.pyx":162
+  /* "chorde/clients/_async.pyx":171
  * @cython.freelist(100)
  * cdef class Future:
  *     def __cinit__(self, logger = None):             # <<<<<<<<<<<<<<
  *         self._cb = None
  *         self._value = NONE
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":171
+/* "chorde/clients/_async.pyx":180
  *         self._cancelled = 0
  * 
  *     cpdef _set_nothreads(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Like set(), but assuming no threading is involved. It won't wake waiting threads,
  */
 
@@ -6245,15 +6371,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_nothreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_nothreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_3_set_nothreads)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6262,15 +6388,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6283,236 +6409,236 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":179
+  /* "chorde/clients/_async.pyx":188
  *         cdef object old, cbs, _cb
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             # No setting twice
  *             return
  */
   __pyx_t_5 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":181
+    /* "chorde/clients/_async.pyx":190
  *         if self._value is not NONE:
  *             # No setting twice
  *             return             # <<<<<<<<<<<<<<
  * 
  *         # start atomic op
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":179
+    /* "chorde/clients/_async.pyx":188
  *         cdef object old, cbs, _cb
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             # No setting twice
  *             return
  */
   }
 
-  /* "chorde/clients/_async.pyx":184
+  /* "chorde/clients/_async.pyx":193
  * 
  *         # start atomic op
  *         old = self._value # avoid deadlocks due to finalizers             # <<<<<<<<<<<<<<
  *         _cb = self._cb
  *         if _cb is not None:
  */
   __pyx_t_1 = __pyx_v_self->_value;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_old = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":185
+  /* "chorde/clients/_async.pyx":194
  *         # start atomic op
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb             # <<<<<<<<<<<<<<
  *         if _cb is not None:
  *             self._cb = None
  */
   __pyx_t_1 = __pyx_v_self->_cb;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v__cb = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":186
+  /* "chorde/clients/_async.pyx":195
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb
  *         if _cb is not None:             # <<<<<<<<<<<<<<
  *             self._cb = None
  *             self._value = value
  */
   __pyx_t_6 = (__pyx_v__cb != Py_None);
   __pyx_t_5 = (__pyx_t_6 != 0);
   if (__pyx_t_5) {
 
-    /* "chorde/clients/_async.pyx":187
+    /* "chorde/clients/_async.pyx":196
  *         _cb = self._cb
  *         if _cb is not None:
  *             self._cb = None             # <<<<<<<<<<<<<<
  *             self._value = value
  *             cbs = list(_cb) # end atomic op
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_cb);
     __Pyx_DECREF(__pyx_v_self->_cb);
     __pyx_v_self->_cb = ((PyObject*)Py_None);
 
-    /* "chorde/clients/_async.pyx":188
+    /* "chorde/clients/_async.pyx":197
  *         if _cb is not None:
  *             self._cb = None
  *             self._value = value             # <<<<<<<<<<<<<<
  *             cbs = list(_cb) # end atomic op
  *         else:
  */
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     __Pyx_GOTREF(__pyx_v_self->_value);
     __Pyx_DECREF(__pyx_v_self->_value);
     __pyx_v_self->_value = __pyx_v_value;
 
-    /* "chorde/clients/_async.pyx":189
+    /* "chorde/clients/_async.pyx":198
  *             self._cb = None
  *             self._value = value
  *             cbs = list(_cb) # end atomic op             # <<<<<<<<<<<<<<
  *         else:
  *             cbs = None
  */
-    __pyx_t_1 = PySequence_List(__pyx_v__cb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+    __pyx_t_1 = PySequence_List(__pyx_v__cb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_cbs = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":186
+    /* "chorde/clients/_async.pyx":195
  *         old = self._value # avoid deadlocks due to finalizers
  *         _cb = self._cb
  *         if _cb is not None:             # <<<<<<<<<<<<<<
  *             self._cb = None
  *             self._value = value
  */
     goto __pyx_L4;
   }
 
-  /* "chorde/clients/_async.pyx":191
+  /* "chorde/clients/_async.pyx":200
  *             cbs = list(_cb) # end atomic op
  *         else:
  *             cbs = None             # <<<<<<<<<<<<<<
  *             self._value = value # end atomic op
  *         self._running = 0
  */
   /*else*/ {
     __Pyx_INCREF(Py_None);
     __pyx_v_cbs = Py_None;
 
-    /* "chorde/clients/_async.pyx":192
+    /* "chorde/clients/_async.pyx":201
  *         else:
  *             cbs = None
  *             self._value = value # end atomic op             # <<<<<<<<<<<<<<
  *         self._running = 0
  *         del old, _cb
  */
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     __Pyx_GOTREF(__pyx_v_self->_value);
     __Pyx_DECREF(__pyx_v_self->_value);
     __pyx_v_self->_value = __pyx_v_value;
   }
   __pyx_L4:;
 
-  /* "chorde/clients/_async.pyx":193
+  /* "chorde/clients/_async.pyx":202
  *             cbs = None
  *             self._value = value # end atomic op
  *         self._running = 0             # <<<<<<<<<<<<<<
  *         del old, _cb
  * 
  */
   __pyx_v_self->_running = 0;
 
-  /* "chorde/clients/_async.pyx":194
+  /* "chorde/clients/_async.pyx":203
  *             self._value = value # end atomic op
  *         self._running = 0
  *         del old, _cb             # <<<<<<<<<<<<<<
  * 
  *         if cbs is not None:
  */
   __Pyx_DECREF(__pyx_v_old);
   __pyx_v_old = NULL;
   __Pyx_DECREF(__pyx_v__cb);
   __pyx_v__cb = NULL;
 
-  /* "chorde/clients/_async.pyx":196
+  /* "chorde/clients/_async.pyx":205
  *         del old, _cb
  * 
  *         if cbs is not None:             # <<<<<<<<<<<<<<
  *             for cb in cbs:
  *                 try:
  */
   __pyx_t_5 = (__pyx_v_cbs != Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":197
+    /* "chorde/clients/_async.pyx":206
  * 
  *         if cbs is not None:
  *             for cb in cbs:             # <<<<<<<<<<<<<<
  *                 try:
  *                     cb(value)
  */
     if (likely(PyList_CheckExact(__pyx_v_cbs)) || PyTuple_CheckExact(__pyx_v_cbs)) {
       __pyx_t_1 = __pyx_v_cbs; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cbs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cbs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 197, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_8(__pyx_t_1);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 197, __pyx_L1_error)
+            else __PYX_ERR(0, 206, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_v_cb, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "chorde/clients/_async.pyx":198
+      /* "chorde/clients/_async.pyx":207
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
       {
@@ -6520,15 +6646,15 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
         /*try:*/ {
 
-          /* "chorde/clients/_async.pyx":199
+          /* "chorde/clients/_async.pyx":208
  *             for cb in cbs:
  *                 try:
  *                     cb(value)             # <<<<<<<<<<<<<<
  *                 except:
  *                     if self._logger is not None:
  */
           __Pyx_INCREF(__pyx_v_cb);
@@ -6540,20 +6666,20 @@
               __Pyx_INCREF(__pyx_t_4);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L8_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "chorde/clients/_async.pyx":198
+          /* "chorde/clients/_async.pyx":207
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
         }
@@ -6562,101 +6688,101 @@
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L15_try_end;
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "chorde/clients/_async.pyx":200
+        /* "chorde/clients/_async.pyx":209
  *                 try:
  *                     cb(value)
  *                 except:             # <<<<<<<<<<<<<<
  *                     if self._logger is not None:
  *                         error = self._logger
  */
         /*except:*/ {
           __Pyx_AddTraceback("chorde.clients._async.Future._set_nothreads", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 200, __pyx_L10_except_error)
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 209, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_4);
 
-          /* "chorde/clients/_async.pyx":201
+          /* "chorde/clients/_async.pyx":210
  *                     cb(value)
  *                 except:
  *                     if self._logger is not None:             # <<<<<<<<<<<<<<
  *                         error = self._logger
  *                     else:
  */
           __pyx_t_6 = (__pyx_v_self->_logger != Py_None);
           __pyx_t_5 = (__pyx_t_6 != 0);
           if (__pyx_t_5) {
 
-            /* "chorde/clients/_async.pyx":202
+            /* "chorde/clients/_async.pyx":211
  *                 except:
  *                     if self._logger is not None:
  *                         error = self._logger             # <<<<<<<<<<<<<<
  *                     else:
  *                         error = logging.error
  */
             __pyx_t_12 = __pyx_v_self->_logger;
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_XDECREF_SET(__pyx_v_error, __pyx_t_12);
             __pyx_t_12 = 0;
 
-            /* "chorde/clients/_async.pyx":201
+            /* "chorde/clients/_async.pyx":210
  *                     cb(value)
  *                 except:
  *                     if self._logger is not None:             # <<<<<<<<<<<<<<
  *                         error = self._logger
  *                     else:
  */
             goto __pyx_L18;
           }
 
-          /* "chorde/clients/_async.pyx":204
+          /* "chorde/clients/_async.pyx":213
  *                         error = self._logger
  *                     else:
  *                         error = logging.error             # <<<<<<<<<<<<<<
  *                     error("Error in async callback", exc_info = True)
  * 
  */
           /*else*/ {
-            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 204, __pyx_L10_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 213, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 204, __pyx_L10_except_error)
+            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 213, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_13);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_XDECREF_SET(__pyx_v_error, __pyx_t_13);
             __pyx_t_13 = 0;
           }
           __pyx_L18:;
 
-          /* "chorde/clients/_async.pyx":205
+          /* "chorde/clients/_async.pyx":214
  *                     else:
  *                         error = logging.error
  *                     error("Error in async callback", exc_info = True)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set(self, value):
  */
-          __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 205, __pyx_L10_except_error)
+          __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 214, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_13);
-          if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_exc_info, Py_True) < 0) __PYX_ERR(0, 205, __pyx_L10_except_error)
-          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_v_error, __pyx_tuple__17, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 205, __pyx_L10_except_error)
+          if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_exc_info, Py_True) < 0) __PYX_ERR(0, 214, __pyx_L10_except_error)
+          __pyx_t_12 = __Pyx_PyObject_Call(__pyx_v_error, __pyx_tuple__17, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 214, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L9_exception_handled;
         }
         __pyx_L10_except_error:;
 
-        /* "chorde/clients/_async.pyx":198
+        /* "chorde/clients/_async.pyx":207
  *         if cbs is not None:
  *             for cb in cbs:
  *                 try:             # <<<<<<<<<<<<<<
  *                     cb(value)
  *                 except:
  */
         __Pyx_XGIVEREF(__pyx_t_9);
@@ -6668,34 +6794,34 @@
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
         __pyx_L15_try_end:;
       }
 
-      /* "chorde/clients/_async.pyx":197
+      /* "chorde/clients/_async.pyx":206
  * 
  *         if cbs is not None:
  *             for cb in cbs:             # <<<<<<<<<<<<<<
  *                 try:
  *                     cb(value)
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":196
+    /* "chorde/clients/_async.pyx":205
  *         del old, _cb
  * 
  *         if cbs is not None:             # <<<<<<<<<<<<<<
  *             for cb in cbs:
  *                 try:
  */
   }
 
-  /* "chorde/clients/_async.pyx":171
+  /* "chorde/clients/_async.pyx":180
  *         self._cancelled = 0
  * 
  *     cpdef _set_nothreads(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Like set(), but assuming no threading is involved. It won't wake waiting threads,
  */
 
@@ -6741,15 +6867,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_nothreads", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__set_nothreads(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__set_nothreads(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6758,15 +6884,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":207
+/* "chorde/clients/_async.pyx":216
  *                     error("Error in async callback", exc_info = True)
  * 
  *     cpdef set(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Set the future's result as either a value, an exception wrappedn in ExceptionWrapper, or
  */
 
@@ -6789,15 +6915,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_5set)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6806,15 +6932,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6827,72 +6953,72 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":212
+  /* "chorde/clients/_async.pyx":221
  *         a cache miss if given CacheMissError (the class itself)
  *         """
  *         self._set_nothreads(value)             # <<<<<<<<<<<<<<
  * 
  *         if self._done_event is not None:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":214
+  /* "chorde/clients/_async.pyx":223
  *         self._set_nothreads(value)
  * 
  *         if self._done_event is not None:             # <<<<<<<<<<<<<<
  *             # wake up waiting threads
  *             self._done_event.set()
  */
   __pyx_t_5 = (__pyx_v_self->_done_event != Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":216
+    /* "chorde/clients/_async.pyx":225
  *         if self._done_event is not None:
  *             # wake up waiting threads
  *             self._done_event.set()             # <<<<<<<<<<<<<<
  * 
  *     def set_result(self, value):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "chorde/clients/_async.pyx":214
+    /* "chorde/clients/_async.pyx":223
  *         self._set_nothreads(value)
  * 
  *         if self._done_event is not None:             # <<<<<<<<<<<<<<
  *             # wake up waiting threads
  *             self._done_event.set()
  */
   }
 
-  /* "chorde/clients/_async.pyx":207
+  /* "chorde/clients/_async.pyx":216
  *                     error("Error in async callback", exc_info = True)
  * 
  *     cpdef set(self, value):             # <<<<<<<<<<<<<<
  *         """
  *         Set the future's result as either a value, an exception wrappedn in ExceptionWrapper, or
  */
 
@@ -6931,15 +7057,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future_set(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future_set(__pyx_v_self, __pyx_v_value, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6948,15 +7074,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":218
+/* "chorde/clients/_async.pyx":227
  *             self._done_event.set()
  * 
  *     def set_result(self, value):             # <<<<<<<<<<<<<<
  *         self.set(value)
  * 
  */
 
@@ -6978,26 +7104,26 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_result", 0);
 
-  /* "chorde/clients/_async.pyx":219
+  /* "chorde/clients/_async.pyx":228
  * 
  *     def set_result(self, value):
  *         self.set(value)             # <<<<<<<<<<<<<<
  * 
  *     def miss(self):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":218
+  /* "chorde/clients/_async.pyx":227
  *             self._done_event.set()
  * 
  *     def set_result(self, value):             # <<<<<<<<<<<<<<
  *         self.set(value)
  * 
  */
 
@@ -7010,15 +7136,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":221
+/* "chorde/clients/_async.pyx":230
  *         self.set(value)
  * 
  *     def miss(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result
  */
 
@@ -7042,29 +7168,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("miss", 0);
 
-  /* "chorde/clients/_async.pyx":225
+  /* "chorde/clients/_async.pyx":234
  *         Shorthand for setting a cache miss result
  *         """
  *         self.set(CacheMissError)             # <<<<<<<<<<<<<<
  * 
  *     def _miss_nothreads(self):
  */
   __pyx_t_1 = __pyx_v_6chorde_7clients_6_async_CacheMissError;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":221
+  /* "chorde/clients/_async.pyx":230
  *         self.set(value)
  * 
  *     def miss(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result
  */
 
@@ -7078,15 +7204,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":227
+/* "chorde/clients/_async.pyx":236
  *         self.set(CacheMissError)
  * 
  *     def _miss_nothreads(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result without thread safety.
  */
 
@@ -7110,29 +7236,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_miss_nothreads", 0);
 
-  /* "chorde/clients/_async.pyx":232
+  /* "chorde/clients/_async.pyx":241
  *         See _set_nothreads
  *         """
  *         self._set_nothreads(CacheMissError)             # <<<<<<<<<<<<<<
  * 
  *     def exc(self, exc_info):
  */
   __pyx_t_1 = __pyx_v_6chorde_7clients_6_async_CacheMissError;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":227
+  /* "chorde/clients/_async.pyx":236
  *         self.set(CacheMissError)
  * 
  *     def _miss_nothreads(self):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting a cache miss result without thread safety.
  */
 
@@ -7146,15 +7272,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":234
+/* "chorde/clients/_async.pyx":243
  *         self._set_nothreads(CacheMissError)
  * 
  *     def exc(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7178,35 +7304,35 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exc", 0);
 
-  /* "chorde/clients/_async.pyx":239
+  /* "chorde/clients/_async.pyx":248
  *         as returned by sys.exc_info()
  *         """
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))             # <<<<<<<<<<<<<<
  * 
  *     def _exc_nothreads(self, exc_info):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_exc_info);
   __Pyx_GIVEREF(__pyx_v_exc_info);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_exc_info);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->set(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":234
+  /* "chorde/clients/_async.pyx":243
  *         self._set_nothreads(CacheMissError)
  * 
  *     def exc(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7220,15 +7346,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":241
+/* "chorde/clients/_async.pyx":250
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def _exc_nothreads(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7252,35 +7378,35 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_exc_nothreads", 0);
 
-  /* "chorde/clients/_async.pyx":247
+  /* "chorde/clients/_async.pyx":256
  *         See _set_nothreads
  *         """
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))             # <<<<<<<<<<<<<<
  * 
  *     def set_exception(self, exception):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_exc_info);
   __Pyx_GIVEREF(__pyx_v_exc_info);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_exc_info);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionWrapper(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_set_nothreads(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "chorde/clients/_async.pyx":241
+  /* "chorde/clients/_async.pyx":250
  *         self.set(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def _exc_nothreads(self, exc_info):             # <<<<<<<<<<<<<<
  *         """
  *         Shorthand for setting an exception result from an exc_info tuple
  */
 
@@ -7294,15 +7420,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":249
+/* "chorde/clients/_async.pyx":258
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def set_exception(self, exception):             # <<<<<<<<<<<<<<
  *         """
  *         Set the Future's exception object.
  */
 
@@ -7332,82 +7458,82 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_exception", 0);
   __Pyx_INCREF(__pyx_v_exception);
 
-  /* "chorde/clients/_async.pyx":253
+  /* "chorde/clients/_async.pyx":262
  *         Set the Future's exception object.
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:             # <<<<<<<<<<<<<<
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))
  */
   __pyx_t_2 = (__pyx_v_6chorde_7clients_6_async_strip_tracebacks != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_exception, __pyx_n_s_traceback, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_exception, __pyx_n_s_traceback, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = (__pyx_t_3 != Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":254
+    /* "chorde/clients/_async.pyx":263
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:
  *             exception = exception.with_traceback(None)             # <<<<<<<<<<<<<<
  *         self.exc((type(exception),exception,None))
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_exception, __pyx_n_s_with_traceback); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, Py_None) : __Pyx_PyObject_CallOneArg(__pyx_t_5, Py_None);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 254, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_exception, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":253
+    /* "chorde/clients/_async.pyx":262
  *         Set the Future's exception object.
  *         """
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:             # <<<<<<<<<<<<<<
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))
  */
   }
 
-  /* "chorde/clients/_async.pyx":255
+  /* "chorde/clients/_async.pyx":264
  *         if strip_tracebacks and getattr(exception, '__traceback__', None) is not None:
  *             exception = exception.with_traceback(None)
  *         self.exc((type(exception),exception,None))             # <<<<<<<<<<<<<<
  * 
  *     def on_value(self, callback):
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_exc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_exc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_exception)));
   __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_exception)));
   PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)Py_TYPE(__pyx_v_exception)));
   __Pyx_INCREF(__pyx_v_exception);
   __Pyx_GIVEREF(__pyx_v_exception);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_exception);
@@ -7423,20 +7549,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "chorde/clients/_async.pyx":249
+  /* "chorde/clients/_async.pyx":258
  *         self._set_nothreads(ExceptionWrapper.__new__(ExceptionWrapper, exc_info))
  * 
  *     def set_exception(self, exception):             # <<<<<<<<<<<<<<
  *         """
  *         Set the Future's exception object.
  */
 
@@ -7453,15 +7579,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exception);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":257
+/* "chorde/clients/_async.pyx":266
  *         self.exc((type(exception),exception,None))
  * 
  *     def on_value(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When and if the operation completes without exception, the callback
  */
 
@@ -7485,38 +7611,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_value", 0);
 
-  /* "chorde/clients/_async.pyx":262
+  /* "chorde/clients/_async.pyx":271
  *         will be invoked with its result.
  *         """
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_miss(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ValueCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ValueCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ValueCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ValueCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":257
+  /* "chorde/clients/_async.pyx":266
  *         self.exc((type(exception),exception,None))
  * 
  *     def on_value(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When and if the operation completes without exception, the callback
  */
 
@@ -7528,15 +7654,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":264
+/* "chorde/clients/_async.pyx":273
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))
  * 
  *     def on_miss(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in a cache miss, the callback will be invoked
  */
 
@@ -7560,38 +7686,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_miss", 0);
 
-  /* "chorde/clients/_async.pyx":269
+  /* "chorde/clients/_async.pyx":278
  *         without arugments.
  *         """
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_exc(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_MissCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_MissCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_MissCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_MissCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":264
+  /* "chorde/clients/_async.pyx":273
  *         return self._on_stuff(ValueCallback.__new__(ValueCallback, callback))
  * 
  *     def on_miss(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in a cache miss, the callback will be invoked
  */
 
@@ -7603,15 +7729,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":271
+/* "chorde/clients/_async.pyx":280
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))
  * 
  *     def on_exc(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in an exception, the callback will be invoked
  */
 
@@ -7635,38 +7761,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_exc", 0);
 
-  /* "chorde/clients/_async.pyx":276
+  /* "chorde/clients/_async.pyx":285
  *         with an exc_info tuple as returned by sys.exc_info.
  *         """
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_ExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_ExceptionCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":271
+  /* "chorde/clients/_async.pyx":280
  *         return self._on_stuff(MissCallback.__new__(MissCallback, callback))
  * 
  *     def on_exc(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation results in an exception, the callback will be invoked
  */
 
@@ -7678,15 +7804,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":278
+/* "chorde/clients/_async.pyx":287
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Handy method to set callbacks for all kinds of results, and it's actually
  */
 
@@ -7739,15 +7865,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any") < 0)) __PYX_ERR(0, 278, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any") < 0)) __PYX_ERR(0, 287, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7759,15 +7885,15 @@
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("on_any", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 278, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("on_any", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 287, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.on_any", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_24on_any(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -7782,44 +7908,44 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_any", 0);
 
-  /* "chorde/clients/_async.pyx":283
+  /* "chorde/clients/_async.pyx":292
  *         faster than calling on_X repeatedly. None callbacks will be ignored.
  *         """
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))             # <<<<<<<<<<<<<<
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_on_value);
   __Pyx_GIVEREF(__pyx_v_on_value);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_on_value);
   __Pyx_INCREF(__pyx_v_on_miss);
   __Pyx_GIVEREF(__pyx_v_on_miss);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_on_miss);
   __Pyx_INCREF(__pyx_v_on_exc);
   __Pyx_GIVEREF(__pyx_v_on_exc);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_on_exc);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":278
+  /* "chorde/clients/_async.pyx":287
  *         return self._on_stuff(ExceptionCallback.__new__(ExceptionCallback, callback))
  * 
  *     def on_any(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Handy method to set callbacks for all kinds of results, and it's actually
  */
 
@@ -7831,15 +7957,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":285
+/* "chorde/clients/_async.pyx":294
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Like on_any, but will only set the callback if no other callback has been set
  */
 
@@ -7892,15 +8018,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_on_exc);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any_once") < 0)) __PYX_ERR(0, 285, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "on_any_once") < 0)) __PYX_ERR(0, 294, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7912,15 +8038,15 @@
     }
     __pyx_v_on_value = values[0];
     __pyx_v_on_miss = values[1];
     __pyx_v_on_exc = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("on_any_once", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 285, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("on_any_once", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 294, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.on_any_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_26on_any_once(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_on_value, __pyx_v_on_miss, __pyx_v_on_exc);
 
@@ -7937,64 +8063,64 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_any_once", 0);
 
-  /* "chorde/clients/_async.pyx":289
+  /* "chorde/clients/_async.pyx":298
  *         Like on_any, but will only set the callback if no other callback has been set
  *         """
  *         if self._cb is None:             # <<<<<<<<<<<<<<
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_cb == ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":290
+    /* "chorde/clients/_async.pyx":299
  *         """
  *         if self._cb is None:
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))             # <<<<<<<<<<<<<<
  * 
  *     def on_done(self, callback):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_on_value);
     __Pyx_GIVEREF(__pyx_v_on_value);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_on_value);
     __Pyx_INCREF(__pyx_v_on_miss);
     __Pyx_GIVEREF(__pyx_v_on_miss);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_on_miss);
     __Pyx_INCREF(__pyx_v_on_exc);
     __Pyx_GIVEREF(__pyx_v_on_exc);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_on_exc);
-    __pyx_t_4 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_4 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_AnyCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_AnyCallback), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(((PyObject *)__pyx_t_4));
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_4), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_4), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(((PyObject *)__pyx_t_4)); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":289
+    /* "chorde/clients/_async.pyx":298
  *         Like on_any, but will only set the callback if no other callback has been set
  *         """
  *         if self._cb is None:             # <<<<<<<<<<<<<<
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  */
   }
 
-  /* "chorde/clients/_async.pyx":285
+  /* "chorde/clients/_async.pyx":294
  *         return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_any_once(self, on_value = None, on_miss = None, on_exc = None):             # <<<<<<<<<<<<<<
  *         """
  *         Like on_any, but will only set the callback if no other callback has been set
  */
 
@@ -8008,15 +8134,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":292
+/* "chorde/clients/_async.pyx":301
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_done(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operation is done, the callback will be invoked without arguments,
  */
 
@@ -8040,38 +8166,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_done", 0);
 
-  /* "chorde/clients/_async.pyx":297
+  /* "chorde/clients/_async.pyx":306
  *         regardless of the outcome. If the operation is cancelled, it won't be invoked.
  *         """
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))             # <<<<<<<<<<<<<<
  * 
  *     def chain(self, defer):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DoneCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DoneCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DoneCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DoneCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":292
+  /* "chorde/clients/_async.pyx":301
  *             return self._on_stuff(AnyCallback.__new__(AnyCallback, on_value, on_miss, on_exc))
  * 
  *     def on_done(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operation is done, the callback will be invoked without arguments,
  */
 
@@ -8083,15 +8209,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":299
+/* "chorde/clients/_async.pyx":308
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))
  * 
  *     def chain(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer
  */
 
@@ -8115,29 +8241,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chain", 0);
 
-  /* "chorde/clients/_async.pyx":303
+  /* "chorde/clients/_async.pyx":312
  *         Invoke all the callbacks of the other defer
  *         """
  *         self._on_stuff(defer.set)             # <<<<<<<<<<<<<<
  * 
  *     def chain_std(self, defer):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "chorde/clients/_async.pyx":299
+  /* "chorde/clients/_async.pyx":308
  *         return self._on_stuff(DoneCallback.__new__(DoneCallback, callback))
  * 
  *     def chain(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer
  */
 
@@ -8151,15 +8277,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":305
+/* "chorde/clients/_async.pyx":314
  *         self._on_stuff(defer.set)
  * 
  *     def chain_std(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer, without assuming the other
  */
 
@@ -8191,58 +8317,58 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chain_std", 0);
 
-  /* "chorde/clients/_async.pyx":310
+  /* "chorde/clients/_async.pyx":319
  *         defer follows our non-standard interface.
  *         """
  *         return self.on_any(             # <<<<<<<<<<<<<<
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "chorde/clients/_async.pyx":311
+  /* "chorde/clients/_async.pyx":320
  *         """
  *         return self.on_any(
  *             defer.set_result,             # <<<<<<<<<<<<<<
  *             functools_partial(defer.set_exception, CacheMissError()),
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "chorde/clients/_async.pyx":312
+  /* "chorde/clients/_async.pyx":321
  *         return self.on_any(
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),             # <<<<<<<<<<<<<<
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)
  *         )
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defer, __pyx_n_s_set_exception); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
   __pyx_t_7 = __pyx_v_6chorde_7clients_6_async_CacheMissError; __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 312, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_functools_partial);
   __pyx_t_7 = __pyx_v_6chorde_7clients_6_async_functools_partial; __pyx_t_8 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
@@ -8253,62 +8379,62 @@
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_6);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "chorde/clients/_async.pyx":313
+  /* "chorde/clients/_async.pyx":322
  *             defer.set_result,
  *             functools_partial(defer.set_exception, CacheMissError()),
  *             DeferExceptionCallback.__new__(DeferExceptionCallback, defer)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_defer);
   __Pyx_GIVEREF(__pyx_v_defer);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_defer);
-  __pyx_t_10 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback), __pyx_t_7, NULL)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_10 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_DeferExceptionCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback), __pyx_t_7, NULL)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_10));
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -8318,58 +8444,58 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_t_10)};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(((PyObject *)__pyx_t_10)); __pyx_t_10 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_t_10)};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(((PyObject *)__pyx_t_10)); __pyx_t_10 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_9, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_9, __pyx_t_4);
     __Pyx_GIVEREF(((PyObject *)__pyx_t_10));
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_9, ((PyObject *)__pyx_t_10));
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":305
+  /* "chorde/clients/_async.pyx":314
  *         self._on_stuff(defer.set)
  * 
  *     def chain_std(self, defer):             # <<<<<<<<<<<<<<
  *         """
  *         Invoke all the callbacks of the other defer, without assuming the other
  */
 
@@ -8388,15 +8514,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":316
+/* "chorde/clients/_async.pyx":325
  *         )
  * 
  *     cpdef _on_stuff(self, callback):             # <<<<<<<<<<<<<<
  *         if self._value is NONE:
  *             if self._cb is None:
  */
 
@@ -8420,15 +8546,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_stuff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_stuff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6chorde_7clients_6_async_6Future_35_on_stuff)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8437,15 +8563,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_callback) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_callback);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 325, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -8458,84 +8584,84 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "chorde/clients/_async.pyx":317
+  /* "chorde/clients/_async.pyx":326
  * 
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:             # <<<<<<<<<<<<<<
  *             if self._cb is None:
  *                 self._cb = list()
  */
   __pyx_t_5 = (__pyx_v_self->_value == ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "chorde/clients/_async.pyx":318
+    /* "chorde/clients/_async.pyx":327
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:
  *             if self._cb is None:             # <<<<<<<<<<<<<<
  *                 self._cb = list()
  *             self._cb.append(callback)
  */
     __pyx_t_6 = (__pyx_v_self->_cb == ((PyObject*)Py_None));
     __pyx_t_5 = (__pyx_t_6 != 0);
     if (__pyx_t_5) {
 
-      /* "chorde/clients/_async.pyx":319
+      /* "chorde/clients/_async.pyx":328
  *         if self._value is NONE:
  *             if self._cb is None:
  *                 self._cb = list()             # <<<<<<<<<<<<<<
  *             self._cb.append(callback)
  *         else:
  */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_v_self->_cb);
       __Pyx_DECREF(__pyx_v_self->_cb);
       __pyx_v_self->_cb = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "chorde/clients/_async.pyx":318
+      /* "chorde/clients/_async.pyx":327
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:
  *             if self._cb is None:             # <<<<<<<<<<<<<<
  *                 self._cb = list()
  *             self._cb.append(callback)
  */
     }
 
-    /* "chorde/clients/_async.pyx":320
+    /* "chorde/clients/_async.pyx":329
  *             if self._cb is None:
  *                 self._cb = list()
  *             self._cb.append(callback)             # <<<<<<<<<<<<<<
  *         else:
  *             callback(self._value)
  */
     if (unlikely(__pyx_v_self->_cb == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-      __PYX_ERR(0, 320, __pyx_L1_error)
+      __PYX_ERR(0, 329, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->_cb, __pyx_v_callback); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->_cb, __pyx_v_callback); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 329, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":317
+    /* "chorde/clients/_async.pyx":326
  * 
  *     cpdef _on_stuff(self, callback):
  *         if self._value is NONE:             # <<<<<<<<<<<<<<
  *             if self._cb is None:
  *                 self._cb = list()
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":322
+  /* "chorde/clients/_async.pyx":331
  *             self._cb.append(callback)
  *         else:
  *             callback(self._value)             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   /*else*/ {
@@ -8548,34 +8674,34 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_self->_value) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->_value);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":323
+  /* "chorde/clients/_async.pyx":332
  *         else:
  *             callback(self._value)
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def add_done_callback(self, callback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":316
+  /* "chorde/clients/_async.pyx":325
  *         )
  * 
  *     cpdef _on_stuff(self, callback):             # <<<<<<<<<<<<<<
  *         if self._value is NONE:
  *             if self._cb is None:
  */
 
@@ -8611,15 +8737,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_on_stuff", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__on_stuff(__pyx_v_self, __pyx_v_callback, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6chorde_7clients_6_async_6Future__on_stuff(__pyx_v_self, __pyx_v_callback, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8628,15 +8754,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":325
+/* "chorde/clients/_async.pyx":334
  *         return self
  * 
  *     def add_done_callback(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operatio is done, the callback will be invoked with the
  */
 
@@ -8660,41 +8786,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_done_callback", 0);
 
-  /* "chorde/clients/_async.pyx":330
+  /* "chorde/clients/_async.pyx":339
  *         future object as argument.
  *         """
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))             # <<<<<<<<<<<<<<
  * 
  *     cdef int c_done(self) except -1:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self));
   __Pyx_INCREF(__pyx_v_callback);
   __Pyx_GIVEREF(__pyx_v_callback);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_callback);
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_WeakCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_6chorde_7clients_6_async_WeakCallback(((PyTypeObject *)__pyx_ptype_6chorde_7clients_6_async_WeakCallback), __pyx_t_1, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_2));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->_on_stuff(__pyx_v_self, ((PyObject *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(((PyObject *)__pyx_t_2)); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":325
+  /* "chorde/clients/_async.pyx":334
  *         return self
  * 
  *     def add_done_callback(self, callback):             # <<<<<<<<<<<<<<
  *         """
  *         When the operatio is done, the callback will be invoked with the
  */
 
@@ -8706,15 +8832,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":332
+/* "chorde/clients/_async.pyx":341
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
  * 
  *     cdef int c_done(self) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -8722,15 +8848,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("c_done", 0);
 
-  /* "chorde/clients/_async.pyx":336
+  /* "chorde/clients/_async.pyx":345
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self._value is not NONE or self._cancelled:             # <<<<<<<<<<<<<<
  *             return 1
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
@@ -8741,60 +8867,60 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = (__pyx_v_self->_cancelled != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":337
+    /* "chorde/clients/_async.pyx":346
  *         """
  *         if self._value is not NONE or self._cancelled:
  *             return 1             # <<<<<<<<<<<<<<
  *         else:
  *             return 0
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":336
+    /* "chorde/clients/_async.pyx":345
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self._value is not NONE or self._cancelled:             # <<<<<<<<<<<<<<
  *             return 1
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":339
+  /* "chorde/clients/_async.pyx":348
  *             return 1
  *         else:
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     def done(self):
  */
   /*else*/ {
     __pyx_r = 0;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":332
+  /* "chorde/clients/_async.pyx":341
  *         return self._on_stuff(WeakCallback.__new__(WeakCallback, self, callback))
  * 
  *     cdef int c_done(self) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":341
+/* "chorde/clients/_async.pyx":350
  *             return 0
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -8818,61 +8944,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("done", 0);
 
-  /* "chorde/clients/_async.pyx":345
+  /* "chorde/clients/_async.pyx":354
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self.c_done():             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_done(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_done(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 354, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":346
+    /* "chorde/clients/_async.pyx":355
  *         """
  *         if self.c_done():
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":345
+    /* "chorde/clients/_async.pyx":354
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  *         """
  *         if self.c_done():             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":348
+  /* "chorde/clients/_async.pyx":357
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def running(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":341
+  /* "chorde/clients/_async.pyx":350
  *             return 0
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has finished, in a result or exception or cancelled, and False if not.
  */
 
@@ -8882,15 +9008,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":350
+/* "chorde/clients/_async.pyx":359
  *             return False
  * 
  *     def running(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation is running and cannot be cancelled. False if not running
  */
 
@@ -8910,75 +9036,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_40running(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("running", 0);
 
-  /* "chorde/clients/_async.pyx":355
+  /* "chorde/clients/_async.pyx":364
  *         (yet or done).
  *         """
  *         if self._running:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_running != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":356
+    /* "chorde/clients/_async.pyx":365
  *         """
  *         if self._running:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":355
+    /* "chorde/clients/_async.pyx":364
  *         (yet or done).
  *         """
  *         if self._running:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":358
+  /* "chorde/clients/_async.pyx":367
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancelled(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":350
+  /* "chorde/clients/_async.pyx":359
  *             return False
  * 
  *     def running(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation is running and cannot be cancelled. False if not running
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":360
+/* "chorde/clients/_async.pyx":369
  *             return False
  * 
  *     def cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has been cancelled successfully.
  */
 
@@ -8998,75 +9124,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_42cancelled(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancelled", 0);
 
-  /* "chorde/clients/_async.pyx":364
+  /* "chorde/clients/_async.pyx":373
  *         Return True if the operation has been cancelled successfully.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancelled != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":365
+    /* "chorde/clients/_async.pyx":374
  *         """
  *         if self._cancelled:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":364
+    /* "chorde/clients/_async.pyx":373
  *         Return True if the operation has been cancelled successfully.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":367
+  /* "chorde/clients/_async.pyx":376
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancel_pending(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":360
+  /* "chorde/clients/_async.pyx":369
  *             return False
  * 
  *     def cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if the operation has been cancelled successfully.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":369
+/* "chorde/clients/_async.pyx":378
  *             return False
  * 
  *     def cancel_pending(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if cancel was called.
  */
 
@@ -9086,75 +9212,75 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_44cancel_pending(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancel_pending", 0);
 
-  /* "chorde/clients/_async.pyx":373
+  /* "chorde/clients/_async.pyx":382
  *         Return True if cancel was called.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancel_pending != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":374
+    /* "chorde/clients/_async.pyx":383
  *         """
  *         if self._cancel_pending:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":373
+    /* "chorde/clients/_async.pyx":382
  *         Return True if cancel was called.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":376
+  /* "chorde/clients/_async.pyx":385
  *             return True
  *         else:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def cancel(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":369
+  /* "chorde/clients/_async.pyx":378
  *             return False
  * 
  *     def cancel_pending(self):             # <<<<<<<<<<<<<<
  *         """
  *         Return True if cancel was called.
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":378
+/* "chorde/clients/_async.pyx":387
  *             return False
  * 
  *     def cancel(self):             # <<<<<<<<<<<<<<
  *         """
  *         Request cancelling of the operation. If the operation cannot be cancelled,
  */
 
@@ -9174,84 +9300,84 @@
 
 static PyObject *__pyx_pf_6chorde_7clients_6_async_6Future_46cancel(struct __pyx_obj_6chorde_7clients_6_async_Future *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("cancel", 0);
 
-  /* "chorde/clients/_async.pyx":383
+  /* "chorde/clients/_async.pyx":392
  *         it will return False. Otherwise, it will return True.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return False
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_cancelled != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":384
+    /* "chorde/clients/_async.pyx":393
  *         """
  *         if self._cancelled:
  *             return False             # <<<<<<<<<<<<<<
  *         else:
  *             self._cancel_pending = 1
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":383
+    /* "chorde/clients/_async.pyx":392
  *         it will return False. Otherwise, it will return True.
  *         """
  *         if self._cancelled:             # <<<<<<<<<<<<<<
  *             return False
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":386
+  /* "chorde/clients/_async.pyx":395
  *             return False
  *         else:
  *             self._cancel_pending = 1             # <<<<<<<<<<<<<<
  *             return True
  * 
  */
   /*else*/ {
     __pyx_v_self->_cancel_pending = 1;
 
-    /* "chorde/clients/_async.pyx":387
+    /* "chorde/clients/_async.pyx":396
  *         else:
  *             self._cancel_pending = 1
  *             return True             # <<<<<<<<<<<<<<
  * 
  *     def set_running_or_notify_cancelled(self):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":378
+  /* "chorde/clients/_async.pyx":387
  *             return False
  * 
  *     def cancel(self):             # <<<<<<<<<<<<<<
  *         """
  *         Request cancelling of the operation. If the operation cannot be cancelled,
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":389
+/* "chorde/clients/_async.pyx":398
  *             return True
  * 
  *     def set_running_or_notify_cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         To be invoked by executors before executing the operation. If it returns True,
  */
 
@@ -9279,65 +9405,65 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_running_or_notify_cancelled", 0);
 
-  /* "chorde/clients/_async.pyx":396
+  /* "chorde/clients/_async.pyx":405
  *         be wakened immediately and the future will be marked as cancelled.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             self._cancelled = 1
  *             self._running = 0
  */
   __pyx_t_1 = (__pyx_v_self->_cancel_pending != 0);
   if (__pyx_t_1) {
 
-    /* "chorde/clients/_async.pyx":397
+    /* "chorde/clients/_async.pyx":406
  *         """
  *         if self._cancel_pending:
  *             self._cancelled = 1             # <<<<<<<<<<<<<<
  *             self._running = 0
  * 
  */
     __pyx_v_self->_cancelled = 1;
 
-    /* "chorde/clients/_async.pyx":398
+    /* "chorde/clients/_async.pyx":407
  *         if self._cancel_pending:
  *             self._cancelled = 1
  *             self._running = 0             # <<<<<<<<<<<<<<
  * 
  *             # Notify waiters and callbacks
  */
     __pyx_v_self->_running = 0;
 
-    /* "chorde/clients/_async.pyx":401
+    /* "chorde/clients/_async.pyx":410
  * 
  *             # Notify waiters and callbacks
  *             self.set_exception(CancelledError())             # <<<<<<<<<<<<<<
  * 
  *             return False
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
     __pyx_t_5 = __pyx_v_6chorde_7clients_6_async_CancelledError; __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9345,64 +9471,64 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "chorde/clients/_async.pyx":403
+    /* "chorde/clients/_async.pyx":412
  *             self.set_exception(CancelledError())
  * 
  *             return False             # <<<<<<<<<<<<<<
  *         else:
  *             self._running = 1
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "chorde/clients/_async.pyx":396
+    /* "chorde/clients/_async.pyx":405
  *         be wakened immediately and the future will be marked as cancelled.
  *         """
  *         if self._cancel_pending:             # <<<<<<<<<<<<<<
  *             self._cancelled = 1
  *             self._running = 0
  */
   }
 
-  /* "chorde/clients/_async.pyx":405
+  /* "chorde/clients/_async.pyx":414
  *             return False
  *         else:
  *             self._running = 1             # <<<<<<<<<<<<<<
  *             return True
  * 
  */
   /*else*/ {
     __pyx_v_self->_running = 1;
 
-    /* "chorde/clients/_async.pyx":406
+    /* "chorde/clients/_async.pyx":415
  *         else:
  *             self._running = 1
  *             return True             # <<<<<<<<<<<<<<
  * 
  *     cdef c_result(self, timeout, int norecurse):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
   }
 
-  /* "chorde/clients/_async.pyx":389
+  /* "chorde/clients/_async.pyx":398
  *             return True
  * 
  *     def set_running_or_notify_cancelled(self):             # <<<<<<<<<<<<<<
  *         """
  *         To be invoked by executors before executing the operation. If it returns True,
  */
 
@@ -9417,15 +9543,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":408
+/* "chorde/clients/_async.pyx":417
  *             return True
  * 
  *     cdef c_result(self, timeout, int norecurse):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -9451,84 +9577,84 @@
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("c_result", 0);
 
-  /* "chorde/clients/_async.pyx":417
+  /* "chorde/clients/_async.pyx":426
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   __pyx_t_1 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":418
+    /* "chorde/clients/_async.pyx":427
  * 
  *         if self._value is not NONE:
  *             value = self._value             # <<<<<<<<<<<<<<
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  */
     __pyx_t_3 = __pyx_v_self->_value;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":419
+    /* "chorde/clients/_async.pyx":428
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":420
+      /* "chorde/clients/_async.pyx":429
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value             # <<<<<<<<<<<<<<
  *                 try:
  *                     exc_value.reraise(False)
  */
       __pyx_t_3 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_exc_value = ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "chorde/clients/_async.pyx":421
+      /* "chorde/clients/_async.pyx":430
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  *                 try:             # <<<<<<<<<<<<<<
  *                     exc_value.reraise(False)
  *                 finally:
  */
       /*try:*/ {
 
-        /* "chorde/clients/_async.pyx":422
+        /* "chorde/clients/_async.pyx":431
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  *                     exc_value.reraise(False)             # <<<<<<<<<<<<<<
  *                 finally:
  *                     del exc_value, value
  */
         __pyx_t_4.__pyx_n = 1;
         __pyx_t_4.strip = 0;
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_exc_value->__pyx_vtab)->reraise(__pyx_v_exc_value, 0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L6_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_v_exc_value->__pyx_vtab)->reraise(__pyx_v_exc_value, 0, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
 
-      /* "chorde/clients/_async.pyx":424
+      /* "chorde/clients/_async.pyx":433
  *                     exc_value.reraise(False)
  *                 finally:
  *                     del exc_value, value             # <<<<<<<<<<<<<<
  *             elif value is CacheMissError:
  *                 raise CacheMissError()
  */
       /*finally:*/ {
@@ -9573,36 +9699,36 @@
           __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_6; __pyx_filename = __pyx_t_7;
           goto __pyx_L1_error;
         }
         __pyx_L7:;
       }
 
-      /* "chorde/clients/_async.pyx":419
+      /* "chorde/clients/_async.pyx":428
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 try:
  */
       goto __pyx_L4;
     }
 
-    /* "chorde/clients/_async.pyx":425
+    /* "chorde/clients/_async.pyx":434
  *                 finally:
  *                     del exc_value, value
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 raise CacheMissError()
  *             else:
  */
     __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "chorde/clients/_async.pyx":426
+      /* "chorde/clients/_async.pyx":435
  *                     del exc_value, value
  *             elif value is CacheMissError:
  *                 raise CacheMissError()             # <<<<<<<<<<<<<<
  *             else:
  *                 return value
  */
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
@@ -9614,66 +9740,66 @@
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 435, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 426, __pyx_L1_error)
+      __PYX_ERR(0, 435, __pyx_L1_error)
 
-      /* "chorde/clients/_async.pyx":425
+      /* "chorde/clients/_async.pyx":434
  *                 finally:
  *                     del exc_value, value
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 raise CacheMissError()
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":428
+    /* "chorde/clients/_async.pyx":437
  *                 raise CacheMissError()
  *             else:
  *                 return value             # <<<<<<<<<<<<<<
  *         elif self._cancelled:
  *             raise CancelledError()
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_value);
       __pyx_r = __pyx_v_value;
       goto __pyx_L0;
     }
     __pyx_L4:;
 
-    /* "chorde/clients/_async.pyx":417
+    /* "chorde/clients/_async.pyx":426
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
     goto __pyx_L3;
   }
 
-  /* "chorde/clients/_async.pyx":429
+  /* "chorde/clients/_async.pyx":438
  *             else:
  *                 return value
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_cancelled != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "chorde/clients/_async.pyx":430
+    /* "chorde/clients/_async.pyx":439
  *                 return value
  *         elif self._cancelled:
  *             raise CancelledError()             # <<<<<<<<<<<<<<
  *         else:
  *             if timeout is not None and timeout == 0:
  */
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -9685,54 +9811,54 @@
         __Pyx_INCREF(__pyx_t_15);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_14, function);
       }
     }
     __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
     __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 430, __pyx_L1_error)
+    __PYX_ERR(0, 439, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":429
+    /* "chorde/clients/_async.pyx":438
  *             else:
  *                 return value
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":432
+  /* "chorde/clients/_async.pyx":441
  *             raise CancelledError()
  *         else:
  *             if timeout is not None and timeout == 0:             # <<<<<<<<<<<<<<
  *                 raise TimeoutError()
  *             else:
  */
   /*else*/ {
     __pyx_t_1 = (__pyx_v_timeout != Py_None);
     __pyx_t_16 = (__pyx_t_1 != 0);
     if (__pyx_t_16) {
     } else {
       __pyx_t_2 = __pyx_t_16;
       goto __pyx_L11_bool_binop_done;
     }
-    __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_timeout, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_v_timeout, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 432, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 441, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = __pyx_t_16;
     __pyx_L11_bool_binop_done:;
     if (unlikely(__pyx_t_2)) {
 
-      /* "chorde/clients/_async.pyx":433
+      /* "chorde/clients/_async.pyx":442
  *         else:
  *             if timeout is not None and timeout == 0:
  *                 raise TimeoutError()             # <<<<<<<<<<<<<<
  *             else:
  *                 # Wait for it
  */
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_TimeoutError);
@@ -9744,85 +9870,85 @@
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 433, __pyx_L1_error)
+      __PYX_ERR(0, 442, __pyx_L1_error)
 
-      /* "chorde/clients/_async.pyx":432
+      /* "chorde/clients/_async.pyx":441
  *             raise CancelledError()
  *         else:
  *             if timeout is not None and timeout == 0:             # <<<<<<<<<<<<<<
  *                 raise TimeoutError()
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":436
+    /* "chorde/clients/_async.pyx":445
  *             else:
  *                 # Wait for it
  *                 if self._done_event is None:             # <<<<<<<<<<<<<<
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_self->_done_event == Py_None);
       __pyx_t_16 = (__pyx_t_2 != 0);
       if (__pyx_t_16) {
 
-        /* "chorde/clients/_async.pyx":437
+        /* "chorde/clients/_async.pyx":446
  *                 # Wait for it
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()             # <<<<<<<<<<<<<<
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_threading); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 437, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_threading); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 446, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_Event); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 437, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_Event); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 446, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_14 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
           __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_15);
           if (likely(__pyx_t_14)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_v_self->_done_event);
         __Pyx_DECREF(__pyx_v_self->_done_event);
         __pyx_v_self->_done_event = __pyx_t_3;
         __pyx_t_3 = 0;
 
-        /* "chorde/clients/_async.pyx":436
+        /* "chorde/clients/_async.pyx":445
  *             else:
  *                 # Wait for it
  *                 if self._done_event is None:             # <<<<<<<<<<<<<<
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  */
       }
 
-      /* "chorde/clients/_async.pyx":438
+      /* "chorde/clients/_async.pyx":447
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):             # <<<<<<<<<<<<<<
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  */
       __pyx_t_2 = ((!(__pyx_v_norecurse != 0)) != 0);
@@ -9834,71 +9960,71 @@
       __pyx_t_2 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
       __pyx_t_1 = (__pyx_t_2 != 0);
       if (!__pyx_t_1) {
       } else {
         __pyx_t_16 = __pyx_t_1;
         goto __pyx_L15_bool_binop_done;
       }
-      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_wait); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 438, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_done_event, __pyx_n_s_wait); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __pyx_t_14 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_15);
         if (likely(__pyx_t_14)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
           __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_15, function);
         }
       }
       __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_14, __pyx_v_timeout) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_v_timeout);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 438, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_16 = __pyx_t_1;
       __pyx_L15_bool_binop_done:;
       if (__pyx_t_16) {
 
-        /* "chorde/clients/_async.pyx":439
+        /* "chorde/clients/_async.pyx":448
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)             # <<<<<<<<<<<<<<
  *                 elif self._cancelled:
  *                     raise CancelledError()
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_int_0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_r = __pyx_t_3;
         __pyx_t_3 = 0;
         goto __pyx_L0;
 
-        /* "chorde/clients/_async.pyx":438
+        /* "chorde/clients/_async.pyx":447
  *                 if self._done_event is None:
  *                     self._done_event = threading.Event()
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):             # <<<<<<<<<<<<<<
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  */
       }
 
-      /* "chorde/clients/_async.pyx":440
+      /* "chorde/clients/_async.pyx":449
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:             # <<<<<<<<<<<<<<
  *                     raise CancelledError()
  *                 else:
  */
       __pyx_t_16 = (__pyx_v_self->_cancelled != 0);
       if (unlikely(__pyx_t_16)) {
 
-        /* "chorde/clients/_async.pyx":441
+        /* "chorde/clients/_async.pyx":450
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:
  *                     raise CancelledError()             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise TimeoutError()
  */
         __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -9910,31 +10036,31 @@
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 441, __pyx_L1_error)
+        __PYX_ERR(0, 450, __pyx_L1_error)
 
-        /* "chorde/clients/_async.pyx":440
+        /* "chorde/clients/_async.pyx":449
  *                 if not norecurse and (self._value is not NONE or self._done_event.wait(timeout)):
  *                     return self.c_result(0, 1)
  *                 elif self._cancelled:             # <<<<<<<<<<<<<<
  *                     raise CancelledError()
  *                 else:
  */
       }
 
-      /* "chorde/clients/_async.pyx":443
+      /* "chorde/clients/_async.pyx":452
  *                     raise CancelledError()
  *                 else:
  *                     raise TimeoutError()             # <<<<<<<<<<<<<<
  * 
  *     def result(self, timeout=None, norecurse=False):
  */
       /*else*/ {
@@ -9947,26 +10073,26 @@
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 443, __pyx_L1_error)
+        __PYX_ERR(0, 452, __pyx_L1_error)
       }
     }
   }
   __pyx_L3:;
 
-  /* "chorde/clients/_async.pyx":408
+  /* "chorde/clients/_async.pyx":417
  *             return True
  * 
  *     cdef c_result(self, timeout, int norecurse):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -9983,15 +10109,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF((PyObject *)__pyx_v_exc_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":445
+/* "chorde/clients/_async.pyx":454
  *                     raise TimeoutError()
  * 
  *     def result(self, timeout=None, norecurse=False):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -10034,15 +10160,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_norecurse);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "result") < 0)) __PYX_ERR(0, 445, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "result") < 0)) __PYX_ERR(0, 454, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -10051,15 +10177,15 @@
       }
     }
     __pyx_v_timeout = values[0];
     __pyx_v_norecurse = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("result", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 445, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("result", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 454, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_50result(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_timeout, __pyx_v_norecurse);
 
@@ -10074,30 +10200,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("result", 0);
 
-  /* "chorde/clients/_async.pyx":451
+  /* "chorde/clients/_async.pyx":460
  *         and the specified time elapses without a result available, raises TimeoutError.
  *         """
  *         return self.c_result(timeout, norecurse)             # <<<<<<<<<<<<<<
  * 
  *     def exception(self, timeout=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_norecurse); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 451, __pyx_L1_error)
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_norecurse); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "chorde/clients/_async.pyx":445
+  /* "chorde/clients/_async.pyx":454
  *                     raise TimeoutError()
  * 
  *     def result(self, timeout=None, norecurse=False):             # <<<<<<<<<<<<<<
  *         """
  *         Return the operation's result, if any. If an exception was the result, re-raise it.
  */
 
@@ -10108,15 +10234,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "chorde/clients/_async.pyx":453
+/* "chorde/clients/_async.pyx":462
  *         return self.c_result(timeout, norecurse)
  * 
  *     def exception(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation resulted in an exception, return the exception object.
  */
 
@@ -10149,29 +10275,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "exception") < 0)) __PYX_ERR(0, 453, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "exception") < 0)) __PYX_ERR(0, 462, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("exception", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 453, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("exception", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 462, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6chorde_7clients_6_async_6Future_52exception(((struct __pyx_obj_6chorde_7clients_6_async_Future *)__pyx_v_self), __pyx_v_timeout);
 
@@ -10197,163 +10323,163 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exception", 0);
 
-  /* "chorde/clients/_async.pyx":463
+  /* "chorde/clients/_async.pyx":472
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   __pyx_t_1 = (__pyx_v_self->_value != ((PyObject *)__pyx_ptype_6chorde_7clients_6_async_NONE));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "chorde/clients/_async.pyx":464
+    /* "chorde/clients/_async.pyx":473
  * 
  *         if self._value is not NONE:
  *             value = self._value             # <<<<<<<<<<<<<<
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  */
     __pyx_t_3 = __pyx_v_self->_value;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "chorde/clients/_async.pyx":465
+    /* "chorde/clients/_async.pyx":474
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "chorde/clients/_async.pyx":466
+      /* "chorde/clients/_async.pyx":475
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value             # <<<<<<<<<<<<<<
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:
  */
       __pyx_t_3 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_3);
       __pyx_v_exc_value = ((struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "chorde/clients/_async.pyx":467
+      /* "chorde/clients/_async.pyx":476
  *             if isinstance(value, ExceptionWrapper):
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]             # <<<<<<<<<<<<<<
  *             elif value is CacheMissError:
  *                 return CacheMissError
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 476, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         __Pyx_INCREF(__pyx_t_4);
         __pyx_t_3 = __pyx_t_4;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         goto __pyx_L5_bool_binop_done;
       }
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_exc_value->value, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_3 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_L5_bool_binop_done:;
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":465
+      /* "chorde/clients/_async.pyx":474
  *         if self._value is not NONE:
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):             # <<<<<<<<<<<<<<
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  */
     }
 
-    /* "chorde/clients/_async.pyx":468
+    /* "chorde/clients/_async.pyx":477
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 return CacheMissError
  *             else:
  */
     __pyx_t_1 = (__pyx_v_value == __pyx_v_6chorde_7clients_6_async_CacheMissError);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "chorde/clients/_async.pyx":469
+      /* "chorde/clients/_async.pyx":478
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:
  *                 return CacheMissError             # <<<<<<<<<<<<<<
  *             else:
  *                 return None
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CacheMissError);
       __pyx_r = __pyx_v_6chorde_7clients_6_async_CacheMissError;
       goto __pyx_L0;
 
-      /* "chorde/clients/_async.pyx":468
+      /* "chorde/clients/_async.pyx":477
  *                 exc_value = <ExceptionWrapper>value
  *                 return exc_value.value[1] or exc_value.value[0]
  *             elif value is CacheMissError:             # <<<<<<<<<<<<<<
  *                 return CacheMissError
  *             else:
  */
     }
 
-    /* "chorde/clients/_async.pyx":471
+    /* "chorde/clients/_async.pyx":480
  *                 return CacheMissError
  *             else:
  *                 return None             # <<<<<<<<<<<<<<
  *         elif self._cancelled:
  *             raise CancelledError()
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
 
-    /* "chorde/clients/_async.pyx":463
+    /* "chorde/clients/_async.pyx":472
  *         cdef ExceptionWrapper exc_value
  * 
  *         if self._value is not NONE:             # <<<<<<<<<<<<<<
  *             value = self._value
  *             if isinstance(value, ExceptionWrapper):
  */
   }
 
-  /* "chorde/clients/_async.pyx":472
+  /* "chorde/clients/_async.pyx":481
  *             else:
  *                 return None
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   __pyx_t_2 = (__pyx_v_self->_cancelled != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "chorde/clients/_async.pyx":473
+    /* "chorde/clients/_async.pyx":482
  *                 return None
  *         elif self._cancelled:
  *             raise CancelledError()             # <<<<<<<<<<<<<<
  *         else:
  *             try:
  */
     __Pyx_INCREF(__pyx_v_6chorde_7clients_6_async_CancelledError);
@@ -10365,31 +10491,31 @@
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 473, __pyx_L1_error)
+    __PYX_ERR(0, 482, __pyx_L1_error)
 
-    /* "chorde/clients/_async.pyx":472
+    /* "chorde/clients/_async.pyx":481
  *             else:
  *                 return None
  *         elif self._cancelled:             # <<<<<<<<<<<<<<
  *             raise CancelledError()
  *         else:
  */
   }
 
-  /* "chorde/clients/_async.pyx":475
+  /* "chorde/clients/_async.pyx":484
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
   /*else*/ {
@@ -10398,106 +10524,106 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_8);
       /*try:*/ {
 
-        /* "chorde/clients/_async.pyx":476
+        /* "chorde/clients/_async.pyx":485
  *         else:
  *             try:
  *                 self.c_result(timeout, 0)             # <<<<<<<<<<<<<<
  *                 return None
  *             except CancelledError:
  */
-        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L7_error)
+        __pyx_t_3 = ((struct __pyx_vtabstruct_6chorde_7clients_6_async_Future *)__pyx_v_self->__pyx_vtab)->c_result(__pyx_v_self, __pyx_v_timeout, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "chorde/clients/_async.pyx":477
+        /* "chorde/clients/_async.pyx":486
  *             try:
  *                 self.c_result(timeout, 0)
  *                 return None             # <<<<<<<<<<<<<<
  *             except CancelledError:
  *                 raise
  */
         __Pyx_XDECREF(__pyx_r);
         __pyx_r = Py_None; __Pyx_INCREF(Py_None);
         goto __pyx_L11_try_return;
 
-        /* "chorde/clients/_async.pyx":475
+        /* "chorde/clients/_async.pyx":484
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
       }
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "chorde/clients/_async.pyx":478
+      /* "chorde/clients/_async.pyx":487
  *                 self.c_result(timeout, 0)
  *                 return None
  *             except CancelledError:             # <<<<<<<<<<<<<<
  *                 raise
  *             except Exception as e:
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_v_6chorde_7clients_6_async_CancelledError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 478, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 487, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_5);
 
-        /* "chorde/clients/_async.pyx":479
+        /* "chorde/clients/_async.pyx":488
  *                 return None
  *             except CancelledError:
  *                 raise             # <<<<<<<<<<<<<<
  *             except Exception as e:
  *                 try:
  */
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_4);
         __Pyx_XGIVEREF(__pyx_t_5);
         __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_4, __pyx_t_5);
         __pyx_t_3 = 0; __pyx_t_4 = 0; __pyx_t_5 = 0; 
-        __PYX_ERR(0, 479, __pyx_L9_except_error)
+        __PYX_ERR(0, 488, __pyx_L9_except_error)
       }
 
-      /* "chorde/clients/_async.pyx":480
+      /* "chorde/clients/_async.pyx":489
  *             except CancelledError:
  *                 raise
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 try:
  *                     return e
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_9) {
         __Pyx_AddTraceback("chorde.clients._async.Future.exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3) < 0) __PYX_ERR(0, 480, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3) < 0) __PYX_ERR(0, 489, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __pyx_v_e = __pyx_t_4;
 
-        /* "chorde/clients/_async.pyx":481
+        /* "chorde/clients/_async.pyx":490
  *                 raise
  *             except Exception as e:
  *                 try:             # <<<<<<<<<<<<<<
  *                     return e
  *                 finally:
  */
         /*try:*/ {
 
-          /* "chorde/clients/_async.pyx":482
+          /* "chorde/clients/_async.pyx":491
  *             except Exception as e:
  *                 try:
  *                     return e             # <<<<<<<<<<<<<<
  *                 finally:
  *                     del e
  */
           __Pyx_XDECREF(__pyx_r);
@@ -10505,15 +10631,15 @@
           __pyx_r = __pyx_v_e;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L19_return;
         }
 
-        /* "chorde/clients/_async.pyx":484
+        /* "chorde/clients/_async.pyx":493
  *                     return e
  *                 finally:
  *                     del e             # <<<<<<<<<<<<<<
  * 
  */
         /*finally:*/ {
           __pyx_L19_return: {
@@ -10526,15 +10652,15 @@
             goto __pyx_L10_except_return;
           }
         }
       }
       goto __pyx_L9_except_error;
       __pyx_L9_except_error:;
 
-      /* "chorde/clients/_async.pyx":475
+      /* "chorde/clients/_async.pyx":484
  *             raise CancelledError()
  *         else:
  *             try:             # <<<<<<<<<<<<<<
  *                 self.c_result(timeout, 0)
  *                 return None
  */
       __Pyx_XGIVEREF(__pyx_t_6);
@@ -10553,15 +10679,15 @@
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_XGIVEREF(__pyx_t_8);
       __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
       goto __pyx_L0;
     }
   }
 
-  /* "chorde/clients/_async.pyx":453
+  /* "chorde/clients/_async.pyx":462
  *         return self.c_result(timeout, norecurse)
  * 
  *     def exception(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """
  *         If the operation resulted in an exception, return the exception object.
  */
 
@@ -12607,14 +12733,15 @@
   {&__pyx_n_s_ValueCallback, __pyx_k_ValueCallback, sizeof(__pyx_k_ValueCallback), 0, 0, 1, 1},
   {&__pyx_n_s_WeakCallback, __pyx_k_WeakCallback, sizeof(__pyx_k_WeakCallback), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_callback, __pyx_k_callback, sizeof(__pyx_k_callback), 0, 0, 1, 1},
   {&__pyx_n_s_chorde_clients, __pyx_k_chorde_clients, sizeof(__pyx_k_chorde_clients), 0, 0, 1, 1},
   {&__pyx_n_s_chorde_clients__async, __pyx_k_chorde_clients__async, sizeof(__pyx_k_chorde_clients__async), 0, 0, 1, 1},
+  {&__pyx_n_s_clear, __pyx_k_clear, sizeof(__pyx_k_clear), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_defer, __pyx_k_defer, sizeof(__pyx_k_defer), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_exc, __pyx_k_exc, sizeof(__pyx_k_exc), 0, 0, 1, 1},
   {&__pyx_n_s_exc_info, __pyx_k_exc_info, sizeof(__pyx_k_exc_info), 0, 0, 1, 1},
   {&__pyx_n_s_functools, __pyx_k_functools, sizeof(__pyx_k_functools), 0, 0, 1, 1},
@@ -12654,14 +12781,16 @@
   {&__pyx_n_s_set_nothreads, __pyx_k_set_nothreads, sizeof(__pyx_k_set_nothreads), 0, 0, 1, 1},
   {&__pyx_n_s_set_result, __pyx_k_set_result, sizeof(__pyx_k_set_result), 0, 0, 1, 1},
   {&__pyx_n_s_set_strip_tracebacks, __pyx_k_set_strip_tracebacks, sizeof(__pyx_k_set_strip_tracebacks), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_strip, __pyx_k_strip, sizeof(__pyx_k_strip), 0, 0, 1, 1},
+  {&__pyx_n_s_tb_frame, __pyx_k_tb_frame, sizeof(__pyx_k_tb_frame), 0, 0, 1, 1},
+  {&__pyx_n_s_tb_next, __pyx_k_tb_next, sizeof(__pyx_k_tb_next), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_s_timeout, __pyx_k_timeout, sizeof(__pyx_k_timeout), 0, 0, 1, 1},
   {&__pyx_n_s_tornado_web, __pyx_k_tornado_web, sizeof(__pyx_k_tornado_web), 0, 0, 1, 1},
   {&__pyx_n_s_traceback, __pyx_k_traceback, sizeof(__pyx_k_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
@@ -12830,22 +12959,22 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "chorde/clients/_async.pyx":205
+  /* "chorde/clients/_async.pyx":214
  *                     else:
  *                         error = logging.error
  *                     error("Error in async callback", exc_info = True)             # <<<<<<<<<<<<<<
  * 
  *     cpdef set(self, value):
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Error_in_async_callback); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 205, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Error_in_async_callback); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -12953,25 +13082,25 @@
   /*--- Type init code ---*/
   __pyx_vtabptr_6chorde_7clients_6_async_Future = &__pyx_vtable_6chorde_7clients_6_async_Future;
   __pyx_vtable_6chorde_7clients_6_async_Future.c_done = (int (*)(struct __pyx_obj_6chorde_7clients_6_async_Future *))__pyx_f_6chorde_7clients_6_async_6Future_c_done;
   __pyx_vtable_6chorde_7clients_6_async_Future.c_result = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int))__pyx_f_6chorde_7clients_6_async_6Future_c_result;
   __pyx_vtable_6chorde_7clients_6_async_Future._set_nothreads = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future__set_nothreads;
   __pyx_vtable_6chorde_7clients_6_async_Future.set = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future_set;
   __pyx_vtable_6chorde_7clients_6_async_Future._on_stuff = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_Future *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6chorde_7clients_6_async_6Future__on_stuff;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_Future.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_Future.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_Future.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_Future.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_Future.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Future, (PyObject *)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_Future.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Future, (PyObject *)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_Future.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_Future.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_Future, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_Future) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_Future = &__pyx_type_6chorde_7clients_6_async_Future;
   __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper = &__pyx_vtable_6chorde_7clients_6_async_ExceptionWrapper;
   __pyx_vtable_6chorde_7clients_6_async_ExceptionWrapper.reraise = (PyObject *(*)(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper *, int __pyx_skip_dispatch, struct __pyx_opt_args_6chorde_7clients_6_async_16ExceptionWrapper_reraise *__pyx_optional_args))__pyx_f_6chorde_7clients_6_async_16ExceptionWrapper_reraise;
   if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_print = 0;
   #endif
@@ -12979,100 +13108,100 @@
     __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_dict, __pyx_vtabptr_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionWrapper, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ExceptionWrapper.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ExceptionWrapper, __weakref__);
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionWrapper) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ExceptionWrapper = &__pyx_type_6chorde_7clients_6_async_ExceptionWrapper;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_WeakCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WeakCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WeakCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_WeakCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_WeakCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_WeakCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_WeakCallback) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_WeakCallback = &__pyx_type_6chorde_7clients_6_async_WeakCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DeferExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DeferExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_DeferExceptionCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_DeferExceptionCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_DeferExceptionCallback = &__pyx_type_6chorde_7clients_6_async_DeferExceptionCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ValueCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ValueCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ValueCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ValueCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ValueCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ValueCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ValueCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ValueCallback = &__pyx_type_6chorde_7clients_6_async_ValueCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_MissCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_MissCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_MissCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_MissCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MissCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MissCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_MissCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_MissCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_MissCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_MissCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_MissCallback = &__pyx_type_6chorde_7clients_6_async_MissCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ExceptionCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_ExceptionCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_ExceptionCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_ExceptionCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_ExceptionCallback = &__pyx_type_6chorde_7clients_6_async_ExceptionCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_AnyCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnyCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnyCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_AnyCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_AnyCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_AnyCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_AnyCallback) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_AnyCallback = &__pyx_type_6chorde_7clients_6_async_AnyCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_DoneCallback.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DoneCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_DoneCallback, (PyObject *)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
   if (__pyx_type_6chorde_7clients_6_async_DoneCallback.tp_weaklistoffset == 0) __pyx_type_6chorde_7clients_6_async_DoneCallback.tp_weaklistoffset = offsetof(struct __pyx_obj_6chorde_7clients_6_async_DoneCallback, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_DoneCallback) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_DoneCallback = &__pyx_type_6chorde_7clients_6_async_DoneCallback;
-  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6chorde_7clients_6_async_NONE.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6chorde_7clients_6_async_NONE.tp_dictoffset && __pyx_type_6chorde_7clients_6_async_NONE.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6chorde_7clients_6_async_NONE.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NONE, (PyObject *)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NONE, (PyObject *)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6chorde_7clients_6_async_NONE) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
   __pyx_ptype_6chorde_7clients_6_async_NONE = &__pyx_type_6chorde_7clients_6_async_NONE;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -14507,27 +14636,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
 /* PyObjectCallNoArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
@@ -14542,14 +14658,27 @@
             return __Pyx_PyObject_CallMethO(func, NULL);
         }
     }
     return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
 }
 #endif
 
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
```

### Comparing `chorde-1.0.6/lib/chorde/clients/_async.pyx` & `chorde-1.0.7/lib/chorde/clients/_async.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,23 @@
                 kwargs = {}
                 if _HTTPError is not None and isinstance(exc_obj, _HTTPError):
                     # Workaround for tornado's HTTPError which does not function
                     # correctly without a reason, and reason is given only as kwarg
                     kwargs["reason"] = exc_obj.reason
                 raise exc_typ(*exc_obj.args, **kwargs) from exc_obj
             elif exc_tb is not None:
+                # clear any non-running traceback's frames to avoid leaking locals
+                tb = exc_tb
+                while tb is not None:
+                    try:
+                        tb.tb_frame.clear()
+                    except:
+                        pass
+                    tb = tb.tb_next
+
                 if exc_obj is not None:
                     if getattr(exc_obj, '__traceback__') is not exc_tb:
                         exc_obj = exc_obj.with_traceback(exc_tb)
                     raise exc_obj
                 else:
                     raise exc_typ().with_traceback(exc_tb)
             elif exc_obj is not None:
```

### Comparing `chorde-1.0.6/lib/chorde/clients/async.c` & `chorde-1.0.7/lib/chorde/clients/async.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/asyncache.c` & `chorde-1.0.7/lib/chorde/clients/asyncache.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/asyncache.py` & `chorde-1.0.7/lib/chorde/clients/asyncache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/base.c` & `chorde-1.0.7/lib/chorde/clients/base.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/base.py` & `chorde-1.0.7/lib/chorde/clients/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/coherent.py` & `chorde-1.0.7/lib/chorde/clients/coherent.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/elasticache.py` & `chorde-1.0.7/lib/chorde/clients/elasticache.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/files.py` & `chorde-1.0.7/lib/chorde/clients/files.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/inproc.c` & `chorde-1.0.7/lib/chorde/clients/inproc.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/inproc.py` & `chorde-1.0.7/lib/chorde/clients/inproc.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/memcached.py` & `chorde-1.0.7/lib/chorde/clients/memcached.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/tiered.c` & `chorde-1.0.7/lib/chorde/clients/tiered.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/clients/tiered.py` & `chorde-1.0.7/lib/chorde/clients/tiered.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/decorators.c` & `chorde-1.0.7/lib/chorde/decorators.c`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/decorators.pxd` & `chorde-1.0.7/lib/chorde/decorators.pxd`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/decorators.py` & `chorde-1.0.7/lib/chorde/decorators.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/dnsutils.py` & `chorde-1.0.7/lib/chorde/dnsutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/external_integration.py` & `chorde-1.0.7/lib/chorde/external_integration.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/mq/coherence.py` & `chorde-1.0.7/lib/chorde/mq/coherence.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/mq/ipsub/base.py` & `chorde-1.0.7/lib/chorde/mq/ipsub/base.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/mq/ipsub/ipsub_zmq.py` & `chorde-1.0.7/lib/chorde/mq/ipsub/ipsub_zmq.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/sPickle.py` & `chorde-1.0.7/lib/chorde/sPickle.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/serialize.py` & `chorde-1.0.7/lib/chorde/serialize.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/shmemutils.py` & `chorde-1.0.7/lib/chorde/shmemutils.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/threadpool.py` & `chorde-1.0.7/lib/chorde/threadpool.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde/worker.py` & `chorde-1.0.7/lib/chorde/worker.py`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/lib/chorde.egg-info/PKG-INFO` & `chorde-1.0.7/lib/chorde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chorde
-Version: 1.0.6
+Version: 1.0.7
 Summary: Clustered Caching Library
 Home-page: https://github.com/klaussfreire/chorde
 Author: Claudio Freire
 Author-email: klaussfreire@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `chorde-1.0.6/lib/chorde.egg-info/SOURCES.txt` & `chorde-1.0.7/lib/chorde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chorde-1.0.6/setup.py` & `chorde-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 no_pyrex = False
 try:
     from Cython.Distutils import build_ext, Extension
     from Cython.Build import cythonize
 except:
     no_pyrex = True
 
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 
 version_path = os.path.join(os.path.dirname(__file__), 'lib', 'chorde', '_version.py')
 if not os.path.exists(version_path):
     with open(version_path, "w") as version_file:
         pass
 with open(version_path, "r+") as version_file:
     version_content = "__version__ = %r" % (VERSION,)
```

