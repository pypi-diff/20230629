# Comparing `tmp/featurelayers-1.5.2.tar.gz` & `tmp/featurelayers-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.5.2.tar", last modified: Thu Jun 29 10:25:47 2023, max compression
+gzip compressed data, was "featurelayers-1.5.3.tar", last modified: Thu Jun 29 10:48:37 2023, max compression
```

## Comparing `featurelayers-1.5.2.tar` & `featurelayers-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:25:47.924060 featurelayers-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 10:25:47.924060 featurelayers-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 10:25:27.000000 featurelayers-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:25:47.920060 featurelayers-1.5.2/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:25:47.920060 featurelayers-1.5.2/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/layers/LDP.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:25:47.920060 featurelayers-1.5.2/featurelayers/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/models/LBC_xception.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-29 10:25:27.000000 featurelayers-1.5.2/featurelayers/models/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:25:47.920060 featurelayers-1.5.2/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 10:25:47.000000 featurelayers-1.5.2/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 10:25:47.000000 featurelayers-1.5.2/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:25:47.000000 featurelayers-1.5.2/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 10:25:47.000000 featurelayers-1.5.2/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 10:25:47.000000 featurelayers-1.5.2/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:25:47.924060 featurelayers-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 10:25:27.000000 featurelayers-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:48:37.086625 featurelayers-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 10:48:37.086625 featurelayers-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 10:48:17.000000 featurelayers-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:48:37.086625 featurelayers-1.5.3/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:48:37.086625 featurelayers-1.5.3/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/layers/LDP.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:48:37.086625 featurelayers-1.5.3/featurelayers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/models/LBC_xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-29 10:48:17.000000 featurelayers-1.5.3/featurelayers/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:48:37.086625 featurelayers-1.5.3/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 10:48:37.000000 featurelayers-1.5.3/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 10:48:37.000000 featurelayers-1.5.3/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:48:37.000000 featurelayers-1.5.3/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 10:48:37.000000 featurelayers-1.5.3/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 10:48:37.000000 featurelayers-1.5.3/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:48:37.086625 featurelayers-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 10:48:17.000000 featurelayers-1.5.3/setup.py
```

### Comparing `featurelayers-1.5.2/PKG-INFO` & `featurelayers-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.5.2
+Version: 1.5.3
 Summary: FeatureLayers Package
 Author: khengyun
 Author-email: khaangnguyeen@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
@@ -47,8 +47,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.5.2""
+__version__ = ""1.5.3""
```

### Comparing `featurelayers-1.5.2/README.md` & `featurelayers-1.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.5.2""
+__version__ = ""1.5.3""
```

### Comparing `featurelayers-1.5.2/featurelayers/layers/LBC.py` & `featurelayers-1.5.3/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.2/featurelayers/layers/LDP.py` & `featurelayers-1.5.3/featurelayers/layers/LDP.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.2/featurelayers/models/LBC_xception.py` & `featurelayers-1.5.3/featurelayers/models/LBC_xception.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.2/featurelayers/models/xception.py` & `featurelayers-1.5.3/featurelayers/models/xception.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.2/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.5.3/featurelayers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.5.2
+Version: 1.5.3
 Summary: FeatureLayers Package
 Author: khengyun
 Author-email: khaangnguyeen@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
@@ -47,8 +47,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.5.2""
+__version__ = ""1.5.3""
```

### Comparing `featurelayers-1.5.2/setup.py` & `featurelayers-1.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         'keras',
         'scipy',
         'rich',
         'matplotlib',
         'scikit-learn',
         'graphviz',
         'pydot',
+        'keras_applications',
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

