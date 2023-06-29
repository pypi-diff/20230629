# Comparing `tmp/istruthy-0.11.tar.gz` & `tmp/istruthy-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istruthy-0.11.tar", last modified: Thu Jun 29 20:04:35 2023, max compression
+gzip compressed data, was "istruthy-0.12.tar", last modified: Thu Jun 29 20:27:05 2023, max compression
```

## Comparing `istruthy-0.11.tar` & `istruthy-0.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:04:35.984889 istruthy-0.11/
--rw-rw-rw-   0        0        0     1148 2023-06-29 20:04:31.000000 istruthy-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0       95 2023-06-29 20:04:30.000000 istruthy-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     6942 2023-06-29 20:04:35.985887 istruthy-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     6219 2023-06-29 20:04:09.000000 istruthy-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:04:35.981897 istruthy-0.11/istruthy/
--rw-rw-rw-   0        0        0     6219 2023-06-29 20:04:09.000000 istruthy-0.11/istruthy/README.MD
--rw-rw-rw-   0        0        0      949 2023-06-29 19:56:27.000000 istruthy-0.11/istruthy/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-06-29 20:04:35.984889 istruthy-0.11/istruthy.egg-info/
--rw-rw-rw-   0        0        0     6942 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-29 20:04:35.985887 istruthy-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-29 20:04:35.000000 istruthy-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:27:05.493774 istruthy-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-06-29 20:26:58.000000 istruthy-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0       95 2023-06-29 20:26:57.000000 istruthy-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     6910 2023-06-29 20:27:05.493774 istruthy-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     6187 2023-06-29 20:25:56.000000 istruthy-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:27:05.490781 istruthy-0.12/istruthy/
+-rw-rw-rw-   0        0        0     6187 2023-06-29 20:25:56.000000 istruthy-0.12/istruthy/README.MD
+-rw-rw-rw-   0        0        0      948 2023-06-29 20:25:34.000000 istruthy-0.12/istruthy/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 20:27:04.000000 istruthy-0.12/istruthy/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 20:27:04.000000 istruthy-0.12/istruthy/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-29 20:27:05.492776 istruthy-0.12/istruthy.egg-info/
+-rw-rw-rw-   0        0        0     6910 2023-06-29 20:27:05.000000 istruthy-0.12/istruthy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-29 20:27:05.000000 istruthy-0.12/istruthy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:27:05.000000 istruthy-0.12/istruthy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 20:27:05.000000 istruthy-0.12/istruthy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-29 20:27:05.494771 istruthy-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2023-06-29 20:27:04.000000 istruthy-0.12/setup.py
```

### Comparing `istruthy-0.11/LICENSE.rst` & `istruthy-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `istruthy-0.11/PKG-INFO` & `istruthy-0.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istruthy
-Version: 0.11
+Version: 0.12
 Summary: extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 Home-page: https://github.com/hansalemaos/istruthy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numpy,pandas,truthy,falsy
 Classifier: Development Status :: 4 - Beta
@@ -49,139 +49,139 @@
 empty_byte = b""
 empty_bytearray = bytearray(b"")
 empty_set = set()
 empty_np_array = np.array([])
 
 if not v_bool:
     print(f"1) {v_bool} is falsy")
-    if not is_truthty(v_bool):
+    if not is_truthy(v_bool):
         print(f"2) {v_bool} is falsy")
 else:
     print(f"1) {v_bool} is truthy")
-    if is_truthty(v_bool):
+    if is_truthy(v_bool):
         print(f"2) {v_bool} is truthy")
 if not v_none:
     print(f"1) {v_none} is falsy")
-    if not is_truthty(v_none):
+    if not is_truthy(v_none):
         print(f"2) {v_none} is falsy")
 else:
     print(f"1) {v_none} is truthy")
-    if is_truthty(v_none):
+    if is_truthy(v_none):
         print(f"2) {v_none} is truthy")
 if not v_0_0:
     print(f"1) {v_0_0} is falsy")
-    if not is_truthty(v_0_0):
+    if not is_truthy(v_0_0):
         print(f"2) {v_0_0} is falsy")
 else:
     print(f"1) {v_0_0} is truthy")
-    if is_truthty(v_0_0):
+    if is_truthy(v_0_0):
         print(f"2) {v_0_0} is truthy")
 if not v_0_1:
     print(f"1) {v_0_1} is falsy")
-    if not is_truthty(v_0_1):
+    if not is_truthy(v_0_1):
         print(f"2) {v_0_1} is falsy")
 else:
     print(f"1) {v_0_1} is truthy")
-    if is_truthty(v_0_1):
+    if is_truthy(v_0_1):
         print(f"2) {v_0_1} is truthy")
 if not v_0_2:
     print(f"1) {v_0_2} is falsy")
-    if not is_truthty(v_0_2):
+    if not is_truthy(v_0_2):
         print(f"2) {v_0_2} is falsy")
 else:
     print(f"1) {v_0_2} is truthy")
-    if is_truthty(v_0_2):
+    if is_truthy(v_0_2):
         print(f"2) {v_0_2} is truthy")
 if not empty_list:
     print(f"1) {empty_list} is falsy")
-    if not is_truthty(empty_list):
+    if not is_truthy(empty_list):
         print(f"2) {empty_list} is falsy")
 else:
     print(f"1) {empty_list} is truthy")
-    if is_truthty(empty_list):
+    if is_truthy(empty_list):
         print(f"2) {empty_list} is truthy")
 if not empty_tuple:
     print(f"1) {empty_tuple} is falsy")
-    if not is_truthty(empty_tuple):
+    if not is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is falsy")
 else:
     print(f"1) {empty_tuple} is truthy")
-    if is_truthty(empty_tuple):
+    if is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is truthy")
 if not empty_dict:
     print(f"1) {empty_dict} is falsy")
-    if not is_truthty(empty_dict):
+    if not is_truthy(empty_dict):
         print(f"2) {empty_dict} is falsy")
 else:
     print(f"1) {empty_dict} is truthy")
-    if is_truthty(empty_dict):
+    if is_truthy(empty_dict):
         print(f"2) {empty_dict} is truthy")
 if not empty_string:
     print(f"1) {empty_string} is falsy")
-    if not is_truthty(empty_string):
+    if not is_truthy(empty_string):
         print(f"2) {empty_string} is falsy")
 else:
     print(f"1) {empty_string} is truthy")
-    if is_truthty(empty_string):
+    if is_truthy(empty_string):
         print(f"2) {empty_string} is truthy")
 if not empty_byte:
     print(f"1) {empty_byte} is falsy")
-    if not is_truthty(empty_byte):
+    if not is_truthy(empty_byte):
         print(f"2) {empty_byte} is falsy")
 else:
     print(f"1) {empty_byte} is truthy")
-    if is_truthty(empty_byte):
+    if is_truthy(empty_byte):
         print(f"2) {empty_byte} is truthy")
 if not empty_bytearray:
     print(f"1) {empty_bytearray} is falsy")
-    if not is_truthty(empty_bytearray):
+    if not is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is falsy")
 else:
     print(f"1) {empty_bytearray} is truthy")
-    if is_truthty(empty_bytearray):
+    if is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is truthy")
 if not empty_set:
     print(f"1) {empty_set} is falsy")
-    if not is_truthty(empty_set):
+    if not is_truthy(empty_set):
         print(f"2) {empty_set} is falsy")
 else:
     print(f"1) {empty_set} is truthy")
-    if is_truthty(empty_set):
+    if is_truthy(empty_set):
         print(f"2) {empty_set} is truthy")
 print("----------------")
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception:
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 empty_np_array = pd.DataFrame()
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception as fe:
     print(fe)
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 
 
 
 1) False is falsy
 2) False is falsy
```

