# Comparing `tmp/autodistill-dinov2-0.0.1.tar.gz` & `tmp/autodistill-dinov2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-dinov2-0.0.1.tar", last modified: Wed Jun  7 12:12:51 2023, max compression
+gzip compressed data, was "autodistill-dinov2-0.1.0.tar", last modified: Thu Jun 29 13:32:16 2023, max compression
```

## Comparing `autodistill-dinov2-0.0.1.tar` & `autodistill-dinov2-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:12:51.400886 autodistill-dinov2-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      895 2023-06-07 12:12:51.400763 autodistill-dinov2-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      550 2023-06-07 12:12:49.000000 autodistill-dinov2-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:12:51.399753 autodistill-dinov2-0.0.1/autodistill_dinov2/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 12:12:49.000000 autodistill-dinov2-0.0.1/autodistill_dinov2/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:12:51.400581 autodistill-dinov2-0.0.1/autodistill_dinov2.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      895 2023-06-07 12:12:51.000000 autodistill-dinov2-0.0.1/autodistill_dinov2.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      258 2023-06-07 12:12:51.000000 autodistill-dinov2-0.0.1/autodistill_dinov2.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 12:12:51.000000 autodistill-dinov2-0.0.1/autodistill_dinov2.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 12:12:51.000000 autodistill-dinov2-0.0.1/autodistill_dinov2.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       19 2023-06-07 12:12:51.000000 autodistill-dinov2-0.0.1/autodistill_dinov2.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 12:12:51.400925 autodistill-dinov2-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      981 2023-06-07 12:12:49.000000 autodistill-dinov2-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:32:16.153230 autodistill-dinov2-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)    19333 2023-06-09 11:00:53.000000 autodistill-dinov2-0.1.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2298 2023-06-29 13:32:16.153108 autodistill-dinov2-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1822 2023-06-09 11:08:10.000000 autodistill-dinov2-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:32:16.152250 autodistill-dinov2-0.1.0/autodistill_dinov2/
+-rw-r--r--   0 james      (501) staff       (20)       55 2023-06-29 13:32:12.000000 autodistill-dinov2-0.1.0/autodistill_dinov2/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3275 2023-06-29 13:30:13.000000 autodistill-dinov2-0.1.0/autodistill_dinov2/dinov2_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:32:16.152930 autodistill-dinov2-0.1.0/autodistill_dinov2.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2298 2023-06-29 13:32:16.000000 autodistill-dinov2-0.1.0/autodistill_dinov2.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      301 2023-06-29 13:32:16.000000 autodistill-dinov2-0.1.0/autodistill_dinov2.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 13:32:16.000000 autodistill-dinov2-0.1.0/autodistill_dinov2.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      123 2023-06-29 13:32:16.000000 autodistill-dinov2-0.1.0/autodistill_dinov2.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       19 2023-06-29 13:32:16.000000 autodistill-dinov2-0.1.0/autodistill_dinov2.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 13:32:16.153272 autodistill-dinov2-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1240 2023-06-29 13:31:52.000000 autodistill-dinov2-0.1.0/setup.py
```

### Comparing `autodistill-dinov2-0.0.1/setup.py` & `autodistill-dinov2-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./autodistill_dinov2/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="autodistill-dinov2",
+    name="autodistill-dinov2",  
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="DINOv2 module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/autodistill/autodistill-dinov2",
+    install_requires=[
+        "torch",
+        "torchvision",
+        "supervision",
+        "numpy",
+        "PIL",
+        "tqdm",
+        "scikit-learn",
+        "autodistill",
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
-
```

