# Comparing `tmp/llm-lens-0.0.0.2.tar.gz` & `tmp/llm-lens-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-lens-0.0.0.2.tar", last modified: Tue Jun 20 18:40:08 2023, max compression
+gzip compressed data, was "llm-lens-0.0.0.3.tar", last modified: Thu Jun 29 06:26:57 2023, max compression
```

## Comparing `llm-lens-0.0.0.2.tar` & `llm-lens-0.0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        0 2023-06-20 18:40:08.436407 llm-lens-0.0.0.2/
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      523 2023-06-20 18:40:08.432519 llm-lens-0.0.0.2/PKG-INFO
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     9747 2023-06-20 17:36:52.000000 llm-lens-0.0.0.2/README.md
-drwxr-xr-x   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        0 2023-06-20 18:40:08.346055 llm-lens-0.0.0.2/lens/
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)       54 2023-06-20 18:36:57.000000 llm-lens-0.0.0.2/lens/__init__.py
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)    12715 2023-06-20 17:36:52.000000 llm-lens-0.0.0.2/lens/blip_captions.py
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     9927 2023-06-20 17:36:52.000000 llm-lens-0.0.0.2/lens/clip_attributes.py
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     1030 2023-06-20 17:36:53.000000 llm-lens-0.0.0.2/lens/utils.py
-drwxr-xr-x   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        0 2023-06-20 18:40:08.414653 llm-lens-0.0.0.2/llm_lens.egg-info/
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      523 2023-06-20 18:40:08.000000 llm-lens-0.0.0.2/llm_lens.egg-info/PKG-INFO
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      254 2023-06-20 18:40:08.000000 llm-lens-0.0.0.2/llm_lens.egg-info/SOURCES.txt
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        1 2023-06-20 18:40:08.000000 llm-lens-0.0.0.2/llm_lens.egg-info/dependency_links.txt
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      174 2023-06-20 18:40:08.000000 llm-lens-0.0.0.2/llm_lens.egg-info/requires.txt
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        5 2023-06-20 18:40:08.000000 llm-lens-0.0.0.2/llm_lens.egg-info/top_level.txt
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)       38 2023-06-20 18:40:08.440139 llm-lens-0.0.0.2/setup.cfg
--rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     1071 2023-06-20 18:39:52.000000 llm-lens-0.0.0.2/setup.py
+drwxr-xr-x   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        0 2023-06-29 06:26:57.375011 llm-lens-0.0.0.3/
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      523 2023-06-29 06:26:57.370669 llm-lens-0.0.0.3/PKG-INFO
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     3939 2023-06-29 04:59:18.000000 llm-lens-0.0.0.3/README.md
+drwxr-xr-x   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        0 2023-06-29 06:26:57.240077 llm-lens-0.0.0.3/lens/
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      119 2023-06-29 04:59:18.000000 llm-lens-0.0.0.3/lens/__init__.py
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)    15723 2023-06-29 04:59:18.000000 llm-lens-0.0.0.3/lens/model.py
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     4096 2023-06-29 04:59:18.000000 llm-lens-0.0.0.3/lens/utils.py
+drwxr-xr-x   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        0 2023-06-29 06:26:57.346783 llm-lens-0.0.0.3/llm_lens.egg-info/
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      523 2023-06-29 06:26:56.000000 llm-lens-0.0.0.3/llm_lens.egg-info/PKG-INFO
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      222 2023-06-29 06:26:57.000000 llm-lens-0.0.0.3/llm_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        1 2023-06-29 06:26:56.000000 llm-lens-0.0.0.3/llm_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)      174 2023-06-29 06:26:56.000000 llm-lens-0.0.0.3/llm_lens.egg-info/requires.txt
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)        5 2023-06-29 06:26:56.000000 llm-lens-0.0.0.3/llm_lens.egg-info/top_level.txt
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)       38 2023-06-29 06:26:57.380221 llm-lens-0.0.0.3/setup.cfg
+-rw-r--r--   0 tristan_contextual_ai (2022869475) tristan_contextual_ai (2022869475)     1071 2023-06-29 06:20:23.000000 llm-lens-0.0.0.3/setup.py
```

### Comparing `llm-lens-0.0.0.2/PKG-INFO` & `llm-lens-0.0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-lens
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: llm-lens is a Python package for CV as NLP, where you can run very descriptive image modules on images, and then pass those descriptions to a Large Language Model (LLM) to reason about those images.
 Home-page: https://github.com/ContextualAI/lens
 Author: The Contextual AI Tech Team
 Author-email: tech@contextual.ai
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
```

### Comparing `llm-lens-0.0.0.2/llm_lens.egg-info/PKG-INFO` & `llm-lens-0.0.0.3/llm_lens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-lens
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: llm-lens is a Python package for CV as NLP, where you can run very descriptive image modules on images, and then pass those descriptions to a Large Language Model (LLM) to reason about those images.
 Home-page: https://github.com/ContextualAI/lens
 Author: The Contextual AI Tech Team
 Author-email: tech@contextual.ai
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
```

### Comparing `llm-lens-0.0.0.2/setup.py` & `llm-lens-0.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "wandb",
     "fairscale",
     "huggingface_hub",
 ]
 
 setup(
     name="llm-lens",
-    version="0.0.0.2",
+    version="0.0.0.3",
     description=(
         "llm-lens is a Python package for CV as NLP, "
         "where you can run very descriptive image modules "
         "on images, and then pass those descriptions to a "
         "Large Language Model (LLM) to reason about those "
         "images."
     ),
```

