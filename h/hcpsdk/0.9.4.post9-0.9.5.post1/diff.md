# Comparing `tmp/hcpsdk-0.9.4.post9.tar.gz` & `tmp/hcpsdk-0.9.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hcpsdk-0.9.4.post9.tar", last modified: Sat Aug 26 18:46:16 2017, max compression
+gzip compressed data, was "hcpsdk-0.9.5.post1.tar", last modified: Thu Jun 29 12:32:19 2023, max compression
```

## Comparing `hcpsdk-0.9.4.post9.tar` & `hcpsdk-0.9.5.post1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/
--rw-r--r--   0 sm         (501) staff       (20)     8625 2017-08-26 18:46:13.000000 hcpsdk-0.9.4.post9/CHANGELOG.rst
--rwxr-xr-x   0 sm         (501) staff       (20)     3176 2016-12-19 18:54:22.000000 hcpsdk-0.9.4.post9/DESCRIPTION.rst
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/
--rw-r--r--   0 sm         (501) staff       (20)    49608 2017-08-26 18:44:16.000000 hcpsdk-0.9.4.post9/hcpsdk/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/httpclient/
--rw-r--r--   0 sm         (501) staff       (20)     9425 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/httpclient/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/ips/
--rw-r--r--   0 sm         (501) staff       (20)     8448 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/ips/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/
--rw-r--r--   0 sm         (501) staff       (20)     1258 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/chargeback/
--rw-r--r--   0 sm         (501) staff       (20)     6456 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/chargeback/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/logs/
--rwxr-xr-x   0 sm         (501) staff       (20)    14670 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/logs/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/replication/
--rwxr-xr-x   0 sm         (501) staff       (20)     9474 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/replication/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/tenant/
--rw-r--r--   0 sm         (501) staff       (20)     5780 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/mapi/tenant/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/namespace/
--rw-r--r--   0 sm         (501) staff       (20)     7946 2016-12-19 20:37:19.000000 hcpsdk-0.9.4.post9/hcpsdk/namespace/__init__.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk/pathbuilder/
--rw-r--r--   0 sm         (501) staff       (20)     5435 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/hcpsdk/pathbuilder/__init__.py
--rw-r--r--   0 sm         (501) staff       (20)     1545 2017-08-26 18:46:13.000000 hcpsdk-0.9.4.post9/hcpsdk/version.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk.egg-info/
--rw-r--r--   0 sm         (501) staff       (20)        1 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sm         (501) staff       (20)     4747 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk.egg-info/PKG-INFO
--rw-r--r--   0 sm         (501) staff       (20)       18 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk.egg-info/requires.txt
--rw-r--r--   0 sm         (501) staff       (20)      975 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sm         (501) staff       (20)       13 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/hcpsdk.egg-info/top_level.txt
--rw-r--r--   0 sm         (501) staff       (20)       45 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/MANIFEST.in
--rw-r--r--   0 sm         (501) staff       (20)     4747 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/PKG-INFO
--rwxr-xr-x   0 sm         (501) staff       (20)     3285 2016-12-19 18:54:22.000000 hcpsdk-0.9.4.post9/README.rst
--rw-r--r--   0 sm         (501) staff       (20)       59 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/setup.cfg
--rw-r--r--   0 sm         (501) staff       (20)     4986 2017-06-10 19:17:31.000000 hcpsdk-0.9.4.post9/setup.py
-drwxr-xr-x   0 sm         (501) staff       (20)        0 2017-08-26 18:46:16.000000 hcpsdk-0.9.4.post9/tests/
--rw-r--r--   0 sm         (501) staff       (20)       23 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/__init__.py
--rw-r--r--   0 sm         (501) staff       (20)     2187 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/failtest.py
--rw-r--r--   0 sm         (501) staff       (20)     6060 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/idletimertest.py
--rw-r--r--   0 sm         (501) staff       (20)     2737 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/init_tests.py
--rw-r--r--   0 sm         (501) staff       (20)     8188 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/loadtest.py
--rw-r--r--   0 sm         (501) staff       (20)     1886 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/nsstatstest.py
--rw-r--r--   0 sm         (501) staff       (20)      360 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/replicatest.py
--rw-r--r--   0 sm         (501) staff       (20)     4547 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/retrytest.py
--rw-r--r--   0 sm         (501) staff       (20)     2538 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_010_ips.py
--rw-r--r--   0 sm         (501) staff       (20)     7736 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_020_hcpsdk.py
--rw-r--r--   0 sm         (501) staff       (20)     6813 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_021_hcpsdk_w_certs.py
--rw-r--r--   0 sm         (501) staff       (20)     3864 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_030_namespace.py
--rwxr-xr-x   0 sm         (501) staff       (20)     2848 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_040_mapi_replication.py
--rwxr-xr-x   0 sm         (501) staff       (20)     4603 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_041_mapi_logs.py
--rwxr-xr-x   0 sm         (501) staff       (20)     3760 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_042_mapi_chargeback.py
--rwxr-xr-x   0 sm         (501) staff       (20)     2177 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_043_mapi_tenant.py
--rw-r--r--   0 sm         (501) staff       (20)     2165 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/test_050_pathbuilder.py
--rw-r--r--   0 sm         (501) staff       (20)      621 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/timeouttest.py
--rw-r--r--   0 sm         (501) staff       (20)     1486 2016-12-19 18:48:55.000000 hcpsdk-0.9.4.post9/tests/trysdk.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.791484 hcpsdk-0.9.5.post1/
+-rw-r--r--   0 tsimons    (501) staff       (20)     9177 2023-06-29 11:24:32.000000 hcpsdk-0.9.5.post1/CHANGELOG.rst
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     2784 2023-06-29 12:32:10.000000 hcpsdk-0.9.5.post1/DESCRIPTION.rst
+-rw-r--r--   0 tsimons    (501) staff       (20)       45 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/MANIFEST.in
+-rw-r--r--   0 tsimons    (501) staff       (20)     3460 2023-06-29 12:32:19.791318 hcpsdk-0.9.5.post1/PKG-INFO
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     3285 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/README.rst
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.784696 hcpsdk-0.9.5.post1/hcpsdk/
+-rw-r--r--   0 tsimons    (501) staff       (20)    49942 2023-06-29 11:24:32.000000 hcpsdk-0.9.5.post1/hcpsdk/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.785660 hcpsdk-0.9.5.post1/hcpsdk/httpclient/
+-rw-r--r--   0 tsimons    (501) staff       (20)     9287 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/httpclient/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.785971 hcpsdk-0.9.5.post1/hcpsdk/ips/
+-rw-r--r--   0 tsimons    (501) staff       (20)     8448 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/ips/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.786308 hcpsdk-0.9.5.post1/hcpsdk/mapi/
+-rw-r--r--   0 tsimons    (501) staff       (20)     1258 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/mapi/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.786500 hcpsdk-0.9.5.post1/hcpsdk/mapi/chargeback/
+-rw-r--r--   0 tsimons    (501) staff       (20)     6456 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/mapi/chargeback/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.786680 hcpsdk-0.9.5.post1/hcpsdk/mapi/logs/
+-rwxr-xr-x   0 tsimons    (501) staff       (20)    14670 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/mapi/logs/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.786854 hcpsdk-0.9.5.post1/hcpsdk/mapi/replication/
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     9474 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/mapi/replication/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.787035 hcpsdk-0.9.5.post1/hcpsdk/mapi/tenant/
+-rw-r--r--   0 tsimons    (501) staff       (20)     5780 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/mapi/tenant/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.787200 hcpsdk-0.9.5.post1/hcpsdk/namespace/
+-rw-r--r--   0 tsimons    (501) staff       (20)     7946 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/namespace/__init__.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.787359 hcpsdk-0.9.5.post1/hcpsdk/pathbuilder/
+-rw-r--r--   0 tsimons    (501) staff       (20)     5435 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/hcpsdk/pathbuilder/__init__.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     1545 2023-06-29 11:24:32.000000 hcpsdk-0.9.5.post1/hcpsdk/version.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.785499 hcpsdk-0.9.5.post1/hcpsdk.egg-info/
+-rw-r--r--   0 tsimons    (501) staff       (20)     3460 2023-06-29 12:32:19.000000 hcpsdk-0.9.5.post1/hcpsdk.egg-info/PKG-INFO
+-rw-r--r--   0 tsimons    (501) staff       (20)      975 2023-06-29 12:32:19.000000 hcpsdk-0.9.5.post1/hcpsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tsimons    (501) staff       (20)        1 2023-06-29 12:32:19.000000 hcpsdk-0.9.5.post1/hcpsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tsimons    (501) staff       (20)       18 2023-06-29 12:32:19.000000 hcpsdk-0.9.5.post1/hcpsdk.egg-info/requires.txt
+-rw-r--r--   0 tsimons    (501) staff       (20)       13 2023-06-29 12:32:19.000000 hcpsdk-0.9.5.post1/hcpsdk.egg-info/top_level.txt
+-rw-r--r--   0 tsimons    (501) staff       (20)       38 2023-06-29 12:32:19.791537 hcpsdk-0.9.5.post1/setup.cfg
+-rw-r--r--   0 tsimons    (501) staff       (20)     4986 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/setup.py
+drwxr-xr-x   0 tsimons    (501) staff       (20)        0 2023-06-29 12:32:19.791051 hcpsdk-0.9.5.post1/tests/
+-rw-r--r--   0 tsimons    (501) staff       (20)       23 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/__init__.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     2187 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/failtest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     6060 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/idletimertest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     2737 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/init_tests.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     8188 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/loadtest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     1886 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/nsstatstest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)      360 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/replicatest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     4547 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/retrytest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     2538 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_010_ips.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     7736 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_020_hcpsdk.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     6813 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_021_hcpsdk_w_certs.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     3865 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_030_namespace.py
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     2849 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_040_mapi_replication.py
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     4603 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_041_mapi_logs.py
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     3760 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_042_mapi_chargeback.py
+-rwxr-xr-x   0 tsimons    (501) staff       (20)     2177 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_043_mapi_tenant.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     2166 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/test_050_pathbuilder.py
+-rw-r--r--   0 tsimons    (501) staff       (20)      621 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/timeouttest.py
+-rw-r--r--   0 tsimons    (501) staff       (20)     1486 2023-06-29 10:36:49.000000 hcpsdk-0.9.5.post1/tests/trysdk.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hcpsdk-0.9.4.post9/CHANGELOG.rst` & `hcpsdk-0.9.5.post1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 Release History
 ===============
 
