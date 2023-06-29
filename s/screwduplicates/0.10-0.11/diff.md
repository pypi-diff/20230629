# Comparing `tmp/screwduplicates-0.10.tar.gz` & `tmp/screwduplicates-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwduplicates-0.10.tar", last modified: Thu Jun 29 17:15:23 2023, max compression
+gzip compressed data, was "screwduplicates-0.11.tar", last modified: Thu Jun 29 18:43:39 2023, max compression
```

## Comparing `screwduplicates-0.10.tar` & `screwduplicates-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:23.258947 screwduplicates-0.10/
--rw-rw-rw-   0        0        0     1148 2023-06-29 17:15:17.000000 screwduplicates-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      116 2023-06-29 17:15:16.000000 screwduplicates-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     9860 2023-06-29 17:15:23.258947 screwduplicates-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     9140 2023-06-29 17:10:42.000000 screwduplicates-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:23.253961 screwduplicates-0.10/screwduplicates/
--rw-rw-rw-   0        0        0     9140 2023-06-29 17:10:42.000000 screwduplicates-0.10/screwduplicates/README.MD
--rw-rw-rw-   0        0        0     3630 2023-06-29 17:09:54.000000 screwduplicates-0.10/screwduplicates/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-29 17:15:20.000000 screwduplicates-0.10/screwduplicates/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 17:15:20.000000 screwduplicates-0.10/screwduplicates/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:23.257950 screwduplicates-0.10/screwduplicates.egg-info/
--rw-rw-rw-   0        0        0     9860 2023-06-29 17:15:23.000000 screwduplicates-0.10/screwduplicates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-06-29 17:15:23.000000 screwduplicates-0.10/screwduplicates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 17:15:23.000000 screwduplicates-0.10/screwduplicates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 17:15:23.000000 screwduplicates-0.10/screwduplicates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-29 17:15:23.259944 screwduplicates-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-06-29 17:15:20.000000 screwduplicates-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:43:39.842954 screwduplicates-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-29 18:43:33.000000 screwduplicates-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      116 2023-06-29 18:43:31.000000 screwduplicates-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     9648 2023-06-29 18:43:39.843945 screwduplicates-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     8928 2023-06-29 18:42:08.000000 screwduplicates-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 18:43:39.838956 screwduplicates-0.11/screwduplicates/
+-rw-rw-rw-   0        0        0     8928 2023-06-29 18:42:08.000000 screwduplicates-0.11/screwduplicates/README.MD
+-rw-rw-rw-   0        0        0     4398 2023-06-29 18:40:44.000000 screwduplicates-0.11/screwduplicates/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 18:43:38.000000 screwduplicates-0.11/screwduplicates/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 18:43:38.000000 screwduplicates-0.11/screwduplicates/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-29 18:43:39.842954 screwduplicates-0.11/screwduplicates.egg-info/
+-rw-rw-rw-   0        0        0     9648 2023-06-29 18:43:39.000000 screwduplicates-0.11/screwduplicates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-29 18:43:39.000000 screwduplicates-0.11/screwduplicates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:43:39.000000 screwduplicates-0.11/screwduplicates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 18:43:39.000000 screwduplicates-0.11/screwduplicates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-29 18:43:39.843945 screwduplicates-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-06-29 18:43:38.000000 screwduplicates-0.11/setup.py
```

### Comparing `screwduplicates-0.10/LICENSE.rst` & `screwduplicates-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `screwduplicates-0.10/PKG-INFO` & `screwduplicates-0.11/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screwduplicates
-Version: 0.10
+Version: 0.11
 Summary: provides a simple and efficient way to remove duplicates from an iterable (even with unhashable elements, optional order preservation)
 Home-page: https://github.com/hansalemaos/screwduplicates
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: remove,duplicates
 Classifier: Development Status :: 4 - Beta
@@ -43,14 +43,15 @@
 testdict = {
     "List": [5, 4, 1, 2, 2, 3, 4, 5],
     "Set": {1, 2, 3, 4, 5},
     "Tuple": (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1),
     "Dictionary": {"a": 1, "b": 2, "c": 3},
     "String": "Hello",
     "Bytes": b"Hello",
+    "Bytearray": bytearray(b"Hello"),
     "List of strings": ["Hello", "World", "Hello"],
     "List of numbers": [2.5, 3.5, 1.5, 2.5, 3.5],
     "Empty list": [],
     "Set of strings": {"apple", "banana", "cherry"},
     "Set of numbers": {1, 2, 3, 4, 5},
     "Tuple of strings": ("apple", "banana", "cherry", "banana", "banana"),
     "Tuple of numbers": (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5),
@@ -73,193 +74,197 @@
     "Tuple with repeated values": (1, 1, 1, 1, 1),
     "List with mixed types and duplicates": [1, "a", 2, "a", 3, True, 3],
     "Set with mixed types and duplicates": {1, "a", 2, "a", 3, True},
     "Tuple with mixed types and duplicates": (1, "a", 2, "a", 3, True),
     "List with empty strings": ["", "World", "World", "Hello", "World"],
     "Set with empty strings": {"", "World", "Hello", "World", "World"},
 }
-
 from screwduplicates import del_duplicates
 for key, item in testdict.items():
     print(f"\n---------------\n{key}:")
     print(f"Original: {item}")
-    print(f"dont't keep order: {del_duplicates(item,keep_order=False)}")
-    print(f"Keep order: {del_duplicates(item,keep_order=True)}")
+    print(f"dont't keep order: {del_duplicates(item, keep_order=False)}")
+    print(f"Keep order: {del_duplicates(item, keep_order=True)}")
 
+---------------
+List:
+Original: [5, 4, 1, 2, 2, 3, 4, 5]
+dont't keep order: [1, 2, 3, 4, 5]
+Keep order: [5, 4, 1, 2, 3]
+---------------
+Set:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple:
+Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (1, 3, 4, 2, 5)
+---------------
+Dictionary:
+Original: {'a': 1, 'b': 2, 'c': 3}
+dont't keep order: {'a': 1, 'b': 2, 'c': 3}
+Keep order: {'a': 1, 'b': 2, 'c': 3}
+---------------
+String:
+Original: Hello
+dont't keep order: loeH
+Keep order: Helo
+---------------
+Bytes:
+Original: b'Hello'
+dont't keep order: b'Hleo'
+Keep order: b'Helo'
+---------------
+Bytearray:
+Original: bytearray(b'Hello')
+dont't keep order: bytearray(b'Hleo')
+Keep order: bytearray(b'Helo')
+---------------
+List of strings:
+Original: ['Hello', 'World', 'Hello']
+dont't keep order: ['World', 'Hello']
+Keep order: ['Hello', 'World']
+---------------
+List of numbers:
+Original: [2.5, 3.5, 1.5, 2.5, 3.5]
+dont't keep order: [1.5, 2.5, 3.5]
+Keep order: [2.5, 3.5, 1.5]
+---------------
+Empty list:
+Original: []
+dont't keep order: []
+Keep order: []
+---------------
+Set of strings:
+Original: {'cherry', 'banana', 'apple'}
+dont't keep order: {'cherry', 'banana', 'apple'}
+Keep order: {'cherry', 'banana', 'apple'}
+---------------
+Set of numbers:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple of strings:
+Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
+dont't keep order: ('cherry', 'banana', 'apple')
+Keep order: ('apple', 'banana', 'cherry')
+---------------
+Tuple of numbers:
+Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (3, 4, 5, 1, 2)
+---------------
+Dictionary with numbers:
+Original: {1: 'one', 2: 'two', 3: 'three'}
+dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
+Keep order: {1: 'one', 2: 'two', 3: 'three'}
+---------------
+Dictionary with strings:
+Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+---------------
+List of mixed types:
+Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
+dont't keep order: [1, 2.5, 'a', 'Hello']
+Keep order: [1, 'a', 2.5, 'Hello']
+---------------
+Set of mixed types:
+Original: {1, 2.5, 'a', 'Hello'}
+dont't keep order: {1, 2.5, 'a', 'Hello'}
+Keep order: {1, 2.5, 'a', 'Hello'}
+---------------
+Tuple of mixed types:
+Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
+dont't keep order: (1, 2.5, 'a', 'Hello')
+Keep order: (1, 'a', 2.5, 'Hello')
+---------------
+Nested list:
+Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
+dont't keep order: [[1, 2], [3, 4], [5, 6]]
+Keep order: [[1, 2], [3, 4], [5, 6]]
+---------------
+Nested set:
+Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+---------------
+Nested tuple:
+Original: ((1, 2), (3, 4), (5, 6), (3, 4))
+dont't keep order: ((1, 2), (3, 4), (5, 6))
+Keep order: ((1, 2), (3, 4), (5, 6))
+---------------
+List with None value:
+Original: [1, None, 3, None, 5]
+dont't keep order: [1, 3, None, 5]
+Keep order: [1, None, 3, 5]
+---------------
+Set with None value:
+Original: {1, 3, None, 5}
+dont't keep order: {1, 3, None, 5}
+Keep order: {1, 3, None, 5}
+---------------
+Tuple with None value:
+Original: (1, None, 3, None, 5)
+dont't keep order: (1, 3, None, 5)
+Keep order: (1, None, 3, 5)
+---------------
+List with boolean values:
+Original: [True, False, True]
+dont't keep order: [False, True]
+Keep order: [True, False]
+---------------
+Set with boolean values:
+Original: {False, True}
+dont't keep order: {False, True}
+Keep order: {False, True}
+---------------
+Tuple with boolean values:
+Original: (True, False, True)
+dont't keep order: (False, True)
+Keep order: (True, False)
+---------------
+List with repeated values:
+Original: [1, 1, 1, 1, 1]
+dont't keep order: [1]
+Keep order: [1]
+---------------
+Set with repeated values:
+Original: {1}
+dont't keep order: {1}
+Keep order: {1}
+---------------
+Tuple with repeated values:
+Original: (1, 1, 1, 1, 1)
+dont't keep order: (1,)
+Keep order: (1,)
+---------------
+List with mixed types and duplicates:
+Original: [1, 'a', 2, 'a', 3, True, 3]
+dont't keep order: [3, 1, 2, 'a']
+Keep order: [True, 'a', 2, 3]
+---------------
+Set with mixed types and duplicates:
+Original: {'a', 1, 2, 3}
+dont't keep order: {'a', 1, 2, 3}
+Keep order: {'a', 1, 2, 3}
+---------------
+Tuple with mixed types and duplicates:
+Original: (1, 'a', 2, 'a', 3, True)
+dont't keep order: (3, 1, 2, 'a')
+Keep order: (True, 'a', 2, 3)
+---------------
+List with empty strings:
+Original: ['', 'World', 'World', 'Hello', 'World']
+dont't keep order: ['', 'World', 'Hello']
+Keep order: ['', 'World', 'Hello']
+---------------
+Set with empty strings:
+Original: {'', 'World', 'Hello'}
+dont't keep order: {'', 'World', 'Hello'}
+Keep order: {'', 'World', 'Hello'}
 
-# ---------------
-# List:
-# Original: [5, 4, 1, 2, 2, 3, 4, 5]
-# dont't keep order: [1, 2, 3, 4, 5]
-# Keep order: [5, 4, 1, 2, 3]
-# ---------------
-# Set:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple:
-# Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (1, 3, 4, 2, 5)
-# ---------------
-# Dictionary:
-# Original: {'a': 1, 'b': 2, 'c': 3}
-# dont't keep order: {'a': 1, 'b': 2, 'c': 3}
-# Keep order: {'a': 1, 'b': 2, 'c': 3}
-# ---------------
-# String:
-# Original: Hello
-# dont't keep order: {'H', 'o', 'l', 'e'}
-# Keep order: ['H', 'e', 'l', 'o']
-# ---------------
-# Bytes:
-# Original: b'Hello'
-# dont't keep order: b'Hleo'
-# Keep order: b'Helo'
-# ---------------
-# List of strings:
-# Original: ['Hello', 'World', 'Hello']
-# dont't keep order: ['World', 'Hello']
-# Keep order: ['Hello', 'World']
-# ---------------
-# List of numbers:
-# Original: [2.5, 3.5, 1.5, 2.5, 3.5]
-# dont't keep order: [1.5, 2.5, 3.5]
-# Keep order: [2.5, 3.5, 1.5]
-# ---------------
-# Empty list:
-# Original: []
-# dont't keep order: []
-# Keep order: []
-# ---------------
-# Set of strings:
-# Original: {'cherry', 'apple', 'banana'}
-# dont't keep order: {'cherry', 'apple', 'banana'}
-# Keep order: {'cherry', 'apple', 'banana'}
-# ---------------
-# Set of numbers:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple of strings:
-# Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
-# dont't keep order: ('cherry', 'apple', 'banana')
-# Keep order: ('apple', 'banana', 'cherry')
-# ---------------
-# Tuple of numbers:
-# Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (3, 4, 5, 1, 2)
-# ---------------
-# Dictionary with numbers:
-# Original: {1: 'one', 2: 'two', 3: 'three'}
-# dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
-# Keep order: {1: 'one', 2: 'two', 3: 'three'}
-# ---------------
-# Dictionary with strings:
-# Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# ---------------
-# List of mixed types:
-# Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
-# dont't keep order: [1, 2.5, 'a', 'Hello']
-# Keep order: [1, 'a', 2.5, 'Hello']
-# ---------------
-# Set of mixed types:
-# Original: {1, 2.5, 'a', 'Hello'}
-# dont't keep order: {1, 2.5, 'a', 'Hello'}
-# Keep order: {1, 2.5, 'a', 'Hello'}
-# ---------------
-# Tuple of mixed types:
-# Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
-# dont't keep order: (1, 2.5, 'a', 'Hello')
-# Keep order: (1, 'a', 2.5, 'Hello')
-# ---------------
-# Nested list:
-# Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
-# dont't keep order: [[1, 2], [3, 4], [5, 6]]
-# Keep order: [[1, 2], [3, 4], [5, 6]]
-# ---------------
-# Nested set:
-# Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# ---------------
-# Nested tuple:
-# Original: ((1, 2), (3, 4), (5, 6), (3, 4))
-# dont't keep order: ((1, 2), (3, 4), (5, 6))
-# Keep order: ((1, 2), (3, 4), (5, 6))
-# ---------------
-# List with None value:
-# Original: [1, None, 3, None, 5]
-# dont't keep order: [1, 3, None, 5]
-# Keep order: [1, None, 3, 5]
-# ---------------
-# Set with None value:
-# Original: {1, 3, None, 5}
-# dont't keep order: {1, 3, None, 5}
-# Keep order: {1, 3, None, 5}
-# ---------------
-# Tuple with None value:
-# Original: (1, None, 3, None, 5)
-# dont't keep order: (1, 3, None, 5)
-# Keep order: (1, None, 3, 5)
-# ---------------
-# List with boolean values:
-# Original: [True, False, True]
-# dont't keep order: [False, True]
-# Keep order: [True, False]
-# ---------------
-# Set with boolean values:
-# Original: {False, True}
-# dont't keep order: {False, True}
-# Keep order: {False, True}
-# ---------------
-# Tuple with boolean values:
-# Original: (True, False, True)
-# dont't keep order: (False, True)
-# Keep order: (True, False)
-# ---------------
-# List with repeated values:
-# Original: [1, 1, 1, 1, 1]
-# dont't keep order: [1]
-# Keep order: [1]
-# ---------------
-# Set with repeated values:
-# Original: {1}
-# dont't keep order: {1}
-# Keep order: {1}
-# ---------------
-# Tuple with repeated values:
-# Original: (1, 1, 1, 1, 1)
-# dont't keep order: (1,)
-# Keep order: (1,)
-# ---------------
-# List with mixed types and duplicates:
-# Original: [1, 'a', 2, 'a', 3, True, 3]
-# dont't keep order: [1, 2, 3, 'a']
-# Keep order: [True, 'a', 2, 3]
-# ---------------
-# Set with mixed types and duplicates:
-# Original: {1, 2, 3, 'a'}
-# dont't keep order: {1, 2, 3, 'a'}
-# Keep order: {1, 2, 3, 'a'}
-# ---------------
-# Tuple with mixed types and duplicates:
-# Original: (1, 'a', 2, 'a', 3, True)
-# dont't keep order: (1, 2, 3, 'a')
-# Keep order: (True, 'a', 2, 3)
-# ---------------
-# List with empty strings:
-# Original: ['', 'World', 'World', 'Hello', 'World']
-# dont't keep order: ['', 'World', 'Hello']
-# Keep order: ['', 'World', 'Hello']
-# ---------------
-# Set with empty strings:
-# Original: {'', 'World', 'Hello'}
-# dont't keep order: {'', 'World', 'Hello'}
-# Keep order: {'', 'World', 'Hello'}
 
 ```
