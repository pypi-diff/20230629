# Comparing `tmp/suger-0.2.0.tar.gz` & `tmp/suger-0.2.1.tar.gz`

## Comparing `suger-0.2.0.tar` & `suger-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 suger-0.2.0/RoadMap.md
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 suger-0.2.0/setup.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.2.0/upload.sh
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 suger-0.2.0/安装.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.2.0/suger/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/FileCompareUtils.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/FileUtils.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/StringUtils.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/CsvUtils.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/ExcelUtils.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/JsonUtils.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/XmlUtils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.2.0/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.2.0/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 suger-0.2.0/suger/stream/Stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/suger/stream/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.2.0/suger/terminal/SSH.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.2.0/suger/terminal/TerminalUtils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.2.0/suger/terminal/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_CsvUtils.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_ExcelUtils.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_FileCompareUtils.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_FileUtils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_JsonUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_SSH.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_Stream.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_StringUtils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_TerminalUtils.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_XmlUtils.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/tests/decorator/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.2.0/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.2.0/LICENSE
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 suger-0.2.0/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 suger-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 suger-0.2.1/RoadMap.md
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 suger-0.2.1/setup.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.2.1/upload.sh
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 suger-0.2.1/安装.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.2.1/suger/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/FileUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/CsvUtils.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/ExcelUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/JsonUtils.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/XmlUtils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.2.1/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.2.1/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 suger-0.2.1/suger/stream/Stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/suger/stream/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.2.1/suger/terminal/SSH.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.2.1/suger/terminal/TerminalUtils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.2.1/suger/terminal/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_ExcelUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_SSH.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_Stream.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_StringUtils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_XmlUtils.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 suger-0.2.1/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 suger-0.2.1/PKG-INFO
```

### Comparing `suger-0.2.0/RoadMap.md` & `suger-0.2.1/RoadMap.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # RoadMap
 
-# v0.2.0
+# v0.2.1
 加入了流式计算 Stream 
 
 迁移了 Java Stream / C# Linq 特性
 
 ```python
 
 class TestStream(TestCase):
 
     def test_demo(self):
         # 使用map操作将每个元素加倍
-        result = Stream(globalData).filter(lambda x: x % 2 == 0)\
-            .sort(reverse=True) \
-            .map(lambda x: x * 2)\
+        result = Stream(globalData).filter(lambda x: x % 2 == 0)
+            .sort(reverse=True)
+            .map(lambda x: x * 2)
             .toSet()
         self.assertEqual(result, {8, 4})
 
     def test_sort_numeric(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
-        result = Stream(data).sort(key=lambda x: x).toList()
+        result = Stream(data).sort(sortedFunc=lambda x: x).toList()
         self.assertEqual(result, [1, 2, 3, 4, 5, 6, 7, 8])
 
     def test_sort_numeric_reverse(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
-        result = Stream(data).sort(key=lambda x: x, reverse=True).toList()
+        result = Stream(data).sort(sortedFunc=lambda x: x, reverse=True).toList()
         self.assertEqual(result, [8, 7, 6, 5, 4, 3, 2, 1])
 
     def test_sort(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
         result = Stream(data).sort().toList()
         self.assertEqual(result, [1, 2, 3, 4, 5, 6, 7, 8])
 
     def test_sort_reverse(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
         result = Stream(data).sort(reverse=True).toList()
         self.assertEqual(result, [8, 7, 6, 5, 4, 3, 2, 1])
 
     def test_sort_key(self):
         data = ['apple', 'banana', 'cherry', 'date', 'elderberry']
-        result = Stream(data).sort(key=len).toList()
+        result = Stream(data).sort(sortedFunc=len).toList()
         self.assertEqual(result, ['date', 'apple', 'banana', 'cherry', 'elderberry'])
 
     def test_map(self):
         # 使用map操作将每个元素加倍
         result = Stream(globalData).map(lambda x: x * 2).toList()
         self.assertEqual(result, [2, 4, 6, 6, 8, 10])
```

### Comparing `suger-0.2.0/suger/common/FileCompareUtils.py` & `suger-0.2.1/suger/common/FileCompareUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/common/FileUtils.py` & `suger-0.2.1/suger/common/FileUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/common/ObjectUtils.py` & `suger-0.2.1/suger/common/ObjectUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/common/StringUtils.py` & `suger-0.2.1/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/data_operator/CsvUtils.py` & `suger-0.2.1/suger/data_operator/CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/data_operator/ExcelUtils.py` & `suger-0.2.1/suger/data_operator/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/data_operator/JsonUtils.py` & `suger-0.2.1/suger/data_operator/JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/data_operator/XmlUtils.py` & `suger-0.2.1/suger/data_operator/XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/decorator/csv_decorator.py` & `suger-0.2.1/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/stream/Stream.py` & `suger-0.2.1/suger/stream/Stream.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable, Iterable, Dict, Any, Set
 
 
 class Stream:
     def __init__(self, data: Iterable) -> None:
         self.data = data
 
