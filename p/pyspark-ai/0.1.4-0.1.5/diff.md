# Comparing `tmp/pyspark_ai-0.1.4.tar.gz` & `tmp/pyspark_ai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_ai-0.1.4.tar", max compression
+gzip compressed data, was "pyspark_ai-0.1.5.tar", max compression
```

## Comparing `pyspark_ai-0.1.4.tar` & `pyspark_ai-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.4/LICENSE
--rw-r--r--   0        0        0     3735 2023-06-24 22:36:00.071711 pyspark_ai-0.1.4/README.md
--rw-r--r--   0        0        0      978 2023-06-28 00:17:47.823398 pyspark_ai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.4/pyspark_ai/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.4/pyspark_ai/ai_utils.py
--rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.4/pyspark_ai/cache.py
--rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.4/pyspark_ai/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.4/pyspark_ai/file_cache.py
--rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.4/pyspark_ai/llm_chain_with_cache.py
--rw-r--r--   0        0        0     9237 2023-06-27 23:52:32.149278 pyspark_ai-0.1.4/pyspark_ai/prompt.py
--rw-r--r--   0        0        0    17498 2023-06-25 04:04:32.148887 pyspark_ai-0.1.4/pyspark_ai/pyspark_ai.py
--rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.4/pyspark_ai/search_tool_with_cache.py
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 pyspark_ai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3774 2023-06-29 05:42:50.986345 pyspark_ai-0.1.5/README.md
+-rw-r--r--   0        0        0      978 2023-06-29 05:47:29.563933 pyspark_ai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.5/pyspark_ai/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.5/pyspark_ai/ai_utils.py
+-rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.5/pyspark_ai/cache.py
+-rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.5/pyspark_ai/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.5/pyspark_ai/file_cache.py
+-rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.5/pyspark_ai/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     9288 2023-06-28 23:32:33.674290 pyspark_ai-0.1.5/pyspark_ai/prompt.py
+-rw-r--r--   0        0        0    17555 2023-06-29 00:12:04.660577 pyspark_ai-0.1.5/pyspark_ai/pyspark_ai.py
+-rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.5/pyspark_ai/search_tool_with_cache.py
+-rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 pyspark_ai-0.1.5/PKG-INFO
```

### Comparing `pyspark_ai-0.1.4/LICENSE` & `pyspark_ai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/README.md` & `pyspark_ai-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# English SDK for Apache Spark
-
 <div align="center">
+
+![English SDK for Apache Spark](./docs/_static/english-sdk-spark.svg)
 <h2>
 English is the new programming language;<br />
 Generative AI is the new compiler;<br />
 Python is ... the new byte code.
 </h2>
 </div>
```

### Comparing `pyspark_ai-0.1.4/pyproject.toml` & `pyspark_ai-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyspark-ai"
-version = "0.1.4"
+version = "0.1.5"
 description = "English SDK for Apache Spark"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/databrickslabs/pyspark-ai"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyspark_ai-0.1.4/pyspark_ai/ai_utils.py` & `pyspark_ai-0.1.5/pyspark_ai/ai_utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/pyspark_ai/cache.py` & `pyspark_ai-0.1.5/pyspark_ai/cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/pyspark_ai/code_logger.py` & `pyspark_ai-0.1.5/pyspark_ai/code_logger.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/pyspark_ai/file_cache.py` & `pyspark_ai-0.1.5/pyspark_ai/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/pyspark_ai/llm_chain_with_cache.py` & `pyspark_ai-0.1.5/pyspark_ai/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/pyspark_ai/prompt.py` & `pyspark_ai-0.1.5/pyspark_ai/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 VERIFY_TEMPLATE = """
 Given 1) a PySpark dataframe, df, and 2) a description of expected properties, desc,
 generate a Python function to test whether the given dataframe satisfies the expected properties.
 Your generated function should take 1 parameter, df, and the return type should be a boolean.
 You will call the function, passing in df as the parameter, and return the output (True/False).
 
 In total, your output must follow the format below, exactly (no explanation words):
