# Comparing `tmp/apminsight-1.0.3.tar.gz` & `tmp/apminsight-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apminsight-1.0.3.tar", last modified: Tue May 31 09:08:53 2022, max compression
+gzip compressed data, was "apminsight-1.1.0.tar", last modified: Thu Jun 29 06:30:11 2023, max compression
```

## Comparing `apminsight-1.0.3.tar` & `apminsight-1.1.0.tar`

### file list

```diff
@@ -1,66 +1,83 @@
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.090195 apminsight-1.0.3/
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)     4055 2022-05-31 09:08:53.090195 apminsight-1.0.3/PKG-INFO
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3237 2022-05-30 06:56:03.000000 apminsight-1.0.3/README.md
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.086196 apminsight-1.0.3/apminsight/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      405 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4353 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/agent.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      433 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/agentfactory.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.086196 apminsight-1.0.3/apminsight/collector/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2344 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/connhandler.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1903 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/datahandler.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3280 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/insinfo.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1191 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/reqhandler.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3415 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/rescodes.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2212 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/collector/reshandler.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.086196 apminsight-1.0.3/apminsight/config/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/config/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     8264 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/config/configuration.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4131 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/config/threshold.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4303 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/constants.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      658 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/context.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.086196 apminsight-1.0.3/apminsight/contrib/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/contrib/__init__.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.086196 apminsight-1.0.3/apminsight/contrib/django/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)       71 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/contrib/django/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      703 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/contrib/django/apps.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1126 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/contrib/django/wrapper.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.090195 apminsight-1.0.3/apminsight/instrumentation/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2759 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     6325 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/dbapi2.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1019 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/modules.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.090195 apminsight-1.0.3/apminsight/instrumentation/packages/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      162 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1598 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/cassandra.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      963 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/django.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1460 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/flask.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      433 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/jinja2.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1247 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/memcache.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1662 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/mysql.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      439 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/psycopg2.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1488 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/pymemcache.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1539 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/redis.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      561 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/packages/sqlite.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      798 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/util.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3638 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/instrumentation/wrapper.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1637 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/logger.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.090195 apminsight-1.0.3/apminsight/metric/
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/__init__.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     6587 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/apdexmetric.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2623 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/component.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1101 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/dbmetric.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2513 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/dbtracker.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1350 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/error.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     6079 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/metricstore.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4557 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/tracker.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     5544 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/metric/txn.py
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2781 2022-05-30 06:56:03.000000 apminsight-1.0.3/apminsight/util.py
-drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2022-05-31 09:08:53.086196 apminsight-1.0.3/apminsight.egg-info/
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)     4055 2022-05-31 09:08:53.000000 apminsight-1.0.3/apminsight.egg-info/PKG-INFO
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)     1824 2022-05-31 09:08:53.000000 apminsight-1.0.3/apminsight.egg-info/SOURCES.txt
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)        1 2022-05-31 09:08:53.000000 apminsight-1.0.3/apminsight.egg-info/dependency_links.txt
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)        1 2022-05-31 09:08:53.000000 apminsight-1.0.3/apminsight.egg-info/not-zip-safe
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)        9 2022-05-31 09:08:53.000000 apminsight-1.0.3/apminsight.egg-info/requires.txt
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)       11 2022-05-31 09:08:53.000000 apminsight-1.0.3/apminsight.egg-info/top_level.txt
--rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)       38 2022-05-31 09:08:53.090195 apminsight-1.0.3/setup.cfg
--rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      665 2022-05-30 06:56:03.000000 apminsight-1.0.3/setup.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.846569 apminsight-1.1.0/
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)     6926 2023-06-29 06:30:11.846569 apminsight-1.1.0/PKG-INFO
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     5740 2023-06-26 18:27:16.000000 apminsight-1.1.0/README.md
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      253 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     5871 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/agent.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      642 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/agentfactory.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4280 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/apm_run.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/bootstrap/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/bootstrap/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1941 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/bootstrap/sitecustomize.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/collector/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2781 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/connhandler.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1903 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/datahandler.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4657 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/ins_info.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)    10666 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/metric_dispatcher.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1191 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/reqhandler.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3415 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/rescodes.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2212 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/collector/reshandler.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/config/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/config/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)    13494 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/config/configuration.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4591 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/config/threshold.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     8384 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/constants.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      658 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/context.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/contrib/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/contrib/__init__.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/contrib/django/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)       71 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/contrib/django/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2585 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/contrib/django/apps.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1126 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/contrib/django/wrapper.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight/instrumentation/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3558 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     8896 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/dbapi2.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1937 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/modules.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.846569 apminsight-1.1.0/apminsight/instrumentation/packages/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      303 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2161 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/bottle.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2151 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/cassandra.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2562 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/cherrypy.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1482 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/django.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1530 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/flask.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      451 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/genshi.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     6855 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/http.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1267 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/httplib2.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1344 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/httpx.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      433 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/jinja2.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      519 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/mako.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1257 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/memcache.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2248 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/mysql.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2119 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/psycopg2.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1562 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/pymemcache.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1899 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/pyramid.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1625 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/redis.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      734 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/sqlite.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2009 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/urllib.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2001 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/packages/urllib3.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     9117 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/proxy.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      810 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/util.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     4989 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/instrumentation/wrapper.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     3191 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/logger.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.846569 apminsight-1.1.0/apminsight/metric/
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/__init__.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     6589 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/apdexmetric.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2763 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/component.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1086 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/dbmetric.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1469 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/dbtracker.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     1412 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/error.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     6115 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/metricstore.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     8573 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/tracker.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     8117 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/metric/txn.py
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)     2357 2023-06-26 18:27:16.000000 apminsight-1.1.0/apminsight/util.py
+drwxr-xr-x   0 pawan-2008 (618143181) domain^users (618136065)        0 2023-06-29 06:30:11.842569 apminsight-1.1.0/apminsight.egg-info/
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)     6926 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/PKG-INFO
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)     2494 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/SOURCES.txt
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)        1 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/dependency_links.txt
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)       60 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/entry_points.txt
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)        1 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/not-zip-safe
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)        9 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/requires.txt
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)       11 2023-06-29 06:30:11.000000 apminsight-1.1.0/apminsight.egg-info/top_level.txt
+-rw-r--r--   0 pawan-2008 (618143181) domain^users (618136065)       38 2023-06-29 06:30:11.846569 apminsight-1.1.0/setup.cfg
+-rw-rw-r--   0 pawan-2008 (618143181) domain^users (618136065)      805 2023-06-26 18:27:16.000000 apminsight-1.1.0/setup.py
```

### Comparing `apminsight-1.0.3/apminsight/collector/connhandler.py` & `apminsight-1.1.0/apminsight/collector/connhandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 
 """
     initate connect request and schedule 1min task
 """
 
 import platform
-import requests
-import json
 import time
+import json
+from apminsight import constants
 from apminsight.agentfactory import get_agent
 from apminsight.constants import arh_connect, arh_data
 from apminsight.logger import agentlogger
 from apminsight.collector.reqhandler import send_req
 from apminsight.collector.reshandler import handle_connect_response
 from apminsight.collector.datahandler import process_collected_data
 
@@ -47,35 +47,45 @@
             agentlogger.exception('apm task error')
         finally:
             #get_agent().get_metric_store().cleanup()
             time.sleep(60)
 
 
 def send_connect():
-    payload = getconn_payload() if conn_payload is None else conn_payload
-    res_data = send_req(arh_connect, payload)
+    global conn_payload
+    conn_payload = getconn_payload() if conn_payload is None else conn_payload
+    res_data = send_req(arh_connect, conn_payload)
     return handle_connect_response(res_data)
 
 
-def getconn_payload():
-    global conn_payload
+def getconn_payload(wsgi_environ=None):
     config = get_agent().get_config()
     conn_payload = { 
+        "connect_info" : {
             "agent_info" : { 
-            "application.type": 'PYTHON', 
-            "agent.version": '1.0.3', 
+            "application.type": constants.python_str, 
+            "agent.version": config.get_agent_version(), 
             "application.name": config.get_app_name(), 
             "port": config.get_app_port(), 
             "host.type": config.get_host_type(),
             "hostname": config.get_host_name(),
+            "fqdn" : config.get_fqdn()
         }, "environment" : { 
             #"UserName": process.env.USER, 
             "OSVersion": platform.release(), 
             "MachineName": platform.node(), 
             'AgentInstallPath': config.get_installed_dir(), 
             "Python version": platform.python_version(), 
             "OSArch": platform.machine(), 
             "OS": platform.system(),
             "Python implementation" : platform.python_implementation()
         }
+    },
+        "misc_info" : {}
     }
