# Comparing `tmp/fortext-0.0.3.tar.gz` & `tmp/fortext-0.0.4.tar.gz`

## Comparing `fortext-0.0.3.tar` & `fortext-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fortext-0.0.3/requirements.txt
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 fortext-0.0.3/img/syntax_highlighting.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/__init__.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/ansi.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/permutation.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/style.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/syntax.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fortext-0.0.3/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fortext-0.0.3/LICENSE
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 fortext-0.0.3/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fortext-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fortext-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fortext-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 fortext-0.0.4/img/syntax_highlighting.png
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fortext-0.0.4/src/fortext/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 fortext-0.0.4/src/fortext/ansi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fortext-0.0.4/src/fortext/permutation.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 fortext-0.0.4/src/fortext/style.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 fortext-0.0.4/src/fortext/syntax.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fortext-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fortext-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 fortext-0.0.4/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fortext-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 fortext-0.0.4/PKG-INFO
```

### Comparing `fortext-0.0.3/img/syntax_highlighting.png` & `fortext-0.0.4/img/syntax_highlighting.png`

 * *Files identical despite different names*

### Comparing `fortext-0.0.3/src/fortext/ansi.py` & `fortext-0.0.4/src/fortext/ansi.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.3/src/fortext/permutation.py` & `fortext-0.0.4/src/fortext/permutation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from itertools import permutations
+from itertools import permutations as _permutations
 from typing import Generator
 
 
-def string_permutations(string: str,
-                        max_len: int = None) -> Generator[str, None, None]:
+def permutations(string: str,
+                 max_len: int = None) -> Generator[str, None, None]:
     """Generates all permutations of a string.
 
     Args:
         string (str): String to permute.
         max_len (int, optional): Maximum length of permutations. Defaults to length of the string.
 
     Yields:
         str: Permutations of the string.
     """
     if max_len is None:
         max_len = len(string)
 
     for i in range(1, max_len + 1):
-        for p in permutations(string, i):
+        for p in _permutations(string, i):
             yield ''.join(p)
```

### Comparing `fortext-0.0.3/src/fortext/style.py` & `fortext-0.0.4/src/fortext/style.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.3/src/fortext/syntax.py` & `fortext-0.0.4/src/fortext/syntax.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.3/.gitignore` & `fortext-0.0.4/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,10 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# manually added
+token.txt
```

### Comparing `fortext-0.0.3/LICENSE` & `fortext-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fortext-0.0.3/README.md` & `fortext-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,37 +48,40 @@
 ```
 
 ## Usage
 
 ### Text styling
 
 ```python
+from fortext import style, Bg, Frmt
 print(style('Hi, human.', fg='#ff0000'))
 print(style('RGB tuple or list also works.', fg=(0, 255, 0)))
 print(style('You can also use predefined colors.', bg=Bg.BLACK))
 print(style('Want to be bold?.', frmt=[Frmt.BOLD]))
 
 print(
     style('Want to go all in?',
           fg='#ff0000', bg=Bg.BLACK,
           frmt=[Frmt.BOLD, Frmt.UNDERLINE, Frmt.ITALIC]))
 ```
 
 ### Syntax highlighting
 
 ```python
+from fortext import highlight
 print(highlight({'somekey': 'somevalue', 'anotherkey': [12.4, True, 23]}))
 ```
 Output:
 
 ![syntax highlighting example output](./img/syntax_highlighting.png)
 
 ### Permutations
 ```python
-for perm in string_permutations('abc'):
+from fortext import permutations
+for perm in permutations('abc'):
     print(perm)
 ```
 Output:
 ```
 a
 b
 c
```

### Comparing `fortext-0.0.3/pyproject.toml` & `fortext-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fortext"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="4MBL" },
 ]
 description = "Text stylizer for Python. Mainly useful for CLI output."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `fortext-0.0.3/PKG-INFO` & `fortext-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortext
-Version: 0.0.3
+Version: 0.0.4
 Summary: Text stylizer for Python. Mainly useful for CLI output.
 Project-URL: Homepage, https://github.com/4MBL/fortext
 Project-URL: Bug Tracker, https://github.com/4MBL/fortext/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
@@ -83,37 +83,40 @@
 ```
 
 ## Usage
 
 ### Text styling
 
 ```python
+from fortext import style, Bg, Frmt
 print(style('Hi, human.', fg='#ff0000'))
 print(style('RGB tuple or list also works.', fg=(0, 255, 0)))
 print(style('You can also use predefined colors.', bg=Bg.BLACK))
 print(style('Want to be bold?.', frmt=[Frmt.BOLD]))
 
 print(
     style('Want to go all in?',
           fg='#ff0000', bg=Bg.BLACK,
           frmt=[Frmt.BOLD, Frmt.UNDERLINE, Frmt.ITALIC]))
 ```
 
 ### Syntax highlighting
 
 ```python
+from fortext import highlight
 print(highlight({'somekey': 'somevalue', 'anotherkey': [12.4, True, 23]}))
 ```
 Output:
 
 ![syntax highlighting example output](./img/syntax_highlighting.png)
 
 ### Permutations
 ```python
-for perm in string_permutations('abc'):
+from fortext import permutations
+for perm in permutations('abc'):
     print(perm)
 ```
 Output:
 ```
 a
 b
 c
```