```

### Comparing `screwduplicates-0.10/README.md` & `screwduplicates-0.11/screwduplicates.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: screwduplicates
+Version: 0.11
+Summary: provides a simple and efficient way to remove duplicates from an iterable (even with unhashable elements, optional order preservation)
+Home-page: https://github.com/hansalemaos/screwduplicates
+Author: Johannes Fischer
+Author-email: aulasparticularesdealemaosp@gmail.com
+License: MIT
+Keywords: remove,duplicates
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
+
 # provides a simple and efficient way to remove duplicates from an iterable (even with unhashable elements, optional order preservation)
 
 ## pip install screwduplicates
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ### Duplicate Removal: 
@@ -25,14 +43,15 @@
 testdict = {
     "List": [5, 4, 1, 2, 2, 3, 4, 5],
     "Set": {1, 2, 3, 4, 5},
     "Tuple": (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1),
     "Dictionary": {"a": 1, "b": 2, "c": 3},
     "String": "Hello",
     "Bytes": b"Hello",
+    "Bytearray": bytearray(b"Hello"),
     "List of strings": ["Hello", "World", "Hello"],
     "List of numbers": [2.5, 3.5, 1.5, 2.5, 3.5],
     "Empty list": [],
     "Set of strings": {"apple", "banana", "cherry"},
     "Set of numbers": {1, 2, 3, 4, 5},
     "Tuple of strings": ("apple", "banana", "cherry", "banana", "banana"),
     "Tuple of numbers": (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5),
@@ -55,193 +74,197 @@
     "Tuple with repeated values": (1, 1, 1, 1, 1),
     "List with mixed types and duplicates": [1, "a", 2, "a", 3, True, 3],
     "Set with mixed types and duplicates": {1, "a", 2, "a", 3, True},
     "Tuple with mixed types and duplicates": (1, "a", 2, "a", 3, True),
     "List with empty strings": ["", "World", "World", "Hello", "World"],
     "Set with empty strings": {"", "World", "Hello", "World", "World"},
 }