-1. function definition f, in Python
+1. function definition f, in Python (Do NOT surround the function definition with quotes)
 2. 1 blank new line
 3. Call f on df and assign the result to a variable, result: result = name_of_f(df)
 
 Include any necessary import statements INSIDE the function definition.
 For example:
 def gen_random():
     import random
@@ -158,25 +158,25 @@
 
 For example:
 Input:
 df = DataFrame[name: string, age: int]
 desc = "expect 5 columns"
 
 Output:
-"def has_5_columns(df) -> bool:
+def has_5_columns(df) -> bool:
     # Get the number of columns in the DataFrame
     num_columns = len(df.columns)
 
     # Check if the number of columns is equal to 5
     if num_columns == 5:
         return True
     else:
         return False
 
-result = has_5_columns(df)"
+result = has_5_columns(df)
 
 Here is your input df: {df}
 Here is your input description: {desc}
 """
 
 VERIFY_PROMPT = PromptTemplate(input_variables=["df", "desc"], template=VERIFY_TEMPLATE)
 
@@ -187,15 +187,15 @@
 and by default returns a String (although it can return any data type). 
 The point is to reuse a function on several dataframes and SQL functions.
 
 Given 1) input arguments, 2) a description of the udf functionality,
 3) the udf return type, and 4) the udf function name, 
 generate and return a callable udf.
         
-Return ONLY the callable resulting udf function (no explanation words). 
+Return ONLY the callable resulting udf function (no explanation words).
 Include any necessary import statements INSIDE the function definition.
 For example:
 def gen_random():
     import random
     return random.randint(0, 10)
 """
```

### Comparing `pyspark_ai-0.1.4/pyspark_ai/pyspark_ai.py` & `pyspark_ai-0.1.5/pyspark_ai/pyspark_ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         " (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
         "Accept-Language": "en-US,en;q=0.5",
     }
 
     def __init__(
         self,
-        llm: BaseLanguageModel = ChatOpenAI(model_name='gpt-4', temperature=0),
+        llm: Optional[BaseLanguageModel] = None,
         web_search_tool: Optional[Callable[[str], str]] = None,
         spark_session: Optional[SparkSession] = None,
         enable_cache: bool = True,
         cache_file_format: str = "json",
         cache_file_location: Optional[str] = None,
         encoding: Optional[Encoding] = None,
         max_tokens_of_web_content: int = 3000,
@@ -60,14 +60,16 @@
         :param web_search_tool: optional function to perform web search,
                                 Google search will be used if not provided
         :param spark_session: optional SparkSession, a new one will be created if not provided
         :param encoding: optional Encoding, cl100k_base will be used if not provided
         :param max_tokens_of_web_content: maximum tokens of web content after encoding
         """
         self._spark = spark_session or SparkSession.builder.getOrCreate()
+        if llm is None:
+            llm = ChatOpenAI(model_name='gpt-4', temperature=0)
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
         if enable_cache:
             self._enable_cache = enable_cache
             if cache_file_location is not None:
                 # if there is parameter setting for it, use the parameter
                 self._cache_file_location = cache_file_location
```

### Comparing `pyspark_ai-0.1.4/pyspark_ai/search_tool_with_cache.py` & `pyspark_ai-0.1.5/pyspark_ai/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.4/PKG-INFO` & `pyspark_ai-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-ai
-Version: 0.1.4
+Version: 0.1.5
 Summary: English SDK for Apache Spark
 Home-page: https://github.com/databrickslabs/pyspark-ai
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -22,17 +22,17 @@
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (==0.4.0)
 Description-Content-Type: text/markdown
 
-# English SDK for Apache Spark
-
 <div align="center">
+
+![English SDK for Apache Spark](./docs/_static/english-sdk-spark.svg)
 <h2>
 English is the new programming language;<br />
 Generative AI is the new compiler;<br />
 Python is ... the new byte code.
 </h2>
 </div>
```