-    return conn_payload
+    if wsgi_environ is not None:
+        txn_name = wsgi_environ.get(constants.path_info_str, '')
+        conn_payload["misc_info"]["txn.name"] = txn_name
+    if config.is_using_exporter():
+        conn_payload = json.dumps(conn_payload)
+        conn_payload+="\n"
+    return conn_payload
```

### Comparing `apminsight-1.0.3/apminsight/collector/datahandler.py` & `apminsight-1.1.0/apminsight/collector/datahandler.py`

 * *Files identical despite different names*

### Comparing `apminsight-1.0.3/apminsight/collector/reqhandler.py` & `apminsight-1.1.0/apminsight/collector/reqhandler.py`

 * *Files identical despite different names*

### Comparing `apminsight-1.0.3/apminsight/collector/rescodes.py` & `apminsight-1.1.0/apminsight/collector/rescodes.py`

 * *Files identical despite different names*

### Comparing `apminsight-1.0.3/apminsight/collector/reshandler.py` & `apminsight-1.1.0/apminsight/collector/reshandler.py`

 * *Files identical despite different names*

### Comparing `apminsight-1.0.3/apminsight/config/configuration.py` & `apminsight-1.1.0/apminsight/config/configuration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,104 @@
 
 import os
 import requests
 import apminsight
+import socket
+import platform
+import json
 import apminsight.constants as constants
 from apminsight.logger import agentlogger
 from apminsight.util import is_empty_string, is_non_empty_string
-import platform
 
 class Configuration:
     __license_key = None
     __app_name = None
     __app_port =  None
+    __app_port_set = None
     __collector_host = None
     __collector_host = None
     __proxy_server_host = None
     __proxy_server_port = None
     __proxy_username = None
     __proxy_password = None
     __agent_version = None
     __installed_path = None
     __cloud_instance_id = None
     __is_cloud_instance = None
     __cloud_type = None
+    __exporter = None
+    __exporter_status_port = None
+    __exporter_data_port = None
+    __exporter_host = None
+    __host_type = None
+    __is_docker = None
+    __host_name = None
+    __fqdn = None
 
     def __init__(self, info):
-        self.__license_key = get_license_key(info)
+        self.__license_key = None#get_license_key(info)   Not reading from user config
         self.__app_name = get_app_name(info)
-        self.__app_port = get_app_port(info)
+        self.__app_port = None
+        self.__app_port_set = False
         self.__collector_host = get_collector_host(self.__license_key, info)
         self.__collector_port = get_collector_port(info)
         self.__proxy_server_host = get_proxy_server_host(info)
         self.__proxy_server_port = get_proxy_server_port(info)
         self.__proxy_username = get_proxy_auth_username(info)
         self.__proxy_password = get_proxy_auth_password(info)
         self.__agent_version = apminsight.version
         payload_config = os.getenv(constants.apm_print_payload, '')
         self.print_payload = False if is_empty_string(payload_config) else True
         self.__installed_path = apminsight.installed_path
-        self.__is_cloud_instance, self.__cloud_type, self.__cloud_instance_id = get_cloud_details(self)
-        
+        self.__is_cloud_instance, self.__cloud_type, self.__cloud_instance_id = get_cloud_details() if not using_exporter(info) else (None, None, None)
+        self.__exporter = using_exporter(info)
+        self.__exporter_status_port = get_exporter_status_port(info)
+        self.__exporter_data_port = get_exporter_data_port(info)
+        self.__exporter_host = get_exporter_host(info)
+        self.__is_docker, self.__host_type, self.__host_name = get_docker_env_details()
+        self.__fqdn = get_fqdn()
         
     def is_configured_properly(self):
         if is_empty_string(self.__license_key):
             return False
        
         return True
 
     def update_collector_info(self, collector_info):
         if collector_info is None:
             return
 
         try:
-            self.__collector_host = collector_info.get('host', self.__collector_host)
-            self.__collector_port = collector_info.get('port', self.__collector_port)
+            self.__collector_host = collector_info.get(constants.host_str, self.__collector_host)
+            self.__collector_port = collector_info.get(constants.port_str, self.__collector_port)
         except Exception:
             agentlogger.exception('while updating collector info')
             
     def get_license_key(self):
         return self.__license_key
 
     def get_app_name(self):
         return self.__app_name
 
-    def get_app_port(self):
-        return self.__app_port
+    def set_app_name(self, appname):
+        self.__app_name = appname
+        
+    def get_app_port(self, for_exporter=True):
+        if self.__app_port is not None:
+            if not for_exporter or not self.__exporter:
+                return self.__app_port
+            return int(self.__app_port)
         
+    def set_app_port(self, app_port):
+        self.__app_port = app_port
+        self.__app_port_set = True
+        
+    def app_port_set(self):
+        return self.__app_port_set
+    
     def get_collector_host(self):
         return self.__collector_host
 
     def get_collector_port(self):
         return self.__collector_port
 
     def get_agent_version(self):
@@ -85,21 +115,28 @@
 
     def get_cloud_instance_id(self):
         return self.__cloud_instance_id
 
     def get_cloud_type(self):
         return self.__cloud_type
 
-    def get_host_name(self):
-        if  self.__cloud_instance_id:
+    def get_fqdn(self):
+        return self.__fqdn
+        
+    def get_host_name(self, for_exporter=True):
+        if self.__is_docker:
+            return self.__host_name
+        if not for_exporter or not self.__exporter and self.__cloud_instance_id:
             return self.__cloud_instance_id
         return platform.node()
         
-    def get_host_type(self):
-        if self.__cloud_type:
+    def get_host_type(self, for_exporter=True):
+        if self.__is_docker:
+            return self.__host_type
+        if not for_exporter or not self.__exporter and self.__cloud_type:
             return self.__cloud_type
         return platform.system()
 
     def get_proxy_details(self):
         if not self.__proxy_server_host or not self.__proxy_server_port:
             return False
         if self.__proxy_username and self.__proxy_password :
@@ -107,15 +144,44 @@
                     'https': 'http://' + self.__proxy_username + ':' + self.__proxy_password + '@' + self.__proxy_server_host + ':' + self.__proxy_server_port
                     }
         else:
             proxy_details = { 'http': 'http://' + self.__proxy_server_host + ':' + self.__proxy_server_port,
                     'https': 'http://' + self.__proxy_server_host + ':' + self.__proxy_server_port
                     }
         return proxy_details
+
+    def is_using_exporter(self):
+        return self.__exporter
+
+    def get_exporter_status_port(self):
+        return self.__exporter_status_port 
         
+    def get_exporter_data_port(self):
+        return self.__exporter_data_port
+
+    def get_exporter_host(self):
+        return self.__exporter_host
+
+    def set_license_key(self, license_str):
+        if is_non_empty_string(license_str):
+            self.__license_key = license_str
+    
+    def get_user_setup_config(self):
+        return {
+                        constants.APP_NAME : self.get_app_name(),
+                        constants.HOST_NAME : self.get_host_name(),
+                        constants.APP_PORT : self.get_app_port(),
+                        constants.EXP_HOST : self.get_exporter_host(),
+                        constants.EXP_STATUS_PORT : self.get_exporter_status_port(),
+                        constants.EXP_DATA_PORT : self.get_exporter_data_port(),
+                        constants.PROXY_DETAILS : self.get_proxy_details(),
+                        constants.AGENT_VERSION : self.get_agent_version()
+            },
+        
+    
 def get_collector_host(license_key, info):
 
     host = os.getenv(constants.apm_collector_host, '')
     if is_non_empty_string(host):
         return host
 
     if 'apm_collector_host' in info and is_non_empty_string(info['apm_collector_host']):
@@ -128,28 +194,30 @@
         if license_key.startswith('cn_'):
             return constants.cn_collector_host
 
         if license_key.startswith('in_'):
             return constants.ind_collector_host
 
         if license_key.startswith('au_'):
-            return constants.aus_collector_host 
+            return constants.aus_collector_host
+        
+        if license_key.startswith('jp_'):
+            return constants.jp_collector_host
 
         return constants.us_collector_host
 
     return ''
 
 
 def get_license_key(info):
     license_key = os.getenv(constants.license_key_env)
     if is_non_empty_string(license_key):
         return license_key
     if 'license_key' in info and is_non_empty_string(info['license_key']):
         return info['license_key']
-
     return ''
 
 def get_app_name(info):
 
     app_name = os.getenv(constants.apm_app_name)
     if is_non_empty_string(app_name) :
         return app_name
@@ -205,41 +273,106 @@
     proxy_auth_password = os.getenv('PROXY_AUTH_PASSWORD')
     if is_non_empty_string(proxy_auth_password):
         return proxy_auth_password
     if 'proxy_auth_password' in info and is_non_empty_string(info['proxy_auth_password']):
         return info['proxy_auth_password']
     return None
 
-def is_aws(self):
+def get_fqdn():
+    try:
+        return socket.getfqdn()
+    except Exception:
+        agentlogger.info("while fetching fqdn")
+    return ''
+        
+def is_aws():
     try: 
         response = requests.get(constants.aws_url, timeout=0.005)
-        # rep.encoding = 'utf8'
         if(response.status_code == 200 and  is_non_empty_string(response.text)):
             cloud_instance_id = response.text
             cloud_type = "AWS"
             return (True, cloud_type, cloud_instance_id)
     except Exception:
         agentlogger.info('AWS instance checking Failed')
 
     return False
 
