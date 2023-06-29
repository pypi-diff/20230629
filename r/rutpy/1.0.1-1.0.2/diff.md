# Comparing `tmp/rutpy-1.0.1.tar.gz` & `tmp/rutpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutpy-1.0.1.tar", last modified: Mon Jun  5 02:55:21 2023, max compression
+gzip compressed data, was "rutpy-1.0.2.tar", last modified: Thu Jun 29 09:07:22 2023, max compression
```

## Comparing `rutpy-1.0.1.tar` & `rutpy-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:55:21.273735 rutpy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 02:55:21.273735 rutpy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-05 02:55:10.000000 rutpy-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-05 02:55:10.000000 rutpy-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:55:21.273735 rutpy-1.0.1/rutpy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 02:55:10.000000 rutpy-1.0.1/rutpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:55:21.273735 rutpy-1.0.1/rutpy/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 02:55:10.000000 rutpy-1.0.1/rutpy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-05 02:55:10.000000 rutpy-1.0.1/rutpy/core/rut.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 02:55:10.000000 rutpy-1.0.1/rutpy/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:55:21.273735 rutpy-1.0.1/rutpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 02:55:21.000000 rutpy-1.0.1/rutpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 02:55:21.000000 rutpy-1.0.1/rutpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 02:55:21.000000 rutpy-1.0.1/rutpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 02:55:21.000000 rutpy-1.0.1/rutpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 02:55:21.273735 rutpy-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:22.004213 rutpy-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 09:07:22.004213 rutpy-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-29 09:06:58.000000 rutpy-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 09:06:58.000000 rutpy-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:22.000213 rutpy-1.0.2/rutpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 09:06:58.000000 rutpy-1.0.2/rutpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:22.004213 rutpy-1.0.2/rutpy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:06:58.000000 rutpy-1.0.2/rutpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-29 09:06:58.000000 rutpy-1.0.2/rutpy/core/rut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 09:06:58.000000 rutpy-1.0.2/rutpy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:22.000213 rutpy-1.0.2/rutpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 09:07:21.000000 rutpy-1.0.2/rutpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-29 09:07:21.000000 rutpy-1.0.2/rutpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:07:21.000000 rutpy-1.0.2/rutpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 09:07:21.000000 rutpy-1.0.2/rutpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:07:22.004213 rutpy-1.0.2/setup.cfg
```

### Comparing `rutpy-1.0.1/README.md` & `rutpy-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Rut.py
 
