# Comparing `tmp/mik_py-0.0.1.tar.gz` & `tmp/mik_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mik_py-0.0.1.tar", last modified: Sun Mar 26 21:14:18 2023, max compression
+gzip compressed data, was "mik_py-0.0.2.tar", last modified: Thu Jun 29 12:56:08 2023, max compression
```

## Comparing `mik_py-0.0.1.tar` & `mik_py-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-03-26 21:14:18.092566 mik_py-0.0.1/
--rw-r--r--   0 michaelchung   (501) staff       (20)       67 2023-03-23 23:33:28.000000 mik_py-0.0.1/MANIFEST.in
--rw-r--r--   0 michaelchung   (501) staff       (20)      349 2023-03-26 21:14:18.092244 mik_py-0.0.1/PKG-INFO
--rw-r--r--   0 michaelchung   (501) staff       (20)       15 2023-03-22 12:57:49.000000 mik_py-0.0.1/README.md
--rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.1/eicar.com
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-03-26 21:14:18.090129 mik_py-0.0.1/mik_pack_10/
--rw-r--r--   0 michaelchung   (501) staff       (20)       34 2023-03-26 21:06:06.000000 mik_py-0.0.1/mik_pack_10/__init__.py
--rw-r--r--   0 michaelchung   (501) staff       (20)      680 2023-03-26 21:01:11.000000 mik_py-0.0.1/mik_pack_10/mik_py_.py
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-03-26 21:14:18.091863 mik_py-0.0.1/mik_py.egg-info/
--rw-r--r--   0 michaelchung   (501) staff       (20)      349 2023-03-26 21:14:17.000000 mik_py-0.0.1/mik_py.egg-info/PKG-INFO
--rw-r--r--   0 michaelchung   (501) staff       (20)      207 2023-03-26 21:14:18.000000 mik_py-0.0.1/mik_py.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)        1 2023-03-26 21:14:17.000000 mik_py-0.0.1/mik_py.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)       12 2023-03-26 21:14:17.000000 mik_py-0.0.1/mik_py.egg-info/top_level.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)       38 2023-03-26 21:14:18.092661 mik_py-0.0.1/setup.cfg
--rw-r--r--   0 michaelchung   (501) staff       (20)      765 2023-03-26 21:13:36.000000 mik_py-0.0.1/setup.py
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-06-29 12:56:08.581893 mik_py-0.0.2/
+-rw-r--r--   0 michaelchung   (501) staff       (20)       67 2023-03-23 23:33:28.000000 mik_py-0.0.2/MANIFEST.in
+-rw-r--r--   0 michaelchung   (501) staff       (20)      554 2023-06-29 12:56:08.581433 mik_py-0.0.2/PKG-INFO
+-rw-r--r--   0 michaelchung   (501) staff       (20)      169 2023-06-29 12:54:22.000000 mik_py-0.0.2/README.md
+-rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.2/eicar.com
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-06-29 12:56:08.578273 mik_py-0.0.2/eicar_pack_10/
+-rw-r--r--   0 michaelchung   (501) staff       (20)       34 2023-03-26 21:01:11.000000 mik_py-0.0.2/eicar_pack_10/__init__.py
+-rw-r--r--   0 michaelchung   (501) staff       (20)      680 2023-03-26 21:01:11.000000 mik_py-0.0.2/eicar_pack_10/eic_py_.py
+-rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.2/eicar_pack_10/eicar.com
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-06-29 12:56:08.580734 mik_py-0.0.2/mik_py.egg-info/
+-rw-r--r--   0 michaelchung   (501) staff       (20)      554 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchung   (501) staff       (20)      235 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)        1 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)       14 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/top_level.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)       38 2023-06-29 12:56:08.582054 mik_py-0.0.2/setup.cfg
+-rw-r--r--   0 michaelchung   (501) staff       (20)      970 2023-06-29 12:55:34.000000 mik_py-0.0.2/setup.py
```

### Comparing `mik_py-0.0.1/mik_pack_10/mik_py_.py` & `mik_py-0.0.2/eicar_pack_10/eic_py_.py`

 * *Files identical despite different names*

### Comparing `mik_py-0.0.1/setup.py` & `mik_py-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="mik_py",
-    version="0.0.1",
+    version="0.0.2",
     author="Mike",
-    author_email="mike@gmail.com",
-    description="eicar test package",
-    long_description="eicar test package",
+    author_email="michaelrchung@gmail.com",
+    description="A Python Package created to help test application security tools",
+    long_description="Installing this python package will download a malware file that isn't maliciious. This package can be used to help test any application or open source security tools. ",
     long_description_content_type="text/markdown",
     #url="www.test.com",
     packages=find_packages(),
     include_package_data=True,
     packages_data={
         'eicar_py':['eicar.com'],
     },
```