-def is_azure(self): 
+def is_azure(): 
     try:
         headers = {'content-type': 'application/json'}
         response = requests.get(constants.azure_url, headers=headers, timeout=0.005)
         if(response.status_code == 200 and is_non_empty_string(response.json().get('ID'))):
             cloud_instance_id = response.json().get('ID')
             cloud_type = "AZURE"
             return (True, cloud_type, cloud_instance_id)
     except Exception:
         agentlogger.info('Azure instance checking Failed')
 
     return False
 
-def get_cloud_details(self):
-    aws =  is_aws(self)
-    azure = is_azure(self)
+def get_docker_env_details():
+    host_name = None
+    host_type = None
+    try:
+        with open('/proc/self/cgroup','r') as cgroup:
+            cgroup_info = cgroup.read()
+            if(isinstance(cgroup_info,str) and is_non_empty_string(cgroup_info)):
+                line_with_id = [ info for info in cgroup_info.split('\n') if "docker/" in info]
+                if (line_with_id) :
+                    id = line_with_id[0].split('docker/').pop()
+                    host_name = id
+                    host_type = 'DOCKER'
+                    return (True, host_type, host_name) 
+                else :
+                    agentlogger.info("Not a docker environment.") 
+            else:
+                with open('/proc/self/cpuset','r') as cpuset:
+                    cpuset_info = cpuset.read()
+                    if(isinstance(cpuset_info,str) and is_non_empty_string(cpuset_info)):
+                        id = cgroup_info.replace("/docker/","")
+                        host_name = id
+                        host_type = 'DOCKER'
+                        return (True, host_type, host_name)
+                    else :
+                        agentlogger.info("Not a docker environment.") 
+    except Exception:
+        agentlogger.info('Exception checking docker environment')
+    return (False, host_type, host_name)
+
+def get_cloud_details():
+    aws =  is_aws()
+    azure = is_azure()
     if aws:
         return aws 
     elif azure:
         return azure
     return (False, None, None)
+
+def using_exporter(info):
+    using_exporter = info.get('exporter', True)
+    if using_exporter:
+        return True
+    return False
+
+def get_exporter_status_port(info):
+    exporter_status_port = os.getenv(constants.APM_EXP_STATUS_PORT)
+    if is_non_empty_string(exporter_status_port):
+        return exporter_status_port
+    if 'exporter_status_port' in info and is_non_empty_string(info['exporter_status_port']):
+        return info['exporter_status_port']
+    return '20021'
+
+def get_exporter_data_port(info):
+    exporter_data_port = os.getenv(constants.APM_EXP_DATA_PORT)
+    if is_non_empty_string(exporter_data_port):
+        return exporter_data_port
+    if 'exporter_data_port' in info and is_non_empty_string(info['exporter_data_port']):
+        return info['exporter_data_port']
+    return '20022'
+ 
+def get_exporter_host(info):
+    exporter_host = os.getenv(constants.APM_EXP_HOST)
+    if is_non_empty_string(exporter_host):
+        return exporter_host
+    if 'exporter_host' in info and is_non_empty_string(info['exporter_host']):
+        return info['exporter_host']
+    return constants.localhost_str
```

### Comparing `apminsight-1.0.3/apminsight/config/threshold.py` & `apminsight-1.1.0/apminsight/config/threshold.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 
 import re
 import apminsight.constants as constants
 from apminsight.logger import agentlogger
-from apminsight.util import current_milli_time, is_empty_string
-
+from apminsight.util import current_milli_time, is_empty_string, is_non_empty_string
 class Threshold:
 
     def __init__(self):
         self.thresholdmap = {}
         self.last_modified = current_milli_time()
 
-    
+    def update_sql_trace_threshold(self, sql_trace_threshold):
+        if sql_trace_threshold is not None and isinstance(sql_trace_threshold, int):
+            self.thresholdmap[constants.sql_stracktrace] = float(sql_trace_threshold)
+
+    def update_sql_capture_enabled(self, sql_capture_enabled):
+        if is_non_empty_string(sql_capture_enabled):
+            self.thresholdmap[constants.sql_capture] = True if sql_capture_enabled else False
+
     def update(self, custom_config, agent_specific):
         try:
             if custom_config is not None:
                 self.thresholdmap.update(custom_config)
 
             if agent_specific is not None:
                 self.thresholdmap.update(agent_specific)
@@ -118,8 +124,7 @@
     def is_bgtxn_trace_enabled(self):
         return self.thresholdmap.get(constants.bgtxn_trace_enabled, True)
 
     def get_bgtxn_trace_threshold(self):
         th_seconds = self.thresholdmap.get(constants.bgtxn_traceth, 5)
         return th_seconds * 1000
 
-
```

### Comparing `apminsight-1.0.3/apminsight/context.py` & `apminsight-1.1.0/apminsight/context.py`

 * *Files identical despite different names*

### Comparing `apminsight-1.0.3/apminsight/contrib/django/wrapper.py` & `apminsight-1.1.0/apminsight/contrib/django/wrapper.py`

 * *Files identical despite different names*

### Comparing `apminsight-1.0.3/apminsight/instrumentation/dbapi2.py` & `apminsight-1.1.0/apminsight/agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,161 @@
 
+import copy
+from apminsight.collector.connhandler import init_connection
+from apminsight.metric.txn import Transaction
+from apminsight.metric.tracker import Tracker
+from apminsight.metric.dbtracker import DbTracker
+from apminsight.metric.metricstore import Metricstore
+from apminsight.config.configuration import Configuration
+from apminsight.collector.ins_info import Instanceinfo
+from apminsight.config.threshold import Threshold
+from apminsight import context
 from apminsight import constants
-from .wrapper import default_wrapper
-from apminsight.util import is_non_empty_string
-from apminsight.agentfactory import get_agent
 from apminsight.logger import agentlogger
-class CursorProxy():
-
-    def __init__(self, cursor, conn):
-        self._apm_wrap_cursor = cursor
-        self._apm_wrap_conn = conn
+from apminsight.util import check_and_create_base_dir
+from apminsight import agentfactory
+from apminsight.context import get_cur_txn
+from apminsight.collector.metric_dispatcher import MetricDispatcher
+from apminsight.collector.rescodes import res_codes_info
+
+
+def initalize(options={}):
+    options['agentbasedir'] = check_and_create_base_dir()
+    agentfactory.agent_instance = Agent(options)
+    agent_instance = agentfactory.agent_instance
+    if not agent_instance.get_config().is_using_exporter():
+        if not agent_instance.get_config().is_configured_properly():
+            raise RuntimeError('Configure license key properly')
+        init_connection()
+    return agent_instance
+
+class Agent:
+    def __init__(self, info):
+        self.config = Configuration(info)
+        self.ins_info = Instanceinfo(info)
+        self.threshold = Threshold()
+        self.metricstore = Metricstore() if not self.config.is_using_exporter() else None
+        self.txn_queue = [] if not self.config.is_using_exporter() else None
+        self.metric_dispatcher = MetricDispatcher(self.config) if self.config.is_using_exporter() else None
         
-    def __getattr__(self, key):
-        if key in self.__dict__:
-            return getattr(self, key)
-
-        return getattr(self._apm_wrap_cursor, key)
-
-    def __setattr__(self, key, value):
-        if( key in ['_apm_wrap_cursor', '_apm_wrap_conn', 'execute', 'executemany']):
-            self.__dict__[key] = value
-        else:
-            return setattr(self._apm_wrap_conn, key, value)
-
-    def execute(self, *args, **kwargs):
-
-        if hasattr(self._apm_wrap_cursor, 'execute'):
-            actual = getattr(self._apm_wrap_cursor, 'execute')
-            method_info = {
-                constants.method_str : 'execute',
-                constants.component_str : self._apm_wrap_conn._apm_comp_name,
-                constants.extract_info : self._apm_extract_query,
-                constants.is_db_tracker : True
-            }
-            wrapper = default_wrapper(actual, 'Cursor', method_info)
-            return wrapper(*args, **kwargs)
-        else:
-            return self._apm_wrap_cursor.execute(*args, **kwargs)
-
-    def executemany(self, *args, **kwargs):
+    def update_app_port(self, app_port):
+        self.config.set_app_port(app_port)
+        self.metric_dispatcher.update_app_port(app_port)
         
-        if hasattr(self._apm_wrap_cursor, 'executemany'):
-            actual = getattr(self._apm_wrap_cursor, 'executemany')
-            method_info = {
-                constants.method_str : 'executemany',
-                constants.component_str : self._apm_wrap_conn._apm_comp_name,
-                constants.extract_info : self._apm_extract_query,
-                constants.is_db_tracker : True
-            }
-            wrapper = default_wrapper(actual, 'Cursor', method_info)
-            return wrapper(*args, **kwargs)
-        else:
-            return self._apm_wrap_cursor.executemany(*args, **kwargs)
-
-    def _apm_extract_query(self, tracker, args=(), kwargs={}, return_value=None):
-        tracker.set_info(self._apm_wrap_conn._apm_host_info)
-        threshold = get_agent().get_threshold()
-        if threshold.is_sql_capture_enabled() is not True:
-            return
+    def push_to_queue(self, txn):
+        self.txn_queue.append(txn)
 
