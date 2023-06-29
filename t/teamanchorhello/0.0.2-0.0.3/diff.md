# Comparing `tmp/teamanchorhello-0.0.2.tar.gz` & `tmp/teamanchorhello-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamanchorhello-0.0.2.tar", last modified: Thu Jun 29 18:15:47 2023, max compression
+gzip compressed data, was "teamanchorhello-0.0.3.tar", last modified: Thu Jun 29 18:39:40 2023, max compression
```

## Comparing `teamanchorhello-0.0.2.tar` & `teamanchorhello-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:15:47.611620 teamanchorhello-0.0.2/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.2/LICENSE
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      433 2023-06-29 18:15:47.611620 teamanchorhello-0.0.2/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       79 2023-06-29 17:26:48.000000 teamanchorhello-0.0.2/README.md
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-29 18:15:47.611620 teamanchorhello-0.0.2/setup.cfg
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-29 18:15:39.000000 teamanchorhello-0.0.2/setup.py
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:15:47.601619 teamanchorhello-0.0.2/teamanchorhello/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:15:47.601619 teamanchorhello-0.0.2/teamanchorhello/src/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:15:47.611620 teamanchorhello-0.0.2/teamanchorhello/src/teamanchorhello.egg-info/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      433 2023-06-29 18:15:47.000000 teamanchorhello-0.0.2/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-29 18:15:47.000000 teamanchorhello-0.0.2/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-29 18:15:47.000000 teamanchorhello-0.0.2/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-29 18:15:47.000000 teamanchorhello-0.0.2/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-29 18:15:46.000000 teamanchorhello-0.0.2/teamanchorhello/src/teamanchorhello.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.3/LICENSE
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1329 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      729 2023-06-29 18:37:56.000000 teamanchorhello-0.0.3/README.md
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/setup.cfg
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-29 18:32:06.000000 teamanchorhello-0.0.3/setup.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/teamanchorhello/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/teamanchorhello/src/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1329 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-29 18:32:01.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.py
```

### Comparing `teamanchorhello-0.0.2/setup.py` & `teamanchorhello-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="teamanchorhello",
-    version="0.0.2",
+    version="0.0.3",
     author="fanis",
     description="teamanchor say hello using Pypi package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