### Comparing `istruthy-0.11/README.md` & `istruthy-0.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,139 +31,139 @@
 empty_byte = b""
 empty_bytearray = bytearray(b"")
 empty_set = set()
 empty_np_array = np.array([])
 
 if not v_bool:
     print(f"1) {v_bool} is falsy")
-    if not is_truthty(v_bool):
+    if not is_truthy(v_bool):
         print(f"2) {v_bool} is falsy")
 else:
     print(f"1) {v_bool} is truthy")
-    if is_truthty(v_bool):
+    if is_truthy(v_bool):
         print(f"2) {v_bool} is truthy")
 if not v_none:
     print(f"1) {v_none} is falsy")
-    if not is_truthty(v_none):
+    if not is_truthy(v_none):
         print(f"2) {v_none} is falsy")
 else:
     print(f"1) {v_none} is truthy")
-    if is_truthty(v_none):
+    if is_truthy(v_none):
         print(f"2) {v_none} is truthy")
 if not v_0_0:
     print(f"1) {v_0_0} is falsy")
-    if not is_truthty(v_0_0):
+    if not is_truthy(v_0_0):
         print(f"2) {v_0_0} is falsy")
 else:
     print(f"1) {v_0_0} is truthy")
-    if is_truthty(v_0_0):
+    if is_truthy(v_0_0):
         print(f"2) {v_0_0} is truthy")
 if not v_0_1:
     print(f"1) {v_0_1} is falsy")
