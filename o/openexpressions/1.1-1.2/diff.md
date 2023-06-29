# Comparing `tmp/openexpressions-1.1.tar.gz` & `tmp/openexpressions-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openexpressions-1.1.tar", last modified: Thu Jun 29 07:53:33 2023, max compression
+gzip compressed data, was "openexpressions-1.2.tar", last modified: Thu Jun 29 07:59:57 2023, max compression
```

## Comparing `openexpressions-1.1.tar` & `openexpressions-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:53:33.658735 openexpressions-1.1/
--rw-rw-rw-   0        0        0     1082 2023-06-28 06:29:12.000000 openexpressions-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1068 2023-06-29 07:53:33.658735 openexpressions-1.1/PKG-INFO
--rw-rw-rw-   0        0        0    18694 2023-06-29 07:50:07.000000 openexpressions-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 07:53:33.652248 openexpressions-1.1/openexpressions/
--rw-rw-rw-   0        0        0      655 2023-06-28 05:27:12.000000 openexpressions-1.1/openexpressions/Automata.py
--rw-rw-rw-   0        0        0     8233 2023-06-28 22:12:47.000000 openexpressions-1.1/openexpressions/ExpressionNodes.py
--rw-rw-rw-   0        0        0     6388 2023-06-28 06:08:15.000000 openexpressions-1.1/openexpressions/Grammar.py
--rw-rw-rw-   0        0        0     1997 2023-06-28 06:08:24.000000 openexpressions-1.1/openexpressions/ParseTable.py
--rw-rw-rw-   0        0        0    11624 2023-06-29 06:19:09.000000 openexpressions-1.1/openexpressions/Parser.py
--rw-rw-rw-   0        0        0     1191 2023-06-28 05:27:12.000000 openexpressions-1.1/openexpressions/Tokenizer.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:03:50.000000 openexpressions-1.1/openexpressions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:53:33.657233 openexpressions-1.1/openexpressions.egg-info/
--rw-rw-rw-   0        0        0     1068 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 07:53:33.000000 openexpressions-1.1/openexpressions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 07:53:33.659743 openexpressions-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1389 2023-06-29 07:52:57.000000 openexpressions-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:59:57.349320 openexpressions-1.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-28 06:29:12.000000 openexpressions-1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    20223 2023-06-29 07:59:57.349320 openexpressions-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18694 2023-06-29 07:50:07.000000 openexpressions-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:59:57.334341 openexpressions-1.2/openexpressions/
+-rw-rw-rw-   0        0        0      655 2023-06-28 05:27:12.000000 openexpressions-1.2/openexpressions/Automata.py
+-rw-rw-rw-   0        0        0     8233 2023-06-28 22:12:47.000000 openexpressions-1.2/openexpressions/ExpressionNodes.py
+-rw-rw-rw-   0        0        0     6388 2023-06-28 06:08:15.000000 openexpressions-1.2/openexpressions/Grammar.py
+-rw-rw-rw-   0        0        0     1997 2023-06-28 06:08:24.000000 openexpressions-1.2/openexpressions/ParseTable.py
+-rw-rw-rw-   0        0        0    11624 2023-06-29 06:19:09.000000 openexpressions-1.2/openexpressions/Parser.py
+-rw-rw-rw-   0        0        0     1191 2023-06-28 05:27:12.000000 openexpressions-1.2/openexpressions/Tokenizer.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 06:03:50.000000 openexpressions-1.2/openexpressions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:59:57.349320 openexpressions-1.2/openexpressions.egg-info/
+-rw-rw-rw-   0        0        0    20223 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 07:59:57.000000 openexpressions-1.2/openexpressions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 07:59:57.350495 openexpressions-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1609 2023-06-29 07:59:56.000000 openexpressions-1.2/setup.py
```

### Comparing `openexpressions-1.1/LICENSE.txt` & `openexpressions-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/README.md` & `openexpressions-1.2/README.md`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/openexpressions/Automata.py` & `openexpressions-1.2/openexpressions/Automata.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/openexpressions/ExpressionNodes.py` & `openexpressions-1.2/openexpressions/ExpressionNodes.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/openexpressions/Grammar.py` & `openexpressions-1.2/openexpressions/Grammar.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/openexpressions/ParseTable.py` & `openexpressions-1.2/openexpressions/ParseTable.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/openexpressions/Parser.py` & `openexpressions-1.2/openexpressions/Parser.py`

 * *Files identical despite different names*

### Comparing `openexpressions-1.1/openexpressions/Tokenizer.py` & `openexpressions-1.2/openexpressions/Tokenizer.py`

 * *Files identical despite different names*

