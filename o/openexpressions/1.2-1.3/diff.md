# Comparing `tmp/openexpressions-1.2.tar.gz` & `tmp/openexpressions-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openexpressions-1.2.tar", last modified: Thu Jun 29 07:59:57 2023, max compression
+gzip compressed data, was "openexpressions-1.3.tar", last modified: Thu Jun 29 08:20:55 2023, max compression
```

## Comparing `openexpressions-1.2.tar` & `openexpressions-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:59:57.349320 openexpressions-1.2/
--rw-rw-rw-   0        0        0     1082 2023-06-28 06:29:12.000000 openexpressions-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    20223 2023-06-29 07:59:57.349320 openexpressions-1.2/PKG-INFO
--rw-rw-rw-   0        0        0    18694 2023-06-29 07:50:07.000000 openexpressions-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 07:59:57.334341 openexpressions-1.2/openexpressions/
--rw-rw-rw-   0        0        0      655 2023-06-28 05:27:12.000000 openexpressions-1.2/openexpressions/Automata.py
--rw-rw-rw-   0        0        0     8233 2023-06-28 22:12:47.000000 openexpressions-1.2/openexpressions/ExpressionNodes.py
--rw-rw-rw-   0        0        0     6388 2023-06-28 06:08:15.000000 openexpressions-1.2/openexpressions/Grammar.py
--rw-rw-rw-   0        0        0     1997 2023-06-28 06:08:24.000000 openexpressions-1.2/openexpressions/ParseTable.py
--rw-rw-rw-   0        0        0    11624 2023-06-29 06:19:09.000000 openexpressions-1.2/openexpressions/Parser.py
--rw-rw-rw-   0        0        0     1191 2023-06-28 05:27:12.000000 openexpressions-1.2/openexpressions/Tokenizer.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:03:50.000000 openexpressions-1.2/openexpressions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:59:57.349320 openexpressions-1.2/openexpressions.egg-info/
--rw-rw-rw-   0        0        0    20223 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 07:59:57.350495 openexpressions-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1609 2023-06-29 07:59:56.000000 openexpressions-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:55.564980 openexpressions-1.3/
+-rw-rw-rw-   0        0        0     1082 2023-06-28 06:29:12.000000 openexpressions-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    20307 2023-06-29 08:20:55.565970 openexpressions-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    18777 2023-06-29 08:20:33.000000 openexpressions-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:55.548981 openexpressions-1.3/openexpressions/
+-rw-rw-rw-   0        0        0      655 2023-06-28 05:27:12.000000 openexpressions-1.3/openexpressions/Automata.py
+-rw-rw-rw-   0        0        0     8233 2023-06-28 22:12:47.000000 openexpressions-1.3/openexpressions/ExpressionNodes.py
+-rw-rw-rw-   0        0        0     6388 2023-06-28 06:08:15.000000 openexpressions-1.3/openexpressions/Grammar.py
+-rw-rw-rw-   0        0        0     1997 2023-06-28 06:08:24.000000 openexpressions-1.3/openexpressions/ParseTable.py
+-rw-rw-rw-   0        0        0    11624 2023-06-29 06:19:09.000000 openexpressions-1.3/openexpressions/Parser.py
+-rw-rw-rw-   0        0        0     1191 2023-06-28 05:27:12.000000 openexpressions-1.3/openexpressions/Tokenizer.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 06:03:50.000000 openexpressions-1.3/openexpressions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:20:55.564980 openexpressions-1.3/openexpressions.egg-info/
+-rw-rw-rw-   0        0        0    20307 2023-06-29 08:20:55.000000 openexpressions-1.3/openexpressions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-06-29 08:20:55.000000 openexpressions-1.3/openexpressions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:20:55.000000 openexpressions-1.3/openexpressions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 08:20:55.000000 openexpressions-1.3/openexpressions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 08:20:55.567473 openexpressions-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1609 2023-06-29 08:19:41.000000 openexpressions-1.3/setup.py
```

### Comparing `openexpressions-1.2/LICENSE.txt` & `openexpressions-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/PKG-INFO` & `openexpressions-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openexpressions
-Version: 1.2
+Version: 1.3
 Summary: A easy to use and expandable expression parser
 Home-page: https://github.com/AaryamanBhute/OpenExpressions
 Download-URL: https://github.com/AaryamanBhute/OpenExpressions/v_10.tar.gz
 Author: Aaryaman Bhute
 Author-email: aryamanbhute@gmail.com
 License: MIT
 Keywords: EXPRESSION,PARSER,EXPANDABLE,CUSTOMIZABLE
