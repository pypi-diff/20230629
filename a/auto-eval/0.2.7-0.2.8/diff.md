# Comparing `tmp/auto-eval-0.2.7.tar.gz` & `tmp/auto-eval-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.7.tar", last modified: Tue Jun 27 06:40:23 2023, max compression
+gzip compressed data, was "auto-eval-0.2.8.tar", last modified: Thu Jun 29 07:44:40 2023, max compression
```

## Comparing `auto-eval-0.2.7.tar` & `auto-eval-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.955586 auto-eval-0.2.7/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.7/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-27 06:40:23.955322 auto-eval-0.2.7/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.2.7/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.952563 auto-eval-0.2.7/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.953132 auto-eval-0.2.7/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.7/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.7/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.953606 auto-eval-0.2.7/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.7/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.7/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.954511 auto-eval-0.2.7/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.7/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.2.7/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2418 2023-06-27 06:37:14.000000 auto-eval-0.2.7/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.954962 auto-eval-0.2.7/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.7/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4152 2023-06-13 06:59:50.000000 auto-eval-0.2.7/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-27 06:40:23.955629 auto-eval-0.2.7/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-27 06:40:14.000000 auto-eval-0.2.7/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.326116 auto-eval-0.2.8/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.8/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-29 07:44:40.325723 auto-eval-0.2.8/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.2.8/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.322790 auto-eval-0.2.8/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.323333 auto-eval-0.2.8/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.8/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.8/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.324002 auto-eval-0.2.8/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.8/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.8/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.325067 auto-eval-0.2.8/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.8/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.2.8/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.2.8/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.325493 auto-eval-0.2.8/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.8/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.2.8/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-29 07:44:40.326206 auto-eval-0.2.8/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-29 07:44:30.000000 auto-eval-0.2.8/setup.py
```

### Comparing `auto-eval-0.2.7/LICENSE` & `auto-eval-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.7/PKG-INFO` & `auto-eval-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.7
+Version: 0.2.8
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.2.7/README.md` & `auto-eval-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.7/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.8/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.7
+Version: 0.2.8
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.2.7/eval/auto_llms_eval.py` & `auto-eval-0.2.8/eval/auto_llms_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.7/eval/commands/auto_eval.py` & `auto-eval-0.2.8/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.7/eval/prompt_template/prompter.py` & `auto-eval-0.2.8/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.7/eval/prompt_template/prompts.py` & `auto-eval-0.2.8/eval/prompt_template/prompts.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```
 
 Candidate answers:
 ```text
 {answers}
 ```
 
-Please evaluate each candidate's answer based on its accuracy, professionalism, and ability to provide necessary information without being too verbose.
+Please first answer the question independently without referring to candidate answers to obtain the correct answer, then evaluate each candidate's answer based on its accuracy, professionalism, and ability to provide necessary information without being too verbose.
 Then assign a rating score between 0-1 along with brief comments.
 Finally, output all [Candidate answers] scores in JSON format: {{"number": "{{score}}"}}.
 """
 
 
 EVAL_WITH_TARGET_TEMPLATE_ECOMMERCE = """
 The following text contains a question along with some context and sevaral candidate answers. A reference answer is also provided for comparison purposes.
@@ -75,12 +75,12 @@
 ```
 
 Candidate answers:
 ```text
 {answers}
 ```
 
-Please evaluate each candidate's answer based on its accuracy, professionalism, and ability to provide necessary information without being too verbose.
+Please first answer the question independently without referring to candidate answers to obtain the correct answer, then evaluate each candidate's answer based on its accuracy, professionalism, and ability to provide necessary information without being too verbose.
 Then assign a rating score between -1 and 1 along with brief comments.
 Finally, output all [Candidate answers] scores in JSON format: {{"number": "{{score}}"}}.
 """
```

### Comparing `auto-eval-0.2.7/eval/utils/data_utils.py` & `auto-eval-0.2.8/eval/utils/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,16 +62,17 @@
 def extract_scores(text) -> float:
     pattern = r"([A-Z])['\"]?[:.]\s*([\d.]+|\"[\d.]+\")"
     result = re.findall(pattern, text)
     scores = {item[0]: float(item[1].replace("\"", "")) for item in result}    
     return scores 
 
 def extract_numbers(text):
-    numbers = re.findall(r'\d+', text)
-    numbers = [float(number) for number in numbers]
+    pattern = r"[-+]?\d*\.\d+|\d+"
+    result = re.findall(pattern, text)
+    return [float(i) if '.' in i else int(i) for i in result]
 
 
 def df2xlsx(df: pd.DataFrame, save_path: str, sheet_name='Sheet1', mode='w', index=False):
     if mode not in ['w', 'a']:
         raise AssertionError('mode not in [\'w\', \'a\']')
     if mode == 'a' and not os.path.isfile(save_path):
         mode = 'w'
```

### Comparing `auto-eval-0.2.7/setup.py` & `auto-eval-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

