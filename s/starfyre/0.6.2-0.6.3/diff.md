# Comparing `tmp/starfyre-0.6.2.tar.gz` & `tmp/starfyre-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.6.2.tar", max compression
+gzip compressed data, was "starfyre-0.6.3.tar", max compression
```

## Comparing `starfyre-0.6.2.tar` & `starfyre-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4382 2023-06-27 20:12:52.122850 starfyre-0.6.2/README.md
--rw-r--r--   0        0        0      454 2023-06-27 20:12:52.122850 starfyre-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      949 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/__init__.py
--rw-r--r--   0        0        0     1637 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/__main__.py
--rw-r--r--   0        0        0     4539 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/component.py
--rw-r--r--   0        0        0     3550 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/js/store.js
--rw-r--r--   0        0        0     9071 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/transpiler.py
--rw-r--r--   0        0        0     4920 1970-01-01 00:00:00.000000 starfyre-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4382 2023-06-29 18:21:17.921291 starfyre-0.6.3/README.md
+-rw-r--r--   0        0        0      454 2023-06-29 18:21:17.921291 starfyre-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      949 2023-06-29 18:21:17.921291 starfyre-0.6.3/starfyre/__init__.py
+-rw-r--r--   0        0        0     1637 2023-06-29 18:21:17.921291 starfyre-0.6.3/starfyre/__main__.py
+-rw-r--r--   0        0        0     4539 2023-06-29 18:21:17.921291 starfyre-0.6.3/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/component.py
+-rw-r--r--   0        0        0     3550 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/js/store.js
+-rw-r--r--   0        0        0     9071 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-06-29 18:21:17.925291 starfyre-0.6.3/starfyre/transpiler.py
+-rw-r--r--   0        0        0     4920 1970-01-01 00:00:00.000000 starfyre-0.6.3/PKG-INFO
```

### Comparing `starfyre-0.6.2/README.md` & `starfyre-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/__init__.py` & `starfyre-0.6.3/starfyre/__init__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/__main__.py` & `starfyre-0.6.3/starfyre/__main__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/compiler.py` & `starfyre-0.6.3/starfyre/compiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/component.py` & `starfyre-0.6.3/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/dom_methods.py` & `starfyre-0.6.3/starfyre/dom_methods.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/js/store.js` & `starfyre-0.6.3/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/parser.py` & `starfyre-0.6.3/starfyre/parser.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/starfyre/transpiler.py` & `starfyre-0.6.3/starfyre/transpiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.2/PKG-INFO` & `starfyre-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfyre
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python Framework for writing Reactive web Front-Ends
 License: BSD 2.0
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

