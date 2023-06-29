# Comparing `tmp/autodice-1.0.0.dev2.tar.gz` & `tmp/autodice-1.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodice-1.0.0.dev2.tar", last modified: Wed Jun 28 22:46:31 2023, max compression
+gzip compressed data, was "autodice-1.0.1.dev1.tar", last modified: Thu Jun 29 15:01:36 2023, max compression
```

## Comparing `autodice-1.0.0.dev2.tar` & `autodice-1.0.1.dev1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/
--rw-rw-r--   0 sky       (1000) sky       (1000)     1081 2022-12-01 16:53:46.000000 autodice-1.0.0.dev2/LICENSE.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)     2024 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/PKG-INFO
--rw-rw-r--   0 sky       (1000) sky       (1000)      888 2023-06-28 22:18:48.000000 autodice-1.0.0.dev2/README.md
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/autodice.egg-info/
--rw-rw-r--   0 sky       (1000) sky       (1000)     2024 2023-06-28 22:46:31.000000 autodice-1.0.0.dev2/autodice.egg-info/PKG-INFO
--rw-rw-r--   0 sky       (1000) sky       (1000)      330 2023-06-28 22:46:31.000000 autodice-1.0.0.dev2/autodice.egg-info/SOURCES.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)        1 2023-06-28 22:46:31.000000 autodice-1.0.0.dev2/autodice.egg-info/dependency_links.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       39 2023-06-28 22:46:31.000000 autodice-1.0.0.dev2/autodice.egg-info/entry_points.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       50 2023-06-28 22:46:31.000000 autodice-1.0.0.dev2/autodice.egg-info/requires.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       18 2023-06-28 22:46:31.000000 autodice-1.0.0.dev2/autodice.egg-info/top_level.txt
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/codegen/
--rw-r--r--   0 sky       (1000) sky       (1000)      130 2023-06-28 20:25:54.000000 autodice-1.0.0.dev2/codegen/__init__.py
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/partition/
--rw-r--r--   0 sky       (1000) sky       (1000)      168 2023-06-28 22:11:35.000000 autodice-1.0.0.dev2/partition/__init__.py
--rw-rw-r--   0 sky       (1000) sky       (1000)    59038 2023-06-28 22:44:59.000000 autodice-1.0.0.dev2/partition/dice.py
--rw-rw-r--   0 sky       (1000) sky       (1000)      230 2022-12-01 16:53:46.000000 autodice-1.0.0.dev2/pyproject.toml
--rw-rw-r--   0 sky       (1000) sky       (1000)       78 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/setup.cfg
--rw-rw-r--   0 sky       (1000) sky       (1000)     7990 2023-06-28 22:45:46.000000 autodice-1.0.0.dev2/setup.py
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-28 22:46:31.467894 autodice-1.0.0.dev2/tests/
--rw-rw-r--   0 sky       (1000) sky       (1000)      417 2022-12-01 16:53:46.000000 autodice-1.0.0.dev2/tests/test_simple.py
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:01:36.343886 autodice-1.0.1.dev1/
+-rw-rw-r--   0 sky       (1000) sky       (1000)     1081 2022-12-01 16:53:46.000000 autodice-1.0.1.dev1/LICENSE.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)     3556 2023-06-29 15:01:36.343886 autodice-1.0.1.dev1/PKG-INFO
+-rw-rw-r--   0 sky       (1000) sky       (1000)     2420 2023-06-29 14:22:44.000000 autodice-1.0.1.dev1/README.md
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:01:36.343886 autodice-1.0.1.dev1/autodice.egg-info/
+-rw-rw-r--   0 sky       (1000) sky       (1000)     3556 2023-06-29 15:01:36.000000 autodice-1.0.1.dev1/autodice.egg-info/PKG-INFO
+-rw-rw-r--   0 sky       (1000) sky       (1000)      361 2023-06-29 15:01:36.000000 autodice-1.0.1.dev1/autodice.egg-info/SOURCES.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)        1 2023-06-29 15:01:36.000000 autodice-1.0.1.dev1/autodice.egg-info/dependency_links.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       39 2023-06-29 15:01:36.000000 autodice-1.0.1.dev1/autodice.egg-info/entry_points.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       50 2023-06-29 15:01:36.000000 autodice-1.0.1.dev1/autodice.egg-info/requires.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       10 2023-06-29 15:01:36.000000 autodice-1.0.1.dev1/autodice.egg-info/top_level.txt
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:01:36.343886 autodice-1.0.1.dev1/partition/
+-rw-r--r--   0 sky       (1000) sky       (1000)      192 2023-06-29 14:59:51.000000 autodice-1.0.1.dev1/partition/__init__.py
+-rwxrwxr-x   0 sky       (1000) sky       (1000)     5290 2022-08-01 20:47:57.000000 autodice-1.0.1.dev1/partition/code_generator.py
+-rw-rw-r--   0 sky       (1000) sky       (1000)    44651 2023-06-29 14:19:33.000000 autodice-1.0.1.dev1/partition/dice.py
+-rwxrwxr-x   0 sky       (1000) sky       (1000)    46791 2023-06-29 14:45:33.000000 autodice-1.0.1.dev1/partition/interface.py
+-rw-rw-r--   0 sky       (1000) sky       (1000)      230 2022-12-01 16:53:46.000000 autodice-1.0.1.dev1/pyproject.toml
+-rw-rw-r--   0 sky       (1000) sky       (1000)       78 2023-06-29 15:01:36.343886 autodice-1.0.1.dev1/setup.cfg
+-rw-rw-r--   0 sky       (1000) sky       (1000)     7990 2023-06-29 15:01:26.000000 autodice-1.0.1.dev1/setup.py
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 15:01:36.343886 autodice-1.0.1.dev1/tests/
+-rw-rw-r--   0 sky       (1000) sky       (1000)      417 2022-12-01 16:53:46.000000 autodice-1.0.1.dev1/tests/test_simple.py
```

### Comparing `autodice-1.0.0.dev2/LICENSE.txt` & `autodice-1.0.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autodice-1.0.0.dev2/partition/dice.py` & `autodice-1.0.1.dev1/partition/dice.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import onnx
 import numpy as np
