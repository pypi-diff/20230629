# Comparing `tmp/appier-1.9.8.tar.gz` & `tmp/appier-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/appier-1.9.8.tar", last modified: Tue Feb 14 10:20:03 2017, max compression
+gzip compressed data, was "dist/appier-1.9.9.tar", last modified: Tue Feb 14 11:01:14 2017, max compression
```

## Comparing `appier-1.9.8.tar` & `appier-1.9.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/res/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/res/static/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/res/static/css/
--rw-r--r--   0 travis    (1000) travis    (1000)     1011 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/res/static/css/base.css
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/res/static/images/
--rw-r--r--   0 travis    (1000) travis    (1000)     1150 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/res/static/images/favicon.ico
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/res/templates/
--rw-r--r--   0 travis    (1000) travis    (1000)      525 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/res/templates/error.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      387 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/res/templates/holder.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1205 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/res/templates/layout.html.tpl
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier/test/
--rw-r--r--   0 travis    (1000) travis    (1000)     1213 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7884 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/base.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4805 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/cache.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2680 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/crypt.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1576 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/data.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2485 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3488 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/export.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7008 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/http.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5964 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/legacy.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4258 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/mock.py
--rw-r--r--   0 travis    (1000) travis    (1000)    16315 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/model.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3315 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/part.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5959 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/queuing.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5131 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/request.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2375 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/serialize.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4656 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/session.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2013 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/smtp.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1747 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/structures.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8060 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/typesf.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5322 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/test/util.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6527 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3616 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/amqp.py
--rw-r--r--   0 travis    (1000) travis    (1000)    13758 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/api.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6792 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/async.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3295 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/async_neo.py
--rw-r--r--   0 travis    (1000) travis    (1000)   179546 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/base.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6825 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/cache.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1522 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/common.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4895 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/compress.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7643 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/config.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2224 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/controller.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5938 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/crypt.py
--rw-r--r--   0 travis    (1000) travis    (1000)    12270 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/data.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9951 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/defines.py
--rw-r--r--   0 travis    (1000) travis    (1000)    11355 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)    12519 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/export.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4889 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/geo.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3820 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/git.py
--rw-r--r--   0 travis    (1000) travis    (1000)    34826 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/http.py
--rw-r--r--   0 travis    (1000) travis    (1000)    11667 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/legacy.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8948 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/log.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6724 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/meta.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5936 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/mock.py
--rw-r--r--   0 travis    (1000) travis    (1000)    90148 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/model.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5817 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/mongo.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4524 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/observer.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3511 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/part.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7875 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/queuing.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2395 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/redisdb.py
--rw-r--r--   0 travis    (1000) travis    (1000)    24674 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/request.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2991 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/scheduler.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6684 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/serialize.py
--rw-r--r--   0 travis    (1000) travis    (1000)    18612 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/session.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1359 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/settings.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3550 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/smtp.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7508 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/storage.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2319 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/structures.py
--rw-r--r--   0 travis    (1000) travis    (1000)    29958 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/typesf.py
--rw-r--r--   0 travis    (1000) travis    (1000)    50534 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/util.py
--rw-r--r--   0 travis    (1000) travis    (1000)    21008 2017-02-14 10:19:15.000000 appier-1.9.8/src/appier/validation.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)      978 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1771 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-02-14 10:19:37.000000 appier-1.9.8/src/appier.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)        7 2017-02-14 10:20:03.000000 appier-1.9.8/src/appier.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      159 2017-02-14 10:19:15.000000 appier-1.9.8/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)      689 2017-02-14 10:19:15.000000 appier-1.9.8/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     2726 2017-02-14 10:19:15.000000 appier-1.9.8/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      978 2017-02-14 10:20:03.000000 appier-1.9.8/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       88 2017-02-14 10:20:03.000000 appier-1.9.8/setup.cfg
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/res/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/res/static/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/res/static/css/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1011 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/res/static/css/base.css
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/res/static/images/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1150 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/res/static/images/favicon.ico
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/res/templates/
+-rw-r--r--   0 travis    (1000) travis    (1000)      525 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/res/templates/error.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      387 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/res/templates/holder.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1205 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/res/templates/layout.html.tpl
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier/test/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1213 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7884 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/base.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4805 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/cache.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2680 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/crypt.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1576 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2485 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/exceptions.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3488 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/export.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7008 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/http.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5964 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/legacy.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4258 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/mock.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    16315 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/model.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3315 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/part.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5959 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/queuing.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5131 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/request.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2375 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/serialize.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4656 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/session.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2013 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/smtp.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1747 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/structures.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8060 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/typesf.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5322 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/test/util.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6527 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3616 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/amqp.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    13758 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/api.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6792 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/async.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3295 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/async_neo.py
+-rw-r--r--   0 travis    (1000) travis    (1000)   179546 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/base.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6825 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/cache.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1522 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4895 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/compress.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7643 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/config.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2224 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/controller.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5938 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/crypt.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    12321 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9951 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/defines.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    11355 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/exceptions.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    12519 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/export.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4889 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/geo.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3820 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/git.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    34826 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/http.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    11667 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/legacy.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8948 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/log.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6724 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/meta.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5936 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/mock.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    90210 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/model.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5817 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/mongo.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4524 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/observer.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3511 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/part.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7875 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/queuing.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2395 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/redisdb.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    24674 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/request.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2991 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/scheduler.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6684 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/serialize.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    18612 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/session.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1359 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/settings.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3550 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/smtp.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7508 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/storage.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2319 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/structures.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    29958 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/typesf.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    50534 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/util.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    21008 2017-02-14 11:00:30.000000 appier-1.9.9/src/appier/validation.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)      978 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1771 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-02-14 11:00:51.000000 appier-1.9.9/src/appier.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (1000) travis    (1000)        7 2017-02-14 11:01:14.000000 appier-1.9.9/src/appier.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      159 2017-02-14 11:00:30.000000 appier-1.9.9/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)      689 2017-02-14 11:00:30.000000 appier-1.9.9/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)     2726 2017-02-14 11:00:30.000000 appier-1.9.9/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      978 2017-02-14 11:01:14.000000 appier-1.9.9/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)       88 2017-02-14 11:01:14.000000 appier-1.9.9/setup.cfg
```

### Comparing `appier-1.9.8/src/appier/res/static/css/base.css` & `appier-1.9.9/src/appier/res/static/css/base.css`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/res/static/images/favicon.ico` & `appier-1.9.9/src/appier/res/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/res/templates/error.html.tpl` & `appier-1.9.9/src/appier/res/templates/error.html.tpl`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/res/templates/layout.html.tpl` & `appier-1.9.9/src/appier/res/templates/layout.html.tpl`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/__init__.py` & `appier-1.9.9/src/appier/test/__init__.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/base.py` & `appier-1.9.9/src/appier/test/base.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/cache.py` & `appier-1.9.9/src/appier/test/cache.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/crypt.py` & `appier-1.9.9/src/appier/test/crypt.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/data.py` & `appier-1.9.9/src/appier/test/data.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/exceptions.py` & `appier-1.9.9/src/appier/test/exceptions.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/export.py` & `appier-1.9.9/src/appier/test/export.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/http.py` & `appier-1.9.9/src/appier/test/http.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/legacy.py` & `appier-1.9.9/src/appier/test/legacy.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/mock.py` & `appier-1.9.9/src/appier/test/mock.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/model.py` & `appier-1.9.9/src/appier/test/model.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/part.py` & `appier-1.9.9/src/appier/test/part.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/queuing.py` & `appier-1.9.9/src/appier/test/queuing.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/request.py` & `appier-1.9.9/src/appier/test/request.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/serialize.py` & `appier-1.9.9/src/appier/test/serialize.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/session.py` & `appier-1.9.9/src/appier/test/session.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/smtp.py` & `appier-1.9.9/src/appier/test/smtp.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/structures.py` & `appier-1.9.9/src/appier/test/structures.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/typesf.py` & `appier-1.9.9/src/appier/test/typesf.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/test/util.py` & `appier-1.9.9/src/appier/test/util.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/__init__.py` & `appier-1.9.9/src/appier/__init__.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/amqp.py` & `appier-1.9.9/src/appier/amqp.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/api.py` & `appier-1.9.9/src/appier/api.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/async.py` & `appier-1.9.9/src/appier/async.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/async_neo.py` & `appier-1.9.9/src/appier/async_neo.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/base.py` & `appier-1.9.9/src/appier/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 level that is going to be used for some core assumptions
 in situations where no app is created (eg: api clients) """
 
 NAME = "appier"
 """ The name to be used to describe the framework while working
 on its own environment, this is just a descriptive value """
 
-VERSION = "1.9.8"
+VERSION = "1.9.9"
 """ The version of the framework that is currently installed
 this value may be used for debugging/diagnostic purposes """
 
 PLATFORM = "%s %d.%d.%d.%s %s" % (
     sys.subversion[0] if hasattr(sys, "subversion") else "CPython",
     sys.version_info[0],
     sys.version_info[1],
```

