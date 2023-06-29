# Comparing `tmp/telexy.sam-1.23.634.tar.gz` & `tmp/telexy.sam-1.23.635.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telexy.sam-1.23.634.tar", last modified: Tue Jun 27 16:47:18 2023, max compression
+gzip compressed data, was "telexy.sam-1.23.635.tar", last modified: Thu Jun 29 18:46:48 2023, max compression
```

## Comparing `telexy.sam-1.23.634.tar` & `telexy.sam-1.23.635.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 16:47:18.556291 telexy.sam-1.23.634/
--rw-rw-rw-   0        0        0     1076 2023-06-21 03:48:56.000000 telexy.sam-1.23.634/LICENSE.txt
--rw-rw-rw-   0        0        0      416 2023-06-27 16:47:18.555290 telexy.sam-1.23.634/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-06-21 14:45:02.000000 telexy.sam-1.23.634/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 16:47:18.546291 telexy.sam-1.23.634/sam/
--rw-rw-rw-   0        0        0       20 2023-06-26 22:57:28.000000 telexy.sam-1.23.634/sam/__init__.py
--rw-rw-rw-   0        0        0      125 2023-06-27 16:41:15.000000 telexy.sam-1.23.634/sam/__main__.py
--rw-rw-rw-   0        0        0      463 2023-06-27 16:45:35.000000 telexy.sam-1.23.634/sam/sam.py
--rw-rw-rw-   0        0        0       42 2023-06-27 16:47:18.557293 telexy.sam-1.23.634/setup.cfg
--rw-rw-rw-   0        0        0     1325 2023-06-27 16:46:57.000000 telexy.sam-1.23.634/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 16:47:18.554289 telexy.sam-1.23.634/telexy.sam.egg-info/
--rw-rw-rw-   0        0        0      416 2023-06-27 16:47:18.000000 telexy.sam-1.23.634/telexy.sam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-27 16:47:18.000000 telexy.sam-1.23.634/telexy.sam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:47:18.000000 telexy.sam-1.23.634/telexy.sam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-27 16:47:18.000000 telexy.sam-1.23.634/telexy.sam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-27 16:47:18.000000 telexy.sam-1.23.634/telexy.sam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 18:46:48.131200 telexy.sam-1.23.635/
+-rw-rw-rw-   0        0        0     1076 2023-06-21 03:48:56.000000 telexy.sam-1.23.635/LICENSE.txt
+-rw-rw-rw-   0        0        0      416 2023-06-29 18:46:48.131200 telexy.sam-1.23.635/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-06-21 14:45:02.000000 telexy.sam-1.23.635/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 18:46:48.124170 telexy.sam-1.23.635/sam/
+-rw-rw-rw-   0        0        0       20 2023-06-26 22:57:28.000000 telexy.sam-1.23.635/sam/__init__.py
+-rw-rw-rw-   0        0        0      461 2023-06-29 18:45:12.000000 telexy.sam-1.23.635/sam/__main__.py
+-rw-rw-rw-   0        0        0      836 2023-06-29 18:46:28.000000 telexy.sam-1.23.635/sam/sam.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:46:48.131200 telexy.sam-1.23.635/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-06-29 18:46:25.000000 telexy.sam-1.23.635/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:46:48.130217 telexy.sam-1.23.635/telexy.sam.egg-info/
+-rw-rw-rw-   0        0        0      416 2023-06-29 18:46:48.000000 telexy.sam-1.23.635/telexy.sam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-29 18:46:48.000000 telexy.sam-1.23.635/telexy.sam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:46:48.000000 telexy.sam-1.23.635/telexy.sam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-29 18:46:48.000000 telexy.sam-1.23.635/telexy.sam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 18:46:48.000000 telexy.sam-1.23.635/telexy.sam.egg-info/top_level.txt
```

### Comparing `telexy.sam-1.23.634/LICENSE.txt` & `telexy.sam-1.23.635/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telexy.sam-1.23.634/setup.py` & `telexy.sam-1.23.635/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telexy.sam",                     # This is the name of the package
-    version="1.23.634",                        # The initial release version
+    version="1.23.635",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="SAM Inference service",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.10',                # Minimum version requirement of the package
     py_modules=["sam"],             # Name of the python package
-    install_requires=['telexy.mars'],                     # Install other dependencies if any
+    install_requires=['telexy.mars', "opencv-python", 'torch', 'torchvision', 'numpy'],                     # Install other dependencies if any
 )
```

