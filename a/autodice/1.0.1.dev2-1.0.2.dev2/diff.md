# Comparing `tmp/autodice-1.0.1.dev2.tar.gz` & `tmp/autodice-1.0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodice-1.0.1.dev2.tar", last modified: Thu Jun 29 15:14:18 2023, max compression
+gzip compressed data, was "autodice-1.0.2.dev2.tar", last modified: Thu Jun 29 17:35:00 2023, max compression
```

## Comparing `autodice-1.0.1.dev2.tar` & `autodice-1.0.2.dev2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:14:18.645528 autodice-1.0.1.dev2/
--rw-rw-r--   0 sky       (1000) sky       (1000)     1081 2022-12-01 16:53:46.000000 autodice-1.0.1.dev2/LICENSE.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)     3556 2023-06-29 15:14:18.645528 autodice-1.0.1.dev2/PKG-INFO
--rw-rw-r--   0 sky       (1000) sky       (1000)     2420 2023-06-29 14:22:44.000000 autodice-1.0.1.dev2/README.md
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:14:18.645528 autodice-1.0.1.dev2/autodice.egg-info/
--rw-rw-r--   0 sky       (1000) sky       (1000)     3556 2023-06-29 15:14:18.000000 autodice-1.0.1.dev2/autodice.egg-info/PKG-INFO
--rw-rw-r--   0 sky       (1000) sky       (1000)      361 2023-06-29 15:14:18.000000 autodice-1.0.1.dev2/autodice.egg-info/SOURCES.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)        1 2023-06-29 15:14:18.000000 autodice-1.0.1.dev2/autodice.egg-info/dependency_links.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       39 2023-06-29 15:14:18.000000 autodice-1.0.1.dev2/autodice.egg-info/entry_points.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       50 2023-06-29 15:14:18.000000 autodice-1.0.1.dev2/autodice.egg-info/requires.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       10 2023-06-29 15:14:18.000000 autodice-1.0.1.dev2/autodice.egg-info/top_level.txt
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:14:18.645528 autodice-1.0.1.dev2/partition/
--rw-r--r--   0 sky       (1000) sky       (1000)      174 2023-06-29 15:12:52.000000 autodice-1.0.1.dev2/partition/__init__.py
--rwxrwxr-x   0 sky       (1000) sky       (1000)     5290 2022-08-01 20:47:57.000000 autodice-1.0.1.dev2/partition/code_generator.py
--rw-rw-r--   0 sky       (1000) sky       (1000)    44651 2023-06-29 14:19:33.000000 autodice-1.0.1.dev2/partition/dice.py
--rwxrwxr-x   0 sky       (1000) sky       (1000)    46793 2023-06-29 15:08:09.000000 autodice-1.0.1.dev2/partition/interface.py
--rw-rw-r--   0 sky       (1000) sky       (1000)      230 2022-12-01 16:53:46.000000 autodice-1.0.1.dev2/pyproject.toml
--rw-rw-r--   0 sky       (1000) sky       (1000)       78 2023-06-29 15:14:18.645528 autodice-1.0.1.dev2/setup.cfg
--rw-rw-r--   0 sky       (1000) sky       (1000)     7990 2023-06-29 15:13:02.000000 autodice-1.0.1.dev2/setup.py
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:14:18.645528 autodice-1.0.1.dev2/tests/
--rw-rw-r--   0 sky       (1000) sky       (1000)      417 2022-12-01 16:53:46.000000 autodice-1.0.1.dev2/tests/test_simple.py
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/
+-rw-rw-r--   0 sky       (1000) sky       (1000)     1081 2022-12-01 16:53:46.000000 autodice-1.0.2.dev2/LICENSE.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)     3838 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/PKG-INFO
+-rw-rw-r--   0 sky       (1000) sky       (1000)     2702 2023-06-29 17:34:21.000000 autodice-1.0.2.dev2/README.md
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/autodice.egg-info/
+-rw-rw-r--   0 sky       (1000) sky       (1000)     3838 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/PKG-INFO
+-rw-rw-r--   0 sky       (1000) sky       (1000)      361 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/SOURCES.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)        1 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/dependency_links.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       39 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/entry_points.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       50 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/requires.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       10 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/top_level.txt
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/partition/
+-rw-r--r--   0 sky       (1000) sky       (1000)      174 2023-06-29 15:12:52.000000 autodice-1.0.2.dev2/partition/__init__.py
+-rwxrwxr-x   0 sky       (1000) sky       (1000)     5290 2022-08-01 20:47:57.000000 autodice-1.0.2.dev2/partition/code_generator.py
+-rw-rw-r--   0 sky       (1000) sky       (1000)    44651 2023-06-29 14:19:33.000000 autodice-1.0.2.dev2/partition/dice.py
+-rwxrwxr-x   0 sky       (1000) sky       (1000)    44946 2023-06-29 16:08:22.000000 autodice-1.0.2.dev2/partition/interface.py
+-rw-rw-r--   0 sky       (1000) sky       (1000)      230 2022-12-01 16:53:46.000000 autodice-1.0.2.dev2/pyproject.toml
+-rw-rw-r--   0 sky       (1000) sky       (1000)       78 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/setup.cfg
+-rw-rw-r--   0 sky       (1000) sky       (1000)     7990 2023-06-29 17:34:37.000000 autodice-1.0.2.dev2/setup.py
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/tests/
+-rw-rw-r--   0 sky       (1000) sky       (1000)      417 2022-12-01 16:53:46.000000 autodice-1.0.2.dev2/tests/test_simple.py
```

### Comparing `autodice-1.0.1.dev2/LICENSE.txt` & `autodice-1.0.2.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autodice-1.0.1.dev2/PKG-INFO` & `autodice-1.0.2.dev2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodice
-Version: 1.0.1.dev2
+Version: 1.0.2.dev2
 Summary: Automated Distributed CNN inference at the Edge
 Home-page: https://github.com/parrotsky/AutoDiCE
 Author: Parrotsky
 Author-email: x.guo3@uva.nl
 Project-URL: Bug Reports, https://github.com/parrotsky/AutoDiCE/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://github.com/parrotsky/AutoDiCE
