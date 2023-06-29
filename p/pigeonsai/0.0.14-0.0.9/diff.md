# Comparing `tmp/pigeonsai-0.0.14.tar.gz` & `tmp/pigeonsai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.14.tar", last modified: Wed Jun 28 22:19:42 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.9.tar", last modified: Thu Jun 15 18:46:44 2023, max compression
```

## Comparing `pigeonsai-0.0.14.tar` & `pigeonsai-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-28 22:19:42.449900 pigeonsai-0.0.14/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-06-28 22:19:42.449777 pigeonsai-0.0.14/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.14/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-28 22:19:42.449939 pigeonsai-0.0.14/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2065 2023-06-28 22:19:33.000000 pigeonsai-0.0.14/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-28 22:19:42.448104 pigeonsai-0.0.14/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-28 22:19:42.448754 pigeonsai-0.0.14/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       50 2023-06-15 18:46:00.000000 pigeonsai-0.0.14/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     6397 2023-06-28 22:19:26.000000 pigeonsai-0.0.14/src/pigeonsai/pigeonsdb.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-28 22:19:42.449378 pigeonsai-0.0.14/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-06-28 22:19:42.000000 pigeonsai-0.0.14/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-28 22:19:42.000000 pigeonsai-0.0.14/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-28 22:19:42.000000 pigeonsai-0.0.14/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       77 2023-06-28 22:19:42.000000 pigeonsai-0.0.14/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-28 22:19:42.000000 pigeonsai-0.0.14/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-28 22:19:42.449508 pigeonsai-0.0.14/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.14/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:46:44.440942 pigeonsai-0.0.9/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:46:44.440391 pigeonsai-0.0.9/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.9/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-15 18:46:44.441037 pigeonsai-0.0.9/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-15 18:46:35.000000 pigeonsai-0.0.9/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:46:44.437904 pigeonsai-0.0.9/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:46:44.438713 pigeonsai-0.0.9/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       50 2023-06-15 18:46:00.000000 pigeonsai-0.0.9/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     7830 2023-06-15 18:39:56.000000 pigeonsai-0.0.9/src/pigeonsai/pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:46:44.439845 pigeonsai-0.0.9/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:46:44.000000 pigeonsai-0.0.9/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-15 18:46:44.000000 pigeonsai-0.0.9/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-15 18:46:44.000000 pigeonsai-0.0.9/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       90 2023-06-15 18:46:44.000000 pigeonsai-0.0.9/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-15 18:46:44.000000 pigeonsai-0.0.9/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:46:44.440017 pigeonsai-0.0.9/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.9/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.14/PKG-INFO` & `pigeonsai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.14
+Version: 0.0.9
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.14/README.md` & `pigeonsai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.14/setup.py` & `pigeonsai-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.14",
+    version="0.0.9",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.14/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.9/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.14
+Version: 0.0.9
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.14/tests/test_pigeonsdb.py` & `pigeonsai-0.0.9/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