-    if not is_truthty(v_0_1):
+    if not is_truthy(v_0_1):
         print(f"2) {v_0_1} is falsy")
 else:
     print(f"1) {v_0_1} is truthy")
-    if is_truthty(v_0_1):
+    if is_truthy(v_0_1):
         print(f"2) {v_0_1} is truthy")
 if not v_0_2:
     print(f"1) {v_0_2} is falsy")
-    if not is_truthty(v_0_2):
+    if not is_truthy(v_0_2):
         print(f"2) {v_0_2} is falsy")
 else:
     print(f"1) {v_0_2} is truthy")
-    if is_truthty(v_0_2):
+    if is_truthy(v_0_2):
         print(f"2) {v_0_2} is truthy")
 if not empty_list:
     print(f"1) {empty_list} is falsy")
-    if not is_truthty(empty_list):
+    if not is_truthy(empty_list):
         print(f"2) {empty_list} is falsy")
 else:
     print(f"1) {empty_list} is truthy")
-    if is_truthty(empty_list):
+    if is_truthy(empty_list):
         print(f"2) {empty_list} is truthy")
 if not empty_tuple:
     print(f"1) {empty_tuple} is falsy")
-    if not is_truthty(empty_tuple):
+    if not is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is falsy")
 else:
     print(f"1) {empty_tuple} is truthy")
-    if is_truthty(empty_tuple):
+    if is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is truthy")
 if not empty_dict:
     print(f"1) {empty_dict} is falsy")
-    if not is_truthty(empty_dict):
+    if not is_truthy(empty_dict):
         print(f"2) {empty_dict} is falsy")
 else:
     print(f"1) {empty_dict} is truthy")
-    if is_truthty(empty_dict):
+    if is_truthy(empty_dict):
         print(f"2) {empty_dict} is truthy")
 if not empty_string:
     print(f"1) {empty_string} is falsy")
-    if not is_truthty(empty_string):
+    if not is_truthy(empty_string):
         print(f"2) {empty_string} is falsy")
 else:
     print(f"1) {empty_string} is truthy")
-    if is_truthty(empty_string):
+    if is_truthy(empty_string):
         print(f"2) {empty_string} is truthy")
 if not empty_byte:
     print(f"1) {empty_byte} is falsy")
-    if not is_truthty(empty_byte):
+    if not is_truthy(empty_byte):
         print(f"2) {empty_byte} is falsy")
 else:
     print(f"1) {empty_byte} is truthy")
-    if is_truthty(empty_byte):
+    if is_truthy(empty_byte):
         print(f"2) {empty_byte} is truthy")
 if not empty_bytearray:
     print(f"1) {empty_bytearray} is falsy")
-    if not is_truthty(empty_bytearray):
+    if not is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is falsy")
 else:
     print(f"1) {empty_bytearray} is truthy")
-    if is_truthty(empty_bytearray):
+    if is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is truthy")
 if not empty_set:
     print(f"1) {empty_set} is falsy")
