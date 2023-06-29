# Comparing `tmp/dlai-grader-1.8.0.tar.gz` & `tmp/dlai-grader-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlai-grader-1.8.0.tar", last modified: Tue Feb  7 22:30:07 2023, max compression
+gzip compressed data, was "dlai-grader-1.9.0.tar", last modified: Thu Jun 29 16:00:19 2023, max compression
```

## Comparing `dlai-grader-1.8.0.tar` & `dlai-grader-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 andreszarta   (504) staff       (20)        0 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/
--rw-r--r--   0 andreszarta   (504) staff       (20)     1072 2022-04-13 19:30:14.000000 dlai-grader-1.8.0/LICENSE
--rw-r--r--   0 andreszarta   (504) staff       (20)     8564 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/PKG-INFO
--rw-r--r--   0 andreszarta   (504) staff       (20)     8102 2022-06-21 16:42:26.000000 dlai-grader-1.8.0/README.md
-drwxr-xr-x   0 andreszarta   (504) staff       (20)        0 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader/
--rw-r--r--   0 andreszarta   (504) staff       (20)      210 2023-02-07 22:27:45.000000 dlai-grader-1.8.0/dlai_grader/__init__.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     4369 2023-02-01 20:10:29.000000 dlai-grader-1.8.0/dlai_grader/cli.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     1315 2022-05-24 15:47:11.000000 dlai-grader-1.8.0/dlai_grader/compiler.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     1638 2022-06-08 19:25:57.000000 dlai-grader-1.8.0/dlai_grader/config.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     3376 2022-09-08 16:01:21.000000 dlai-grader-1.8.0/dlai_grader/grading.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     7529 2022-06-16 21:49:38.000000 dlai-grader-1.8.0/dlai_grader/io.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     8599 2023-02-07 22:21:50.000000 dlai-grader-1.8.0/dlai_grader/notebook.py
--rw-r--r--   0 andreszarta   (504) staff       (20)     4119 2022-06-16 21:50:42.000000 dlai-grader-1.8.0/dlai_grader/templates.py
--rw-r--r--   0 andreszarta   (504) staff       (20)      335 2022-05-31 21:09:08.000000 dlai-grader-1.8.0/dlai_grader/types.py
-drwxr-xr-x   0 andreszarta   (504) staff       (20)        0 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/
--rw-r--r--   0 andreszarta   (504) staff       (20)     8564 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/PKG-INFO
--rw-r--r--   0 andreszarta   (504) staff       (20)      438 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/SOURCES.txt
--rw-r--r--   0 andreszarta   (504) staff       (20)        1 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/dependency_links.txt
--rw-r--r--   0 andreszarta   (504) staff       (20)       72 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/entry_points.txt
--rw-r--r--   0 andreszarta   (504) staff       (20)       33 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/requires.txt
--rw-r--r--   0 andreszarta   (504) staff       (20)       12 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/dlai_grader.egg-info/top_level.txt
--rw-r--r--   0 andreszarta   (504) staff       (20)       38 2023-02-07 22:30:07.000000 dlai-grader-1.8.0/setup.cfg
--rw-r--r--   0 andreszarta   (504) staff       (20)      855 2023-02-07 22:29:45.000000 dlai-grader-1.8.0/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-29 16:00:19.267134 dlai-grader-1.9.0/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1072 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/LICENSE
+-rw-rw-r--   0 andres    (1000) andres    (1000)     8544 2023-06-29 16:00:19.263134 dlai-grader-1.9.0/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)     8102 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/README.md
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-29 16:00:19.263134 dlai-grader-1.9.0/dlai_grader/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      210 2023-06-29 15:57:58.000000 dlai-grader-1.9.0/dlai_grader/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     4369 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/cli.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1315 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/compiler.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1638 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/config.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3376 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/grading.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7529 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/io.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     9248 2023-06-29 15:57:48.000000 dlai-grader-1.9.0/dlai_grader/notebook.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     4119 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/templates.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      335 2023-06-29 15:44:16.000000 dlai-grader-1.9.0/dlai_grader/types.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-29 16:00:19.263134 dlai-grader-1.9.0/dlai_grader.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     8544 2023-06-29 16:00:19.000000 dlai-grader-1.9.0/dlai_grader.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      438 2023-06-29 16:00:19.000000 dlai-grader-1.9.0/dlai_grader.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-29 16:00:19.000000 dlai-grader-1.9.0/dlai_grader.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       71 2023-06-29 16:00:19.000000 dlai-grader-1.9.0/dlai_grader.egg-info/entry_points.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       33 2023-06-29 16:00:19.000000 dlai-grader-1.9.0/dlai_grader.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2023-06-29 16:00:19.000000 dlai-grader-1.9.0/dlai_grader.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-29 16:00:19.267134 dlai-grader-1.9.0/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      855 2023-06-29 15:58:03.000000 dlai-grader-1.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dlai-grader-1.8.0/LICENSE` & `dlai-grader-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/PKG-INFO` & `dlai-grader-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dlai-grader
-Version: 1.8.0
+Version: 1.9.0
 Summary: Grading utilities for DLAI courses
 Home-page: https://github.com/https-deeplearning-ai/grader
 Author: Andres Zarta
 Author-email: andrezb5@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # grader
