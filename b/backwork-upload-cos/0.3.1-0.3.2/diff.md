# Comparing `tmp/backwork-upload-cos-0.3.1.tar.gz` & `tmp/backwork-upload-cos-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backwork-upload-cos-0.3.1.tar", last modified: Tue Apr 19 18:47:22 2022, max compression
+gzip compressed data, was "backwork-upload-cos-0.3.2.tar", last modified: Thu Jun 29 18:36:42 2023, max compression
```

## Comparing `backwork-upload-cos-0.3.1.tar` & `backwork-upload-cos-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 winsonyuan   (501) staff       (20)        0 2022-04-19 18:47:22.858193 backwork-upload-cos-0.3.1/
--rw-r--r--   0 winsonyuan   (501) staff       (20)      697 2022-04-19 16:49:33.000000 backwork-upload-cos-0.3.1/CHANGELOG.md
--rw-r--r--   0 winsonyuan   (501) staff       (20)      477 2022-04-19 16:49:33.000000 backwork-upload-cos-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 winsonyuan   (501) staff       (20)    11357 2022-04-19 16:49:33.000000 backwork-upload-cos-0.3.1/LICENSE
--rw-r--r--   0 winsonyuan   (501) staff       (20)       13 2022-04-19 16:49:33.000000 backwork-upload-cos-0.3.1/MANIFEST.in
--rw-r--r--   0 winsonyuan   (501) staff       (20)     5863 2022-04-19 18:47:22.857666 backwork-upload-cos-0.3.1/PKG-INFO
--rw-r--r--   0 winsonyuan   (501) staff       (20)     4150 2022-04-19 16:49:33.000000 backwork-upload-cos-0.3.1/README.md
-drwxr-xr-x   0 winsonyuan   (501) staff       (20)        0 2022-04-19 18:47:22.855431 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/
--rw-r--r--   0 winsonyuan   (501) staff       (20)     5863 2022-04-19 18:47:22.000000 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/PKG-INFO
--rw-r--r--   0 winsonyuan   (501) staff       (20)      354 2022-04-19 18:47:22.000000 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/SOURCES.txt
--rw-r--r--   0 winsonyuan   (501) staff       (20)        1 2022-04-19 18:47:22.000000 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/dependency_links.txt
--rw-r--r--   0 winsonyuan   (501) staff       (20)      165 2022-04-19 18:47:22.000000 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/entry_points.txt
--rw-r--r--   0 winsonyuan   (501) staff       (20)       28 2022-04-19 18:47:22.000000 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/requires.txt
--rw-r--r--   0 winsonyuan   (501) staff       (20)        4 2022-04-19 18:47:22.000000 backwork-upload-cos-0.3.1/backwork_upload_cos.egg-info/top_level.txt
-drwxr-xr-x   0 winsonyuan   (501) staff       (20)        0 2022-04-19 18:47:22.856799 backwork-upload-cos-0.3.1/cos/
--rw-r--r--   0 winsonyuan   (501) staff       (20)      174 2022-04-19 16:49:33.000000 backwork-upload-cos-0.3.1/cos/__init__.py
--rw-r--r--   0 winsonyuan   (501) staff       (20)     9450 2022-04-19 17:59:27.000000 backwork-upload-cos-0.3.1/cos/cos.py
--rw-r--r--   0 winsonyuan   (501) staff       (20)       38 2022-04-19 18:47:22.858405 backwork-upload-cos-0.3.1/setup.cfg
--rw-r--r--   0 winsonyuan   (501) staff       (20)     1465 2022-04-19 18:47:17.000000 backwork-upload-cos-0.3.1/setup.py
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 18:36:42.132149 backwork-upload-cos-0.3.2/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      697 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/CHANGELOG.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      477 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)    11357 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/LICENSE
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       13 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/MANIFEST.in
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     4867 2023-06-29 18:36:42.131951 backwork-upload-cos-0.3.2/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     4150 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/README.md
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 18:36:42.131138 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     4867 2023-06-29 18:36:42.000000 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      354 2023-06-29 18:36:42.000000 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/SOURCES.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        1 2023-06-29 18:36:42.000000 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/dependency_links.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      164 2023-06-29 18:36:42.000000 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/entry_points.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       28 2023-06-29 18:36:42.000000 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/requires.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        4 2023-06-29 18:36:42.000000 backwork-upload-cos-0.3.2/backwork_upload_cos.egg-info/top_level.txt
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 18:36:42.131578 backwork-upload-cos-0.3.2/cos/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      174 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/cos/__init__.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     9450 2023-06-29 17:33:38.000000 backwork-upload-cos-0.3.2/cos/cos.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       38 2023-06-29 18:36:42.132202 backwork-upload-cos-0.3.2/setup.cfg
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1378 2023-06-29 18:35:14.000000 backwork-upload-cos-0.3.2/setup.py
```

### Comparing `backwork-upload-cos-0.3.1/CHANGELOG.md` & `backwork-upload-cos-0.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `backwork-upload-cos-0.3.1/LICENSE` & `backwork-upload-cos-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backwork-upload-cos-0.3.1/README.md` & `backwork-upload-cos-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `backwork-upload-cos-0.3.1/cos/cos.py` & `backwork-upload-cos-0.3.2/cos/cos.py`

 * *Files identical despite different names*

### Comparing `backwork-upload-cos-0.3.1/setup.py` & `backwork-upload-cos-0.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 """Add support for SoftLayer uploads
 """
 
 from os import path
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(HERE, 'README.md')) as f:
+with open(path.join(HERE, "README.md")) as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="backwork-upload-cos",
-    version="0.3.1",
+    version="0.3.2",
     description="Backwork plug-in for IBM Cloud Object Storage uploads.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/backwork-upload-cos",
-    author="Skills Network",
-    author_email="admin@skills.network",
+    author="Michael Lin",
+    author_email="michael.lin1@ibm.com",
     license="Apache 2",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Operating System :: POSIX :: Linux",
-        'License :: OSI Approved :: Apache Software License',
+        "License :: OSI Approved :: Apache Software License",
         "Topic :: Database",
         "Topic :: System :: Archiving :: Backup",
-        "Topic :: Utilities"
+        "Topic :: Utilities",
     ],
     packages=find_packages(),
-    install_requires=[
-        "backwork",
-        "ibm-cos-sdk>=2.4.4"
-    ],
+    install_requires=["backwork", "ibm-cos-sdk>=2.4.4"],
     entry_points={
-        "backwork.uploads": [
-            "cos=cos:CloudObjectStorageUpload"
-        ],
-        "backwork.shows": [
-            "cos=cos:CloudObjectStorageShow"
-        ],
-        "backwork.downloads": [
-            "cos=cos:CloudObjectStorageDownload"
-        ]
-    }
+        "backwork.uploads": ["cos=cos:CloudObjectStorageUpload"],
+        "backwork.shows": ["cos=cos:CloudObjectStorageShow"],
+        "backwork.downloads": ["cos=cos:CloudObjectStorageDownload"],
+    },
 )
```