-
 from screwduplicates import del_duplicates
 for key, item in testdict.items():
     print(f"\n---------------\n{key}:")
     print(f"Original: {item}")
-    print(f"dont't keep order: {del_duplicates(item,keep_order=False)}")
-    print(f"Keep order: {del_duplicates(item,keep_order=True)}")
+    print(f"dont't keep order: {del_duplicates(item, keep_order=False)}")
+    print(f"Keep order: {del_duplicates(item, keep_order=True)}")
 
+---------------
+List:
+Original: [5, 4, 1, 2, 2, 3, 4, 5]
+dont't keep order: [1, 2, 3, 4, 5]
+Keep order: [5, 4, 1, 2, 3]
+---------------
+Set:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple:
+Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (1, 3, 4, 2, 5)
+---------------
+Dictionary:
+Original: {'a': 1, 'b': 2, 'c': 3}
+dont't keep order: {'a': 1, 'b': 2, 'c': 3}
+Keep order: {'a': 1, 'b': 2, 'c': 3}
+---------------
+String:
+Original: Hello
+dont't keep order: loeH
+Keep order: Helo
+---------------
+Bytes:
+Original: b'Hello'
+dont't keep order: b'Hleo'
+Keep order: b'Helo'
+---------------
+Bytearray:
+Original: bytearray(b'Hello')
+dont't keep order: bytearray(b'Hleo')
+Keep order: bytearray(b'Helo')
+---------------
+List of strings:
+Original: ['Hello', 'World', 'Hello']
+dont't keep order: ['World', 'Hello']
+Keep order: ['Hello', 'World']
+---------------
+List of numbers:
+Original: [2.5, 3.5, 1.5, 2.5, 3.5]
+dont't keep order: [1.5, 2.5, 3.5]
+Keep order: [2.5, 3.5, 1.5]
+---------------
+Empty list:
+Original: []
+dont't keep order: []
+Keep order: []
+---------------
+Set of strings:
+Original: {'cherry', 'banana', 'apple'}
+dont't keep order: {'cherry', 'banana', 'apple'}
+Keep order: {'cherry', 'banana', 'apple'}
+---------------
+Set of numbers:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple of strings:
+Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
+dont't keep order: ('cherry', 'banana', 'apple')
+Keep order: ('apple', 'banana', 'cherry')
+---------------
+Tuple of numbers:
+Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (3, 4, 5, 1, 2)
+---------------
+Dictionary with numbers:
+Original: {1: 'one', 2: 'two', 3: 'three'}
+dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
+Keep order: {1: 'one', 2: 'two', 3: 'three'}
+---------------
+Dictionary with strings:
+Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+---------------
+List of mixed types:
+Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
+dont't keep order: [1, 2.5, 'a', 'Hello']
+Keep order: [1, 'a', 2.5, 'Hello']
+---------------
+Set of mixed types:
+Original: {1, 2.5, 'a', 'Hello'}
+dont't keep order: {1, 2.5, 'a', 'Hello'}
+Keep order: {1, 2.5, 'a', 'Hello'}
+---------------
+Tuple of mixed types:
+Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
+dont't keep order: (1, 2.5, 'a', 'Hello')
+Keep order: (1, 'a', 2.5, 'Hello')
+---------------
+Nested list:
+Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
+dont't keep order: [[1, 2], [3, 4], [5, 6]]
+Keep order: [[1, 2], [3, 4], [5, 6]]
+---------------
+Nested set:
+Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+---------------
+Nested tuple:
+Original: ((1, 2), (3, 4), (5, 6), (3, 4))
+dont't keep order: ((1, 2), (3, 4), (5, 6))
+Keep order: ((1, 2), (3, 4), (5, 6))
+---------------
+List with None value:
+Original: [1, None, 3, None, 5]
+dont't keep order: [1, 3, None, 5]
+Keep order: [1, None, 3, 5]
+---------------
+Set with None value:
+Original: {1, 3, None, 5}
+dont't keep order: {1, 3, None, 5}
+Keep order: {1, 3, None, 5}
+---------------
+Tuple with None value:
+Original: (1, None, 3, None, 5)
+dont't keep order: (1, 3, None, 5)
+Keep order: (1, None, 3, 5)
+---------------
+List with boolean values:
+Original: [True, False, True]
+dont't keep order: [False, True]
+Keep order: [True, False]
+---------------
+Set with boolean values:
+Original: {False, True}
+dont't keep order: {False, True}
+Keep order: {False, True}
+---------------
+Tuple with boolean values:
+Original: (True, False, True)
+dont't keep order: (False, True)
+Keep order: (True, False)
+---------------
+List with repeated values:
+Original: [1, 1, 1, 1, 1]
+dont't keep order: [1]
+Keep order: [1]
+---------------
+Set with repeated values:
+Original: {1}
+dont't keep order: {1}
+Keep order: {1}
+---------------
+Tuple with repeated values:
+Original: (1, 1, 1, 1, 1)
+dont't keep order: (1,)
+Keep order: (1,)
+---------------
+List with mixed types and duplicates:
+Original: [1, 'a', 2, 'a', 3, True, 3]
+dont't keep order: [3, 1, 2, 'a']
+Keep order: [True, 'a', 2, 3]
+---------------
+Set with mixed types and duplicates:
+Original: {'a', 1, 2, 3}
+dont't keep order: {'a', 1, 2, 3}
+Keep order: {'a', 1, 2, 3}
+---------------
+Tuple with mixed types and duplicates:
+Original: (1, 'a', 2, 'a', 3, True)
+dont't keep order: (3, 1, 2, 'a')
+Keep order: (True, 'a', 2, 3)
+---------------
+List with empty strings:
+Original: ['', 'World', 'World', 'Hello', 'World']
+dont't keep order: ['', 'World', 'Hello']
+Keep order: ['', 'World', 'Hello']
+---------------
+Set with empty strings:
+Original: {'', 'World', 'Hello'}
+dont't keep order: {'', 'World', 'Hello'}
+Keep order: {'', 'World', 'Hello'}
 