@@ -179,9 +178,7 @@
 new_y = 7.0
 prediction = model.predict([new_y])[0]
 print(prediction)
 ```
 
 ## Download the assignment
 
-
-
```

### Comparing `dlai-grader-1.8.0/README.md` & `dlai-grader-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader/cli.py` & `dlai-grader-1.9.0/dlai_grader/cli.py`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader/compiler.py` & `dlai-grader-1.9.0/dlai_grader/compiler.py`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader/config.py` & `dlai-grader-1.9.0/dlai_grader/config.py`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader/grading.py` & `dlai-grader-1.9.0/dlai_grader/grading.py`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader/io.py` & `dlai-grader-1.9.0/dlai_grader/io.py`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader/notebook.py` & `dlai-grader-1.9.0/dlai_grader/notebook.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,14 +112,33 @@
 
         notebook["cells"] = filtered_cells
         return notebook
 
     return inner
 
 
+def partial_grading_enabled(
+    notebook: NotebookNode,
+    regex_pattern: str = "(grade)(.|[ \t]*)(up)(.|[ \t]*)(to)(.|[ \t]*)(here)",
+) -> bool:
+    """Checks for the existence of the partial grading tag.
+
+    Args:
+        notebook (NotebookNode): The notebook from the learner.
+        regex_pattern (str, optional): Pattern to check. Defaults to "(grade)(.|[ \t]*)(up)(.|[ \t]*)(to)(.|[ \t]*)(here)".
+
+    Returns:
+        bool: True if the pattern if found, False otherwise.
+    """
+    for cell in notebook["cells"]:
+        if cell["cell_type"] == "code" and re.search(regex_pattern, cell["source"]):
+            return True
+    return False
+
+
 def get_named_cells(
     notebook: NotebookNode,
 ) -> dict:
     """Returns the named cells for cases when grading is done using cell's output.
     Args:
         notebook (NotebookNode): The notebook from the learner.
     Returns:
@@ -145,17 +164,15 @@
         tag (str): The tag to include in the code cell's metadata. Defaults to "graded".
     Returns:
         NotebookNode: The filtered notebook.
     """
     filtered_cells = []
 
     for cell in notebook["cells"]:
-
         if cell["cell_type"] == "code":
-
             if not "tags" in cell["metadata"]:
                 cell["metadata"]["tags"] = []
 
             tags = cell["metadata"]["tags"]
 
             if not tag in tags:
                 tags.append(tag)
@@ -246,15 +263,14 @@
 
     code_block = False
     omit_block = False
 
     formatted_lines = []
 
     for ln in cell_code.splitlines():
-
         if tag_start in ln:
             code_block = True
 
         if tag_end in ln:
             code_block = False
 
         if tag_start_omit_block in ln:
@@ -280,15 +296,14 @@
         if tag_keep in ln:
             splitted = ln.split(f"# {tag_keep}")
             new_ln = splitted[0]
             formatted_lines.append(new_ln)
             continue
 
         if (tag_start not in ln) and code_block:
-
             if tag_replace_equals in ln:
                 splitted = ln.split(tag_replace_equals)
                 new_val = splitted[1]
                 splitted_eq = splitted[0].split("=")
                 new_ln = splitted_eq[0] + "=" + new_val
                 formatted_lines.append(new_ln)
                 continue
```

### Comparing `dlai-grader-1.8.0/dlai_grader/templates.py` & `dlai-grader-1.9.0/dlai_grader/templates.py`

 * *Files identical despite different names*

### Comparing `dlai-grader-1.8.0/dlai_grader.egg-info/PKG-INFO` & `dlai-grader-1.9.0/dlai_grader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dlai-grader
-Version: 1.8.0
+Version: 1.9.0
 Summary: Grading utilities for DLAI courses
 Home-page: https://github.com/https-deeplearning-ai/grader
 Author: Andres Zarta
 Author-email: andrezb5@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # grader
@@ -179,9 +178,7 @@
 new_y = 7.0
 prediction = model.predict([new_y])[0]
 print(prediction)
 ```
 
 ## Download the assignment
 
-
-
```

### Comparing `dlai-grader-1.8.0/setup.py` & `dlai-grader-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="dlai-grader",
-    version="1.8.0",
+    version="1.9.0",
     description="Grading utilities for DLAI courses",
     url="https://github.com/https-deeplearning-ai/grader",
     author="Andres Zarta",
     author_email="andrezb5@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT License",
```

