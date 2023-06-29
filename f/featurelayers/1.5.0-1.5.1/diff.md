# Comparing `tmp/featurelayers-1.5.0.tar.gz` & `tmp/featurelayers-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.5.0.tar", last modified: Thu Jun 29 08:36:16 2023, max compression
+gzip compressed data, was "featurelayers-1.5.1.tar", last modified: Thu Jun 29 08:54:42 2023, max compression
```

## Comparing `featurelayers-1.5.0.tar` & `featurelayers-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.771573 featurelayers-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:36:16.771573 featurelayers-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:35:57.000000 featurelayers-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.767573 featurelayers-1.5.0/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.771573 featurelayers-1.5.0/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.767573 featurelayers-1.5.0/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:36:16.771573 featurelayers-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:35:57.000000 featurelayers-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:54:42.843857 featurelayers-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:54:42.843857 featurelayers-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:54:22.000000 featurelayers-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:54:42.839857 featurelayers-1.5.1/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:54:42.843857 featurelayers-1.5.1/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/layers/LDP.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:54:42.843857 featurelayers-1.5.1/featurelayers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/models/LBC_xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-29 08:54:22.000000 featurelayers-1.5.1/featurelayers/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:54:42.843857 featurelayers-1.5.1/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:54:42.000000 featurelayers-1.5.1/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 08:54:42.000000 featurelayers-1.5.1/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:54:42.000000 featurelayers-1.5.1/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:54:42.000000 featurelayers-1.5.1/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:54:42.000000 featurelayers-1.5.1/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:54:42.843857 featurelayers-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:54:22.000000 featurelayers-1.5.1/setup.py
```

### Comparing `featurelayers-1.5.0/PKG-INFO` & `featurelayers-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.5.0
+Version: 1.5.1
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
 
-__version__ = ""1.5.0""
+__version__ = ""1.5.1""
```

### Comparing `featurelayers-1.5.0/README.md` & `featurelayers-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.5.0""
+__version__ = ""1.5.1""
```

### Comparing `featurelayers-1.5.0/featurelayers/layers/LBC.py` & `featurelayers-1.5.1/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.0/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.5.1/featurelayers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.5.0
+Version: 1.5.1
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
 
-__version__ = ""1.5.0""
+__version__ = ""1.5.1""
```

### Comparing `featurelayers-1.5.0/setup.py` & `featurelayers-1.5.1/setup.py`

 * *Files identical despite different names*