-# ---------------
-# List:
-# Original: [5, 4, 1, 2, 2, 3, 4, 5]
-# dont't keep order: [1, 2, 3, 4, 5]
-# Keep order: [5, 4, 1, 2, 3]
-# ---------------
-# Set:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple:
-# Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (1, 3, 4, 2, 5)
-# ---------------
-# Dictionary:
-# Original: {'a': 1, 'b': 2, 'c': 3}
-# dont't keep order: {'a': 1, 'b': 2, 'c': 3}
-# Keep order: {'a': 1, 'b': 2, 'c': 3}
-# ---------------
-# String:
-# Original: Hello
-# dont't keep order: {'H', 'o', 'l', 'e'}
-# Keep order: ['H', 'e', 'l', 'o']
-# ---------------
-# Bytes:
-# Original: b'Hello'
-# dont't keep order: b'Hleo'
-# Keep order: b'Helo'
-# ---------------
-# List of strings:
-# Original: ['Hello', 'World', 'Hello']
-# dont't keep order: ['World', 'Hello']
-# Keep order: ['Hello', 'World']
-# ---------------
-# List of numbers:
-# Original: [2.5, 3.5, 1.5, 2.5, 3.5]
-# dont't keep order: [1.5, 2.5, 3.5]
-# Keep order: [2.5, 3.5, 1.5]
-# ---------------
-# Empty list:
-# Original: []
-# dont't keep order: []
-# Keep order: []
-# ---------------
-# Set of strings:
-# Original: {'cherry', 'apple', 'banana'}
-# dont't keep order: {'cherry', 'apple', 'banana'}
-# Keep order: {'cherry', 'apple', 'banana'}
-# ---------------
-# Set of numbers:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple of strings:
-# Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
-# dont't keep order: ('cherry', 'apple', 'banana')
-# Keep order: ('apple', 'banana', 'cherry')
-# ---------------
-# Tuple of numbers:
-# Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (3, 4, 5, 1, 2)
-# ---------------
-# Dictionary with numbers:
-# Original: {1: 'one', 2: 'two', 3: 'three'}
-# dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
-# Keep order: {1: 'one', 2: 'two', 3: 'three'}
-# ---------------
-# Dictionary with strings:
-# Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# ---------------
-# List of mixed types:
-# Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
-# dont't keep order: [1, 2.5, 'a', 'Hello']
-# Keep order: [1, 'a', 2.5, 'Hello']
-# ---------------
-# Set of mixed types:
-# Original: {1, 2.5, 'a', 'Hello'}
-# dont't keep order: {1, 2.5, 'a', 'Hello'}
-# Keep order: {1, 2.5, 'a', 'Hello'}
-# ---------------
-# Tuple of mixed types:
-# Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
-# dont't keep order: (1, 2.5, 'a', 'Hello')
-# Keep order: (1, 'a', 2.5, 'Hello')
-# ---------------
-# Nested list:
-# Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
-# dont't keep order: [[1, 2], [3, 4], [5, 6]]
-# Keep order: [[1, 2], [3, 4], [5, 6]]
-# ---------------
-# Nested set:
-# Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# ---------------
-# Nested tuple:
-# Original: ((1, 2), (3, 4), (5, 6), (3, 4))
-# dont't keep order: ((1, 2), (3, 4), (5, 6))
-# Keep order: ((1, 2), (3, 4), (5, 6))
-# ---------------
-# List with None value:
-# Original: [1, None, 3, None, 5]
-# dont't keep order: [1, 3, None, 5]
-# Keep order: [1, None, 3, 5]
-# ---------------
-# Set with None value:
-# Original: {1, 3, None, 5}
-# dont't keep order: {1, 3, None, 5}
-# Keep order: {1, 3, None, 5}
-# ---------------
-# Tuple with None value:
-# Original: (1, None, 3, None, 5)
-# dont't keep order: (1, 3, None, 5)
-# Keep order: (1, None, 3, 5)
-# ---------------
-# List with boolean values:
-# Original: [True, False, True]
-# dont't keep order: [False, True]
-# Keep order: [True, False]
-# ---------------
-# Set with boolean values:
-# Original: {False, True}
-# dont't keep order: {False, True}
-# Keep order: {False, True}
-# ---------------
-# Tuple with boolean values:
-# Original: (True, False, True)
-# dont't keep order: (False, True)
-# Keep order: (True, False)
-# ---------------
-# List with repeated values:
-# Original: [1, 1, 1, 1, 1]
-# dont't keep order: [1]
-# Keep order: [1]
-# ---------------
-# Set with repeated values:
-# Original: {1}
-# dont't keep order: {1}
-# Keep order: {1}
-# ---------------
-# Tuple with repeated values:
-# Original: (1, 1, 1, 1, 1)
-# dont't keep order: (1,)
-# Keep order: (1,)
-# ---------------
-# List with mixed types and duplicates:
-# Original: [1, 'a', 2, 'a', 3, True, 3]
-# dont't keep order: [1, 2, 3, 'a']
-# Keep order: [True, 'a', 2, 3]
-# ---------------
-# Set with mixed types and duplicates:
-# Original: {1, 2, 3, 'a'}
-# dont't keep order: {1, 2, 3, 'a'}
-# Keep order: {1, 2, 3, 'a'}
-# ---------------
-# Tuple with mixed types and duplicates:
-# Original: (1, 'a', 2, 'a', 3, True)
-# dont't keep order: (1, 2, 3, 'a')
-# Keep order: (True, 'a', 2, 3)
-# ---------------
-# List with empty strings:
-# Original: ['', 'World', 'World', 'Hello', 'World']
-# dont't keep order: ['', 'World', 'Hello']
-# Keep order: ['', 'World', 'Hello']
-# ---------------
-# Set with empty strings:
-# Original: {'', 'World', 'Hello'}
-# dont't keep order: {'', 'World', 'Hello'}
-# Keep order: {'', 'World', 'Hello'}
 
