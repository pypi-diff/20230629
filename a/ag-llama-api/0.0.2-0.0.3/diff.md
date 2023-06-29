# Comparing `tmp/ag_llama_api-0.0.2.tar.gz` & `tmp/ag_llama_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api-0.0.2.tar", last modified: Thu Jun 29 12:22:42 2023, max compression
+gzip compressed data, was "dist\ag_llama_api-0.0.3.tar", last modified: Thu Jun 29 12:54:26 2023, max compression
```

## Comparing `ag_llama_api-0.0.2.tar` & `ag_llama_api-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:42.012708 ag_llama_api-0.0.2/
--rw-rw-rw-   0        0        0      354 2023-06-29 12:22:42.011714 ag_llama_api-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:41.992372 ag_llama_api-0.0.2/ag_llama_api.egg-info/
--rw-rw-rw-   0        0        0      354 2023-06-29 12:22:41.000000 ag_llama_api-0.0.2/ag_llama_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-29 12:22:41.000000 ag_llama_api-0.0.2/ag_llama_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:22:41.000000 ag_llama_api-0.0.2/ag_llama_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      290 2023-06-29 12:22:41.000000 ag_llama_api-0.0.2/ag_llama_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 12:22:41.000000 ag_llama_api-0.0.2/ag_llama_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:42.001795 ag_llama_api-0.0.2/llama_api/
--rw-rw-rw-   0        0        0     2186 2023-06-27 12:34:01.000000 ag_llama_api-0.0.2/llama_api/__init__.py
--rw-rw-rw-   0        0        0     9158 2023-06-28 17:09:08.000000 ag_llama_api-0.0.2/llama_api/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:42.010227 ag_llama_api-0.0.2/llama_api/ag_llama_api.egg-info/
--rw-rw-rw-   0        0        0      354 2023-06-29 12:17:47.000000 ag_llama_api-0.0.2/llama_api/ag_llama_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-06-29 12:16:06.000000 ag_llama_api-0.0.2/llama_api/ag_llama_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:17:47.000000 ag_llama_api-0.0.2/llama_api/ag_llama_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      290 2023-06-29 12:17:47.000000 ag_llama_api-0.0.2/llama_api/ag_llama_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 12:17:47.000000 ag_llama_api-0.0.2/llama_api/ag_llama_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api-0.0.2/llama_api/choice.py
--rw-rw-rw-   0        0        0    13780 2023-06-28 17:04:18.000000 ag_llama_api-0.0.2/llama_api/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api-0.0.2/llama_api/tokenizer.py
--rw-rw-rw-   0        0        0       42 2023-06-29 12:22:42.013203 ag_llama_api-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1240 2023-06-29 12:22:04.000000 ag_llama_api-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:54:26.320219 ag_llama_api-0.0.3/
+-rw-rw-rw-   0        0        0      354 2023-06-29 12:54:26.319228 ag_llama_api-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:54:26.320717 ag_llama_api-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-29 12:54:13.000000 ag_llama_api-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:54:26.291949 ag_llama_api-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 12:54:26.301868 ag_llama_api-0.0.3/src/ag_llama_api.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-06-29 12:54:26.000000 ag_llama_api-0.0.3/src/ag_llama_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-06-29 12:54:26.000000 ag_llama_api-0.0.3/src/ag_llama_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:54:26.000000 ag_llama_api-0.0.3/src/ag_llama_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      290 2023-06-29 12:54:26.000000 ag_llama_api-0.0.3/src/ag_llama_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-29 12:54:26.000000 ag_llama_api-0.0.3/src/ag_llama_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 12:54:26.311787 ag_llama_api-0.0.3/src/llama_api/
+-rw-rw-rw-   0        0        0     2186 2023-06-27 12:34:01.000000 ag_llama_api-0.0.3/src/llama_api/__init__.py
+-rw-rw-rw-   0        0        0     9158 2023-06-28 17:09:08.000000 ag_llama_api-0.0.3/src/llama_api/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api-0.0.3/src/llama_api/choice.py
+-rw-rw-rw-   0        0        0    13780 2023-06-28 17:04:18.000000 ag_llama_api-0.0.3/src/llama_api/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api-0.0.3/src/llama_api/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:54:26.317739 ag_llama_api-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api-0.0.3/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api-0.0.3/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api-0.0.3/tests/test_tokenizer.py
```

### Comparing `ag_llama_api-0.0.2/llama_api/__init__.py` & `ag_llama_api-0.0.3/src/llama_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.2/llama_api/__main__.py` & `ag_llama_api-0.0.3/src/llama_api/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.2/llama_api/choice.py` & `ag_llama_api-0.0.3/src/llama_api/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.2/llama_api/model.py` & `ag_llama_api-0.0.3/src/llama_api/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.2/llama_api/tokenizer.py` & `ag_llama_api-0.0.3/src/llama_api/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.2/setup.py` & `ag_llama_api-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="ag_llama_api",                     # This is the name of the package
-    version="0.0.2",                        # The initial release version
+    version="0.0.3",                        # The initial release version
     author="AA",                     # Full name of the author
     description="ag_llama_api Test Package for Somthing",
     long_description="long_description",      # Long description read from the the readme file
     long_description_content_type="text/markdown",
-    packages= setuptools.find_packages(),    # List of all python modules to be installed
+    packages= setuptools.find_packages(where="src"),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.8',                # Minimum version requirement of the package
     # py_modules=["ag_llama_api"],             # Name of the python package
-    # package_dir={'':'llama_api'},     # Directory of the source code of the package
+    package_dir={'':'src'},     # Directory of the source code of the package
     install_requires=required                     # Install other dependencies if any
 )
```

