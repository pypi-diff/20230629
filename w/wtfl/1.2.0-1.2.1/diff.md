# Comparing `tmp/wtfl-1.2.0.tar.gz` & `tmp/wtfl-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtfl-1.2.0.tar", max compression
+gzip compressed data, was "wtfl-1.2.1.tar", max compression
```

## Comparing `wtfl-1.2.0.tar` & `wtfl-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-04-20 22:33:19.586953 wtfl-1.2.0/LICENSE
--rw-r--r--   0        0        0     9899 2023-04-20 22:33:19.586953 wtfl-1.2.0/README.md
--rw-r--r--   0        0        0      578 2023-04-20 22:33:19.586953 wtfl-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-20 22:33:19.586953 wtfl-1.2.0/wtfl/__init__.py
--rw-r--r--   0        0        0     5035 2023-04-20 22:33:19.586953 wtfl-1.2.0/wtfl/grammar.py
--rw-r--r--   0        0        0     2789 2023-04-20 22:33:19.586953 wtfl-1.2.0/wtfl/internal_types.py
--rw-r--r--   0        0        0     6349 2023-04-20 22:33:19.590953 wtfl-1.2.0/wtfl/parser.py
--rw-r--r--   0        0        0     6899 2023-04-20 22:33:19.590953 wtfl-1.2.0/wtfl/reader.py
--rw-r--r--   0        0        0     4557 2023-04-20 22:33:19.590953 wtfl-1.2.0/wtfl/writer.py
--rw-r--r--   0        0        0    10738 1970-01-01 00:00:00.000000 wtfl-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-29 18:58:56.609459 wtfl-1.2.1/LICENSE
+-rw-r--r--   0        0        0     9899 2023-06-29 18:58:56.609459 wtfl-1.2.1/README.md
+-rw-r--r--   0        0        0      578 2023-06-29 18:58:56.609459 wtfl-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-29 18:58:56.609459 wtfl-1.2.1/wtfl/__init__.py
+-rw-r--r--   0        0        0     5035 2023-06-29 18:58:56.609459 wtfl-1.2.1/wtfl/grammar.py
+-rw-r--r--   0        0        0     2789 2023-06-29 18:58:56.609459 wtfl-1.2.1/wtfl/internal_types.py
+-rw-r--r--   0        0        0     6384 2023-06-29 18:58:56.609459 wtfl-1.2.1/wtfl/parser.py
+-rw-r--r--   0        0        0     6899 2023-06-29 18:58:56.609459 wtfl-1.2.1/wtfl/reader.py
+-rw-r--r--   0        0        0     4557 2023-06-29 18:58:56.609459 wtfl-1.2.1/wtfl/writer.py
+-rw-r--r--   0        0        0    10738 1970-01-01 00:00:00.000000 wtfl-1.2.1/PKG-INFO
```

### Comparing `wtfl-1.2.0/LICENSE` & `wtfl-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfl-1.2.0/README.md` & `wtfl-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wtfl-1.2.0/pyproject.toml` & `wtfl-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wtfl"
-version = "1.2.0"
+version = "1.2.1"
 description = "Well-designed Text-based Friendly Language"
 authors = ["Dmitry Gritsenko <k01419q45@ya.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/wtfl"
 homepage = "https://github.com/evtn/wtfl"
 keywords = ["markup", "config"]
```

### Comparing `wtfl-1.2.0/wtfl/grammar.py` & `wtfl-1.2.1/wtfl/grammar.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.2.0/wtfl/internal_types.py` & `wtfl-1.2.1/wtfl/internal_types.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.2.0/wtfl/parser.py` & `wtfl-1.2.1/wtfl/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import typing
 import codecs
-from typing import Callable, List, Dict, Tuple
+from typing import Callable, List, Dict, Optional, Tuple
 
 from lark import Lark, Transformer
 from lark.exceptions import UnexpectedCharacters, UnexpectedToken
 
 from .internal_types import ARRAY_KEY, Also, Constraint, Object, Assign, Operation
 from .grammar import g as grammar  # type: ignore
 
@@ -246,9 +246,12 @@
     transformer=transformer,
 )
 
 from .reader import PythonValue
 
 ParseFunc = Callable[[str], PythonValue]
 ParseFuncs = Tuple[
-    ParseFunc | None, ParseFunc | None, ParseFunc | None, ParseFunc | None
+    Optional[ParseFunc],
+    Optional[ParseFunc],
+    Optional[ParseFunc],
+    Optional[ParseFunc],
 ]
```

### Comparing `wtfl-1.2.0/wtfl/reader.py` & `wtfl-1.2.1/wtfl/reader.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.2.0/wtfl/writer.py` & `wtfl-1.2.1/wtfl/writer.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.2.0/PKG-INFO` & `wtfl-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtfl
-Version: 1.2.0
+Version: 1.2.1
 Summary: Well-designed Text-based Friendly Language
 Home-page: https://github.com/evtn/wtfl
 License: MIT
 Keywords: markup,config
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.7,<4.0
```