-```
+```
```

### Comparing `screwduplicates-0.10/screwduplicates/README.MD` & `screwduplicates-0.11/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 testdict = {
     "List": [5, 4, 1, 2, 2, 3, 4, 5],
     "Set": {1, 2, 3, 4, 5},
     "Tuple": (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1),
     "Dictionary": {"a": 1, "b": 2, "c": 3},
     "String": "Hello",
     "Bytes": b"Hello",
+    "Bytearray": bytearray(b"Hello"),
     "List of strings": ["Hello", "World", "Hello"],
     "List of numbers": [2.5, 3.5, 1.5, 2.5, 3.5],
     "Empty list": [],
     "Set of strings": {"apple", "banana", "cherry"},
     "Set of numbers": {1, 2, 3, 4, 5},
     "Tuple of strings": ("apple", "banana", "cherry", "banana", "banana"),
     "Tuple of numbers": (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5),
@@ -55,193 +56,197 @@
     "Tuple with repeated values": (1, 1, 1, 1, 1),
     "List with mixed types and duplicates": [1, "a", 2, "a", 3, True, 3],
     "Set with mixed types and duplicates": {1, "a", 2, "a", 3, True},
     "Tuple with mixed types and duplicates": (1, "a", 2, "a", 3, True),
     "List with empty strings": ["", "World", "World", "Hello", "World"],
     "Set with empty strings": {"", "World", "Hello", "World", "World"},
 }
-
 from screwduplicates import del_duplicates
 for key, item in testdict.items():
     print(f"\n---------------\n{key}:")
     print(f"Original: {item}")
-    print(f"dont't keep order: {del_duplicates(item,keep_order=False)}")
-    print(f"Keep order: {del_duplicates(item,keep_order=True)}")
+    print(f"dont't keep order: {del_duplicates(item, keep_order=False)}")
+    print(f"Keep order: {del_duplicates(item, keep_order=True)}")
 
+---------------
+List:
+Original: [5, 4, 1, 2, 2, 3, 4, 5]
+dont't keep order: [1, 2, 3, 4, 5]
+Keep order: [5, 4, 1, 2, 3]
+---------------
+Set:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple:
+Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (1, 3, 4, 2, 5)
+---------------
+Dictionary:
+Original: {'a': 1, 'b': 2, 'c': 3}
+dont't keep order: {'a': 1, 'b': 2, 'c': 3}
+Keep order: {'a': 1, 'b': 2, 'c': 3}
+---------------
+String:
+Original: Hello
+dont't keep order: loeH
+Keep order: Helo
+---------------
+Bytes:
+Original: b'Hello'
+dont't keep order: b'Hleo'
+Keep order: b'Helo'
+---------------
+Bytearray:
+Original: bytearray(b'Hello')
+dont't keep order: bytearray(b'Hleo')
+Keep order: bytearray(b'Helo')
+---------------
+List of strings:
+Original: ['Hello', 'World', 'Hello']
+dont't keep order: ['World', 'Hello']
+Keep order: ['Hello', 'World']
+---------------
+List of numbers:
+Original: [2.5, 3.5, 1.5, 2.5, 3.5]
+dont't keep order: [1.5, 2.5, 3.5]
+Keep order: [2.5, 3.5, 1.5]
+---------------
+Empty list:
+Original: []
+dont't keep order: []
+Keep order: []
+---------------
+Set of strings:
+Original: {'cherry', 'banana', 'apple'}
+dont't keep order: {'cherry', 'banana', 'apple'}
+Keep order: {'cherry', 'banana', 'apple'}
+---------------
+Set of numbers:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple of strings:
+Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
+dont't keep order: ('cherry', 'banana', 'apple')
+Keep order: ('apple', 'banana', 'cherry')
+---------------
+Tuple of numbers:
+Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (3, 4, 5, 1, 2)
+---------------
+Dictionary with numbers:
+Original: {1: 'one', 2: 'two', 3: 'three'}
+dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
+Keep order: {1: 'one', 2: 'two', 3: 'three'}
+---------------
+Dictionary with strings:
+Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+---------------
+List of mixed types:
+Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
+dont't keep order: [1, 2.5, 'a', 'Hello']
+Keep order: [1, 'a', 2.5, 'Hello']
+---------------
+Set of mixed types:
+Original: {1, 2.5, 'a', 'Hello'}
+dont't keep order: {1, 2.5, 'a', 'Hello'}
+Keep order: {1, 2.5, 'a', 'Hello'}
+---------------
+Tuple of mixed types:
+Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
+dont't keep order: (1, 2.5, 'a', 'Hello')
+Keep order: (1, 'a', 2.5, 'Hello')
+---------------
+Nested list:
+Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
+dont't keep order: [[1, 2], [3, 4], [5, 6]]
+Keep order: [[1, 2], [3, 4], [5, 6]]
+---------------
+Nested set:
+Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+---------------
+Nested tuple:
+Original: ((1, 2), (3, 4), (5, 6), (3, 4))
+dont't keep order: ((1, 2), (3, 4), (5, 6))
+Keep order: ((1, 2), (3, 4), (5, 6))
+---------------
+List with None value:
+Original: [1, None, 3, None, 5]
+dont't keep order: [1, 3, None, 5]
+Keep order: [1, None, 3, 5]
+---------------
+Set with None value:
+Original: {1, 3, None, 5}
+dont't keep order: {1, 3, None, 5}
+Keep order: {1, 3, None, 5}
+---------------
+Tuple with None value:
+Original: (1, None, 3, None, 5)
+dont't keep order: (1, 3, None, 5)
+Keep order: (1, None, 3, 5)
+---------------
+List with boolean values:
+Original: [True, False, True]
+dont't keep order: [False, True]
+Keep order: [True, False]
+---------------
+Set with boolean values:
+Original: {False, True}
+dont't keep order: {False, True}
+Keep order: {False, True}
+---------------
+Tuple with boolean values:
+Original: (True, False, True)
+dont't keep order: (False, True)
+Keep order: (True, False)
+---------------
+List with repeated values:
+Original: [1, 1, 1, 1, 1]
+dont't keep order: [1]
+Keep order: [1]
+---------------
+Set with repeated values:
+Original: {1}
+dont't keep order: {1}
+Keep order: {1}
+---------------
+Tuple with repeated values:
+Original: (1, 1, 1, 1, 1)
+dont't keep order: (1,)
+Keep order: (1,)
+---------------
+List with mixed types and duplicates:
+Original: [1, 'a', 2, 'a', 3, True, 3]
+dont't keep order: [3, 1, 2, 'a']
+Keep order: [True, 'a', 2, 3]
+---------------
+Set with mixed types and duplicates:
+Original: {'a', 1, 2, 3}
+dont't keep order: {'a', 1, 2, 3}
+Keep order: {'a', 1, 2, 3}
+---------------
+Tuple with mixed types and duplicates:
+Original: (1, 'a', 2, 'a', 3, True)
+dont't keep order: (3, 1, 2, 'a')
+Keep order: (True, 'a', 2, 3)
+---------------
+List with empty strings:
+Original: ['', 'World', 'World', 'Hello', 'World']
+dont't keep order: ['', 'World', 'Hello']
+Keep order: ['', 'World', 'Hello']
+---------------
+Set with empty strings:
+Original: {'', 'World', 'Hello'}
+dont't keep order: {'', 'World', 'Hello'}
+Keep order: {'', 'World', 'Hello'}
 
