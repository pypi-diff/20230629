# Comparing `tmp/featurelayers-1.4.9.tar.gz` & `tmp/featurelayers-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.4.9.tar", last modified: Thu Jun 29 08:26:08 2023, max compression
+gzip compressed data, was "featurelayers-1.5.0.tar", last modified: Thu Jun 29 08:36:16 2023, max compression
```

## Comparing `featurelayers-1.4.9.tar` & `featurelayers-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.884168 featurelayers-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:26:08.884168 featurelayers-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:25:51.000000 featurelayers-1.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.880168 featurelayers-1.4.9/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.884168 featurelayers-1.4.9/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:25:51.000000 featurelayers-1.4.9/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:26:08.880168 featurelayers-1.4.9/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:26:08.000000 featurelayers-1.4.9/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:26:08.884168 featurelayers-1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:25:51.000000 featurelayers-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.771573 featurelayers-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:36:16.771573 featurelayers-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 08:35:57.000000 featurelayers-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.767573 featurelayers-1.5.0/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.771573 featurelayers-1.5.0/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:35:57.000000 featurelayers-1.5.0/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:16.767573 featurelayers-1.5.0/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:36:16.000000 featurelayers-1.5.0/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:36:16.771573 featurelayers-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 08:35:57.000000 featurelayers-1.5.0/setup.py
```

### Comparing `featurelayers-1.4.9/PKG-INFO` & `featurelayers-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.4.9
+Version: 1.5.0
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
 
-__version__ = ""1.4.9""
+__version__ = ""1.5.0""
```

### Comparing `featurelayers-1.4.9/README.md` & `featurelayers-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.4.9""
+__version__ = ""1.5.0""
```

### Comparing `featurelayers-1.4.9/featurelayers/layers/LBC.py` & `featurelayers-1.5.0/featurelayers/layers/LBC.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,43 +41,43 @@
     return weights
 
 
 class LBC(Layer):
     def __init__(self, 
                  filters, 
                  kernel_size, 
-                 stride=1, 
+                 strides=1, 
                  padding='same', 
                  activation='relu', 
                  dilation=1, 
                  sparsity=0.9, 
                  use_bias=False,
                  name="khengyun"):
         """
               Local Binary Convolution (LBC) layer.
 
                Args:
                    - filters: Number of filters (output channels) in the convolution.
                    - kernel_size: Size of the convolution kernel.
-                   - stride: Stride of the convolution. Default is 1.
+                   - strides: strides of the convolution. Default is 1.
                    - padding: Padding mode for the convolution. Default is 'same'.
                    - activation: Activation function to use. Default is 'relu'.
                    - dilation: Dilation rate for the convolution. Default is 1.
                    - sparsity: Sparsity level of the non-trainable weights. Default is 0.9.
                    - name: Name of the layer. Default is 'lbc_layer'.
 
                Returns:
                    - The LBC layer.
 
                """
         super(LBC, self).__init__()
         self.nOutputPlane = filters
         self.kW = kernel_size
         self.sparsity = sparsity
-        self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=stride, padding=padding,
+        self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=strides, padding=padding,
                           dilation_rate=dilation, activation=activation, use_bias=use_bias, name=name)
 
     def build(self, input_shape):
         nInputPlane = input_shape[-1]
 
         with K.name_scope(self.LBC.name):
             self.LBC.build(input_shape)
@@ -95,15 +95,15 @@
         return self.LBC.compute_output_shape(input_shape)
 
     def get_config(self):
         config = super(LBC, self).get_config()
         config.update({
             'filters': self.nOutputPlane,
             'kernel_size': self.kW,
-            'stride': self.LBC.strides[0],
+            'strides': self.LBC.stridess[0],
             'padding': self.LBC.padding,
             'activation': self.LBC.activation,
             'dilation': self.LBC.dilation_rate[0],
             'sparsity': self.sparsity,
             'name': self.LBC.name
         })
         return config
```

### Comparing `featurelayers-1.4.9/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.5.0/featurelayers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.4.9
+Version: 1.5.0
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
 
-__version__ = ""1.4.9""
+__version__ = ""1.5.0""
```

### Comparing `featurelayers-1.4.9/setup.py` & `featurelayers-1.5.0/setup.py`

 * *Files identical despite different names*

