# Comparing `tmp/blight-0.0.53a1.tar.gz` & `tmp/blight-0.0.53a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blight-0.0.53a1.tar", last modified: Tue Mar 14 21:15:54 2023, max compression
+gzip compressed data, was "blight-0.0.53a2.tar", last modified: Thu Mar 16 14:21:41 2023, max compression
```

## Comparing `blight-0.0.53a1.tar` & `blight-0.0.53a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11358 2023-03-14 21:15:46.688208 blight-0.0.53a1/LICENSE
--rw-r--r--   0        0        0    11235 2023-03-14 21:15:46.688208 blight-0.0.53a1/README.md
--rw-r--r--   0        0        0     2010 2023-03-14 21:15:46.688208 blight-0.0.53a1/pyproject.toml
--rw-r--r--   0        0        0       58 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/__init__.py
--rw-r--r--   0        0        0     6338 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/_cli.py
--rw-r--r--   0        0        0     3391 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/action.py
--rw-r--r--   0        0        0      622 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/__init__.py
--rw-r--r--   0        0        0     1448 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/benchmark.py
--rw-r--r--   0        0        0     1733 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/cc_for_cxx.py
--rw-r--r--   0        0        0      397 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/demo.py
--rw-r--r--   0        0        0      951 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/embed_bitcode.py
--rw-r--r--   0        0        0     2896 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/find_inputs.py
--rw-r--r--   0        0        0     5491 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/find_outputs.py
--rw-r--r--   0        0        0     1228 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/ignore_flags.py
--rw-r--r--   0        0        0      954 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/ignore_flto.py
--rw-r--r--   0        0        0     1047 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/ignore_werror.py
--rw-r--r--   0        0        0     2302 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/inject_flags.py
--rw-r--r--   0        0        0      919 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/record.py
--rw-r--r--   0        0        0      538 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/actions/skip_strip.py
--rw-r--r--   0        0        0     1778 2023-03-14 21:15:46.688208 blight-0.0.53a1/src/blight/constants.py
--rw-r--r--   0        0        0    11077 2023-03-14 21:15:46.692208 blight-0.0.53a1/src/blight/enums.py
--rw-r--r--   0        0        0      423 2023-03-14 21:15:46.692208 blight-0.0.53a1/src/blight/exceptions.py
--rw-r--r--   0        0        0      917 2023-03-14 21:15:46.692208 blight-0.0.53a1/src/blight/protocols.py
--rw-r--r--   0        0        0    38463 2023-03-14 21:15:46.692208 blight-0.0.53a1/src/blight/tool.py
--rw-r--r--   0        0        0     8821 2023-03-14 21:15:46.692208 blight-0.0.53a1/src/blight/util.py
--rw-r--r--   0        0        0    12366 1970-01-01 00:00:00.000000 blight-0.0.53a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-16 14:21:29.988534 blight-0.0.53a2/LICENSE
+-rw-r--r--   0        0        0    11235 2023-03-16 14:21:29.992534 blight-0.0.53a2/README.md
+-rw-r--r--   0        0        0     2010 2023-03-16 14:21:29.992534 blight-0.0.53a2/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/__init__.py
+-rw-r--r--   0        0        0     6338 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/_cli.py
+-rw-r--r--   0        0        0     3391 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/action.py
+-rw-r--r--   0        0        0      622 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/__init__.py
+-rw-r--r--   0        0        0     1448 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/benchmark.py
+-rw-r--r--   0        0        0     1733 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/cc_for_cxx.py
+-rw-r--r--   0        0        0      397 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/demo.py
+-rw-r--r--   0        0        0      951 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/embed_bitcode.py
+-rw-r--r--   0        0        0     2896 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/find_inputs.py
+-rw-r--r--   0        0        0     5491 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/find_outputs.py
+-rw-r--r--   0        0        0     1228 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/ignore_flags.py
+-rw-r--r--   0        0        0      954 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/ignore_flto.py
+-rw-r--r--   0        0        0     1047 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/ignore_werror.py
+-rw-r--r--   0        0        0     2302 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/inject_flags.py
+-rw-r--r--   0        0        0      919 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/record.py
+-rw-r--r--   0        0        0      538 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/actions/skip_strip.py
+-rw-r--r--   0        0        0     1778 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/constants.py
+-rw-r--r--   0        0        0    11077 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/enums.py
+-rw-r--r--   0        0        0      423 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/exceptions.py
+-rw-r--r--   0        0        0      917 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/protocols.py
+-rw-r--r--   0        0        0    38463 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/tool.py
+-rw-r--r--   0        0        0     8821 2023-03-16 14:21:29.992534 blight-0.0.53a2/src/blight/util.py
+-rw-r--r--   0        0        0    12366 1970-01-01 00:00:00.000000 blight-0.0.53a2/PKG-INFO
```

### Comparing `blight-0.0.53a1/LICENSE` & `blight-0.0.53a2/LICENSE`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/README.md` & `blight-0.0.53a2/README.md`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/pyproject.toml` & `blight-0.0.53a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/_cli.py` & `blight-0.0.53a2/src/blight/_cli.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/action.py` & `blight-0.0.53a2/src/blight/action.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/__init__.py` & `blight-0.0.53a2/src/blight/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/benchmark.py` & `blight-0.0.53a2/src/blight/actions/benchmark.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/cc_for_cxx.py` & `blight-0.0.53a2/src/blight/actions/cc_for_cxx.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/embed_bitcode.py` & `blight-0.0.53a2/src/blight/actions/embed_bitcode.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/find_inputs.py` & `blight-0.0.53a2/src/blight/actions/find_inputs.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/find_outputs.py` & `blight-0.0.53a2/src/blight/actions/find_outputs.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/ignore_flags.py` & `blight-0.0.53a2/src/blight/actions/ignore_flags.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/ignore_flto.py` & `blight-0.0.53a2/src/blight/actions/ignore_flto.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/ignore_werror.py` & `blight-0.0.53a2/src/blight/actions/ignore_werror.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/inject_flags.py` & `blight-0.0.53a2/src/blight/actions/inject_flags.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/record.py` & `blight-0.0.53a2/src/blight/actions/record.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/actions/skip_strip.py` & `blight-0.0.53a2/src/blight/actions/skip_strip.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/constants.py` & `blight-0.0.53a2/src/blight/constants.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/enums.py` & `blight-0.0.53a2/src/blight/enums.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/protocols.py` & `blight-0.0.53a2/src/blight/protocols.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/tool.py` & `blight-0.0.53a2/src/blight/tool.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/src/blight/util.py` & `blight-0.0.53a2/src/blight/util.py`

 * *Files identical despite different names*

### Comparing `blight-0.0.53a1/PKG-INFO` & `blight-0.0.53a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blight
-Version: 0.0.53a1
+Version: 0.0.53a2
 Summary: A catch-all compile-tool wrapper
 Author-email: William Woodruff <william@trailofbits.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
```