-    if not is_truthty(empty_set):
+    if not is_truthy(empty_set):
         print(f"2) {empty_set} is falsy")
 else:
     print(f"1) {empty_set} is truthy")
-    if is_truthty(empty_set):
+    if is_truthy(empty_set):
         print(f"2) {empty_set} is truthy")
 print("----------------")
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception:
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 empty_np_array = pd.DataFrame()
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception as fe:
     print(fe)
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 
 
 
 1) False is falsy
 2) False is falsy
```

### Comparing `istruthy-0.11/istruthy/README.MD` & `istruthy-0.12/istruthy/README.MD`

 * *Files 10% similar despite different names*

```diff
@@ -31,139 +31,139 @@
 empty_byte = b""
 empty_bytearray = bytearray(b"")
 empty_set = set()
 empty_np_array = np.array([])
 
 if not v_bool:
     print(f"1) {v_bool} is falsy")
-    if not is_truthty(v_bool):
+    if not is_truthy(v_bool):
         print(f"2) {v_bool} is falsy")
 else:
     print(f"1) {v_bool} is truthy")
-    if is_truthty(v_bool):
+    if is_truthy(v_bool):
         print(f"2) {v_bool} is truthy")
 if not v_none:
     print(f"1) {v_none} is falsy")
-    if not is_truthty(v_none):
+    if not is_truthy(v_none):
         print(f"2) {v_none} is falsy")
 else:
     print(f"1) {v_none} is truthy")
-    if is_truthty(v_none):
+    if is_truthy(v_none):
         print(f"2) {v_none} is truthy")
 if not v_0_0:
     print(f"1) {v_0_0} is falsy")
-    if not is_truthty(v_0_0):
+    if not is_truthy(v_0_0):
         print(f"2) {v_0_0} is falsy")
 else:
     print(f"1) {v_0_0} is truthy")
-    if is_truthty(v_0_0):
+    if is_truthy(v_0_0):
         print(f"2) {v_0_0} is truthy")
 if not v_0_1:
     print(f"1) {v_0_1} is falsy")
-    if not is_truthty(v_0_1):
+    if not is_truthy(v_0_1):
         print(f"2) {v_0_1} is falsy")
 else:
     print(f"1) {v_0_1} is truthy")
-    if is_truthty(v_0_1):
+    if is_truthy(v_0_1):
         print(f"2) {v_0_1} is truthy")
 if not v_0_2:
     print(f"1) {v_0_2} is falsy")
-    if not is_truthty(v_0_2):
+    if not is_truthy(v_0_2):
         print(f"2) {v_0_2} is falsy")
 else:
     print(f"1) {v_0_2} is truthy")
-    if is_truthty(v_0_2):
+    if is_truthy(v_0_2):
         print(f"2) {v_0_2} is truthy")
 if not empty_list:
     print(f"1) {empty_list} is falsy")
-    if not is_truthty(empty_list):
+    if not is_truthy(empty_list):
         print(f"2) {empty_list} is falsy")
 else:
     print(f"1) {empty_list} is truthy")
-    if is_truthty(empty_list):
+    if is_truthy(empty_list):
         print(f"2) {empty_list} is truthy")
 if not empty_tuple:
     print(f"1) {empty_tuple} is falsy")
-    if not is_truthty(empty_tuple):
+    if not is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is falsy")
 else:
     print(f"1) {empty_tuple} is truthy")
-    if is_truthty(empty_tuple):
+    if is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is truthy")
 if not empty_dict:
     print(f"1) {empty_dict} is falsy")
-    if not is_truthty(empty_dict):
+    if not is_truthy(empty_dict):
         print(f"2) {empty_dict} is falsy")
 else:
     print(f"1) {empty_dict} is truthy")
-    if is_truthty(empty_dict):
+    if is_truthy(empty_dict):
         print(f"2) {empty_dict} is truthy")
 if not empty_string:
     print(f"1) {empty_string} is falsy")