- 
+import json
+
 def format_onnx(input_model):
     # Load an ONNX model from the given path and assign names if not provided or invalid.
 
     model = onnx.load(input_model)
     model = onnx.shape_inference.infer_shapes(model)
     graph = model.graph
     for init_i in range(len(graph.initializer)):
@@ -194,113 +195,14 @@
                         # trace input node's inputs 
                         node_input_names = traceUpNodes(graph,ninput,node_input_names,node_map, start_index, initializer_map)                                        
     # don't forget the initializers they can be terminal inputs on a path.                    
     if name in initializer_map.keys():
         node_input_names.append(name)                    
     return node_input_names    
 
-#         """ edits and modifies an onnx model to extract a subgraph based on input/output node names and shapes.
-#     Arguments:
-#         input_model: path of input onnx model
-#         output_model: path base of output onnx model
-#         input_names_list: list of input_name.
-
-#     """
-def extract_subgraph(graph, subgraph, sub_nodes):
-    input_tensors = getInputlayers(graph)
-    input_map = generate_node_dict(graph.input)
-    output_map = generate_node_dict(graph.output)
-    initializer_map = generate_node_dict(graph.initializer)
-    value_map = generate_node_dict(graph.value_info)
-    node_map = generate_node_dict(graph.node)
-
-    sub_node_names = [n for n in list(node_map) if n in sub_node_names_list]
-    #  找出节点名称
-
-    input_names = []
-    output_names =[]
-    # GET ALL INPUT NAMES (including weights)
-    for node in sub_node_names:
-        for input_name in node_map[node].input:
-            input_names.append(input_name)
-
-    # GET ALL OUTPUT NAMES (including weights)
-    for node in sub_node_names:
-        for output_name in node_map[node].output:
-            output_names.append(output_name)
-
-    #print (output_names)
-    # needs to be topology sorted.
-    graph_node_names = [n for n in list(node_map) if n in sub_node_names]
-    input_node_names = [n for n in list(input_map) if n in input_names]
-    output_node_names = [n for n in list(output_map) if n in output_names]
-    print (input_node_names)
-
-    [removed_names,retained_names]=split_name_list(graph.input, input_node_names)
-
-
-    for name in removed_names:
-        if name in input_map.keys():
-            graph.input.remove(input_map[name])
-
-    [removed_names,retained_names]=split_name_list(graph.output, output_names)
-    for name in removed_names:
-        if name in output_map.keys():
-            graph.output.remove(output_map[name])
-
-    valid_node_names = set(graph_node_names) | set(input_node_names)
-
-
-    #print (valid_node_names)
-    invalid_node_names = list( (set(node_map.keys()) | set(initializer_map.keys())) - set(valid_node_names))
-    print ("invalid-----")
-    print (invalid_node_names)
-    #print ("invalid_node names: ", invalid_node_names)
-
-    #removed_node_names = [n for n in node_map.keys() if n in invalid_node_names]
-    #print ("removed_node: ", removed_node_names)
-
-    # Remove all the invalid nodes from the graph
-    for name in invalid_node_names:
-        if name in initializer_map.keys():
-            graph.initializer.remove(initializer_map[name])
-        #if name in input_map.keys():
-        #    graph.input.remove(input_map[name])
-        if name in node_map.keys():
-            graph.node.remove(node_map[name])
-
-    #print ("invalid node names: ", invalid_node_names)
-    new_node_map = generate_node_dict(graph.node)
-    new_input_map = generate_node_dict(graph.input)
-    new_output_map = generate_node_dict(graph.output)
-    new_initializer_map = generate_node_dict(graph.initializer)
-    new_value_map = generate_node_dict(graph.value_info)
-    new_input_all= []
-
-
-
-    for n in graph.node:
-        for input_name in n.input:
-            new_input_all.append(input_name)
-    new_input_all = set(new_input_all)
-    extra_tensor = list(set(new_input_all) - (set(new_node_map.keys()) | set(new_initializer_map.keys())))
-    #print ("need input tensor: ", extra_tensor)
-    extra_tensor = list(set(extra_tensor) - set(input_tensors))
-    for per_tensor in extra_tensor:
-        try:
-            new_tensor_input = onnx.helper.make_tensor_value_info(per_tensor,
-                               onnx.TensorProto.FLOAT,get_node_output_shape(value_map[per_tensor]))
-        except:
-            new_tensor_input = onnx.helper.make_tensor_value_info(per_tensor,
-                               onnx.TensorProto.FLOAT,[1])
-        graph.input.extend([new_tensor_input])
-
-    subgraph = graph
-
-
 def onnx_extract(input_model, output_model, sub_node_names_list):
     model = onnx.load(input_model)
     #model = onnx.shape_inference.infer_shapes(model)
     graph = model.graph
 
    ## print("Check input model Errors: ", onnx.checker.check_model(model))
 