### Comparing `appier-1.9.8/src/appier/cache.py` & `appier-1.9.9/src/appier/cache.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/common.py` & `appier-1.9.9/src/appier/common.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/compress.py` & `appier-1.9.9/src/appier/compress.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/config.py` & `appier-1.9.9/src/appier/config.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/controller.py` & `appier-1.9.9/src/appier/controller.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/crypt.py` & `appier-1.9.9/src/appier/crypt.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/data.py` & `appier-1.9.9/src/appier/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,16 +257,17 @@
 
     def count(self, *args, **kwargs):
         self.log("count", *args, **kwargs)
         return self._base.count(*args, **kwargs)
 
     def ensure_index(self, *args, **kwargs):
         self.log("ensure_index", *args, **kwargs)
-        simple = kwargs.pop("simple", False)
-        if simple: return mongo._store_ensure_index(self._base, *args, **kwargs)
+        direction = kwargs.pop("direction", True)
+        is_simple = direction == "simple"
+        if is_simple: return mongo._store_ensure_index(self._base, *args, **kwargs)
         else: return mongo._store_ensure_index_all(self._base, *args, **kwargs)
 
 class TinyCollection(Collection):
 
     def __init__(self, owner, name, base):
         Collection.__init__(self, owner, name)
         self._base = base