-# ---------------
-# List:
-# Original: [5, 4, 1, 2, 2, 3, 4, 5]
-# dont't keep order: [1, 2, 3, 4, 5]
-# Keep order: [5, 4, 1, 2, 3]
-# ---------------
-# Set:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple:
-# Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (1, 3, 4, 2, 5)
-# ---------------
-# Dictionary:
-# Original: {'a': 1, 'b': 2, 'c': 3}
-# dont't keep order: {'a': 1, 'b': 2, 'c': 3}
-# Keep order: {'a': 1, 'b': 2, 'c': 3}
-# ---------------
-# String:
-# Original: Hello
-# dont't keep order: {'H', 'o', 'l', 'e'}
-# Keep order: ['H', 'e', 'l', 'o']
-# ---------------
-# Bytes:
-# Original: b'Hello'
-# dont't keep order: b'Hleo'
-# Keep order: b'Helo'
-# ---------------
-# List of strings:
-# Original: ['Hello', 'World', 'Hello']
-# dont't keep order: ['World', 'Hello']
-# Keep order: ['Hello', 'World']
-# ---------------
-# List of numbers:
-# Original: [2.5, 3.5, 1.5, 2.5, 3.5]
-# dont't keep order: [1.5, 2.5, 3.5]
-# Keep order: [2.5, 3.5, 1.5]
-# ---------------
-# Empty list:
-# Original: []
-# dont't keep order: []
-# Keep order: []
-# ---------------
-# Set of strings:
-# Original: {'cherry', 'apple', 'banana'}
-# dont't keep order: {'cherry', 'apple', 'banana'}
-# Keep order: {'cherry', 'apple', 'banana'}
-# ---------------
-# Set of numbers:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple of strings:
-# Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
-# dont't keep order: ('cherry', 'apple', 'banana')
-# Keep order: ('apple', 'banana', 'cherry')
-# ---------------
-# Tuple of numbers:
-# Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (3, 4, 5, 1, 2)
-# ---------------
-# Dictionary with numbers:
-# Original: {1: 'one', 2: 'two', 3: 'three'}
-# dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
-# Keep order: {1: 'one', 2: 'two', 3: 'three'}
-# ---------------
-# Dictionary with strings:
-# Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# ---------------
-# List of mixed types:
-# Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
-# dont't keep order: [1, 2.5, 'a', 'Hello']
-# Keep order: [1, 'a', 2.5, 'Hello']
-# ---------------
-# Set of mixed types:
-# Original: {1, 2.5, 'a', 'Hello'}
-# dont't keep order: {1, 2.5, 'a', 'Hello'}
-# Keep order: {1, 2.5, 'a', 'Hello'}
-# ---------------
-# Tuple of mixed types:
-# Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
-# dont't keep order: (1, 2.5, 'a', 'Hello')
-# Keep order: (1, 'a', 2.5, 'Hello')
-# ---------------
-# Nested list:
-# Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
-# dont't keep order: [[1, 2], [3, 4], [5, 6]]
-# Keep order: [[1, 2], [3, 4], [5, 6]]
-# ---------------
-# Nested set:
-# Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# ---------------
-# Nested tuple:
-# Original: ((1, 2), (3, 4), (5, 6), (3, 4))
-# dont't keep order: ((1, 2), (3, 4), (5, 6))
-# Keep order: ((1, 2), (3, 4), (5, 6))
-# ---------------
-# List with None value:
-# Original: [1, None, 3, None, 5]
-# dont't keep order: [1, 3, None, 5]
-# Keep order: [1, None, 3, 5]
-# ---------------
-# Set with None value:
-# Original: {1, 3, None, 5}
-# dont't keep order: {1, 3, None, 5}
-# Keep order: {1, 3, None, 5}
-# ---------------
-# Tuple with None value:
-# Original: (1, None, 3, None, 5)
-# dont't keep order: (1, 3, None, 5)
-# Keep order: (1, None, 3, 5)
-# ---------------
-# List with boolean values:
-# Original: [True, False, True]
-# dont't keep order: [False, True]
-# Keep order: [True, False]
-# ---------------
-# Set with boolean values:
-# Original: {False, True}
-# dont't keep order: {False, True}
-# Keep order: {False, True}
-# ---------------
-# Tuple with boolean values:
-# Original: (True, False, True)
-# dont't keep order: (False, True)
-# Keep order: (True, False)
-# ---------------
-# List with repeated values:
-# Original: [1, 1, 1, 1, 1]
-# dont't keep order: [1]
-# Keep order: [1]
-# ---------------
-# Set with repeated values:
-# Original: {1}
-# dont't keep order: {1}
-# Keep order: {1}
-# ---------------
-# Tuple with repeated values:
-# Original: (1, 1, 1, 1, 1)
-# dont't keep order: (1,)
-# Keep order: (1,)
-# ---------------
-# List with mixed types and duplicates:
-# Original: [1, 'a', 2, 'a', 3, True, 3]
-# dont't keep order: [1, 2, 3, 'a']
-# Keep order: [True, 'a', 2, 3]
-# ---------------
-# Set with mixed types and duplicates:
-# Original: {1, 2, 3, 'a'}
-# dont't keep order: {1, 2, 3, 'a'}
-# Keep order: {1, 2, 3, 'a'}
-# ---------------
-# Tuple with mixed types and duplicates:
-# Original: (1, 'a', 2, 'a', 3, True)
-# dont't keep order: (1, 2, 3, 'a')
-# Keep order: (True, 'a', 2, 3)
-# ---------------
-# List with empty strings:
-# Original: ['', 'World', 'World', 'Hello', 'World']
-# dont't keep order: ['', 'World', 'Hello']
-# Keep order: ['', 'World', 'Hello']
-# ---------------
-# Set with empty strings:
-# Original: {'', 'World', 'Hello'}
-# dont't keep order: {'', 'World', 'Hello'}
-# Keep order: {'', 'World', 'Hello'}
 
 ```
```