-        if isinstance(args, (list, tuple)) and len(args)>0:
-            if is_non_empty_string(args[0]):
-                tracker.set_info({'query' : args[0]})
+    def get_txn_queue_for_metrics_processing(self):
+        txn_list = copy.copy(self.txn_queue)
+        self.txn_queue = []
+        return txn_list
+
+    def is_data_collection_allowed(self):
+        cur_status = self.ins_info.get_status()
+        if cur_status in [constants.manage_agent, constants.agent_config_updated]:
+            return True
+        
+        return False
 
+    def check_and_create_txn(self, wsgi_environ, root_tracker_info):
+        try:
+            if not self.get_config().app_port_set():
+                if not wsgi_environ.get(constants.server_port_str).isnumeric():
+                    agentlogger.info('Auto detection of port failed due to absense of SERVER PORT details in environ')
+                    return
+                self.update_app_port(wsgi_environ[constants.server_port_str])
+                    
+            if self.get_config().is_using_exporter():
+                self.metric_dispatcher.update_threshold_config(wsgi_environ)
+                if not self.metric_dispatcher.started():
+                    self.metric_dispatcher.start_dispatching()
+
+            context.clear_cur_context()
+            if not self.is_data_collection_allowed():
+                if not self.get_ins_info().get_status():
+                    agentlogger.info('data collection stopped due to no response code')
+                else:
+                    agentlogger.info('data collection stopped due to response code %s %s', str(self.get_ins_info().get_status()), res_codes_info.get(self.get_ins_info().get_status()).get('name'))
+                return
+
+            if type(wsgi_environ) is not dict:
+                return
+
+            if type(root_tracker_info) is not dict:
+                return
+
+            uri = wsgi_environ.get(constants.path_info_str, '')
+            if not self.threshold.is_txn_allowed(uri):
+                agentlogger.info(uri + ' txn skipped')
+                return
+
+            txn = Transaction(wsgi_environ, root_tracker_info)
+            context.ser_cur_context(txn, txn.get_root_tracker())
+            # handle cross app response
+            return txn
+        except Exception:
+            agentlogger.exception("while creating txn obj")
+        return Transaction(wsgi_environ, root_tracker_info)
+
+    def check_and_create_tracker(self, tracker_info):
+        track = None
+        cur_txn = get_cur_txn()
+        try:
+            if type(tracker_info) is not dict:
+                return None
 
-class ConnectionProxy():
+            if context.is_txn_active() is not True:
+                return None
 
-    def __init__(self, conn, comp, host_info):
-        self._apm_wrap_conn = conn
-        self._apm_comp_name = comp
-        self._apm_host_info = host_info
+            if 'parent' not in tracker_info:
+                tracker_info['parent'] = context.get_cur_tracker()
 
-    def cursor(self, *args, **kwargs):
-        real_cursor = self._apm_wrap_conn.cursor(*args, **kwargs)
-        try:
-            cur = CursorProxy(real_cursor, self)
-            return cur
-        except:
-            agentlogger.exception("While creating CursorProxy object")
-            return real_cursor
+            if constants.is_db_tracker_str in tracker_info:
+                track = DbTracker(tracker_info)
+            else:
+                track = Tracker(tracker_info)
 
-    #Special case for capturing SQLITE calls when executed with Connection object
-    def execute(self, *args, **kwargs):
+            cur_txn.increment_method_count(1)
 
-        if hasattr(self._apm_wrap_conn, 'execute'):
-            actual = getattr(self._apm_wrap_conn, 'execute')
-            method_info = {
-                constants.method_str : 'execute',
-                constants.component_str : self._apm_comp_name,
-                constants.extract_info : self._apm_extract_query,
-                constants.is_db_tracker : True
-            }
-            wrapper = default_wrapper(actual, 'Connection', method_info)
-            return wrapper(*args, **kwargs)
-        else:
-            return self._apm_wrap_conn.execute(*args, **kwargs)
-
-
-    def executemany(self, *args, **kwargs):
-
-        if hasattr(self._apm_wrap_conn, 'executemany'):
-            actual = getattr(self._apm_wrap_conn, 'executemany')
-            method_info = {
-                constants.method_str : 'executemany',
-                constants.component_str : self._apm_comp_name,
-                constants.extract_info : self._apm_extract_query,
-                constants.is_db_tracker : True
-            }
-            wrapper = default_wrapper(actual, 'Connection', method_info)
-            return wrapper(*args, **kwargs)
-        else:
-            return self._apm_wrap_conn.executemany(*args, **kwargs)
-    
-    def _apm_extract_query(self, tracker, args=(), kwargs={}, return_value=None):
-        tracker.set_info(self._apm_host_info)
-        threshold = get_agent().get_threshold()
-        if threshold.is_sql_capture_enabled() is not True:
-            return
+            context.set_cur_tracker(track)
+        except:
+            agentlogger.exception("While creating Tracker")
+        
+        return track
 
-        if isinstance(args, (list, tuple)) and len(args)>0:
-            if is_non_empty_string(args[0]):
-                tracker.set_info({'query' : args[0]})
-
-    def __getattr__(self, key):
-        if key in self.__dict__:
-            return getattr(self, key)
-
-        return getattr(self._apm_wrap_conn, key)
-
-    def __setattr__(self, key, value):
-        if( key in ['_apm_wrap_conn', '_apm_comp_name', '_apm_host_info']):
-            self.__dict__[key] = value
-        else:
-            return setattr(self._apm_wrap_conn, key, value)
     
-    @staticmethod
-    def get_host_info(method_info, conn_kwargs):
-        host_info = {}
+    def end_txn(self, txn, res=None, err=None):
         try:
-            if constants.host in conn_kwargs:
-                host_info[constants.host] = conn_kwargs[constants.host]
-            elif constants.default_host in method_info:
-                host_info[constants.host] = method_info[constants.default_host]
-
-            if constants.port in conn_kwargs:
-                host_info[constants.port] = conn_kwargs[constants.port]
-            elif constants.default_port in method_info:
-                host_info[constants.port] = method_info[constants.default_port]
-        except:
-            agentlogger.exception("While extracting host_info")
-        return host_info
+            if txn is None:
+                return
 
-    @staticmethod
-    def instrument_conn(original, module, method_info):
-        def conn_wrapper(*args, **kwargs):
-            conn = original(*args, **kwargs)
-            if conn is not None:
-                comp = method_info.get(constants.component_str, '')
-                host_info = ConnectionProxy.get_host_info(method_info, kwargs)
-                new_conn = ConnectionProxy(conn, comp, host_info)
-                return new_conn
+            if isinstance(txn, Transaction):
+                txn.end_txn(res, err)
+        except Exception:
+            agentlogger.exception("tracking end txn")
 
-            return conn
 
-        return conn_wrapper
+    def end_tracker(self, tracker, err=None):
+        if isinstance(tracker, Tracker) is not True:
+            return
 
+        txn=context.get_cur_txn()
+        if isinstance(txn, Transaction):
+            tracker.end_tracker(err)
+            cur_txn = context.get_cur_txn()
+            cur_txn.handle_end_tracker(tracker)
+
+
+    def get_config(self):
+        return self.config
+
+    def get_threshold(self):
+        return self.threshold
+
+    def get_ins_info(self):
+        return self.ins_info
+
+    def get_metric_store(self):
+        for txn in self.get_txn_queue_for_metrics_processing():
+            self.metricstore.add_web_txn(txn)
+        return self.metricstore
+
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/modules.py` & `apminsight-1.1.0/apminsight/instrumentation/modules.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,42 @@
-
-from apminsight import constants
 from apminsight.instrumentation.packages import django
 from apminsight.instrumentation.packages import sqlite
 from apminsight.instrumentation.packages import mysql
 from apminsight.instrumentation.packages import flask
 from apminsight.instrumentation.packages import redis
 from apminsight.instrumentation.packages import jinja2
 from apminsight.instrumentation.packages import pymemcache
 from apminsight.instrumentation.packages import psycopg2
 from apminsight.instrumentation.packages import cassandra
 from apminsight.instrumentation.packages import memcache
+from apminsight.instrumentation.packages import bottle
+from apminsight.instrumentation.packages import cherrypy
+from apminsight.instrumentation.packages import pyramid
+from apminsight.instrumentation.packages import mako
+from apminsight.instrumentation.packages import genshi
+from apminsight.instrumentation.packages import http
+from apminsight.instrumentation.packages import httpx
+from apminsight.instrumentation.packages import httplib2
+from apminsight.instrumentation.packages import urllib
+from apminsight.instrumentation.packages import urllib3
 
 modules_info = {}
 modules_info.update(django.module_info)
 modules_info.update(sqlite.module_info)
 modules_info.update(mysql.module_info)
 modules_info.update(flask.module_info)
 modules_info.update(redis.module_info)
 modules_info.update(jinja2.module_info)
 modules_info.update(pymemcache.module_info)
 modules_info.update(psycopg2.module_info)
 modules_info.update(cassandra.module_info)
 modules_info.update(memcache.module_info)