-    def sort(self, key=None, reverse=False):
-        return Stream(sorted(self.data, key=key, reverse=reverse))
+    def sort(self, sortedFunc=None, reverse=False):
+        return Stream(sorted(self.data, key=sortedFunc, reverse=reverse))
 
     def map(self, func: Callable) -> "Stream":
         return Stream(func(item) for item in self.data)
 
     def flatMap(self, func: Callable) -> "Stream":
         return Stream(item for sublist in self.data for item in func(sublist))
```

### Comparing `suger-0.2.0/suger/terminal/SSH.py` & `suger-0.2.1/suger/terminal/SSH.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/suger/terminal/TerminalUtils.py` & `suger-0.2.1/suger/terminal/TerminalUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/tests/test_CsvUtils.py` & `suger-0.2.1/tests/test_CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/tests/test_ExcelUtils.py` & `suger-0.2.1/tests/test_ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/tests/test_JsonUtils.py` & `suger-0.2.1/tests/test_JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/tests/test_Stream.py` & `suger-0.2.1/tests/test_Stream.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,43 +5,45 @@
 globalData = [1, 2, 3, 3, 4, 5]
 
 
 class TestStream(TestCase):
 
     def test_demo(self):
         data = [1, 2, 3, 3, 4, 5]
-        result = Stream(data).filter(lambda x: x % 2 == 0) \
+
+        result = Stream(data)\
+            .filter(lambda x: x % 2 == 0) \
             .sort(reverse=True) \
             .map(lambda x: x * 2) \
             .toSet()
         self.assertEqual(result, {8, 4})
 
     def test_sort_numeric(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
-        result = Stream(data).sort(key=lambda x: x).toList()
+        result = Stream(data).sort(sortedFunc=lambda x: x).toList()
         self.assertEqual(result, [1, 2, 3, 4, 5, 6, 7, 8])
 
     def test_sort_numeric_reverse(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
-        result = Stream(data).sort(key=lambda x: x, reverse=True).toList()
+        result = Stream(data).sort(sortedFunc=lambda x: x, reverse=True).toList()
         self.assertEqual(result, [8, 7, 6, 5, 4, 3, 2, 1])
 
     def test_sort(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
         result = Stream(data).sort().toList()
         self.assertEqual(result, [1, 2, 3, 4, 5, 6, 7, 8])
 
     def test_sort_reverse(self):
         data = [5, 2, 8, 3, 1, 7, 4, 6]
         result = Stream(data).sort(reverse=True).toList()
         self.assertEqual(result, [8, 7, 6, 5, 4, 3, 2, 1])
 
     def test_sort_key(self):
         data = ['apple', 'banana', 'cherry', 'date', 'elderberry']
-        result = Stream(data).sort(key=len).toList()
+        result = Stream(data).sort(sortedFunc=len).toList()
         self.assertEqual(result, ['date', 'apple', 'banana', 'cherry', 'elderberry'])
 
     def test_map(self):
         # 使用map操作将每个元素加倍
         result = Stream(globalData).map(lambda x: x * 2).toList()
         self.assertEqual(result, [2, 4, 6, 6, 8, 10])
```

### Comparing `suger-0.2.0/tests/test_StringUtils.py` & `suger-0.2.1/tests/test_StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/tests/test_XmlUtils.py` & `suger-0.2.1/tests/test_XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/LICENSE` & `suger-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.2.0/README.md` & `suger-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # suger
 
-version = 0.2.0
+version = 0.2.1
 
 ## Introduce 介绍
 
 suger is a sugar ~ 
 
 use python with @decorator/@Annotation Like Java、C#、TypeScript 
 
@@ -25,15 +25,15 @@
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
-## Stream 流式计算 / from v0.2.0 
+## Stream 流式计算 / from v0.2.1 
 ```python
 from suger.stream.Stream import Stream
 
     def test_demo(self):
         data = [1, 2, 3, 3, 4, 5]
         result = Stream(data).filter(lambda x: x % 2 == 0) \
             .sort(reverse=True) \
```

### Comparing `suger-0.2.0/pyproject.toml` & `suger-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

### Comparing `suger-0.2.0/PKG-INFO` & `suger-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: suger
-Version: 0.2.0
+Version: 0.2.1
 Summary: suger is a sugar. use python in @decorator/@Annotation like other languages~
 Project-URL: Homepage, https://github.com/SolarisNeko/python-suger
 Project-URL: Bug Tracker, https://github.com/SolarisNeko/python-suger/issues
 Author-email: SolarisNeko <1417015340@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # suger
 
-version = 0.2.0
+version = 0.2.1
 
 ## Introduce 介绍
 
 suger is a sugar ~ 
 
 use python with @decorator/@Annotation Like Java、C#、TypeScript 
 
@@ -39,15 +39,15 @@
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
-## Stream 流式计算 / from v0.2.0 
+## Stream 流式计算 / from v0.2.1 
 ```python
 from suger.stream.Stream import Stream
 
     def test_demo(self):
         data = [1, 2, 3, 3, 4, 5]
         result = Stream(data).filter(lambda x: x % 2 == 0) \
             .sort(reverse=True) \
```