### Comparing `screwduplicates-0.10/screwduplicates.egg-info/PKG-INFO` & `screwduplicates-0.11/screwduplicates/README.MD`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: screwduplicates
-Version: 0.10
-Summary: provides a simple and efficient way to remove duplicates from an iterable (even with unhashable elements, optional order preservation)
-Home-page: https://github.com/hansalemaos/screwduplicates
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: remove,duplicates
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
 # provides a simple and efficient way to remove duplicates from an iterable (even with unhashable elements, optional order preservation)
 
 ## pip install screwduplicates
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ### Duplicate Removal: 
@@ -43,14 +25,15 @@
 testdict = {
     "List": [5, 4, 1, 2, 2, 3, 4, 5],
     "Set": {1, 2, 3, 4, 5},
     "Tuple": (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1),
     "Dictionary": {"a": 1, "b": 2, "c": 3},
     "String": "Hello",
     "Bytes": b"Hello",
+    "Bytearray": bytearray(b"Hello"),
     "List of strings": ["Hello", "World", "Hello"],
     "List of numbers": [2.5, 3.5, 1.5, 2.5, 3.5],
     "Empty list": [],
     "Set of strings": {"apple", "banana", "cherry"},
     "Set of numbers": {1, 2, 3, 4, 5},
     "Tuple of strings": ("apple", "banana", "cherry", "banana", "banana"),
     "Tuple of numbers": (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5),
@@ -73,193 +56,197 @@
     "Tuple with repeated values": (1, 1, 1, 1, 1),
     "List with mixed types and duplicates": [1, "a", 2, "a", 3, True, 3],
     "Set with mixed types and duplicates": {1, "a", 2, "a", 3, True},
     "Tuple with mixed types and duplicates": (1, "a", 2, "a", 3, True),
     "List with empty strings": ["", "World", "World", "Hello", "World"],
     "Set with empty strings": {"", "World", "Hello", "World", "World"},
 }
-
 from screwduplicates import del_duplicates
 for key, item in testdict.items():
     print(f"\n---------------\n{key}:")
     print(f"Original: {item}")
-    print(f"dont't keep order: {del_duplicates(item,keep_order=False)}")
-    print(f"Keep order: {del_duplicates(item,keep_order=True)}")
+    print(f"dont't keep order: {del_duplicates(item, keep_order=False)}")
+    print(f"Keep order: {del_duplicates(item, keep_order=True)}")
 
+---------------
+List:
+Original: [5, 4, 1, 2, 2, 3, 4, 5]
+dont't keep order: [1, 2, 3, 4, 5]
+Keep order: [5, 4, 1, 2, 3]
+---------------
+Set:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple:
+Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (1, 3, 4, 2, 5)
+---------------
+Dictionary:
+Original: {'a': 1, 'b': 2, 'c': 3}
+dont't keep order: {'a': 1, 'b': 2, 'c': 3}
+Keep order: {'a': 1, 'b': 2, 'c': 3}
+---------------
+String:
+Original: Hello
+dont't keep order: loeH
+Keep order: Helo
+---------------
+Bytes:
+Original: b'Hello'
+dont't keep order: b'Hleo'
+Keep order: b'Helo'
+---------------
+Bytearray:
+Original: bytearray(b'Hello')
+dont't keep order: bytearray(b'Hleo')
+Keep order: bytearray(b'Helo')
+---------------
+List of strings:
+Original: ['Hello', 'World', 'Hello']
+dont't keep order: ['World', 'Hello']
+Keep order: ['Hello', 'World']
+---------------
+List of numbers:
+Original: [2.5, 3.5, 1.5, 2.5, 3.5]
+dont't keep order: [1.5, 2.5, 3.5]
+Keep order: [2.5, 3.5, 1.5]
+---------------
+Empty list:
+Original: []
+dont't keep order: []
+Keep order: []
+---------------
+Set of strings:
+Original: {'cherry', 'banana', 'apple'}
+dont't keep order: {'cherry', 'banana', 'apple'}
+Keep order: {'cherry', 'banana', 'apple'}
+---------------
+Set of numbers:
+Original: {1, 2, 3, 4, 5}
+dont't keep order: {1, 2, 3, 4, 5}
+Keep order: {1, 2, 3, 4, 5}
+---------------
+Tuple of strings:
+Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
+dont't keep order: ('cherry', 'banana', 'apple')
+Keep order: ('apple', 'banana', 'cherry')
+---------------
+Tuple of numbers:
+Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
+dont't keep order: (1, 2, 3, 4, 5)
+Keep order: (3, 4, 5, 1, 2)
+---------------
+Dictionary with numbers:
+Original: {1: 'one', 2: 'two', 3: 'three'}
+dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
+Keep order: {1: 'one', 2: 'two', 3: 'three'}
+---------------
+Dictionary with strings:
+Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
+---------------
+List of mixed types:
+Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
+dont't keep order: [1, 2.5, 'a', 'Hello']
+Keep order: [1, 'a', 2.5, 'Hello']
+---------------
+Set of mixed types:
+Original: {1, 2.5, 'a', 'Hello'}
+dont't keep order: {1, 2.5, 'a', 'Hello'}
+Keep order: {1, 2.5, 'a', 'Hello'}
+---------------
+Tuple of mixed types:
+Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
+dont't keep order: (1, 2.5, 'a', 'Hello')
+Keep order: (1, 'a', 2.5, 'Hello')
+---------------
+Nested list:
+Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
+dont't keep order: [[1, 2], [3, 4], [5, 6]]
+Keep order: [[1, 2], [3, 4], [5, 6]]
+---------------
+Nested set:
+Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
+---------------
+Nested tuple:
+Original: ((1, 2), (3, 4), (5, 6), (3, 4))
+dont't keep order: ((1, 2), (3, 4), (5, 6))
+Keep order: ((1, 2), (3, 4), (5, 6))
+---------------
+List with None value:
+Original: [1, None, 3, None, 5]
+dont't keep order: [1, 3, None, 5]
+Keep order: [1, None, 3, 5]
+---------------
+Set with None value:
+Original: {1, 3, None, 5}
+dont't keep order: {1, 3, None, 5}
+Keep order: {1, 3, None, 5}
+---------------
+Tuple with None value:
+Original: (1, None, 3, None, 5)
+dont't keep order: (1, 3, None, 5)
+Keep order: (1, None, 3, 5)
+---------------
+List with boolean values:
+Original: [True, False, True]
+dont't keep order: [False, True]
+Keep order: [True, False]
+---------------
+Set with boolean values:
+Original: {False, True}
+dont't keep order: {False, True}
+Keep order: {False, True}
+---------------
+Tuple with boolean values:
+Original: (True, False, True)
+dont't keep order: (False, True)
+Keep order: (True, False)
+---------------
+List with repeated values:
+Original: [1, 1, 1, 1, 1]
+dont't keep order: [1]
+Keep order: [1]
+---------------
+Set with repeated values:
+Original: {1}
+dont't keep order: {1}
+Keep order: {1}
+---------------
+Tuple with repeated values:
+Original: (1, 1, 1, 1, 1)
+dont't keep order: (1,)
+Keep order: (1,)
+---------------
+List with mixed types and duplicates:
+Original: [1, 'a', 2, 'a', 3, True, 3]
+dont't keep order: [3, 1, 2, 'a']
+Keep order: [True, 'a', 2, 3]
+---------------
+Set with mixed types and duplicates:
+Original: {'a', 1, 2, 3}
+dont't keep order: {'a', 1, 2, 3}
+Keep order: {'a', 1, 2, 3}
+---------------
+Tuple with mixed types and duplicates:
+Original: (1, 'a', 2, 'a', 3, True)
+dont't keep order: (3, 1, 2, 'a')
+Keep order: (True, 'a', 2, 3)
+---------------
+List with empty strings:
+Original: ['', 'World', 'World', 'Hello', 'World']
+dont't keep order: ['', 'World', 'Hello']
+Keep order: ['', 'World', 'Hello']
+---------------
+Set with empty strings:
+Original: {'', 'World', 'Hello'}
+dont't keep order: {'', 'World', 'Hello'}
+Keep order: {'', 'World', 'Hello'}
 
