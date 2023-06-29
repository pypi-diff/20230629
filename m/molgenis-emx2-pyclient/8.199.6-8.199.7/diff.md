# Comparing `tmp/molgenis_emx2_pyclient-8.199.6.tar.gz` & `tmp/molgenis_emx2_pyclient-8.199.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.199.6.tar", last modified: Wed Jun 28 22:45:50 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.199.7.tar", last modified: Thu Jun 29 19:57:40 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.199.6.tar` & `molgenis_emx2_pyclient-8.199.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 22:45:50.813519 molgenis_emx2_pyclient-8.199.6/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-06-28 22:33:05.000000 molgenis_emx2_pyclient-8.199.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-06-28 22:45:50.813519 molgenis_emx2_pyclient-8.199.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-28 22:33:05.000000 molgenis_emx2_pyclient-8.199.6/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-28 22:33:05.000000 molgenis_emx2_pyclient-8.199.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 22:33:05.000000 molgenis_emx2_pyclient-8.199.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 22:45:50.813519 molgenis_emx2_pyclient-8.199.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 22:45:50.809519 molgenis_emx2_pyclient-8.199.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 22:45:50.809519 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-28 22:33:05.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-06-28 22:33:05.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 22:45:50.813519 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-06-28 22:45:50.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-06-28 22:45:50.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 22:45:50.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-28 22:45:50.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-28 22:45:50.000000 molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-28 22:40:06.000000 molgenis_emx2_pyclient-8.199.6/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:57:40.213636 molgenis_emx2_pyclient-8.199.7/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-06-29 19:50:21.000000 molgenis_emx2_pyclient-8.199.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-06-29 19:57:40.213636 molgenis_emx2_pyclient-8.199.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-29 19:50:21.000000 molgenis_emx2_pyclient-8.199.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-29 19:50:21.000000 molgenis_emx2_pyclient-8.199.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 19:50:21.000000 molgenis_emx2_pyclient-8.199.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 19:57:40.213636 molgenis_emx2_pyclient-8.199.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:57:40.213636 molgenis_emx2_pyclient-8.199.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:57:40.213636 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-29 19:50:21.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-06-29 19:50:21.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:57:40.213636 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-06-29 19:57:40.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-06-29 19:57:40.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 19:57:40.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 19:57:40.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-29 19:57:40.000000 molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-29 19:51:49.000000 molgenis_emx2_pyclient-8.199.7/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.199.6/LICENSE` & `molgenis_emx2_pyclient-8.199.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.199.6/PKG-INFO` & `molgenis_emx2_pyclient-8.199.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.199.6
+Version: 8.199.7
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.199.6/README.md` & `molgenis_emx2_pyclient-8.199.7/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.199.6/pyproject.toml` & `molgenis_emx2_pyclient-8.199.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.199.6/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.199.7/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.199.6
+Version: 8.199.7
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