@@ -348,36 +250,31 @@
     for name in removed_names:
         if name in output_map.keys():
             graph.output.remove(output_map[name])
 
     valid_node_names = set(graph_node_names) | set(input_node_names)
 
 
-    #print (valid_node_names)
     invalid_node_names = list( (set(node_map.keys()) | set(initializer_map.keys())) - set(valid_node_names))
-    #print ("invalid_node names: ", invalid_node_names)
-
-    #removed_node_names = [n for n in node_map.keys() if n in invalid_node_names]
-    #print ("removed_node: ", removed_node_names)
 
     # Remove all the invalid nodes from the graph
     for name in invalid_node_names:
         if name in initializer_map.keys():
             graph.initializer.remove(initializer_map[name])
         #if name in input_map.keys():
         #    graph.input.remove(input_map[name])
         if name in node_map.keys():
             graph.node.remove(node_map[name])
 
     #print ("invalid node names: ", invalid_node_names)
     new_node_map = generate_node_dict(graph.node)
-    new_input_map = generate_node_dict(graph.input)
-    new_output_map = generate_node_dict(graph.output)
+
+
     new_initializer_map = generate_node_dict(graph.initializer)
-    new_value_map = generate_node_dict(graph.value_info)
+
     new_input_all = []
     new_output_all = []
 
 
     for n in graph.node:
         for input_name in n.input:
             new_input_all.append(input_name)