-    if not is_truthty(empty_string):
+    if not is_truthy(empty_string):
         print(f"2) {empty_string} is falsy")
 else:
     print(f"1) {empty_string} is truthy")
-    if is_truthty(empty_string):
+    if is_truthy(empty_string):
         print(f"2) {empty_string} is truthy")
 if not empty_byte:
     print(f"1) {empty_byte} is falsy")
-    if not is_truthty(empty_byte):
+    if not is_truthy(empty_byte):
         print(f"2) {empty_byte} is falsy")
 else:
     print(f"1) {empty_byte} is truthy")
-    if is_truthty(empty_byte):
+    if is_truthy(empty_byte):
         print(f"2) {empty_byte} is truthy")
 if not empty_bytearray:
     print(f"1) {empty_bytearray} is falsy")
-    if not is_truthty(empty_bytearray):
+    if not is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is falsy")
 else:
     print(f"1) {empty_bytearray} is truthy")
-    if is_truthty(empty_bytearray):
+    if is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is truthy")
 if not empty_set:
     print(f"1) {empty_set} is falsy")
-    if not is_truthty(empty_set):
+    if not is_truthy(empty_set):
         print(f"2) {empty_set} is falsy")
 else:
     print(f"1) {empty_set} is truthy")
-    if is_truthty(empty_set):
+    if is_truthy(empty_set):
         print(f"2) {empty_set} is truthy")
 print("----------------")
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception:
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 empty_np_array = pd.DataFrame()
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception as fe:
     print(fe)
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 
 
 
 1) False is falsy
 2) False is falsy