+**0.9.5-1 2023-06-29**
+
+*   fixed a bug that caused HTTPS connections to fail
+
+**0.9.4-12 2018-07-25**
+
+*   fixed a bug which caused GETs to fail with
+    *hcpsdk.HcpsdkError: faulty read: 'NoneType' object has no attribute 'read'*
+    caused by idletimer cutting off the connection while transferring data
+
+**0.9.4-11 2018-03-27**
+
+*   fixed a bug in hcpsdk.Connection.request() which caused blanks not to be
+    url-encoded
+
+**0.9.4-10 2018-03-06**
+
+*   fixed a bug in hcpsdk.Connection.request() where some characters were not
+    properly encoded
+
 **0.9.4-9 2017-08-26**
 
 *   Better __repr__ and __str__ for hcpsdk.__init__.py
 
 **0.9.4-8 2017-07-14**
 
 *   Fixed a bug where URLs containing '+' also have to be url-encoded
```

### Comparing `hcpsdk-0.9.4.post9/DESCRIPTION.rst` & `hcpsdk-0.9.5.post1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 ======
 
 HCPsdk provides a simple SDK to access an Hitachi Content Platform (HCP)
 from Python3. It handles name resolution, multiple sessions spread across all
 available HCP nodes, persistent connections and recovery from failing
 connections.
 