@@ -395,200 +292,17 @@
         graph.input.extend([new_tensor_input])
 
     for n in graph.node:
         for output_name in n.output:
             new_output_all.append(output_name)
     new_output_all = set(new_output_all)
 
-    #print("New Output Model", str(output_model), " Generated. Errors: ", onnx.checker.check_model(model))
-    model = helper.make_model(graph, producer_name='AutoDiCE') 
+    model = onnx.helper.make_model(graph, producer_name='AutoDiCE') 
     onnx.save(model, output_model)
 
-def onnx_split(input_model, output_model, split):
-    """ edits and modifies an onnx model to extract a subgraph based on input/output node names and shapes.
-    Arguments: 
-        input_model: path of input onnx model
-        output_model: path base of output onnx model    
-        split: "split.txt", definition of partition.
-        ###根据split.txt的分割点分割模型并产生mapping文件.
-        
-    """
-        
-    # LOAD MODEL AND PREP MAPS
-    model = onnx.load(input_model)
-    #model = onnx.shape_inference.infer_shapes(model)
-
-    graph = model.graph
-    
-    #print(" Check input model Errors: ", onnx.checker.check_model(model))
-    
-    #Generate a name for all node if they have none.
-    nodeIdx = 0;
-    for n in graph.node:
-        if n.name == '':
-            n.name = str(n.output[0])
-    
-    node_map = generate_node_dict(graph.node)
-    input_map = generate_node_dict(graph.input)
-    output_map = generate_node_dict(graph.output)
-    initializer_map = generate_node_dict(graph.initializer)
-    value_map = generate_node_dict(graph.value_info)
-    origin_node_names = list(node_map)
-    origin_input_node_names = list(input_map)
-    origin_output_node_names = list(output_map)
-    
-    origin_input_initializer =  list(initializer_map)
-    net_input = list(set(origin_input_node_names)  - set(origin_input_initializer))
-    
-    #print (net_input, origin_output_node_names)
-    split_definition = []
-    position_definition=[]
-
-    sender_dict = {}
-    
-    with open(split, 'r') as f:
-        temp = f.readlines()
-        for i in temp:
-            split_definition.append(i.rstrip('\n'))
-        position_definition = split_definition[1].split(',')
-        for i in range(len(position_definition)):
-            position_definition[i] = position_definition[i].replace(' ','')
-    position_definition.append(origin_output_node_names[0])
-
-
-    if split_definition[0] == 'vertical':
-        print ("Vertical Partition!")
-    
-    #print (position_definition)
-    
-    parts = 0
-    split_parts = []
-    start_index = 0
-    part_index = 0
-
-
-    mapping_file = 'mapping.json'
-    mapping_dict = {}
-    mapping_dict_list = {}
-    jsonFile = open(mapping_file, "w")
-
-    
-    for n in graph.node:
-        if n.name in position_definition:       
-            output_path = output_model+"/export" + str(parts) +".onnx"
-            model = onnx.load(input_model)
-            model = onnx.shape_inference.infer_shapes(model)
-
-            graph = model.graph
-            for n in graph.node:
-                if n.name == '':
-                    n.name = str(n.output[0])
-            node_map = generate_node_dict(graph.node)
-            input_map = generate_node_dict(graph.input)
-            output_map = generate_node_dict(graph.output)
-            initializer_map = generate_node_dict(graph.initializer)
-            value_map = generate_node_dict(graph.value_info)
-            
-            input_names = []
-            output_names = []
-            graph_node_names = []
-  
-            for i in range(start_index, part_index+1):
-                graph_node_names.append(graph.node[i].name)
-                for input_name in graph.node[i].input:
-                    input_names.append(input_name)
-            for output_name in graph.node[part_index].output:
-                output_names.append(output_name)
-    
-            input_node_names = set(input_names)
-            output_node_names = set(output_names)
-            graph_node_names = set(graph_node_names)
-            # needs to be topology sorted.
-            input_node_names = [n for n in origin_input_node_names if n in input_node_names]
-            graph_node_names = [n for n in origin_node_names if n in graph_node_names]
-            [removed_names,retained_names]=split_name_list(graph.input,input_node_names)
-
-            for name in removed_names:
-                if name in input_map.keys():
-                    graph.input.remove(input_map[name])  
-           
-            #input_map = generate_node_dict(graph.input)   
-            # MODIFY OUTPUTS
-            
-            [removed_names,retained_names]=split_name_list(graph.output,output_node_names)
-            for name in removed_names:
-                if name in output_map.keys():
-                    graph.output.remove(output_map[name])  
-            output_map = generate_node_dict(graph.output)      
-
-            valid_node_names = set(graph_node_names) |set(input_node_names) 
-            
-                    #for output_node_name in output_node_names:
-            #    valid_node_names=traceUpNodes(graph,output_node_name,
-            #                                 valid_node_names,node_map, start_index, initializer_map)
-            #valid_node_names = list(input_node_names)
-            #valid_node_names = set(valid_node_names)
-            print ("-----------")
-
-            #print ("valide_node names: ", valid_node_names)
-            
-            invalid_node_names = list( (set(node_map.keys()) | set(initializer_map.keys())) - set(valid_node_names))
-            #print ("invalide_node names: ", invalid_node_names)
-            
-            
-            removed_node_names = [n for n in node_map.keys() if n in invalid_node_names]
-            #print ("removed_node: ", removed_node_names)
-            
-            
-            # Remove all the invalid nodes from the graph               
-            for name in invalid_node_names:       
-                if name in initializer_map.keys():
-                    graph.initializer.remove(initializer_map[name])
-                #if name in input_map.keys():
-                #    graph.input.remove(input_map[name])  
-                if name in node_map.keys():
-                    graph.node.remove(node_map[name]) 
-                #if name in value_map.keys():
-                #    graph.value_info.remove(value_map[name])  
-            
-            new_node_map = generate_node_dict(graph.node)
-            new_input_map = generate_node_dict(graph.input)
-            new_output_map = generate_node_dict(graph.output)
-            new_initializer_map = generate_node_dict(graph.initializer)
-            new_value_map = generate_node_dict(graph.value_info)
-            new_input_all= []
-            for i in graph.node:
-                for input_name in i.input:
-                    new_input_all.append(input_name)
-            new_input_all = set(new_input_all)
-            extra_tensor = list(set(new_input_all) - (set(new_node_map.keys()) | set(new_initializer_map.keys())))
-            #print ("need input tensor: ", extra_tensor)
-            if parts > 0:
-                for per_tensor in extra_tensor:
-                    new_tensor_input = onnx.helper.make_tensor_value_info(per_tensor,
-                                           onnx.TensorProto.FLOAT,get_node_output_shape(value_map[per_tensor]))
-                    graph.input.extend([new_tensor_input])
-            #print("Output Model ",parts, " Generated. Errors: ", onnx.checker.check_model(model))
-            mapping_dict = {}
-            mapping_dict["export"+str(parts) +".onnx"] = list(new_node_map)            
-            new_mapping_dict = copy.copy(mapping_dict)
-            #mapping_dict_list.append(new_mapping_dict)
-            mapping_dict_list["export"+str(parts) +".onnx"] = list(new_node_map)
-
-            onnx.save(model, output_path)
-            parts += 1
-            start_index = part_index + 1
-        part_index += 1  
-        
-    mapping_content = json.dumps(mapping_dict_list)
-    jsonFile.write(mapping_content)
-    jsonFile.close()
-    print ("Generate ", parts, " models.")
-        # SAVE MODEL
-
 
 def horizontal_split(graph, splitnode_name, split_ranks, split_axis, split_points):
     # split_ranks : record all ranks(node) for distributing horizontally.
     # split_axis: (-1), LOP split. (0) split channel (1) Split Height (2) Split Width.
     # split_points: (-1) output channels split (0) input channel split. (1&2) output height width split.
     # e.g.:
     # split_axis = 1   means split the input data from the height dimension.
