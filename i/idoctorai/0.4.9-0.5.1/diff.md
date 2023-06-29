# Comparing `tmp/idoctorai-0.4.9.tar.gz` & `tmp/idoctorai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.4.9.tar", max compression
+gzip compressed data, was "idoctorai-0.5.1.tar", max compression
```

## Comparing `idoctorai-0.4.9.tar` & `idoctorai-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.9/LICENSE
--rw-r--r--   0        0        0    20610 2023-06-17 08:34:36.128691 idoctorai-0.4.9/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.9/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.9/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.9/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.9/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.9/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.9/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.9/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.9/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.9/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.9/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.9/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.9/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.9/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.9/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.9/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.9/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.4.9/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.9/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.9/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.9/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.9/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.9/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1732 2023-06-17 06:36:26.292817 idoctorai-0.4.9/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.9/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1597 2023-06-17 06:36:37.045220 idoctorai-0.4.9/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1480 2023-06-17 08:34:41.459497 idoctorai-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.9/README.md
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.5.1/LICENSE
+-rw-r--r--   0        0        0    20905 2023-06-29 10:03:27.224271 idoctorai-0.5.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.5.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.5.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.5.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.5.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.5.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.5.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.5.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.5.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.5.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.5.1/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.5.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.5.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.5.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.5.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.5.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.5.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.5.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.5.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.5.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.5.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.5.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.5.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.5.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.5.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1606 2023-06-19 11:43:16.346788 idoctorai-0.5.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1480 2023-06-29 10:04:47.973917 idoctorai-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.5.1/README.md
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.5.1/PKG-INFO
```

### Comparing `idoctorai-0.4.9/LICENSE` & `idoctorai-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/__init__.py` & `idoctorai-0.5.1/pandasai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     """
 
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
-    _max_retries: int = 3
+    _max_retries: int = 1
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "df_columns": None,
         "num_rows": None,
         "num_columns": None,
@@ -231,14 +231,15 @@
                     heads = [
                         anonymize_dataframe_head(dataframe)
                         if anonymize_df
                         else dataframe.head(rows_to_display)
                         for dataframe in data_frame
                     ]
 
+
                     code = self._llm.generate_code(
                         MultipleDataframesPrompt(dataframes=heads),
                         prompt,
                         history,
                     )
 
                     self._original_instructions = {
@@ -310,14 +311,26 @@
             self.last_error = str(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
 
+    def original_chat(self,prompt: str,history: list = None) -> str:
+        """
+        Returns the original chat between the user and the AI.
+
+        Returns (str): Original Chat
+
+        """
+        
+        answer  = self._llm.langchain_input(prompt, history)
+
+        return answer
+    
     def clear_cache(self):
         """
         Clears the cache of the PandasAI instance.
         """
         self._cache.clear()
 
     def __call__(
@@ -491,47 +504,44 @@
             while count < self._max_retries:
                 try:
                     # Execute the code
                     exec(code_to_run, environment)
                     code = code_to_run
                     break
                 except Exception as e:  # pylint: disable=W0718 disable=C0103
-                    if not use_error_correction_framework:
-                        raise e
+                    raise e
 
-                    count += 1
+                    # count += 1
 
-                    if multiple:
-                        error_correcting_instruction = (
-                            CorrectMultipleDataframesErrorPrompt(
-                                code=code,
-                                error_returned=e,
-                                question=self._original_instructions["question"],
-                                df_head=self._original_instructions["df_head"],
-                            )
-                        )
-
-                    else:
-                        error_correcting_instruction = CorrectErrorPrompt(
-                            code=code,
-                            error_returned=e,
-                            question=self._original_instructions["question"],
-                            df_head=self._original_instructions["df_head"],
-                            df_columns=self._original_instructions["df_columns"],
-                            num_rows=self._original_instructions["num_rows"],
-                            num_columns=self._original_instructions["num_columns"],
-                            rows_to_display=self._original_instructions[
-                                "rows_to_display"
-                            ],
-                        )
-
-                    print(error_correcting_instruction.text)
-                    code_to_run = self._llm.generate_code(
-                        error_correcting_instruction, "", self._history
-                    )
+                    # if multiple:
+                    #     error_correcting_instruction = (
+                    #         CorrectMultipleDataframesErrorPrompt(
+                    #             code=code,
+                    #             error_returned=e,
+                    #             question=self._original_instructions["question"],
+                    #             df_head=self._original_instructions["df_head"],
+                    #         )
+                    #     )
+                    # else:
+                    #     error_correcting_instruction = CorrectErrorPrompt(
+                    #         code=code,
+                    #         error_returned=e,
+                    #         question=self._original_instructions["question"],
+                    #         df_head=self._original_instructions["df_head"],
+                    #         df_columns=self._original_instructions["df_columns"],
+                    #         num_rows=self._original_instructions["num_rows"],
+                    #         num_columns=self._original_instructions["num_columns"],
+                    #         rows_to_display=self._original_instructions[
+                    #             "rows_to_display"
+                    #         ],
+                    #     )
+                    # # print(error_correcting_instruction.text)
+                    # code_to_run = self._llm.generate_code(
+                    #     error_correcting_instruction, "", self._history
+                    # )
 
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
```

### Comparing `idoctorai-0.4.9/pandasai/constants.py` & `idoctorai-0.5.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/exceptions.py` & `idoctorai-0.5.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/helpers/_optional.py` & `idoctorai-0.5.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/helpers/anonymizer.py` & `idoctorai-0.5.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/helpers/cache.py` & `idoctorai-0.5.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/helpers/from_excel.py` & `idoctorai-0.5.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/helpers/notebook.py` & `idoctorai-0.5.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/helpers/save_chart.py` & `idoctorai-0.5.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/langchain/__init__.py` & `idoctorai-0.5.1/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/llm/azure_openai.py` & `idoctorai-0.5.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/llm/base.py` & `idoctorai-0.5.1/pandasai/llm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,14 @@
       
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
     
     def langchain_input(self, value:str, history:list = None) -> str:
         response = self.langchain.__call__(value, history)
-        print(response)
         return response
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
 
     LLM base class is extended to be used with HuggingFace LLM Modes APIs
```

### Comparing `idoctorai-0.4.9/pandasai/llm/fake.py` & `idoctorai-0.5.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/llm/google_palm.py` & `idoctorai-0.5.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/llm/open_assistant.py` & `idoctorai-0.5.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/llm/openai.py` & `idoctorai-0.5.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/llm/starcoder.py` & `idoctorai-0.5.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/prompts/base.py` & `idoctorai-0.5.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.5.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.5.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/prompts/generate_python_code.py` & `idoctorai-0.5.1/pandasai/prompts/generate_python_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
 When asked about the data, your response should include a python code(no duplicate) that describes the dataframe `df`.
-Don't add too many code comments.The result must be output at the end.
+Don't add too many code comments.The result must be printed at the end of code.
 Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
             START_CODE_TAG=START_CODE_TAG,
```

### Comparing `idoctorai-0.4.9/pandasai/prompts/generate_response.py` & `idoctorai-0.5.1/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.9/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.5.1/pandasai/prompts/multiple_dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
-Don't add too many code comments.The result must be output at the end.
+Don't add too many code comments.The result must be printed at the end of code.
 Using the provided dataframes and no other dataframes, return the python code(no duplicate) and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
```

### Comparing `idoctorai-0.4.9/pyproject.toml` & `idoctorai-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.4.9"
+version = "0.5.1"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"},{include="pyproject.toml"}]
```

### Comparing `idoctorai-0.4.9/PKG-INFO` & `idoctorai-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.4.9
+Version: 0.5.1
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