+modules_info.update(bottle.module_info)
+modules_info.update(cherrypy.module_info)
+modules_info.update(pyramid.module_info)
+modules_info.update(mako.module_info)
+modules_info.update(genshi.module_info)
+modules_info.update(http.module_info)
+modules_info.update(httpx.module_info)
+modules_info.update(httplib2.module_info)
+modules_info.update(urllib.module_info)
+modules_info.update(urllib3.module_info)
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/cassandra.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/redis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,54 @@
+
 from apminsight import constants
 from apminsight.util import is_non_empty_string
-from apminsight.agentfactory import get_agent
+from apminsight.metric.tracker import Tracker
+from apminsight.context import get_cur_tracker
 from apminsight.logger import agentlogger
+def extract_info(tracker, args):
+    if not isinstance(tracker, Tracker):
+        return
 
-def extract_query(tracker, args=(), kwargs={}, return_value=None):
-    threshold = get_agent().get_threshold()
-    if threshold.is_sql_capture_enabled() is not True:
+    if tracker.get_component()!=constants.redis_comp:
         return
 
     if isinstance(args, (list, tuple)) and len(args)>1:
-
         if is_non_empty_string(args[1]):
-            tracker.set_info({ 'query' : args[1]})
-        elif isinstance(args[1], (bytes, bytearray)):
-            query = args[1].decode("utf-8")
-            tracker.set_info({ 'query' : query})  
-    try:
-        (host,port)=str(return_value.response_future.coordinator_host).split(":")
-        port=int(port)
-        tracker.set_info({'host':host,'port':port})
+            tracker.set_info({constants.OPERATION : args[1]})
 
-    except:
-        agentlogger.exception("Extracting the Host for CASSANDRA query")
+        if hasattr(args[0], constants.host_str) and hasattr(args[0], constants.port_str):
+            host = getattr(args[0], constants.host_str)
+            port = getattr(args[0], constants.port_str)
+            tracker.set_info({constants.host_str : host, constants.port_str : port})
+        
+
+def wrap_send_command(actual, module, method_info):
+    def redis_wrapper(*args, **kwargs):
+        try:
+            tracker = get_cur_tracker()
+            extract_info(tracker, args)
+        except:
+            agentlogger.exception("While extracting Redis call info")
+        finally:
+            return actual(*args, **kwargs)
 
+    return redis_wrapper
 
-module_info = {
-    'cassandra.cluster' : [
-        {   
-            constants.class_str : 'Cluster',
-            constants.method_str : 'connect',
-            constants.component_str : constants.cassandra_comp,
-        },
-
-        {   
-            constants.class_str : 'Cluster',
-            constants.method_str : 'shutdown',
-            constants.component_str : constants.cassandra_comp,
-        },
 
+module_info = {
+    'redis.client' : [
+        {
+            constants.class_str : 'Redis',
+            constants.method_str : 'execute_command',
+            constants.component_str : constants.redis_comp
+        }
+    ],
+    'redis.connection' : [
         {
-            constants.class_str : 'Session',
-            constants.method_str : 'execute',
-            constants.component_str : constants.cassandra_comp,
-            constants.extract_info : extract_query,
-            constants.is_db_tracker : True
-        },
+            constants.class_str : 'Connection',
+            constants.method_str : 'send_command',
+            constants.wrapper_str : wrap_send_command
+        }
+    ]
+}
+
 
-        ],
-    }
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/django.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/django.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 
 from apminsight import constants
 from apminsight.instrumentation.wrapper import wsgi_wrapper
 
+def wrap_get_wsgi_application(original, module, method_info):
+    def wrapper(*args, **kwargs):
+        from apminsight.instrumentation import instrument_django_middlewares
+        instrument_django_middlewares()
+        return original(*args, **kwargs)
+    return wrapper
+
 module_info = {
     'django.core.handlers.wsgi' : [
         {
             constants.class_str : 'WSGIHandler',
             constants.method_str : '__call__',
             constants.wrapper_str : wsgi_wrapper,
             constants.component_str : constants.django_comp
         }
     ],
     'django.conf.urls' : [
         {
             constants.method_str : 'url',
-            constants.wrap_args : 1,
+            constants.wrap_args_str : 1,
             constants.component_str : constants.django_comp
         }
     ],
     'django.urls' : [
         {
             constants.method_str : 'path',
-            constants.wrap_args : 1,
+            constants.wrap_args_str : 1,
             constants.component_str : constants.django_comp
         }
     ],
     'django.template' : [
         {
             constants.class_str : 'Template',
             constants.method_str : 'render',
             constants.component_str : constants.template
         }
-    ]
+    ],
+    'django.core.wsgi' : [
+        {
+            constants.method_str : 'get_wsgi_application',
+            constants.wrapper_str : wrap_get_wsgi_application,
+            constants.component_str : constants.django_comp
+        }
+    ],
 }
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/flask.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/flask.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from apminsight.context import get_cur_txn, is_no_active_txn
 from apminsight.logger import agentlogger
 
 def get_status_code(original, module, method_info):
     def wrapper(*args, **kwargs):
         if is_no_active_txn():
             return original(*args, **kwargs)
-            
-        res = original(*args, **kwargs)
-        cur_txn = get_cur_txn()
         try:
+            res = original(*args, **kwargs)
+        except Exception as exc:
+            raise exc
+        try:
+            cur_txn = get_cur_txn()
             from werkzeug.exceptions import HTTPException
             if isinstance(res, HTTPException):