@@ -1211,73 +925,26 @@
     if nodeIdx>=0:
         graph.node.remove(node_map[splitnode_name])    
 
 
     #onnx.save(model, output_model)
     return graph
     
-
-
-
-class ONNXPartiton:
-    def __init__(self, input_model):
-        self.input_model = input_model
-        self.graph = self.load_model(input_model)
-        self.node_map = self.generate_node_dict(self.graph.node)
-        self.initializer_map = self.generate_node_dict(self.graph.initializer)
-        self.input_map = self.generate_node_dict(self.graph.input)
-        self.output_map = self.generate_node_dict(self.graph.output)
-
-    def load_model(self, model_path):
-        model = onnx.load(model_path)
-        graph = model.graph
-        for n in graph.node:
-            if n.name == '':
-                n.name = str(n.output[0])
-        return graph
-
-    def save_model(self, model, model_path):
-        onnx.save(model, model_path)
-
-    def generate_node_dict(self, graph_member_list):
-        member_map = {n.name: n for n in graph_member_list}
-        return member_map
-
-    def trace_up_nodes(self, name, node_input_names, start_index):
-        for n in self.graph.node[start_index:]:
-            for noutput in n.output:
-                if (noutput == name) and (n.name not in node_input_names):
-                    node_input_names.append(n.name)
-                    if n.name in self.node_map.keys():
-                        for ninput in self.node_map[n.name].input:
-                            node_input_names = self.trace_up_nodes(ninput, node_input_names, start_index)
-        if name in self.initializer_map.keys():
-            node_input_names.append(name)
-        return node_input_names
-
-    def split_name_list(self, name_list, new_names_all):
-        removed_names = [n.name for n in name_list if n.name not in new_names_all]
-        retained_names = [n.name for n in name_list if n.name in new_names_all]
-        return removed_names, retained_names
-
  
