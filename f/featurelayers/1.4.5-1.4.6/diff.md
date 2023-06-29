# Comparing `tmp/featurelayers-1.4.5.tar.gz` & `tmp/featurelayers-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.4.5.tar", last modified: Thu Jun 29 08:16:51 2023, max compression
+gzip compressed data, was "featurelayers-1.4.6.tar", last modified: Thu Jun 29 08:16:58 2023, max compression
```

## Comparing `featurelayers-1.4.5.tar` & `featurelayers-1.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:51.295587 featurelayers-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:16:51.295587 featurelayers-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:16:31.000000 featurelayers-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:51.295587 featurelayers-1.4.5/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:16:31.000000 featurelayers-1.4.5/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:16:31.000000 featurelayers-1.4.5/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:16:31.000000 featurelayers-1.4.5/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:51.295587 featurelayers-1.4.5/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-29 08:16:31.000000 featurelayers-1.4.5/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:16:31.000000 featurelayers-1.4.5/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:51.295587 featurelayers-1.4.5/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:16:51.000000 featurelayers-1.4.5/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:16:51.000000 featurelayers-1.4.5/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:16:51.000000 featurelayers-1.4.5/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:16:51.000000 featurelayers-1.4.5/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:16:51.000000 featurelayers-1.4.5/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:16:51.295587 featurelayers-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:16:31.000000 featurelayers-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:58.156444 featurelayers-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:16:58.156444 featurelayers-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:16:41.000000 featurelayers-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:58.156444 featurelayers-1.4.6/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:16:41.000000 featurelayers-1.4.6/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:16:41.000000 featurelayers-1.4.6/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:16:41.000000 featurelayers-1.4.6/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:58.156444 featurelayers-1.4.6/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-29 08:16:41.000000 featurelayers-1.4.6/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:16:41.000000 featurelayers-1.4.6/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:16:58.156444 featurelayers-1.4.6/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:16:58.000000 featurelayers-1.4.6/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:16:58.000000 featurelayers-1.4.6/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:16:58.000000 featurelayers-1.4.6/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:16:58.000000 featurelayers-1.4.6/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:16:58.000000 featurelayers-1.4.6/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:16:58.156444 featurelayers-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:16:41.000000 featurelayers-1.4.6/setup.py
```

### Comparing `featurelayers-1.4.5/PKG-INFO` & `featurelayers-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.4.5
+Version: 1.4.6
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
 
-__version__ = ""1.4.5""
+__version__ = ""1.4.6""
```

### Comparing `featurelayers-1.4.5/README.md` & `featurelayers-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.4.5""
+__version__ = ""1.4.6""
```

### Comparing `featurelayers-1.4.5/featurelayers/layers/LBC.py` & `featurelayers-1.4.6/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.4.5/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.4.6/featurelayers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.4.5
+Version: 1.4.6
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
 
-__version__ = ""1.4.5""
+__version__ = ""1.4.6""
```

### Comparing `featurelayers-1.4.5/setup.py` & `featurelayers-1.4.6/setup.py`

 * *Files identical despite different names*

