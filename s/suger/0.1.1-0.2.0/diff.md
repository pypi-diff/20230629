# Comparing `tmp/suger-0.1.1.tar.gz` & `tmp/suger-0.2.0.tar.gz`

## Comparing `suger-0.1.1.tar` & `suger-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 suger-0.1.1/setup.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.1.1/upload.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.1.1/suger/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.1.1/suger/common/FileCompareUtils.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.1.1/suger/common/FileUtils.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.1.1/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 suger-0.1.1/suger/common/StringUtils.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.1.1/suger/common/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 suger-0.1.1/suger/data_operator/CsvUtils.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.1.1/suger/data_operator/ExcelUtils.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.1.1/suger/data_operator/JsonUtils.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.1.1/suger/data_operator/XmlUtils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.1.1/suger/data_operator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.1.1/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.1.1/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.1.1/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.1.1/suger/terminal/SSH.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.1.1/suger/terminal/TerminalUtils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.1.1/suger/terminal/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_CsvUtils.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_ExcelUtils.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_FileCompareUtils.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_FileUtils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_JsonUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_SSH.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_StringUtils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_TerminalUtils.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_XmlUtils.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 suger-0.1.1/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.1.1/tests/decorator/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.1.1/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.1.1/LICENSE
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 suger-0.1.1/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 suger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 suger-0.2.0/RoadMap.md
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 suger-0.2.0/setup.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.2.0/upload.sh
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 suger-0.2.0/安装.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.2.0/suger/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/FileUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.2.0/suger/common/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/CsvUtils.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/ExcelUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/JsonUtils.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/XmlUtils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.2.0/suger/data_operator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.2.0/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.2.0/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 suger-0.2.0/suger/stream/Stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/suger/stream/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.2.0/suger/terminal/SSH.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.2.0/suger/terminal/TerminalUtils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.2.0/suger/terminal/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_ExcelUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_SSH.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_Stream.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_StringUtils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_XmlUtils.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 suger-0.2.0/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.0/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 suger-0.2.0/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 suger-0.2.0/PKG-INFO
```

### Comparing `suger-0.1.1/suger/common/FileCompareUtils.py` & `suger-0.2.0/suger/common/FileCompareUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/common/FileUtils.py` & `suger-0.2.0/suger/common/FileUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/common/ObjectUtils.py` & `suger-0.2.0/suger/common/ObjectUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/common/StringUtils.py` & `suger-0.2.0/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/data_operator/CsvUtils.py` & `suger-0.2.0/suger/data_operator/CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/data_operator/ExcelUtils.py` & `suger-0.2.0/suger/data_operator/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/data_operator/JsonUtils.py` & `suger-0.2.0/suger/data_operator/JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/data_operator/XmlUtils.py` & `suger-0.2.0/suger/data_operator/XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/decorator/csv_decorator.py` & `suger-0.2.0/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/terminal/SSH.py` & `suger-0.2.0/suger/terminal/SSH.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/suger/terminal/TerminalUtils.py` & `suger-0.2.0/suger/terminal/TerminalUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/tests/test_CsvUtils.py` & `suger-0.2.0/tests/test_CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/tests/test_ExcelUtils.py` & `suger-0.2.0/tests/test_ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/tests/test_JsonUtils.py` & `suger-0.2.0/tests/test_JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/tests/test_StringUtils.py` & `suger-0.2.0/tests/test_StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/tests/test_XmlUtils.py` & `suger-0.2.0/tests/test_XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/LICENSE` & `suger-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.1.1/README.md` & `suger-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # suger
 
-version = 0.1.1
+version = 0.2.0
 
 ## Introduce 介绍
 
 suger is a sugar ~ 
 
 use python with @decorator/@Annotation Like Java、C#、TypeScript 
 
@@ -25,14 +25,27 @@
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
+## Stream 流式计算 / from v0.2.0 
+```python
+from suger.stream.Stream import Stream
+
+    def test_demo(self):
+        data = [1, 2, 3, 3, 4, 5]
+        result = Stream(data).filter(lambda x: x % 2 == 0) \
+            .sort(reverse=True) \
+            .map(lambda x: x * 2) \
+            .toSet()
+        self.assertEqual(result, {8, 4})
+
+```
 
 ## decorator 装饰器/注解
 ### @string | __str__
 ```python
 @string
 class MockData:
     def __init__(self, age):
```

### Comparing `suger-0.1.1/pyproject.toml` & `suger-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

### Comparing `suger-0.1.1/PKG-INFO` & `suger-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: suger
-Version: 0.1.1
+Version: 0.2.0
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
 
-version = 0.1.1
+version = 0.2.0
 
 ## Introduce 介绍
 
 suger is a sugar ~ 
 
 use python with @decorator/@Annotation Like Java、C#、TypeScript 
 
@@ -39,14 +39,27 @@
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
+## Stream 流式计算 / from v0.2.0 
+```python
+from suger.stream.Stream import Stream
+
+    def test_demo(self):
+        data = [1, 2, 3, 3, 4, 5]
+        result = Stream(data).filter(lambda x: x % 2 == 0) \
+            .sort(reverse=True) \
+            .map(lambda x: x * 2) \
+            .toSet()
+        self.assertEqual(result, {8, 4})
+
+```
 
 ## decorator 装饰器/注解
 ### @string | __str__
 ```python
 @string
 class MockData:
     def __init__(self, age):
```

