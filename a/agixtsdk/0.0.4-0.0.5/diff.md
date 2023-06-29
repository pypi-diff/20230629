# Comparing `tmp/agixtsdk-0.0.4.tar.gz` & `tmp/agixtsdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixtsdk-0.0.4.tar", last modified: Thu Jun 29 17:19:10 2023, max compression
+gzip compressed data, was "agixtsdk-0.0.5.tar", last modified: Thu Jun 29 19:27:17 2023, max compression
```

## Comparing `agixtsdk-0.0.4.tar` & `agixtsdk-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:19:10.191922 agixtsdk-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 17:19:00.000000 agixtsdk-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 17:19:00.000000 agixtsdk-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 17:19:10.191922 agixtsdk-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-29 17:19:00.000000 agixtsdk-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:19:10.191922 agixtsdk-0.0.4/agixtsdk/
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-06-29 17:19:00.000000 agixtsdk-0.0.4/agixtsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:19:10.191922 agixtsdk-0.0.4/agixtsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 17:19:10.000000 agixtsdk-0.0.4/agixtsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-29 17:19:10.000000 agixtsdk-0.0.4/agixtsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:19:10.000000 agixtsdk-0.0.4/agixtsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 17:19:10.000000 agixtsdk-0.0.4/agixtsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 17:19:10.000000 agixtsdk-0.0.4/agixtsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 17:19:00.000000 agixtsdk-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:19:10.195922 agixtsdk-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 17:19:00.000000 agixtsdk-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:27:17.475886 agixtsdk-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 19:27:04.000000 agixtsdk-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 19:27:04.000000 agixtsdk-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 19:27:17.475886 agixtsdk-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-29 19:27:04.000000 agixtsdk-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:27:17.475886 agixtsdk-0.0.5/agixtsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-06-29 19:27:04.000000 agixtsdk-0.0.5/agixtsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:27:17.475886 agixtsdk-0.0.5/agixtsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 19:27:17.000000 agixtsdk-0.0.5/agixtsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-29 19:27:17.000000 agixtsdk-0.0.5/agixtsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:27:17.000000 agixtsdk-0.0.5/agixtsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:27:17.000000 agixtsdk-0.0.5/agixtsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:27:17.000000 agixtsdk-0.0.5/agixtsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 19:27:04.000000 agixtsdk-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:27:17.475886 agixtsdk-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 19:27:04.000000 agixtsdk-0.0.5/setup.py
```

### Comparing `agixtsdk-0.0.4/LICENSE` & `agixtsdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.4/PKG-INFO` & `agixtsdk-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixtsdk-0.0.4/README.md` & `agixtsdk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.4/agixtsdk.egg-info/PKG-INFO` & `agixtsdk-0.0.5/agixtsdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixtsdk-0.0.4/setup.py` & `agixtsdk-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="agixtsdk",
-    version="0.0.4",
+    version="0.0.5",
     description="The AGiXT SDK for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