-    def get_node_output_shape(self, node_value_info):
-        shape = [i.dim_value for i in node_value_info.type.tensor_type.shape.dim]
-        return shape
-
-    def create_initializer_tensor(self, name, tensor_array, data_type=onnx.TensorProto.FLOAT):
-        tensor = onnx.helper.make_tensor(name=name, data_type=data_type, dims=tensor_array.shape, vals=tensor_array.flatten().tolist())
-        return tensor
-
-
-    def extract_subgraph(self, subgraph, sub_nodes):
-        subgraph.input.extend([self.input_map[name] for name in sub_nodes if name in self.input_map])
-        subgraph.output.extend([self.output_map[name] for name in sub_nodes if name in self.output_map])
-        subgraph.node.extend([self.node_map[name] for name in sub_nodes if name in self.node_map])
-        subgraph.initializer.extend([self.initializer_map[name] for name in sub_nodes if name in self.initializer_map])
-
-    def onnx_extract(self, output_model, sub_node_names_list):
-        model = onnx.load(self.input_model)
-        subgraph = onnx.helper.make_graph([], "subgraph", [], [])
-        self.extract_subgraph(subgraph, sub_node_names_list)
-        model.graph.CopyFrom(subgraph)
-        self.save_model(model, output_model)
+def save_json(vod ,output_file):
+    movie_content = json.dumps(vod)
+    jsonFile = open(output_file, "w")
+    jsonFile.write(movie_content)
+    jsonFile.close()
+    #print (str(output_file)+".json saved.")
+
+def print_json(input_file):
+    fileObject = open(input_file, "r")
+    jsonContent = fileObject.read()
+    vod = json.loads(jsonContent)
+    print (vod)
+
+def load_json(input_file):
+    fileObject = open(input_file, "r")
+    jsonContent = fileObject.read()
+    vod = json.loads(jsonContent)
+    return vod
```

### Comparing `autodice-1.0.0.dev2/setup.py` & `autodice-1.0.1.dev1/setup.py`

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
-    version="1.0.0.dev2",  # Required
+    version="1.0.1.dev1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Automated Distributed CNN inference at the Edge",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

