# Comparing `tmp/dauth-0.2.tar.gz` & `tmp/dauth-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauth-0.2.tar", last modified: Sat Apr 15 19:59:07 2023, max compression
+gzip compressed data, was "dauth-0.3.tar", last modified: Thu Jun 29 11:39:45 2023, max compression
```

## Comparing `dauth-0.2.tar` & `dauth-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.851535 dauth-0.2/
--rw-r--r--   0 vvelikovich (161766200) 593637566     2705 2023-04-15 19:59:07.851419 dauth-0.2/PKG-INFO
--rw-r--r--   0 vvelikovich (161766200) 593637566     2569 2023-04-15 19:57:46.000000 dauth-0.2/README.md
--rw-r--r--   0 vvelikovich (161766200) 593637566       38 2023-04-15 19:59:07.851567 dauth-0.2/setup.cfg
--rw-r--r--   0 vvelikovich (161766200) 593637566      600 2023-04-09 22:09:09.000000 dauth-0.2/setup.py
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.850242 dauth-0.2/src/
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.850767 dauth-0.2/src/dauth/
--rw-r--r--   0 vvelikovich (161766200) 593637566      187 2023-04-15 19:47:47.000000 dauth-0.2/src/dauth/__init__.py
--rw-r--r--   0 vvelikovich (161766200) 593637566      890 2023-04-15 19:58:38.000000 dauth-0.2/src/dauth/auth.py
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-15 19:59:07.851284 dauth-0.2/src/dauth.egg-info/
--rw-r--r--   0 vvelikovich (161766200) 593637566     2705 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/PKG-INFO
--rw-r--r--   0 vvelikovich (161766200) 593637566      190 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/SOURCES.txt
--rw-r--r--   0 vvelikovich (161766200) 593637566        1 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/dependency_links.txt
--rw-r--r--   0 vvelikovich (161766200) 593637566        6 2023-04-15 19:59:07.000000 dauth-0.2/src/dauth.egg-info/top_level.txt
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:39:45.983357 dauth-0.3/
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 11:39:45.983357 dauth-0.3/PKG-INFO
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2569 2023-06-21 07:35:06.000000 dauth-0.3/README.md
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)       38 2023-06-29 11:39:45.983357 dauth-0.3/setup.cfg
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      600 2023-06-21 07:35:06.000000 dauth-0.3/setup.py
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:39:45.983357 dauth-0.3/src/
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:39:45.983357 dauth-0.3/src/dauth/
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      187 2023-06-21 07:35:08.000000 dauth-0.3/src/dauth/__init__.py
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      890 2023-06-21 07:35:08.000000 dauth-0.3/src/dauth/auth.py
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:39:45.983357 dauth-0.3/src/dauth.egg-info/
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 11:39:45.000000 dauth-0.3/src/dauth.egg-info/PKG-INFO
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      190 2023-06-29 11:39:45.000000 dauth-0.3/src/dauth.egg-info/SOURCES.txt
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)        1 2023-06-29 11:39:45.000000 dauth-0.3/src/dauth.egg-info/dependency_links.txt
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)        6 2023-06-29 11:39:45.000000 dauth-0.3/src/dauth.egg-info/top_level.txt
```

### Comparing `dauth-0.2/PKG-INFO` & `dauth-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.2
+Version: 0.3
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
```

### Comparing `dauth-0.2/README.md` & `dauth-0.3/README.md`

 * *Files identical despite different names*

### Comparing `dauth-0.2/setup.py` & `dauth-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `dauth-0.2/src/dauth/auth.py` & `dauth-0.3/src/dauth/auth.py`

 * *Files identical despite different names*

### Comparing `dauth-0.2/src/dauth.egg-info/PKG-INFO` & `dauth-0.3/src/dauth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.2
+Version: 0.3
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
```