```

### Comparing `appier-1.9.8/src/appier/defines.py` & `appier-1.9.9/src/appier/defines.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/exceptions.py` & `appier-1.9.9/src/appier/exceptions.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/export.py` & `appier-1.9.9/src/appier/export.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/geo.py` & `appier-1.9.9/src/appier/geo.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/git.py` & `appier-1.9.9/src/appier/git.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/http.py` & `appier-1.9.9/src/appier/http.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/legacy.py` & `appier-1.9.9/src/appier/legacy.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/log.py` & `appier-1.9.9/src/appier/log.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/meta.py` & `appier-1.9.9/src/appier/meta.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/mock.py` & `appier-1.9.9/src/appier/mock.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/model.py` & `appier-1.9.9/src/appier/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -881,15 +881,16 @@
         if lazy: return
         cls.setup()
 
     @classmethod
     def setup(cls):
         indexes = cls.indexes()
         collection = cls._collection()
-        for index in indexes: collection.ensure_index(index)
+        for index, direction in indexes:
+            collection.ensure_index(index, direction = direction)
 
     @classmethod
     def teardown(cls):
         pass
 
     @classmethod
     def validate(cls):
@@ -1117,17 +1118,17 @@
         # the name of the fields associated with their definition
         definition = cls.definition()
 
         # iterate over all the names in the definition to retrieve their
         # definition and check if their are of type index
         for name in definition:
             _definition = cls.definition_n(name)
-            is_index = _definition.get("index", False)
-            if not is_index: continue
-            indexes.append(name)
+            direction = _definition.get("index", False)
+            if not direction: continue
+            indexes.append((name, direction))
 
         # saves the index list under the class and then
         # returns the sequence to the caller method
         cls._indexes = indexes
         return indexes
 
     @classmethod
```

### Comparing `appier-1.9.8/src/appier/mongo.py` & `appier-1.9.9/src/appier/mongo.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/observer.py` & `appier-1.9.9/src/appier/observer.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/part.py` & `appier-1.9.9/src/appier/part.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/queuing.py` & `appier-1.9.9/src/appier/queuing.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/redisdb.py` & `appier-1.9.9/src/appier/redisdb.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/request.py` & `appier-1.9.9/src/appier/request.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/scheduler.py` & `appier-1.9.9/src/appier/scheduler.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/serialize.py` & `appier-1.9.9/src/appier/serialize.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/session.py` & `appier-1.9.9/src/appier/session.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/settings.py` & `appier-1.9.9/src/appier/settings.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/smtp.py` & `appier-1.9.9/src/appier/smtp.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/storage.py` & `appier-1.9.9/src/appier/storage.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/structures.py` & `appier-1.9.9/src/appier/structures.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/typesf.py` & `appier-1.9.9/src/appier/typesf.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/util.py` & `appier-1.9.9/src/appier/util.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier/validation.py` & `appier-1.9.9/src/appier/validation.py`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/src/appier.egg-info/PKG-INFO` & `appier-1.9.9/src/appier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: appier
-Version: 1.9.8
+Version: 1.9.9
 Summary: Appier Framework
 Home-page: http://appier.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: appier framework web json wsgi
```

### Comparing `appier-1.9.8/src/appier.egg-info/SOURCES.txt` & `appier-1.9.9/src/appier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/README.rst` & `appier-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `appier-1.9.8/setup.py` & `appier-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "appier",
-    version = "1.9.8",
+    version = "1.9.9",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Appier Framework",
     license = "Apache License, Version 2.0",
     keywords = "appier framework web json wsgi",
     url = "http://appier.hive.pt",
     zip_safe = False,
```

### Comparing `appier-1.9.8/PKG-INFO` & `appier-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: appier
-Version: 1.9.8
+Version: 1.9.9
 Summary: Appier Framework
 Home-page: http://appier.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: appier framework web json wsgi
```