-It's that easy:
-
-::
+It's that easy::
 
     >>> import hcpsdk
 
     >>> # initialize an *Authorization* object
     >>> auth = hcpsdk.NativeAuthorization('user', 'password')
 
     >>> # initialize a *Target* object
@@ -32,67 +30,74 @@
     >>> c.close()
 
 
 Features
 --------
 
 - Handles HCP as a target object
+- Replica-aware (replica can be part of a target object)
+- Various strategies on how to use a replica
 - Connection objects, while tied to a target object, allow
-  access to HCP through HCPs native http/REST dialect
+  access to HCP through the various http/REST dialects
+  (native, HS3, HSwift)
 - Higher level modules provide easy access to namespace
   statistics and some MAPI functionality, along with
   the ability to create unique object names / paths
 
-Dependencies
-------------
+Documentation
+-------------
 
-**hcpsdk** depends on `dnspython <http://www.dnspython.org>`_, which is used
-for non-cached name resolution when bypassing the system's resolver.
+Hosted at [readthedocs.org](http://hcpsdk.readthedocs.org)
 
 
-Documentation
--------------
+Dependencies
+------------
+
+**hcpsdk** depends on [dnspython](http://www.dnspython.org), which is used for
+non-cached name resolution when bypassing the system's resolver.
 
-To be found at `readthedocs.org <http://hcpsdk.readthedocs.org>`_
 
 Installation
 ------------
 
-Install hcpsdk by running:
+Install hcpsdk by running::
 
-    ``pip install hcpsdk``
+    $ pip install hcpsdk
 
-    -or-
+-or-
 
-    * get the source from `GitHub <https://github.com/simont3/hcpsdk/archive/master.zip>`_
-    * unzip the archive
-    * run ``python setup.py install``
+get the source from
+  [GitHub](https://github.com/Simont3/hcpsdk/archive/master.zip), unzip the
+  archive and run::
+    
+    $ python setup.py install
 
-    -or-
+-or-
 
-    * Fork at `Github <https://github.com/simont3/hcpsdk>`_
+fork at [Github](https://github.com/Simont3/hcpsdk)
 
 Contribute
 ----------
 
-- Issue Tracker: `<https://github.com/simont3/hcpsdk/issues>`_
-- Source Code: `<https://github.com/simont3/hcpsdk>`_
+* [Issue Tracker](https://github.com/simont3/hcpsdk/issues)
+* [Source Code](https://github.com/Simont3/hcpsdk)
 
 Support
 -------
 
-If you find any bugs, please let me know via the Issue Tracker;
-if you have comments or suggestions, send an email to `<sw@snomis.de>`_
+If you find any bugs, please let us know via the Issue Tracker;
+if you have comments or suggestions, send an email to
+[sw@snomis.de](mailto:sw@snomis.de)
 
 License
 -------
 
 The MIT License (MIT)
 
-Copyright (c) 2014-2015 Thorsten Simons (sw@snomis.de)
+Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -24,15 +24,18 @@
 from base64 import b64encode
 from hashlib import md5
 # As of Python 3.4.3, http.client.HTTPSconnection() will default to verify
 # presented certificates against the system's trusted CA chain. To enable
 # the previous behaviour, we switch it off.
 import ssl
 try:
-    SSL_NOVERIFY = ssl._create_unverified_context()
+    SSL_NOVERIFY = ssl.create_default_context()
+    SSL_NOVERIFY.verify_mode = ssl.CERT_REQUIRED
+    SSL_NOVERIFY.check_hostname = False
+    SSL_NOVERIFY.set_ciphers('DEFAULT')
 except (AttributeError, NameError):
     SSL_NOVERIFY = None
 import socket
 import http.client
 from urllib.parse import urlencode, quote
 import logging
 import time
@@ -61,14 +64,15 @@
            'HcpsdkCantConnectError', 'HcpsdkTimeoutError',
            'HcpsdkCertificateError', 'HcpsdkReplicaInitError']
 
 logging.getLogger('hcpsdk').addHandler(logging.NullHandler())
 
 version = _Version()
 
+RFC3986_reserved_chars = ' :?#[]@!$&\'()*+,;='
 
 class HcpsdkError(Exception):
     """
     Raised on generic errors in **hcpsdk**.
     """
     def __init__(self, reason):
         """
@@ -665,19 +669,19 @@
             headers = self.__target.headers
         else:
             headers.update(self.__target.headers)
 
         # if url needs url-encoding, do so...
         try:
             # --> if url can be encoded to ascii and it doesn't contain
-            #     blanks we can go with it.
+            #     forbidden characters, we can go with it.
             url.encode("ascii")
-            if ' ' in url or '+' in url:
-                raise
-        except Exception:
+            if any([x in url for x in RFC3986_reserved_chars]):
+                raise HcpsdkError('')
+        except HcpsdkError:
             # in this case, we need to urlencode it...
             self.logger.log(logging.DEBUG, 'url ({}) does need quoting'.format(url))
             url = quote(url)
             self.logger.log(logging.DEBUG, 'quote(url) = {}'.format(url))
         else:
             self.logger.log(logging.DEBUG, 'url ({}) doesn\'t need quoting'.format(url))
 
@@ -931,15 +935,14 @@
                 else:
                     self.__service_time2 = time.time() - s_t
                     self.logger.log(logging.DEBUG,
                                     '{} Request for {} - after getResponse(): '
                                     'service_time2 = {:0.17f}'
                                     .format(method, url, self.__service_time2))
 
-            self._set_idletimer()
             return self._response
 
     def getheader(self, *args, **kwargs):
         """
         Used to get a single *Response* header. Wraps
         *http.client.Response.getheader()*. Arguments are simply passed
         through.
@@ -958,14 +961,15 @@
         """
         Convenience method for Request() - PUT an object.
         Cleans up and leaves the Connection ready for the next Request.
         For parameter description see *Request()*.
         """
         r = self.request('PUT', url, body, params, headers)
         r.read()  # clean up
+        self._set_idletimer()
         return r
 
     # noinspection PyPep8Naming
     def GET(self, url, params=None, headers=None):
         """
         Convenience method for Request() - GET an object.
         You need to fully *.read()* the requested content from the Connection
@@ -977,15 +981,16 @@
     def HEAD(self, url, params=None, headers=None):
         """
         Convenience method for Request() - HEAD - get metadata of an object.
         Cleans up and leaves the Connection ready for the next Request.
         For parameter description see *Request()*.
         """
         r = self.request('HEAD', url, params=params, headers=headers)
-        r.read()
+        r.read()  # clean up
+        self._set_idletimer()
         return r
 
     def POST(self, url, body=None, params=None, headers=None):
         """
         Convenience method for Request() - POST metadata.
         Does no clean-up, as a POST can have a response body!
         For parameter description see *Request()*.
@@ -997,14 +1002,15 @@
         """
         Convenience method for Request() - DELETE an object.
         Cleans up and leaves the Connection ready for the next Request.
         For parameter description see *Request()*.
         """
         r = self.request('DELETE', url, params=params, headers=headers)
         r.read()  # clean up
+        self._set_idletimer()
         return r
 
     def read(self, amt=None):
         """
         Read amt # of bytes (or all, if amt isn't given) from a *Response*.
 
         :param amt: number of bytes to read
@@ -1036,14 +1042,15 @@
             if readsize:
                 self.logger.log(logging.DEBUG,
                                 '(partial?) read {} bytes: service_time1/2 = '
                                 '{:0.17f}/{:0.17f} secs'
                                 .format(readsize, self.__service_time1,
                                         self.__service_time2))
             else:
+                self._set_idletimer()
                 self.logger.log(logging.DEBUG,
                                 'final read: service_time1/2 = {:0.17f}/'
                                 '{:0.17f} secs'
                                 .format(self.__service_time1,
                                         self.__service_time2))
             return buf
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/httpclient/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/httpclient/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -89,16 +89,15 @@
         # added to standard method:
         if self.sock_keepalive:
             self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
             self.sock.setsockopt(socket.SOL_TCP, TCP_KEEPALIVE, self.tcp_keepalive)
             self.sock.setsockopt(socket.SOL_TCP, TCP_KEEPINTVL, self.tcp_keepintvl)
             self.sock.setsockopt(socket.SOL_TCP, TCP_KEEPCNT, self.tcp_keepcnt)
 
-            # self.logger.debug('enabled TCP keep-alive (TCP_KEEPALIVE = {}, '
-            print('enabled TCP keep-alive (TCP_KEEPALIVE = {}, '
+            self.logger.debug('enabled TCP keep-alive (TCP_KEEPALIVE = {}, '
                               'TCP_KEEPINTVL = {}, TCP_KEEPCNT = {})'
                               .format(self.sock.getsockopt(socket.SOL_TCP,
                                                            TCP_KEEPALIVE),
                                       self.sock.getsockopt(socket.SOL_TCP,
                                                            TCP_KEEPINTVL),
                                       self.sock.getsockopt(socket.SOL_TCP,
                                                            TCP_KEEPCNT)))
@@ -170,16 +169,15 @@
             # added to standard method:
             if self.sock_keepalive:
                 self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
                 self.sock.setsockopt(socket.SOL_TCP, TCP_KEEPALIVE, self.tcp_keepalive)
                 self.sock.setsockopt(socket.SOL_TCP, TCP_KEEPINTVL, self.tcp_keepintvl)
                 self.sock.setsockopt(socket.SOL_TCP, TCP_KEEPCNT, self.tcp_keepcnt)
 
-                # self.logger.debug('enabled TCP keep-alive (TCP_KEEPALIVE = {}, '
-                print('enabled TCP keep-alive (TCP_KEEPALIVE = {}, '
+                self.logger.debug('enabled TCP keep-alive (TCP_KEEPALIVE = {}, '
                                   'TCP_KEEPINTVL = {}, TCP_KEEPCNT = {})'
                                   .format(self.sock.getsockopt(socket.SOL_TCP,
                                                                TCP_KEEPALIVE),
                                           self.sock.getsockopt(socket.SOL_TCP,
                                                                TCP_KEEPINTVL),
                                           self.sock.getsockopt(socket.SOL_TCP,
                                                                TCP_KEEPCNT)))
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/ips/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/ips/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/mapi/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/mapi/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-# -*- coding: utf-8 -*-# The MIT License (MIT)## Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)## Permission is hereby granted, free of charge, to any person obtaining a copy of# this software and associated documentation files (the "Software"), to deal in# the Software without restriction, including without limitation the rights to# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of# the Software, and to permit persons to whom the Software is furnished to do so,# subject to the following conditions:## The above copyright notice and this permission notice shall be included in all# copies or substantial portions of the Software.## THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.from .chargeback import *from .logs import *from .replication import *from .tenant import *
+# -*- coding: utf-8 -*-# The MIT License (MIT)## Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)## Permission is hereby granted, free of charge, to any person obtaining a copy of# this software and associated documentation files (the "Software"), to deal in# the Software without restriction, including without limitation the rights to# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of# the Software, and to permit persons to whom the Software is furnished to do so,# subject to the following conditions:## The above copyright notice and this permission notice shall be included in all# copies or substantial portions of the Software.## THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.from .chargeback import *from .logs import *from .replication import *from .tenant import *
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/mapi/chargeback/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/mapi/chargeback/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/mapi/logs/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/mapi/logs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/mapi/replication/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/mapi/replication/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/mapi/tenant/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/mapi/tenant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/namespace/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/namespace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/pathbuilder/__init__.py` & `hcpsdk-0.9.5.post1/hcpsdk/pathbuilder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk/version.py` & `hcpsdk-0.9.5.post1/hcpsdk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -23,16 +23,16 @@
 
 class _Version(object):
     """
     Defines version and build for the HCPsdk.
     """
     release = 0
     major = 9
-    minor = 4
-    build = 9
+    minor = 5
+    build = 1
 
     fullversion = '{}.{}.{}-{}'.format(release, major, minor, build)
 
     # noinspection PyUnusedLocal
     def __call__(self, *args, **kwargs):
         return self.__str__()
```

### Comparing `hcpsdk-0.9.4.post9/hcpsdk.egg-info/SOURCES.txt` & `hcpsdk-0.9.5.post1/hcpsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/README.rst` & `hcpsdk-0.9.5.post1/DESCRIPTION.rst`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 ======
 
 HCPsdk provides a simple SDK to access an Hitachi Content Platform (HCP)
 from Python3. It handles name resolution, multiple sessions spread across all
 available HCP nodes, persistent connections and recovery from failing
 connections.
 
-It's that easy::
+It's that easy:
+
+::
 
     >>> import hcpsdk
 
     >>> # initialize an *Authorization* object
     >>> auth = hcpsdk.NativeAuthorization('user', 'password')
 
     >>> # initialize a *Target* object
@@ -30,74 +32,49 @@
     >>> c.close()
 
 
 Features
 --------
 
 - Handles HCP as a target object
-- Replica-aware (replica can be part of a target object)
-- Various strategies on how to use a replica
 - Connection objects, while tied to a target object, allow
-  access to HCP through the various http/REST dialects
-  (native, HS3, HSwift)
+  access to HCP through HCPs native http/REST dialect
 - Higher level modules provide easy access to namespace
   statistics and some MAPI functionality, along with
   the ability to create unique object names / paths
 
-Documentation
--------------
-
-Hosted at [readthedocs.org](http://hcpsdk.readthedocs.org)
-
-
 Dependencies
 ------------
 
-**hcpsdk** depends on [dnspython](http://www.dnspython.org), which is used for
-non-cached name resolution when bypassing the system's resolver.
-
+**hcpsdk** depends on `dnspython <http://www.dnspython.org>`_, which is used
+for non-cached name resolution when bypassing the system's resolver.
 
-Installation
-------------
 
-Install hcpsdk by running::
-
-    $ pip install hcpsdk
-
--or-
-
-get the source from
-  [GitHub](https://github.com/Simont3/hcpsdk/archive/master.zip), unzip the
-  archive and run::
-    
-    $ python setup.py install
+Documentation
+-------------
 
--or-
+To be found at `readthedocs.org <http://hcpsdk.readthedocs.org>`_
 
-fork at [Github](https://github.com/Simont3/hcpsdk)
+Installation
+------------
 
-Contribute
-----------
+Install hcpsdk by running:
 
-* [Issue Tracker](https://github.com/simont3/hcpsdk/issues)
-* [Source Code](https://github.com/Simont3/hcpsdk)
+    ``pip install hcpsdk``
 
-Support
--------
 
-If you find any bugs, please let us know via the Issue Tracker;
-if you have comments or suggestions, send an email to
-[sw@snomis.de](mailto:sw@snomis.de)
+If you find any bugs, please let me know via the Issue Tracker;
+if you have comments or suggestions, send an email to `<sw@snomis.de>`_
 
 License
 -------
 
 The MIT License (MIT)
 
-Copyright (c) 2014-2015 Thorsten Simons (sw@snomis.de)
+Copyright (c) 2014-2023 Thorsten Simons (sw@snomis.eu)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/setup.py` & `hcpsdk-0.9.5.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/failtest.py` & `hcpsdk-0.9.5.post1/tests/failtest.py`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/tests/idletimertest.py` & `hcpsdk-0.9.5.post1/tests/idletimertest.py`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/tests/init_tests.py` & `hcpsdk-0.9.5.post1/tests/init_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/loadtest.py` & `hcpsdk-0.9.5.post1/tests/loadtest.py`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/tests/nsstatstest.py` & `hcpsdk-0.9.5.post1/tests/nsstatstest.py`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/tests/retrytest.py` & `hcpsdk-0.9.5.post1/tests/retrytest.py`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/tests/test_010_ips.py` & `hcpsdk-0.9.5.post1/tests/test_010_ips.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_020_hcpsdk.py` & `hcpsdk-0.9.5.post1/tests/test_020_hcpsdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_021_hcpsdk_w_certs.py` & `hcpsdk-0.9.5.post1/tests/test_021_hcpsdk_w_certs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_030_namespace.py` & `hcpsdk-0.9.5.post1/tests/test_030_namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -98,8 +98,8 @@
             self.assertTrue(nsk in ['namespacePermissions',
                                     'namespaceEffectivePermissions',
                                     'userPermissions',
                                     'userEffectivePermissions'])
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_040_mapi_replication.py` & `hcpsdk-0.9.5.post1/tests/test_040_mapi_replication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -72,8 +72,8 @@
         print('test_1_30_good_getLinkDetails({}):'.format(LtVars.linkname))
         r = self.mapi.getlinkdetails(link=LtVars.linkname)
         pprint(r)
         self.assertTrue(True)
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_041_mapi_logs.py` & `hcpsdk-0.9.5.post1/tests/test_041_mapi_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_042_mapi_chargeback.py` & `hcpsdk-0.9.5.post1/tests/test_042_mapi_chargeback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_043_mapi_tenant.py` & `hcpsdk-0.9.5.post1/tests/test_043_mapi_tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `hcpsdk-0.9.4.post9/tests/test_050_pathbuilder.py` & `hcpsdk-0.9.5.post1/tests/test_050_pathbuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # The MIT License (MIT)
 #
-# Copyright (c) 2014-2016 Thorsten Simons (sw@snomis.de)
+# Copyright (c) 2014-2018 Thorsten Simons (sw@snomis.de)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -54,8 +54,8 @@
         for i in t[2].split(sep='\n'):
             print(i)
         self.assertTrue(type(t) == tuple)
         self.assertTrue(len(t) == 3)
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `hcpsdk-0.9.4.post9/tests/timeouttest.py` & `hcpsdk-0.9.5.post1/tests/timeouttest.py`

 * *Files identical despite different names*

### Comparing `hcpsdk-0.9.4.post9/tests/trysdk.py` & `hcpsdk-0.9.5.post1/tests/trysdk.py`

 * *Files identical despite different names*

