# Comparing `tmp/autodistill-clip-0.0.1.tar.gz` & `tmp/autodistill_clip-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-clip-0.0.1.tar", last modified: Wed Jun  7 11:06:30 2023, max compression
+gzip compressed data, was "autodistill_clip-0.1.0.tar", last modified: Thu Jun 29 13:13:49 2023, max compression
```

## Comparing `autodistill-clip-0.0.1.tar` & `autodistill_clip-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:30.547305 autodistill-clip-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      359 2023-06-07 11:06:30.547170 autodistill-clip-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-07 11:06:28.000000 autodistill-clip-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:30.546139 autodistill-clip-0.0.1/autodistill_clip/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 11:06:28.000000 autodistill-clip-0.0.1/autodistill_clip/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:30.546996 autodistill-clip-0.0.1/autodistill_clip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      359 2023-06-07 11:06:30.000000 autodistill-clip-0.0.1/autodistill_clip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      246 2023-06-07 11:06:30.000000 autodistill-clip-0.0.1/autodistill_clip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 11:06:30.000000 autodistill-clip-0.0.1/autodistill_clip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 11:06:30.000000 autodistill-clip-0.0.1/autodistill_clip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-07 11:06:30.000000 autodistill-clip-0.0.1/autodistill_clip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 11:06:30.547346 autodistill-clip-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      977 2023-06-07 11:06:28.000000 autodistill-clip-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:13:49.839389 autodistill_clip-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)     1055 2023-06-06 08:17:22.000000 autodistill_clip-0.1.0/LICENSE.md
+-rw-r--r--   0 james      (501) staff       (20)     2253 2023-06-29 13:13:49.839265 autodistill_clip-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1780 2023-06-06 08:18:00.000000 autodistill_clip-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:13:49.838273 autodistill_clip-0.1.0/autodistill_clip/
+-rw-r--r--   0 james      (501) staff       (20)       68 2023-06-07 12:52:36.000000 autodistill_clip-0.1.0/autodistill_clip/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1710 2023-06-29 13:11:43.000000 autodistill_clip-0.1.0/autodistill_clip/clip_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:13:49.839079 autodistill_clip-0.1.0/autodistill_clip.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2253 2023-06-29 13:13:49.000000 autodistill_clip-0.1.0/autodistill_clip.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      288 2023-06-29 13:13:49.000000 autodistill_clip-0.1.0/autodistill_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 13:13:49.000000 autodistill_clip-0.1.0/autodistill_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       77 2023-06-29 13:13:49.000000 autodistill_clip-0.1.0/autodistill_clip.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       17 2023-06-29 13:13:49.000000 autodistill_clip-0.1.0/autodistill_clip.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 13:13:49.839431 autodistill_clip-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1130 2023-06-29 13:13:36.000000 autodistill_clip-0.1.0/setup.py
```

### Comparing `autodistill-clip-0.0.1/setup.py` & `autodistill_clip-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./autodistill_clip/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="autodistill-clip",
+    name="autodistill_clip",  
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="CLIP module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/autodistill/autodistill-clip",
+    install_requires=[
+        "torch",
+        "supervision",
+        "numpy"
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