-RutPy is a Python library for handling Chilean RUTs (Rol Único Tributario). It provides functions to clean, validate, get the check digit, format, and generate RUTs.
+Rut.py is a Python library for handling Chilean RUTs (Rol Único Tributario). It provides functions to clean, validate, get the check digit, format, and generate RUTs.
 
 This library is based on the JavaScript library [rut.js](https://github.com/jlobos/rut.js) by jlobos. It aims to bring similar functionality to Python developers working with Chilean RUTs.
 
 ## Installation
 
-You can install RutPy using pip:
+You can install Rut.py using pip:
 
 ```shell
 pip install rutpy
 ```
 
 ## Usage
 
@@ -69,12 +69,12 @@
 ```python
 rut = generate()
 print(rut)  # Output: A randomly generated valid RUT
 ```
 
 ## Contributions
 
-Contributions are welcome. If you find any issues, have any improvement ideas, or want to add new features, you can open an issue or submit a pull request on the [GitHub repository](https://github.com/your_username/your_repository).
+Contributions are welcome. If you find any issues, have any improvement ideas, or want to add new features, you can open an issue or submit a pull request on the [GitHub repository](https://github.com/NozzOne/rut.py).
 
 ## License
 
-RutPy is distributed under the [MIT License](https://opensource.org/licenses/MIT).
+Rut.py is distributed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `rutpy-1.0.1/rutpy/core/rut.py` & `rutpy-1.0.2/rutpy/core/rut.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,58 @@
-import re
-import random
+"""
+rut.py
+
+This module provides functions for handling Chilean RUTs (Rol Único Tributario).
+It includes functions to clean, validate, get the check digit, format, and generate RUTs.
 
-from typing import Tuple
+Authors:
+- Valentin Marquez
+
+License:
+MIT License
+
+Functions:
+- clean(rut: str) -> str
+- validate(rut: str) -> bool
+- get_check_digit(input: str) -> str
+- format(rut: str, dots: bool = True, dash: bool = True) -> str
+- generate(n: int = 1) -> str or List[str]
+"""
+import random
+import re
+from typing import List, Union
 
 
 def clean(rut: str) -> str:
     """Function to clean a rut string. Removes all non numeric characters
 
     Args:
         rut (str): The rut to clean
 
     Returns:
         str: The cleaned rut
+    
+    Examples:
+        >>> clean("35.114.652-4")
+        '351146524'
     """
     return re.sub(r'^0+|[^0-9kK]+', '', rut)
 
 
 def validate(rut: str) -> bool:
     """Function to validate a rut
 
     Args:
         rut (str): The rut to validate
 
     Returns:
         bool: Whether the rut is valid or not
 
     Examples:
-        >>> validate("60487586-4")
+        >>> validate("4612837-0")
         True
     """
     if not isinstance(rut, str):
         return False
 
     if rut.startswith('0'):
         return False
@@ -48,37 +70,36 @@
         t = t // 10
         m += 1
 
     v = str(s - 1) if s > 0 else 'K'
     return v == rut[-1]
 
 
-def get_check_digit(input: str) -> str:
+def get_check_digit(digit: str) -> str:
     """Function to get the check digit of a rut
 
     Args:
-        input (str): The rut to get the check digit from
+        digit (str): The rut to get the check digit from
 
     Raises:
         ValueError: If the rut is invalid
 
     Returns:
         str: The check digit
 
     Examples:
         >>> get_check_digit("60487586")
-        '4'
+        '2'
     """
-    rut = list(map(int, clean(input)))
+    rut = list(map(int, clean(digit)))
 
     if len(rut) == 0 or any(map(lambda x: x != x, rut)):
-        raise ValueError(f'"{input}" as RUT is invalid')
+        raise ValueError(f'"{digit}" as RUT is invalid')
 
     modulus = 11
-    initial_value = 0
     sum_result = sum(
         current_value * ((index % 6) + 2)
         for index, current_value in enumerate(reversed(rut))
     )
 
     check_digit = modulus - (sum_result % modulus)
 
@@ -86,15 +107,15 @@
         return 'K'
     elif check_digit == 11:
         return '0'
     else:
         return str(check_digit)
 
 
-def format(rut: str, dots: bool = True, dash: bool = True) -> str:
+def format_rut(rut: str, dots: bool = True, dash: bool = True) -> str:
     """Function to format a rut
 
     Args:
         rut (str): The rut to format
         dots (bool, optional): Whether to add dots or not. Defaults to True.
         dash (bool, optional): Whether to add a dash or not. Defaults to True.
 
@@ -118,30 +139,28 @@
 
     if not dash:
         result = result.replace('-', '')
 
     return result
 
 
-def generate(n: int = 1) -> str:
-    """Genera RUTs chilenos aleatorios válidos.
+def generate(num: int = 1) -> Union[str, List[str]]:
+    """Generates random valid Chilean RUTs.
 
     Args:
-        quantity (int, optional): Cantidad de RUTs a generar. Por defecto, es 1.
+        num (int, optional): Number of RUTs to generate. Defaults to 1.
 
     Returns:
-        str or List[str]: El RUT generado. Si la cantidad es mayor a 1, se devuelve una lista de RUTs.
-
+        str or List[str]: The generated RUT. If the number is greater than 1, a list of RUTs is returned.
     """
     ruts = []
-    for _ in range(n):
+    for _ in range(num):
         rut_base = random.randint(1000000, 25000000)
         rut = str(rut_base)
         dv = get_check_digit(rut)
-        rut = format(rut + dv)
+        rut = format_rut(rut + dv)
         ruts.append(rut)
 
-    if n == 1:
-        return ruts[0]
-    else:
-        return ruts
-    
+    if num == 1:
+        return [ruts[0]]
+
+    return ruts
```

