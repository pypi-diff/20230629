# Comparing `tmp/featurelayers-1.5.4.tar.gz` & `tmp/featurelayers-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.5.4.tar", last modified: Thu Jun 29 14:02:22 2023, max compression
+gzip compressed data, was "featurelayers-1.5.5.tar", last modified: Thu Jun 29 14:02:57 2023, max compression
```

## Comparing `featurelayers-1.5.4.tar` & `featurelayers-1.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:22.720792 featurelayers-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 14:02:22.720792 featurelayers-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 14:02:02.000000 featurelayers-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:22.720792 featurelayers-1.5.4/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:22.720792 featurelayers-1.5.4/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/layers/LDP.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:22.720792 featurelayers-1.5.4/featurelayers/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/models/LBC_xception.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-29 14:02:02.000000 featurelayers-1.5.4/featurelayers/models/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:22.720792 featurelayers-1.5.4/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 14:02:22.000000 featurelayers-1.5.4/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 14:02:22.000000 featurelayers-1.5.4/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:02:22.000000 featurelayers-1.5.4/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 14:02:22.000000 featurelayers-1.5.4/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 14:02:22.000000 featurelayers-1.5.4/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:02:22.720792 featurelayers-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 14:02:02.000000 featurelayers-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:57.959464 featurelayers-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 14:02:57.959464 featurelayers-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 14:02:41.000000 featurelayers-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:57.959464 featurelayers-1.5.5/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:57.959464 featurelayers-1.5.5/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/layers/LDP.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:57.959464 featurelayers-1.5.5/featurelayers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/models/LBC_xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-29 14:02:41.000000 featurelayers-1.5.5/featurelayers/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:02:57.959464 featurelayers-1.5.5/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 14:02:57.000000 featurelayers-1.5.5/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 14:02:57.000000 featurelayers-1.5.5/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:02:57.000000 featurelayers-1.5.5/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 14:02:57.000000 featurelayers-1.5.5/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 14:02:57.000000 featurelayers-1.5.5/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:02:57.959464 featurelayers-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 14:02:41.000000 featurelayers-1.5.5/setup.py
```

### Comparing `featurelayers-1.5.4/PKG-INFO` & `featurelayers-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.5.4
+Version: 1.5.5
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
 
-__version__ = ""1.5.4""
+__version__ = ""1.5.5""
```

### Comparing `featurelayers-1.5.4/README.md` & `featurelayers-1.5.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.5.4""
+__version__ = ""1.5.5""
```

### Comparing `featurelayers-1.5.4/featurelayers/layers/LBC.py` & `featurelayers-1.5.5/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.4/featurelayers/layers/LDP.py` & `featurelayers-1.5.5/featurelayers/layers/LDP.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.4/featurelayers/models/LBC_xception.py` & `featurelayers-1.5.5/featurelayers/models/LBC_xception.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,17 +227,17 @@
     x = BatchNormalization(name='block14_sepconv2_bn')(x)
     x = Activation('relu', name='block14_sepconv2_act')(x)
 
     if include_top:
         x = GlobalAveragePooling2D(name='avg_pool')(x)
         x = Dense(1000, activation='relu')(x)
         x = Dense(500, activation='relu')(x)
-        x = Dense(256, activation='relu', name='predictions')(x)
-        x = Dense(100, activation='relu', name='predictions')(x)
-        x = Dense(50, activation='relu', name='predictions')(x)
+        x = Dense(256, activation='relu')(x)
+        x = Dense(100, activation='relu')(x)
+        x = Dense(50, activation='relu')(x)
         
         x = Dense(classes, activation='softmax', name='predictions')(x)
     else:
         if pooling == 'avg':
             x = GlobalAveragePooling2D()(x)
         elif pooling == 'max':
             x = GlobalMaxPooling2D()(x)
```

### Comparing `featurelayers-1.5.4/featurelayers/models/xception.py` & `featurelayers-1.5.5/featurelayers/models/xception.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.5.4/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.5.5/featurelayers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.5.4
+Version: 1.5.5
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
 
-__version__ = ""1.5.4""
+__version__ = ""1.5.5""
```

### Comparing `featurelayers-1.5.4/setup.py` & `featurelayers-1.5.5/setup.py`

 * *Files identical despite different names*