-# ---------------
-# List:
-# Original: [5, 4, 1, 2, 2, 3, 4, 5]
-# dont't keep order: [1, 2, 3, 4, 5]
-# Keep order: [5, 4, 1, 2, 3]
-# ---------------
-# Set:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple:
-# Original: (1, 3, 4, 2, 3, 4, 5, 5, 5, 2, 2, 1)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (1, 3, 4, 2, 5)
-# ---------------
-# Dictionary:
-# Original: {'a': 1, 'b': 2, 'c': 3}
-# dont't keep order: {'a': 1, 'b': 2, 'c': 3}
-# Keep order: {'a': 1, 'b': 2, 'c': 3}
-# ---------------
-# String:
-# Original: Hello
-# dont't keep order: {'H', 'o', 'l', 'e'}
-# Keep order: ['H', 'e', 'l', 'o']
-# ---------------
-# Bytes:
-# Original: b'Hello'
-# dont't keep order: b'Hleo'
-# Keep order: b'Helo'
-# ---------------
-# List of strings:
-# Original: ['Hello', 'World', 'Hello']
-# dont't keep order: ['World', 'Hello']
-# Keep order: ['Hello', 'World']
-# ---------------
-# List of numbers:
-# Original: [2.5, 3.5, 1.5, 2.5, 3.5]
-# dont't keep order: [1.5, 2.5, 3.5]
-# Keep order: [2.5, 3.5, 1.5]
-# ---------------
-# Empty list:
-# Original: []
-# dont't keep order: []
-# Keep order: []
-# ---------------
-# Set of strings:
-# Original: {'cherry', 'apple', 'banana'}
-# dont't keep order: {'cherry', 'apple', 'banana'}
-# Keep order: {'cherry', 'apple', 'banana'}
-# ---------------
-# Set of numbers:
-# Original: {1, 2, 3, 4, 5}
-# dont't keep order: {1, 2, 3, 4, 5}
-# Keep order: {1, 2, 3, 4, 5}
-# ---------------
-# Tuple of strings:
-# Original: ('apple', 'banana', 'cherry', 'banana', 'banana')
-# dont't keep order: ('cherry', 'apple', 'banana')
-# Keep order: ('apple', 'banana', 'cherry')
-# ---------------
-# Tuple of numbers:
-# Original: (3, 4, 5, 1, 2, 3, 4, 2, 3, 4, 2, 3, 4, 5)
-# dont't keep order: (1, 2, 3, 4, 5)
-# Keep order: (3, 4, 5, 1, 2)
-# ---------------
-# Dictionary with numbers:
-# Original: {1: 'one', 2: 'two', 3: 'three'}
-# dont't keep order: {1: 'one', 2: 'two', 3: 'three'}
-# Keep order: {1: 'one', 2: 'two', 3: 'three'}
-# ---------------
-# Dictionary with strings:
-# Original: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# dont't keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# Keep order: {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
-# ---------------
-# List of mixed types:
-# Original: [1, 'a', 2.5, True, True, True, 1, 'a', 'Hello']
-# dont't keep order: [1, 2.5, 'a', 'Hello']
-# Keep order: [1, 'a', 2.5, 'Hello']
-# ---------------
-# Set of mixed types:
-# Original: {1, 2.5, 'a', 'Hello'}
-# dont't keep order: {1, 2.5, 'a', 'Hello'}
-# Keep order: {1, 2.5, 'a', 'Hello'}
-# ---------------
-# Tuple of mixed types:
-# Original: (1, 'a', 2.5, True, 'Hello', 1, 'a', 2.5)
-# dont't keep order: (1, 2.5, 'a', 'Hello')
-# Keep order: (1, 'a', 2.5, 'Hello')
-# ---------------
-# Nested list:
-# Original: [[1, 2], [3, 4], [5, 6], [1, 2], [3, 4], [3, 4], [5, 6]]
-# dont't keep order: [[1, 2], [3, 4], [5, 6]]
-# Keep order: [[1, 2], [3, 4], [5, 6]]
-# ---------------
-# Nested set:
-# Original: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# dont't keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# Keep order: {frozenset({3, 4}), frozenset({5, 6}), frozenset({1, 2})}
-# ---------------
-# Nested tuple:
-# Original: ((1, 2), (3, 4), (5, 6), (3, 4))
-# dont't keep order: ((1, 2), (3, 4), (5, 6))
-# Keep order: ((1, 2), (3, 4), (5, 6))
-# ---------------
-# List with None value:
-# Original: [1, None, 3, None, 5]
-# dont't keep order: [1, 3, None, 5]
-# Keep order: [1, None, 3, 5]
-# ---------------
-# Set with None value:
-# Original: {1, 3, None, 5}
-# dont't keep order: {1, 3, None, 5}
-# Keep order: {1, 3, None, 5}
-# ---------------
-# Tuple with None value:
-# Original: (1, None, 3, None, 5)
-# dont't keep order: (1, 3, None, 5)
-# Keep order: (1, None, 3, 5)
-# ---------------
-# List with boolean values:
-# Original: [True, False, True]
-# dont't keep order: [False, True]
-# Keep order: [True, False]
-# ---------------
-# Set with boolean values:
-# Original: {False, True}
-# dont't keep order: {False, True}
-# Keep order: {False, True}
-# ---------------
-# Tuple with boolean values:
-# Original: (True, False, True)
-# dont't keep order: (False, True)
-# Keep order: (True, False)
-# ---------------
-# List with repeated values:
-# Original: [1, 1, 1, 1, 1]
-# dont't keep order: [1]
-# Keep order: [1]
-# ---------------
-# Set with repeated values:
-# Original: {1}
-# dont't keep order: {1}
-# Keep order: {1}
-# ---------------
-# Tuple with repeated values:
-# Original: (1, 1, 1, 1, 1)
-# dont't keep order: (1,)
-# Keep order: (1,)
-# ---------------
-# List with mixed types and duplicates:
-# Original: [1, 'a', 2, 'a', 3, True, 3]
-# dont't keep order: [1, 2, 3, 'a']
-# Keep order: [True, 'a', 2, 3]
-# ---------------
-# Set with mixed types and duplicates:
-# Original: {1, 2, 3, 'a'}
-# dont't keep order: {1, 2, 3, 'a'}
-# Keep order: {1, 2, 3, 'a'}
-# ---------------
-# Tuple with mixed types and duplicates:
-# Original: (1, 'a', 2, 'a', 3, True)
-# dont't keep order: (1, 2, 3, 'a')
-# Keep order: (True, 'a', 2, 3)
-# ---------------
-# List with empty strings:
-# Original: ['', 'World', 'World', 'Hello', 'World']
-# dont't keep order: ['', 'World', 'Hello']
-# Keep order: ['', 'World', 'Hello']
-# ---------------
-# Set with empty strings:
-# Original: {'', 'World', 'Hello'}
-# dont't keep order: {'', 'World', 'Hello'}
-# Keep order: {'', 'World', 'Hello'}
 
-```
+```
```

### Comparing `screwduplicates-0.10/setup.py` & `screwduplicates-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''provides a simple and efficient way to remove duplicates from an iterable (even with unhashable elements, optional order preservation)'''
 
 # Setting up
 setup(
     name="screwduplicates",
     version=VERSION,
     license='MIT',
```