```

### Comparing `istruthy-0.11/istruthy/__init__.py` & `istruthy-0.12/istruthy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 
-def is_truthty(x: Any, /) -> Any:
+def is_truthy(x: Any, /) -> Any:
     """
     Determines the truthiness of the given value.
     The is_truthy function can be especially useful
     when dealing with data structures like DataFrames and NumPy arrays,
     allowing you to determine their truthiness.
     It extends the capability of truthiness evaluation beyond
     the standard Python truthiness rules to handle these
```

### Comparing `istruthy-0.11/istruthy.egg-info/PKG-INFO` & `istruthy-0.12/istruthy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istruthy
-Version: 0.11
+Version: 0.12
 Summary: extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 Home-page: https://github.com/hansalemaos/istruthy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numpy,pandas,truthy,falsy
 Classifier: Development Status :: 4 - Beta
@@ -49,139 +49,139 @@
 empty_byte = b""
 empty_bytearray = bytearray(b"")
 empty_set = set()
 empty_np_array = np.array([])
 
 if not v_bool:
     print(f"1) {v_bool} is falsy")
-    if not is_truthty(v_bool):
+    if not is_truthy(v_bool):
         print(f"2) {v_bool} is falsy")
 else:
     print(f"1) {v_bool} is truthy")
-    if is_truthty(v_bool):
+    if is_truthy(v_bool):
         print(f"2) {v_bool} is truthy")
 if not v_none:
     print(f"1) {v_none} is falsy")
-    if not is_truthty(v_none):
+    if not is_truthy(v_none):
         print(f"2) {v_none} is falsy")
 else:
     print(f"1) {v_none} is truthy")
-    if is_truthty(v_none):
+    if is_truthy(v_none):
         print(f"2) {v_none} is truthy")
 if not v_0_0:
     print(f"1) {v_0_0} is falsy")
-    if not is_truthty(v_0_0):
+    if not is_truthy(v_0_0):
         print(f"2) {v_0_0} is falsy")
 else:
     print(f"1) {v_0_0} is truthy")
-    if is_truthty(v_0_0):
+    if is_truthy(v_0_0):
         print(f"2) {v_0_0} is truthy")
 if not v_0_1:
     print(f"1) {v_0_1} is falsy")
-    if not is_truthty(v_0_1):
+    if not is_truthy(v_0_1):
         print(f"2) {v_0_1} is falsy")
 else:
     print(f"1) {v_0_1} is truthy")
-    if is_truthty(v_0_1):
+    if is_truthy(v_0_1):
         print(f"2) {v_0_1} is truthy")
 if not v_0_2:
     print(f"1) {v_0_2} is falsy")
-    if not is_truthty(v_0_2):
+    if not is_truthy(v_0_2):
         print(f"2) {v_0_2} is falsy")
 else:
     print(f"1) {v_0_2} is truthy")
-    if is_truthty(v_0_2):
+    if is_truthy(v_0_2):
         print(f"2) {v_0_2} is truthy")
 if not empty_list:
     print(f"1) {empty_list} is falsy")
-    if not is_truthty(empty_list):
+    if not is_truthy(empty_list):
         print(f"2) {empty_list} is falsy")
 else:
     print(f"1) {empty_list} is truthy")
-    if is_truthty(empty_list):
+    if is_truthy(empty_list):
         print(f"2) {empty_list} is truthy")
 if not empty_tuple:
     print(f"1) {empty_tuple} is falsy")
-    if not is_truthty(empty_tuple):
+    if not is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is falsy")
 else:
     print(f"1) {empty_tuple} is truthy")
-    if is_truthty(empty_tuple):
+    if is_truthy(empty_tuple):
         print(f"2) {empty_tuple} is truthy")
 if not empty_dict:
     print(f"1) {empty_dict} is falsy")
-    if not is_truthty(empty_dict):
+    if not is_truthy(empty_dict):
         print(f"2) {empty_dict} is falsy")
 else:
     print(f"1) {empty_dict} is truthy")
-    if is_truthty(empty_dict):
+    if is_truthy(empty_dict):
         print(f"2) {empty_dict} is truthy")
 if not empty_string:
     print(f"1) {empty_string} is falsy")
-    if not is_truthty(empty_string):
+    if not is_truthy(empty_string):
         print(f"2) {empty_string} is falsy")
 else:
     print(f"1) {empty_string} is truthy")
-    if is_truthty(empty_string):
+    if is_truthy(empty_string):
         print(f"2) {empty_string} is truthy")
 if not empty_byte:
     print(f"1) {empty_byte} is falsy")
-    if not is_truthty(empty_byte):
+    if not is_truthy(empty_byte):
         print(f"2) {empty_byte} is falsy")
 else:
     print(f"1) {empty_byte} is truthy")
-    if is_truthty(empty_byte):
+    if is_truthy(empty_byte):
         print(f"2) {empty_byte} is truthy")
 if not empty_bytearray:
     print(f"1) {empty_bytearray} is falsy")
-    if not is_truthty(empty_bytearray):
+    if not is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is falsy")
 else:
     print(f"1) {empty_bytearray} is truthy")
-    if is_truthty(empty_bytearray):
+    if is_truthy(empty_bytearray):
         print(f"2) {empty_bytearray} is truthy")
 if not empty_set:
     print(f"1) {empty_set} is falsy")
-    if not is_truthty(empty_set):
+    if not is_truthy(empty_set):
         print(f"2) {empty_set} is falsy")
 else:
     print(f"1) {empty_set} is truthy")
-    if is_truthty(empty_set):
+    if is_truthy(empty_set):
         print(f"2) {empty_set} is truthy")
 print("----------------")
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception:
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 empty_np_array = pd.DataFrame()
 try:
     if not empty_np_array:
         print(f"1) {empty_np_array} is falsy")
-        if not is_truthty(empty_np_array):
+        if not is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is falsy")
     else:
         print(f"1) {empty_np_array} is truthy")
-        if is_truthty(empty_np_array):
+        if is_truthy(empty_np_array):
             print(f"2) {empty_np_array} is truthy")
 except Exception as fe:
     print(fe)
-    if not is_truthty(empty_np_array):
+    if not is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is falsy")
-    if is_truthty(empty_np_array):
+    if is_truthy(empty_np_array):
         print(f"2) {empty_np_array} is truthy")
 
 
 
 
 1) False is falsy
 2) False is falsy
```

### Comparing `istruthy-0.11/setup.py` & `istruthy-0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays'''
 
 # Setting up
 setup(
     name="istruthy",
     version=VERSION,
     license='MIT',
```