@@ -26,58 +26,67 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # AutoDiCE Project.
 [The source for this AutoDiCE project is available here][src].
 ![Python Logo](https://www.python.org/static/community_logos/python-logo.png "Sample inline image")
 
-# How to use the ONNXPartition 
-```
 
+# How to use the Partition 
+```
+### Prepare AlexNet Model and Computing nodes
 ### mapping.json Template (AlexNet):
 {"lenovo_cpu0": ["conv1_1", "conv1_2", "norm1_1", "pool1_1", "conv2_1", "conv2_2", "norm2_1", "pool2_1", "conv3_1", "conv3_2", "conv4_1", "conv4_2", "conv5_1", "conv5_2", "pool5_1", "OC2_DUMMY_0", "fc6_1", "fc6_2"], "lenovo_cpu1": ["fc6_3", "fc7_1", "fc7_2", "fc7_3", "fc8_1", "prob_1"]}
 
+### Quick Start.
+import os,sys
+ 
+from partition.interface import *
+
 if __name__ == '__main__':
 
     output_dirs= './models'
     if not os.path.exists(output_dirs):
     # Create a new directory because it does not exist
         os.makedirs(output_dirs)
         print("The output directory %s is created!" % (output_dirs))
 
     origin_model = "bvlcalexnet-9.onnx"
-    #origin_model = "resnet101-v2-7.onnx"
-    #origin_model = "densenet-9.onnx"
+    ### Can be downloaded from:
+    # https://github.com/onnx/models/blob/main/vision/classification/alexnet/model/bvlcalexnet-9.onnx
     input_model = format_onnx(origin_model)
     model =  onnx.load(input_model)
-    model_len = len(model.graph.node)
-    resourceid = { 1:'lenovo_cpu0', 2:'lenovo_cpu1'}
+    # resourceid = { 1:'lenovo_cpu0', 2:'lenovo_cpu1'}
     platforms = ['lenovo']
-    random_map = load_json('./mapping.json')
 
-    #M=3
-    #gene = np.array([0,18]).astype(int)
-    #chromosome = ChromosomePartGen(gene, model_len, resourceid)
-    #random_map = MappingGenerator(resourceid, chromosome, input_model)
-    #print ("Mapping: ", random_map)
-    #save_json(random_map, './mapping.json')
+    ### How the layers in alexnet model distribute over two computing nodes???
+    random_map = {
+            "lenovo_cpu0":
+                ["conv1_1", "conv1_2", "norm1_1", "pool1_1", "conv2_1",
+                "conv2_2", "norm2_1", "pool2_1", "conv3_1", "conv3_2",
+                "conv4_1", "conv4_2", "conv5_1", "conv5_2", "pool5_1",
+                "OC2_DUMMY_0", "fc6_1", "fc6_2"],
+            "lenovo_cpu1":
+                ["fc6_3", "fc7_1", "fc7_2", "fc7_3", "fc8_1", "prob_1"]
+             }
+    
 
-    start_time = time.time()
     InputSpecs = Interface(model=input_model, mappings=random_map, platforms=platforms)
-    print ("Front End time: %f (s)"%(time.time() - start_time))
     #cppname, NodesList, ComputingNodes
+    ### Generate Cpp Files for Multinode-Inference.
     GenerateCode = EngineCode(
         CppName = "./models/multinode",
         Platforms = InputSpecs.platforms,
         NodesList = InputSpecs.nodes,
         ComputingNodes = InputSpecs.computingnodes,
         ValueInfos = InputSpecs.value_map,
         Inputs = InputSpecs.inputs,
         Outputs = InputSpecs.outputs,
         Benchmark = False)
+
 # ...
 ```
 
  
 
 [packaging guide]: https://packaging.python.org
 [distribution tutorial]: https://packaging.python.org/tutorials/packaging-projects/
```

### Comparing `autodice-1.0.1.dev2/autodice.egg-info/PKG-INFO` & `autodice-1.0.2.dev2/autodice.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodice
-Version: 1.0.1.dev2
+Version: 1.0.2.dev2
 Summary: Automated Distributed CNN inference at the Edge
 Home-page: https://github.com/parrotsky/AutoDiCE
 Author: Parrotsky
 Author-email: x.guo3@uva.nl
 Project-URL: Bug Reports, https://github.com/parrotsky/AutoDiCE/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://github.com/parrotsky/AutoDiCE
@@ -26,58 +26,67 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # AutoDiCE Project.
 [The source for this AutoDiCE project is available here][src].
 ![Python Logo](https://www.python.org/static/community_logos/python-logo.png "Sample inline image")
 
-# How to use the ONNXPartition 
-```
 
+# How to use the Partition 
+```
+### Prepare AlexNet Model and Computing nodes
 ### mapping.json Template (AlexNet):
 {"lenovo_cpu0": ["conv1_1", "conv1_2", "norm1_1", "pool1_1", "conv2_1", "conv2_2", "norm2_1", "pool2_1", "conv3_1", "conv3_2", "conv4_1", "conv4_2", "conv5_1", "conv5_2", "pool5_1", "OC2_DUMMY_0", "fc6_1", "fc6_2"], "lenovo_cpu1": ["fc6_3", "fc7_1", "fc7_2", "fc7_3", "fc8_1", "prob_1"]}
 
+### Quick Start.
+import os,sys
+ 
+from partition.interface import *
+
 if __name__ == '__main__':
 
     output_dirs= './models'
     if not os.path.exists(output_dirs):
     # Create a new directory because it does not exist
         os.makedirs(output_dirs)
         print("The output directory %s is created!" % (output_dirs))
 
     origin_model = "bvlcalexnet-9.onnx"
-    #origin_model = "resnet101-v2-7.onnx"
-    #origin_model = "densenet-9.onnx"
+    ### Can be downloaded from:
+    # https://github.com/onnx/models/blob/main/vision/classification/alexnet/model/bvlcalexnet-9.onnx
     input_model = format_onnx(origin_model)
     model =  onnx.load(input_model)
-    model_len = len(model.graph.node)
-    resourceid = { 1:'lenovo_cpu0', 2:'lenovo_cpu1'}
+    # resourceid = { 1:'lenovo_cpu0', 2:'lenovo_cpu1'}
     platforms = ['lenovo']
-    random_map = load_json('./mapping.json')
 
-    #M=3
-    #gene = np.array([0,18]).astype(int)
-    #chromosome = ChromosomePartGen(gene, model_len, resourceid)
-    #random_map = MappingGenerator(resourceid, chromosome, input_model)
-    #print ("Mapping: ", random_map)
-    #save_json(random_map, './mapping.json')
+    ### How the layers in alexnet model distribute over two computing nodes???
+    random_map = {
+            "lenovo_cpu0":
+                ["conv1_1", "conv1_2", "norm1_1", "pool1_1", "conv2_1",
+                "conv2_2", "norm2_1", "pool2_1", "conv3_1", "conv3_2",
+                "conv4_1", "conv4_2", "conv5_1", "conv5_2", "pool5_1",
+                "OC2_DUMMY_0", "fc6_1", "fc6_2"],
+            "lenovo_cpu1":
+                ["fc6_3", "fc7_1", "fc7_2", "fc7_3", "fc8_1", "prob_1"]
+             }
+    
 
-    start_time = time.time()
     InputSpecs = Interface(model=input_model, mappings=random_map, platforms=platforms)
-    print ("Front End time: %f (s)"%(time.time() - start_time))
     #cppname, NodesList, ComputingNodes
+    ### Generate Cpp Files for Multinode-Inference.
     GenerateCode = EngineCode(
         CppName = "./models/multinode",
         Platforms = InputSpecs.platforms,
         NodesList = InputSpecs.nodes,
         ComputingNodes = InputSpecs.computingnodes,
         ValueInfos = InputSpecs.value_map,
         Inputs = InputSpecs.inputs,
         Outputs = InputSpecs.outputs,
         Benchmark = False)
+
 # ...
 ```
 
  
 
 [packaging guide]: https://packaging.python.org
 [distribution tutorial]: https://packaging.python.org/tutorials/packaging-projects/
```

### Comparing `autodice-1.0.1.dev2/partition/code_generator.py` & `autodice-1.0.2.dev2/partition/code_generator.py`

 * *Files identical despite different names*

### Comparing `autodice-1.0.1.dev2/partition/dice.py` & `autodice-1.0.2.dev2/partition/dice.py`

 * *Files identical despite different names*

### Comparing `autodice-1.0.1.dev2/partition/interface.py` & `autodice-1.0.2.dev2/partition/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1000,55 +1000,8 @@
         gene = resourceid[chromosome[i]]   ### name of resource.
         #print (gene)
         mapping.setdefault(gene, []).append(graph.node[i].name)
 
     return mapping
 
 
-if __name__ == '__main__':
-
-    output_dirs= './models'
-    if not os.path.exists(output_dirs):
-    # Create a new directory because it does not exist
-        os.makedirs(output_dirs)
-        print("The output directory %s is created!" % (output_dirs))
-
-    origin_model = "bvlcalexnet-9.onnx"
-    # Can be downloaded from:
-    # https://github.com/onnx/models/blob/main/vision/classification/alexnet/model/bvlcalexnet-9.onnx
-    input_model = format_onnx(origin_model)
-    model =  onnx.load(input_model)
-    model_len = len(model.graph.node)
-    # resourceid = { 1:'lenovo_cpu0', 2:'lenovo_cpu1'}
-    platforms = ['lenovo']
-    random_map = {
-            "lenovo_cpu0":
-                ["conv1_1", "conv1_2", "norm1_1", "pool1_1", "conv2_1",
-                "conv2_2", "norm2_1", "pool2_1", "conv3_1", "conv3_2", 
-                "conv4_1", "conv4_2", "conv5_1", "conv5_2", "pool5_1",
-                "OC2_DUMMY_0", "fc6_1", "fc6_2"],
-            "lenovo_cpu1": 
-                ["fc6_3", "fc7_1", "fc7_2", "fc7_3", "fc8_1", "prob_1"]
-             }
-    # random_map = load_json('./mapping.json')
-
-    #M=3
-    #gene = np.array([0,18]).astype(int)
-    #chromosome = ChromosomePartGen(gene, model_len, resourceid)
-    #random_map = MappingGenerator(resourceid, chromosome, input_model)
-    #print ("Mapping: ", random_map)
-    #save_json(random_map, './mapping.json')
-
-    InputSpecs = Interface(model=input_model, mappings=random_map, platforms=platforms)
-    #cppname, NodesList, ComputingNodes
-    GenerateCode = EngineCode(
-        CppName = "./models/multinode",
-        Platforms = InputSpecs.platforms,
-        NodesList = InputSpecs.nodes,
-        ComputingNodes = InputSpecs.computingnodes,
-        ValueInfos = InputSpecs.value_map,
-        Inputs = InputSpecs.inputs,
-        Outputs = InputSpecs.outputs,
-        Benchmark = False)
-
-
```

### Comparing `autodice-1.0.1.dev2/setup.py` & `autodice-1.0.2.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="autodice",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.1.dev2",  # Required
+    version="1.0.2.dev2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Automated Distributed CNN inference at the Edge",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