@@ -58,14 +58,15 @@
 OpenExpressions is available on PyPi and easily installable on Python 3.3+ using pip
 
 ```sh
 pip install openexpressions
 ```
 
 Source code is available at this [Github Repository](https://github.com/AaryamanBhute/OpenExpressions)
+Module info is available at [PyPi Page](https://pypi.org/project/openexpressions/)
 
 ## Documentation
 
 ### Basic Usage
 The basic usage of this library consists of using the preset of the Parser.
 Currently, the 2 presets are: __math__ (_default_) and __boolean__
 ```python
```

### Comparing `openexpressions-1.2/README.md` & `openexpressions-1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 OpenExpressions is available on PyPi and easily installable on Python 3.3+ using pip
 
 ```sh
 pip install openexpressions
 ```
 
 Source code is available at this [Github Repository](https://github.com/AaryamanBhute/OpenExpressions)
+Module info is available at [PyPi Page](https://pypi.org/project/openexpressions/)
 
 ## Documentation
 
 ### Basic Usage
 The basic usage of this library consists of using the preset of the Parser.
 Currently, the 2 presets are: __math__ (_default_) and __boolean__
 ```python
```

### Comparing `openexpressions-1.2/openexpressions/Automata.py` & `openexpressions-1.3/openexpressions/Automata.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/openexpressions/ExpressionNodes.py` & `openexpressions-1.3/openexpressions/ExpressionNodes.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/openexpressions/Grammar.py` & `openexpressions-1.3/openexpressions/Grammar.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/openexpressions/ParseTable.py` & `openexpressions-1.3/openexpressions/ParseTable.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/openexpressions/Parser.py` & `openexpressions-1.3/openexpressions/Parser.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/openexpressions/Tokenizer.py` & `openexpressions-1.3/openexpressions/Tokenizer.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.2/openexpressions.egg-info/PKG-INFO` & `openexpressions-1.3/openexpressions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openexpressions
-Version: 1.2
+Version: 1.3
 Summary: A easy to use and expandable expression parser
 Home-page: https://github.com/AaryamanBhute/OpenExpressions
 Download-URL: https://github.com/AaryamanBhute/OpenExpressions/v_10.tar.gz
 Author: Aaryaman Bhute
 Author-email: aryamanbhute@gmail.com
 License: MIT
 Keywords: EXPRESSION,PARSER,EXPANDABLE,CUSTOMIZABLE
@@ -58,14 +58,15 @@
 OpenExpressions is available on PyPi and easily installable on Python 3.3+ using pip
 
 ```sh
 pip install openexpressions
 ```
 
 Source code is available at this [Github Repository](https://github.com/AaryamanBhute/OpenExpressions)
+Module info is available at [PyPi Page](https://pypi.org/project/openexpressions/)
 
 ## Documentation
 
 ### Basic Usage
 The basic usage of this library consists of using the preset of the Parser.
 Currently, the 2 presets are: __math__ (_default_) and __boolean__
 ```python
```

### Comparing `openexpressions-1.2/setup.py` & `openexpressions-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'openexpressions',
   packages = ['openexpressions'],
-  version = '1.2',
+  version = '1.3',
   license='MIT',
   description = 'A easy to use and expandable expression parser',
   author = 'Aaryaman Bhute',
   author_email = 'aryamanbhute@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AaryamanBhute/OpenExpressions',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AaryamanBhute/OpenExpressions/v_10.tar.gz',    # I explain this later on
   keywords = ['EXPRESSION', 'PARSER', 'EXPANDABLE', 'CUSTOMIZABLE'],   # Keywords that define your package best
```

