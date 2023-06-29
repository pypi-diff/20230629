# Comparing `tmp/featurelayers-1.4.8.tar.gz` & `tmp/featurelayers-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.4.8.tar", last modified: Thu Jun 29 08:25:37 2023, max compression
+gzip compressed data, was "featurelayers-1.4.9.tar", last modified: Thu Jun 29 08:26:08 2023, max compression
```

## Comparing `featurelayers-1.4.8.tar` & `featurelayers-1.4.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:25:37.438774 featurelayers-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:25:37.438774 featurelayers-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:25:21.000000 featurelayers-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:25:37.434774 featurelayers-1.4.8/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:25:21.000000 featurelayers-1.4.8/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:25:21.000000 featurelayers-1.4.8/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:25:21.000000 featurelayers-1.4.8/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:25:37.438774 featurelayers-1.4.8/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-29 08:25:21.000000 featurelayers-1.4.8/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:25:21.000000 featurelayers-1.4.8/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:25:37.438774 featurelayers-1.4.8/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:25:37.000000 featurelayers-1.4.8/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:25:37.000000 featurelayers-1.4.8/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:25:37.000000 featurelayers-1.4.8/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:25:37.000000 featurelayers-1.4.8/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:25:37.000000 featurelayers-1.4.8/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:25:37.438774 featurelayers-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:25:21.000000 featurelayers-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.884168 featurelayers-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:26:08.884168 featurelayers-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:25:51.000000 featurelayers-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.880168 featurelayers-1.4.9/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.884168 featurelayers-1.4.9/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.880168 featurelayers-1.4.9/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:26:08.884168 featurelayers-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:25:51.000000 featurelayers-1.4.9/setup.py
```

### Comparing `featurelayers-1.4.8/PKG-INFO` & `featurelayers-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.4.8
+Version: 1.4.9
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
 
-__version__ = ""1.4.8""
+__version__ = ""1.4.9""
```

### Comparing `featurelayers-1.4.8/README.md` & `featurelayers-1.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.4.8""
+__version__ = ""1.4.9""
```

### Comparing `featurelayers-1.4.8/featurelayers/layers/LBC.py` & `featurelayers-1.4.9/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.4.8/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.4.9/featurelayers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.4.8
+Version: 1.4.9
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
 
-__version__ = ""1.4.8""
+__version__ = ""1.4.9""
```

### Comparing `featurelayers-1.4.8/setup.py` & `featurelayers-1.4.9/setup.py`

 * *Files identical despite different names*