-                cur_txn.status_code = int(res.code)
+                cur_txn.set_status_code(int(res.code))
         except:
             agentlogger.exception('Exception occured while getting Status Code')
         return res
     return wrapper
 
 module_info = {
     'flask' : [
@@ -28,15 +30,15 @@
             constants.wrapper_str : wsgi_wrapper,
             constants.component_str : constants.flask_comp
         },
         {
             constants.class_str : 'Flask',
             constants.method_str : 'add_url_rule',
             constants.component_str : constants.flask_comp,
-            constants.wrap_args : 3
+            constants.wrap_args_str : 3
         },
         {
             constants.class_str : 'Flask',
             constants.method_str : 'handle_user_exception',
             constants.wrapper_str : get_status_code,
             constants.component_str : constants.flask_comp
         },
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/memcache.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/httpx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-
 from apminsight import constants
-from apminsight.util import is_non_empty_string
+from apminsight.logger import agentlogger
 
-def extract_info(tracker, args=(), kwargs={}, return_value=None):
-    print(args)
-    print(kwargs)
-    if isinstance(args, (list, tuple)) and len(args)>1:
-        if is_non_empty_string(args[1]):
-            tracker.set_info({'opn' : args[1]})
-        elif isinstance(args[1], (bytes, bytearray)):
-            operation = args[1].decode("utf-8")
-            opn = operation.split()[0].upper()
-            tracker.set_info({ 'opn' : opn})
+def extract_req(tracker, args=(), kwargs={}, return_value=None, error=None):
+    try:
+        if args:
+            request = args[1]
+            method = request.method
+            url = request.url
+            url_str = str(url)
+            host = url.host
+            port = url.port
+            status = ''
+            if return_value:
+                status = str(return_value.status_code)
+            if status:
+                tracker.set_tracker_name( tracker.get_tracker_name() + " : " + method + ' - ' + status + ' - ' + url_str)
+                tracker.set_as_http_err() if int(status) >= 400 else 0
+            else:
+                tracker.set_tracker_name( tracker.get_tracker_name() + " : " + method + ' - ' + url_str)
+            info = {constants.HTTP_METHOD: method, constants.HTTP: host, constants.PORT: port, constants.URL: url_str, constants.STATUS: status}
+            tracker.set_info(info)
 
-        if hasattr(args[0], 'address'):
-            address = args[0].address
-            if isinstance(address, (list, tuple)) and len(address)==2:
-                tracker.set_info({'host' : address[0], 'port' : address[1]})
+    except Exception as exc:
+        agentlogger.exception("while extracting HTTPX request")
 
 module_info = {
-
-    'memcache' : [
-        {
-            constants.class_str : '_Host',
-            constants.method_str : 'send_cmd',
-            constants.component_str : constants.memcache_comp,
-            constants.extract_info : extract_info
+    'httpx._client' : [
+        {   constants.class_str : 'Client',
+            constants.method_str : 'send',
+            constants.component_str : constants.http_comp,
+            constants.extract_info_str : extract_req,
         },
-        {
-            constants.class_str : '_Host',
-            constants.method_str : 'send_cmds',
-            constants.component_str : constants.memcache_comp,
-            constants.extract_info : extract_info
-        },   
-    ]
+    ],
 }
-
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/mysql.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/mysql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 
 from apminsight import constants
 from apminsight.util import is_non_empty_string
 from apminsight.agentfactory import get_agent
 from apminsight.logger import agentlogger
+from apminsight.constants import db_opn_regex
+import re
 
-def extract_query(tracker, args=(), kwargs={}, return_value=None):
+
+def track_mysql_query_opn(tracker, args, kwargs):
+    query = ""
+    if is_non_empty_string(args[1]):
+        query = args[1]
+        
+    elif isinstance(args[1], (bytes, bytearray)):
+        query = args[1].decode("utf-8")
+        
+    if query:
+        tracker.set_info({ constants.query_str : query})  
+        opn_name = query.split(' ')[0]
+        if opn_name.lower() in db_opn_regex:
+            regex = db_opn_regex[opn_name.lower()]
+            matchobj = re.match(regex, query, re.IGNORECASE)
+            if matchobj is not None:
+                tracker.set_info({ constants.OPERATION : matchobj.group(1).lower(), constants.OBJECT : matchobj.group(2)})
+
+def extract_query(tracker, args=(), kwargs={}, return_value=None, error=None):
     threshold = get_agent().get_threshold()
     if threshold.is_sql_capture_enabled() is not True:
         return
 
     if isinstance(args, (list, tuple)) and len(args)>1:
-        if is_non_empty_string(args[1]):
-            tracker.set_info({ 'query' : args[1]})
-        elif isinstance(args[1], (bytes, bytearray)):
-            query = args[1].decode("utf-8")
-            tracker.set_info({ 'query' : query})
+        track_mysql_query_opn(tracker,args,kwargs)
         try:
             host= args[0].connection.host
             port= args[0].connection.port
-            tracker.set_info({'host':host,'port':port})
+            tracker.set_info({constants.host_str:host,constants.port_str:port})
         except:
             agentlogger.exception("Extracting host info from MYSQL query")
 
 module_info = {
     'pymysql' : [
         {
             constants.method_str : 'connect',
@@ -30,21 +46,21 @@
         }
     ],
     'pymysql.cursors' : [
         {
             constants.class_str : 'Cursor',
             constants.method_str : 'execute',
             constants.component_str : constants.mysql_comp,
-            constants.extract_info : extract_query,
-            constants.is_db_tracker : True
+            constants.extract_info_str : extract_query,
+            constants.is_db_tracker_str : True
         }
     ],
     'MySQLdb.connections' : [
         {
             constants.class_str : 'Connection',
             constants.method_str : 'query',
             constants.component_str : constants.mysql_comp,
-            constants.extract_info : extract_query,
-            constants.is_db_tracker : True
+            constants.extract_info_str : extract_query,
+            constants.is_db_tracker_str : True
         }
     ]
-}
+}
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/pymemcache.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/psycopg2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,65 @@
-
 from apminsight import constants
-from apminsight.util import is_non_empty_string
-from apminsight.metric.tracker import Tracker
-from apminsight.context import get_cur_tracker
-
-def extract_info(tracker, args=(), kwargs={}, return_value=None):
-    if isinstance(args, (list, tuple)) and len(args)>1:
-        if is_non_empty_string(args[1]):
-            tracker.set_info({'opn' : args[1]})
-        elif isinstance(args[1], (bytes, bytearray)):
-            opn = args[1].decode("utf-8")
-            tracker.set_info({ 'opn' : opn})
-
-        if hasattr(args[0], 'server'):
-            server = args[0].server
-            if isinstance(server, (list, tuple)) and len(server)==2:
-                tracker.set_info({'host' : server[0], 'port' : server[1]})
+from apminsight.instrumentation.dbapi2 import ConnectionProxy
 
+def wrap_register_type(original, module, method_info):
+    def wrapper(*args, **kwargs):
+        def get_arguments(obj, scope=None):
+            return obj, scope
+
+        obj, conn_or_curs = get_arguments(*args, **kwargs)
+        if conn_or_curs:
+            return original(obj, conn_or_curs.__original__)
+        else:
+            return original(obj)
+    return wrapper
+
+def wrap_quote_ident(original, module, method_info):
+    def wrapper(*args, **kwargs):
+        def get_arguments(obj, scope=None):
+            return obj, scope
+
+        obj, conn_or_curs = get_arguments(*args, **kwargs)
+        if conn_or_curs:
+            return original(obj, conn_or_curs.__original__)
+        else:
+            return original(obj)
+    return wrapper
 
 module_info = {
-    'pymemcache.client.base' : [
+    'psycopg2' : [
+        {
+            constants.method_str : 'connect',
+            constants.component_str : constants.postgres_comp,
+            constants.wrapper_str : ConnectionProxy.instrument_conn,
+            constants.default_host_str : constants.localhost_str,
+            constants.default_port_str : 5432,
+            constants.proxy_class_str : ConnectionProxy
+        }
+    ],
+    'psycopg2.extensions': [
         {
-            constants.class_str : 'Client',
-            constants.method_str : '_fetch_cmd',
-            constants.component_str : constants.memcache_comp,
-            constants.extract_info : extract_info
+            constants.method_str : 'register_type',
+            constants.component_str : constants.postgres_comp,
+            constants.wrapper_str : wrap_register_type,
         },
         {
-            constants.class_str : 'Client',
-            constants.method_str : '_store_cmd',
-            constants.component_str : constants.memcache_comp,
-            constants.extract_info : extract_info
+            constants.method_str : 'quote_ident',
+            constants.component_str : constants.postgres_comp,
+            constants.wrapper_str : wrap_quote_ident,
         },
+    ],
+    'psycopg2._psycopg' : [
         {
-            constants.class_str : 'Client',
-            constants.method_str : '_misc_cmd',
-            constants.component_str : constants.memcache_comp,
-            constants.extract_info : extract_info
+            constants.method_str : 'register_type',
+            constants.component_str : constants.postgres_comp,
+            constants.wrapper_str : wrap_register_type,
+        }
+    ],
+    'psycopg2._json' : [
+        {
+            constants.method_str : 'register_type',
+            constants.component_str : constants.postgres_comp,
+            constants.wrapper_str : wrap_register_type,
         }
     ]
 }
-
-
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/redis.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/urllib3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 
 from apminsight import constants
-from apminsight.util import is_non_empty_string
-from apminsight.metric.tracker import Tracker
-from apminsight.context import get_cur_tracker
 from apminsight.logger import agentlogger
-def extract_info(tracker, args):
-    if not isinstance(tracker, Tracker):
-        return
-
-    if tracker.get_component()!=constants.redis_comp:
-        return
-
-    if isinstance(args, (list, tuple)) and len(args)>1:
-        if is_non_empty_string(args[1]):
-            tracker.set_info({'opn' : args[1]})
-
-        if hasattr(args[0], 'host') and hasattr(args[0], 'port'):
-            host = getattr(args[0], 'host')
-            port = getattr(args[0], 'port')
-            tracker.set_info({'host' : host, 'port' : port})
-        
-
-def wrap_send_command(actual, module, method_info):
-    def redis_wrapper(*args, **kwargs):
-        try:
-            tracker = get_cur_tracker()
-            extract_info(tracker, args)
-        except:
-            agentlogger.exception("While extracting Redis call info")
-        finally:
-            return actual(*args, **kwargs)
 
-    return redis_wrapper
+def get_request_url(conn,args, kwargs):
+    from urllib3.connectionpool import HTTPSConnection
+    if isinstance(conn, HTTPSConnection):
+        return 'https://' + conn.host + kwargs.get(constants.URL)
+    else:
+        return 'http://' + conn.host + kwargs.get(constants.URL)
+
+
+def get_conn_object(args):
+    if len(args) :
+        return args[0]
+    return None
+
+def get_conn_host_port( conn):
+    if conn:
+        return conn.host, conn.port
+    return None, None
+    
+def extract_urllib3_request(tracker, args=(), kwargs={}, return_value=None, error=None):
+    try:
+        conn = get_conn_object(args)
+        host, port = get_conn_host_port(conn) 
+        method = ""
+        url = ""
+        
+        if conn and len(args)==1:
+            method = 'REQUESTS' + ' - ' + kwargs.get('method')
+            url  = get_request_url(conn, args, kwargs)   
+        elif len(args)==3:
+            method = args[1]
+            url = kwargs.get(constants.REQUEST_URL)
+
+        if conn:
+            status = str(return_value.status) if return_value is not None else None
+            if status:
+                tracker.set_tracker_name( tracker.get_tracker_name() + " : " + method + ' - ' + status + ' - ' + url)
+                tracker.set_as_http_err() if int(status) >= 400 else 0
+            else:
+                tracker.set_tracker_name( tracker.get_tracker_name() + " : " + method + ' - ' + url)
+            tracker.set_info({constants.HTTP_METHOD: method, constants.HOST: host, constants.PORT: port, constants.URL: url, constants.STATUS: status})
 
+    except:
+        agentlogger.exception("while extracting URLLIB3 request")
 
 module_info = {
-    'redis.client' : [
-        {
-            constants.class_str : 'Redis',
-            constants.method_str : 'execute_command',
-            constants.component_str : constants.redis_comp
+
+    'urllib3.connectionpool' : [
+        {   constants.class_str : 'HTTPConnectionPool',
+            constants.method_str : 'urlopen',
+            constants.component_str : constants.http_comp,
+            constants.extract_info_str : extract_urllib3_request
         }
     ],
-    'redis.connection' : [
-        {
-            constants.class_str : 'Connection',
-            constants.method_str : 'send_command',
-            constants.wrapper_str : wrap_send_command
-        }
-    ]
 }
-
-
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/packages/sqlite.py` & `apminsight-1.1.0/apminsight/instrumentation/packages/sqlite.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 
 from apminsight import constants
-from apminsight.instrumentation.dbapi2 import ConnectionProxy
+from apminsight.instrumentation.dbapi2 import ConnectionProxySqlite
 
 module_info = {
     'sqlite3' : [
         {
             constants.method_str : 'connect',
             constants.component_str : constants.sqlite_comp,
-            constants.wrapper_str : ConnectionProxy.instrument_conn
+            constants.wrapper_str : ConnectionProxySqlite.instrument_conn,
+            constants.proxy_class_str : ConnectionProxySqlite
+
         }
     ],
     'sqlite3.dbapi2' : [
         {
             constants.method_str : 'connect',
             constants.component_str : constants.sqlite_comp,
-            constants.wrapper_str : ConnectionProxy.instrument_conn
+            constants.wrapper_str : ConnectionProxySqlite.instrument_conn,
+            constants.proxy_class_str : ConnectionProxySqlite
         }
     ]
 }
+
+from sqlite3 import connect
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/util.py` & `apminsight-1.1.0/apminsight/instrumentation/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
-from apminsight.constants import method_str, component_str, is_db_tracker
+from apminsight.constants import method_str, component_str, is_db_tracker_str
 from apminsight.metric.tracker import Tracker
 from apminsight.logger import agentlogger
 
 def create_tracker_info(module, method_info, parent_tracker=None):
     tracker_info = None
     try:
         tracker_name = module + '.' + method_info[method_str]
         tracker_info = { 'name' : tracker_name }
         if isinstance(parent_tracker, Tracker):
             tracker_info['parent'] = parent_tracker
 
         if component_str in method_info:
             tracker_info[component_str] = method_info[component_str]
 
-        if is_db_tracker in method_info:
-            tracker_info[is_db_tracker] = True
+        if is_db_tracker_str in method_info:
+            tracker_info[is_db_tracker_str] = True
     except Exception:
         agentlogger.exception("while creating tracker info")
     finally:
         return tracker_info
```

### Comparing `apminsight-1.0.3/apminsight/instrumentation/wrapper.py` & `apminsight-1.1.0/apminsight/instrumentation/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,100 @@
 
+from importlib import import_module
+from apminsight import constants
 from apminsight.agentfactory import get_agent
 from apminsight.logger import agentlogger
-from apminsight.constants import wrap_args
 from apminsight.util import is_callable
-from apminsight.context import clear_cur_context
-from apminsight.metric.tracker import Tracker
-from apminsight.constants import component_str, extract_info
-from apminsight.instrumentation.util import create_tracker_info
-from apminsight.context import is_no_active_txn, get_cur_tracker, set_cur_tracker
+from apminsight.constants import class_str, method_str, wrapper_str, wrap_args_str
+from apminsight.instrumentation.modules import modules_info
+from apminsight.instrumentation.wrapper import default_wrapper, args_wrapper
 
+def check_and_instrument(module_name, act_module):
+    if not module_name:
+        return
 
-def wsgi_wrapper(original, module, method_info):
-    def wrapper(*args, **kwargs):
-        cur_txn = None 
-        res = None
-        agent = get_agent()
-        try:
-            wsgi_environ = args[1]
-            tracker_info = create_tracker_info(module, method_info)
-            cur_txn = agent.check_and_create_txn(wsgi_environ, tracker_info)
-            res = original(*args, **kwargs)
-            agent.end_txn(cur_txn, res)
-        except Exception as exc:
-            agent.end_txn(cur_txn, err=exc)
-            raise exc
-        finally:
-            clear_cur_context()
-                 
-        return res
-
-    return wrapper
-
-
-def default_wrapper(original, module, method_info):
-    def wrapper(*args, **kwargs):
-        if is_no_active_txn():
-            return original(*args, **kwargs)
-       
-        res = None 
-        err = None
-        agent = get_agent()
-        parent_tracker = get_cur_tracker()
-        tracker_info = create_tracker_info(module, method_info, parent_tracker)
-        cur_tracker = agent.check_and_create_tracker(tracker_info)
-        try:
-            res = original(*args, **kwargs)
-        except Exception as exc:
-            err = exc
-            raise exc
-        finally:
-            handle_tracker_end(cur_tracker, method_info, args, kwargs, res, err)
-            set_cur_tracker(parent_tracker)
-
-        return res
-
-    # special handling for flask route decorator
-    wrapper.__name__ = original.__name__
-    return wrapper
+    if hasattr(act_module, constants.APM_INSTRUMENTED):
+        return 
 
+    if module_name in modules_info.keys():
+        methods_info = modules_info.get(module_name)
+        for each_method_info in methods_info:
+            instrument_method(module_name, act_module, each_method_info)
 
-def handle_tracker_end(tracker, method_info, args, kwargs, res, err):
-    try:
-        if isinstance(tracker, Tracker) is not True:
-            return
-
-        if type(method_info) is dict and extract_info in method_info:
-            extractor = method_info[extract_info]
-            extractor(tracker, args=args, kwargs=kwargs, return_value=res)
+        setattr(act_module, constants.APM_INSTRUMENTED, True)
+        agentlogger.info(module_name+' instrumented')
 
-        get_agent().end_tracker(tracker, err=err)
-    except Exception:
-        agentlogger.exception("While handling tracker end")
 
+def instrument_method(module_name, act_module, method_info):
+    parent_ref = act_module
+    class_name = ''
 
-def copy_attributes(source, dest):
-    try:
-        for att in source.__dict__:
-            setattr(dest, att, getattr(source, att))
-        
-    except Exception:
-        agentlogger.exception('copying attribute')
+    if type(method_info) is not dict:
+        return
 
+    if class_str in method_info:
+        class_name = method_info.get(class_str)
+        if hasattr(act_module, class_name):
+            parent_ref = getattr(act_module, class_name)
+            module_name = module_name+'.'+class_name
 
 
-def args_wrapper(original, module, method_info):
-    def wrapper(*args, **kwargs): 
-        if wrap_args in method_info:
-            args_index = method_info[wrap_args]
-            if isinstance(args, (list, tuple)) and len(args)> args_index:
-                if is_callable(args[args_index]):
-                    try:
-                        act_method = args[args_index]
-                        temp = list(args)
-                        module_name = act_method.__module__
-                        args_method_info = { 'method' : act_method.__name__ }
-                        new_method = default_wrapper(act_method, module_name, args_method_info)
-                        copy_attributes(act_method, new_method)
-                        temp[args_index] = new_method
-                        args = temp
-                    except Exception:
-                        agentlogger.exception('error in args wrapper')
+    method_name = method_info.get(method_str, '')
+    if hasattr(parent_ref, method_name):
+        original = getattr(parent_ref, method_name)
+        if not is_callable(original):
+            return
+        
+        # use default wrapper if there is no wrapper attribute
+        wrapper_factory = default_wrapper
+        if wrap_args_str in method_info:
+            wrapper_factory = args_wrapper
+        elif wrapper_str in method_info:
+            wrapper_factory = method_info.get(wrapper_str)
+        
+        wrapper = wrapper_factory(original, module_name, method_info)
+        setattr(parent_ref,  method_name, wrapper)
 
+def instrument_django_middlewares():
+    methods = ['process_request', 'process_view', 'process_exception', 'process_template_response', 'process_response']
+    try:
+        from django.conf import settings
         
-        return original(*args, **kwargs)
-    
-    return wrapper
+        wsgi_app = settings.WSGI_APPLICATION
+        appname = wsgi_app.split('.')[0]
+        if appname and get_agent() and get_agent().get_config().get_app_name()== constants.DEFAULT_APM_APP_NAME:
+            get_agent().get_config().set_app_name(appname)
+
+        middleware = getattr(settings, constants.MIDDLEWARE, None) or \
+            getattr(settings, constants.MIDDLEWARE_CLASSES, None)
 
+        if middleware is None:
+            return
+
+        for each in middleware:
+            module_path, class_name = each.rsplit('.', 1)
+            act_module = import_module(module_path)
+            for each_method in methods:
+                method_info = {
+                    constants.class_str : class_name,
+                    constants.method_str : each_method,
+                    constants.component_str : constants.middleware
+                }
+                instrument_method(module_path, act_module, method_info)
+    except Exception as exc:
+        agentlogger('django middleware instrumentation error', exc)
+
+initialized = False
+
+def init_instrumentation():
+    global initialized
+    if initialized:
+        return
+    for each_mod in modules_info:
+        try:
+            act_module = import_module(each_mod)
+            check_and_instrument(each_mod, act_module)
+        except Exception:
+            agentlogger.info(each_mod +' is not present')
 
+    initialized = True
```

### Comparing `apminsight-1.0.3/apminsight/metric/apdexmetric.py` & `apminsight-1.1.0/apminsight/metric/apdexmetric.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         if self.max_rt==0 or self.max_rt<txn.get_rt():
             self.max_rt = txn.get_rt()
 
 
     def aggregate_txn_sub_resources(self, txn):
         self.aggregate_errorcode(txn)
-        self.db_calls += txn.get_dbcalls()
+        self.db_calls += txn.get_db_calls()
         self.aggregate_exceptions(txn.get_exceptions_info())
         self.aggregate_int_comps(txn.get_internal_comps())
         self.aggregate_ext_comps(txn.get_external_comps())
 
     
     def aggregate_exceptions(self, cur_exc_info={}):
         if len(cur_exc_info)<=0:
@@ -191,15 +191,15 @@
 
     def get_tolerated(self):
         return self.tolerating
 
     def get_frustrated(self):
         return self.frustrated
 
-    def get_dbcalls(self):
+    def get_db_calls(self):
         return self.db_calls
 
     def get_internal_comps(self):
         return self.internal_comps
 
     def get_external_comps(self):
         return self.external_comps
```

### Comparing `apminsight-1.0.3/apminsight/metric/component.py` & `apminsight-1.1.0/apminsight/metric/component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 
+from apminsight import constants
 from apminsight.util import is_ext_comp, is_non_empty_string
 
 class Component:
 
     def __init__(self, tracker):
         self.name = tracker.get_component()
         self.rt = tracker.get_rt()
         self.ext = is_ext_comp(tracker.get_component())
         self.count = 0
         self.errcount = 0
-        self.host = tracker.get_info().get('host', '')
-        self.port = tracker.get_info().get('port', '-1')
-        if tracker.is_error():
+        self.http_err = 0
+        self.host = tracker.get_info().get(constants.host_str, '')
+        self.port = tracker.get_info().get(constants.port_str, '-1') or '-1'
+        if tracker.is_error() or tracker.is_http_err():
             self.errcount+=1
         else:
             self.count+=1
 
 
     def get_name(self):
         return self.name
@@ -84,13 +86,13 @@
         info['ct'] = self.count
         info['isExt'] = 1 if self.is_ext() else 0
         if self.errcount>0:
             info['error'] = self.get_error_count()
         
         port_number = int(self.port)
         if is_non_empty_string(self.host) and port_number>0:
-            info['host'] = self.host
-            info['port'] = self.port
+            info[constants.host_str] = self.host
+            info[constants.port_str] = self.port
 
         return info
```

### Comparing `apminsight-1.0.3/apminsight/metric/dbmetric.py` & `apminsight-1.1.0/apminsight/metric/dbmetric.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.count = 0
         self.time = 0
         self.minrt = None
         self.maxrt = None
 
 
     def accumulate(self, dbtracker):
-        info = dbtracker.extract_operartion_info()
+        info = dbtracker.get_info()
         if 'opn' not in info or 'obj' not in info:
             return
             
         self.opn = info['opn']
         self.obj = info['obj']
         self.component = dbtracker.get_component()
         if dbtracker.is_error():
```

### Comparing `apminsight-1.0.3/apminsight/metric/error.py` & `apminsight-1.1.0/apminsight/metric/error.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,17 +37,18 @@
             if self.stackframes:
                 return self.stackframes
 
             frames = []
             tb = self.exc.__traceback__
             while tb is not None:
                 file_name = tb.tb_frame.f_code.co_filename
-                func_name = tb.tb_frame.f_code.co_name
-                line_no = tb.tb_lineno
-                frames.append(['', file_name, func_name, line_no])
+                if not 'apminsight' in file_name:
+                    func_name = tb.tb_frame.f_code.co_name
+                    line_no = tb.tb_lineno
+                    frames.append(['', file_name, func_name, line_no])
                 tb = tb.tb_next
 
             self.stackframes = frames
             return frames
             
         except Exception:
             agentlogger.exception('unable to get exc stackframes')
```

### Comparing `apminsight-1.0.3/apminsight/metric/metricstore.py` & `apminsight-1.1.0/apminsight/metric/metricstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         try:
             if(txn.is_completed() is not True):
                 return False
 
             occurence = 0    
             namespace = webtxn_prefix + txn.get_url()
             match = namespace in self.web_txn_metric  
-        
+            txn.aggregate_trackers(txn.get_root_tracker())
             if match is not True:
                 metric = TxnMetric()
                 metric.aggregate(txn)
                 self.web_txn_metric[namespace] = metric
                 self.check_and_include_in_trace(txn)
                 return True
 
@@ -111,16 +111,16 @@
         for txn_namespace in self.web_txn_metric.keys():
             txnmetric = self.web_txn_metric[txn_namespace]
             txn_data = txnmetric.get_formatted_data(ns=txn_namespace)
             formatted_data.append(txn_data)
             instance_metric.accumulate(txnmetric)
 
             txn_dbmetric = {}
-            for dbtracker in txnmetric.get_dbcalls():
-                info = dbtracker.extract_operartion_info()
+            for dbtracker in txnmetric.get_db_calls():
+                info = dbtracker.get_info()
                 opn = info.get('opn', '')
                 obj = info.get('obj', '')
                 if is_empty_string(opn) or is_empty_string(obj):
                     continue
 
                 dbtracker.accumulate('db/'+opn+'/'+obj+'/dummy-db', txn_dbmetric)
                 dbtracker.accumulate('db/'+opn+'/all/dummy-db', opn_dbmetric)
```

### Comparing `apminsight-1.0.3/apminsight.egg-info/SOURCES.txt` & `apminsight-1.1.0/apminsight.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 README.md
 setup.py
 apminsight/__init__.py
 apminsight/agent.py
 apminsight/agentfactory.py
+apminsight/apm_run.py
 apminsight/constants.py
 apminsight/context.py
 apminsight/logger.py
 apminsight/util.py
 apminsight.egg-info/PKG-INFO
 apminsight.egg-info/SOURCES.txt
 apminsight.egg-info/dependency_links.txt
+apminsight.egg-info/entry_points.txt
 apminsight.egg-info/not-zip-safe
 apminsight.egg-info/requires.txt
 apminsight.egg-info/top_level.txt
+apminsight/bootstrap/__init__.py
+apminsight/bootstrap/sitecustomize.py
 apminsight/collector/__init__.py
 apminsight/collector/connhandler.py
 apminsight/collector/datahandler.py
-apminsight/collector/insinfo.py
+apminsight/collector/ins_info.py
+apminsight/collector/metric_dispatcher.py
 apminsight/collector/reqhandler.py
 apminsight/collector/rescodes.py
 apminsight/collector/reshandler.py
 apminsight/config/__init__.py
 apminsight/config/configuration.py
 apminsight/config/threshold.py
 apminsight/contrib/__init__.py
 apminsight/contrib/django/__init__.py
 apminsight/contrib/django/apps.py
 apminsight/contrib/django/wrapper.py
 apminsight/instrumentation/__init__.py
 apminsight/instrumentation/dbapi2.py
 apminsight/instrumentation/modules.py
+apminsight/instrumentation/proxy.py
 apminsight/instrumentation/util.py
 apminsight/instrumentation/wrapper.py
 apminsight/instrumentation/packages/__init__.py
+apminsight/instrumentation/packages/bottle.py
 apminsight/instrumentation/packages/cassandra.py
+apminsight/instrumentation/packages/cherrypy.py
 apminsight/instrumentation/packages/django.py
 apminsight/instrumentation/packages/flask.py
+apminsight/instrumentation/packages/genshi.py
+apminsight/instrumentation/packages/http.py
+apminsight/instrumentation/packages/httplib2.py
+apminsight/instrumentation/packages/httpx.py
 apminsight/instrumentation/packages/jinja2.py
+apminsight/instrumentation/packages/mako.py
 apminsight/instrumentation/packages/memcache.py
 apminsight/instrumentation/packages/mysql.py
 apminsight/instrumentation/packages/psycopg2.py
 apminsight/instrumentation/packages/pymemcache.py
+apminsight/instrumentation/packages/pyramid.py
 apminsight/instrumentation/packages/redis.py
 apminsight/instrumentation/packages/sqlite.py
+apminsight/instrumentation/packages/urllib.py
+apminsight/instrumentation/packages/urllib3.py
 apminsight/metric/__init__.py
 apminsight/metric/apdexmetric.py
 apminsight/metric/component.py
 apminsight/metric/dbmetric.py
 apminsight/metric/dbtracker.py
 apminsight/metric/error.py
 apminsight/metric/metricstore.py
```

### Comparing `apminsight-1.0.3/setup.py` & `apminsight-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='apminsight',
-      version='1.0.3',
+      version='1.1.0',
       description='Site24x7 application performance monitoring',
       url='https://site24x7.com',
       author='apm-insight',
       author_email='apm-insight@zohocorp.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='LICENSE.txt',
       packages=find_packages(exclude=['tests', 'tests.*']),
       include_package_data = True,
       python_requires='>=3.5',
       install_requires=[
             "requests"
       ],
-      zip_safe=False)
+      entry_points={
+            "console_scripts":[
+                  "apminsight-run = apminsight.apm_run:main",
+            ],
+      },
+      zip_safe=False)
```

