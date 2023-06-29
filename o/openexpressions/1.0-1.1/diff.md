# Comparing `tmp/openexpressions-1.0.tar.gz` & `tmp/openexpressions-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openexpressions-1.0.tar", last modified: Wed Jun 28 06:29:37 2023, max compression
+gzip compressed data, was "openexpressions-1.1.tar", last modified: Thu Jun 29 07:53:33 2023, max compression
```

## Comparing `openexpressions-1.0.tar` & `openexpressions-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 06:29:37.050413 openexpressions-1.0/
--rw-rw-rw-   0        0        0     1082 2023-06-28 06:29:12.000000 openexpressions-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1068 2023-06-28 06:29:37.050413 openexpressions-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-28 06:22:57.000000 openexpressions-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 06:29:37.033365 openexpressions-1.0/openexpressions/
--rw-rw-rw-   0        0        0      655 2023-06-28 05:27:12.000000 openexpressions-1.0/openexpressions/Automata.py
--rw-rw-rw-   0        0        0     8222 2023-06-28 05:27:12.000000 openexpressions-1.0/openexpressions/ExpressionNodes.py
--rw-rw-rw-   0        0        0     6388 2023-06-28 06:08:15.000000 openexpressions-1.0/openexpressions/Grammar.py
--rw-rw-rw-   0        0        0     1997 2023-06-28 06:08:24.000000 openexpressions-1.0/openexpressions/ParseTable.py
--rw-rw-rw-   0        0        0    11624 2023-06-28 06:08:00.000000 openexpressions-1.0/openexpressions/Parser.py
--rw-rw-rw-   0        0        0     1191 2023-06-28 05:27:12.000000 openexpressions-1.0/openexpressions/Tokenizer.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:03:50.000000 openexpressions-1.0/openexpressions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 06:29:37.049417 openexpressions-1.0/openexpressions.egg-info/
--rw-rw-rw-   0        0        0     1068 2023-06-28 06:29:37.000000 openexpressions-1.0/openexpressions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-28 06:29:37.000000 openexpressions-1.0/openexpressions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 06:29:37.000000 openexpressions-1.0/openexpressions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-28 06:29:37.000000 openexpressions-1.0/openexpressions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-28 06:29:37.051408 openexpressions-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1389 2023-06-28 06:28:35.000000 openexpressions-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:53:33.658735 openexpressions-1.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-28 06:29:12.000000 openexpressions-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1068 2023-06-29 07:53:33.658735 openexpressions-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18694 2023-06-29 07:50:07.000000 openexpressions-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:53:33.652248 openexpressions-1.1/openexpressions/
+-rw-rw-rw-   0        0        0      655 2023-06-28 05:27:12.000000 openexpressions-1.1/openexpressions/Automata.py
+-rw-rw-rw-   0        0        0     8233 2023-06-28 22:12:47.000000 openexpressions-1.1/openexpressions/ExpressionNodes.py
+-rw-rw-rw-   0        0        0     6388 2023-06-28 06:08:15.000000 openexpressions-1.1/openexpressions/Grammar.py
+-rw-rw-rw-   0        0        0     1997 2023-06-28 06:08:24.000000 openexpressions-1.1/openexpressions/ParseTable.py
+-rw-rw-rw-   0        0        0    11624 2023-06-29 06:19:09.000000 openexpressions-1.1/openexpressions/Parser.py
+-rw-rw-rw-   0        0        0     1191 2023-06-28 05:27:12.000000 openexpressions-1.1/openexpressions/Tokenizer.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 06:03:50.000000 openexpressions-1.1/openexpressions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:53:33.657233 openexpressions-1.1/openexpressions.egg-info/
+-rw-rw-rw-   0        0        0     1068 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 07:53:33.659743 openexpressions-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1389 2023-06-29 07:52:57.000000 openexpressions-1.1/setup.py
```

### Comparing `openexpressions-1.0/LICENSE.txt` & `openexpressions-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openexpressions-1.0/PKG-INFO` & `openexpressions-1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openexpressions
-Version: 1.0
+Version: 1.1
 Summary: A easy to use and expandable expression parser
 Home-page: https://github.com/AaryamanBhute/OpenExpressions
 Download-URL: https://github.com/AaryamanBhute/OpenExpressions/v_10.tar.gz
 Author: Aaryaman Bhute
 Author-email: aryamanbhute@gmail.com
 License: MIT
 Keywords: EXPRESSION,PARSER,EXPANDABLE,CUSTOMIZABLE
```

### Comparing `openexpressions-1.0/openexpressions/Automata.py` & `openexpressions-1.1/openexpressions/Automata.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.0/openexpressions/ExpressionNodes.py` & `openexpressions-1.1/openexpressions/ExpressionNodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from abc import ABC, abstractmethod
 
-class Operand(ABC):
-    @property
+class ExpressionNode(ABC):
     @abstractmethod
-    def identifier(self):pass
+    def eval(self):
+        pass
 
+class Operand(ExpressionNode):
+    @property
     @abstractmethod
+    def identifier(self):pass
+    
     def __init__(self, v) -> None:
         self.val = v
-    def eval(self):
-        pass
+
 class Int(Operand):
     identifier = r"\d+(?!\.)"
     def __init__(self, v) -> None:
         super().__init__(int(v))
     def eval(self, context=None):
         return(self.val)
 
@@ -50,18 +53,16 @@
        if(self.val not in context): raise Exception("Attempting to evaluate variable with no definition in context")
        val = context[self.val]
        if(int(val) != val): raise Exception("Boolean Var must be 0 or 1")
        val = int(val)
        if(val > 1 or val < 0): raise Exception("Boolean Var must be 0 or 1")
        return(val)
 
-class Operator(ABC):
-    @abstractmethod
-    def eval(self):
-        pass
+class Operator(ExpressionNode):
+    pass
 
 class BinOp(Operator):
     @property
     @abstractmethod
     def identifier(self):pass
 
     def __init__(self, l, r) -> None:
```

### Comparing `openexpressions-1.0/openexpressions/Grammar.py` & `openexpressions-1.1/openexpressions/Grammar.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.0/openexpressions/ParseTable.py` & `openexpressions-1.1/openexpressions/ParseTable.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.0/openexpressions/Parser.py` & `openexpressions-1.1/openexpressions/Parser.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.0/openexpressions/Tokenizer.py` & `openexpressions-1.1/openexpressions/Tokenizer.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.0/openexpressions.egg-info/PKG-INFO` & `openexpressions-1.1/openexpressions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openexpressions
-Version: 1.0
+Version: 1.1
 Summary: A easy to use and expandable expression parser
 Home-page: https://github.com/AaryamanBhute/OpenExpressions
 Download-URL: https://github.com/AaryamanBhute/OpenExpressions/v_10.tar.gz
 Author: Aaryaman Bhute
 Author-email: aryamanbhute@gmail.com
 License: MIT
 Keywords: EXPRESSION,PARSER,EXPANDABLE,CUSTOMIZABLE
```

### Comparing `openexpressions-1.0/setup.py` & `openexpressions-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'openexpressions',
   packages = ['openexpressions'],
-  version = '1.0',
+  version = '1.1',
   license='MIT',
   description = 'A easy to use and expandable expression parser',
   author = 'Aaryaman Bhute',
   author_email = 'aryamanbhute@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AaryamanBhute/OpenExpressions',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AaryamanBhute/OpenExpressions/v_10.tar.gz',    # I explain this later on
   keywords = ['EXPRESSION', 'PARSER', 'EXPANDABLE', 'CUSTOMIZABLE'],   # Keywords that define your package best
```

