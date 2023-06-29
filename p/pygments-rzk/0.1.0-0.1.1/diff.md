# Comparing `tmp/pygments-rzk-0.1.0.tar.gz` & `tmp/pygments-rzk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments-rzk-0.1.0.tar", last modified: Thu Jun 29 16:14:53 2023, max compression
+gzip compressed data, was "pygments-rzk-0.1.1.tar", last modified: Thu Jun 29 16:18:39 2023, max compression
```

## Comparing `pygments-rzk-0.1.0.tar` & `pygments-rzk-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:14:53.334585 pygments-rzk-0.1.0/
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)     1502 2023-06-29 14:06:43.000000 pygments-rzk-0.1.0/LICENSE
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)       42 2023-06-29 14:14:50.000000 pygments-rzk-0.1.0/MANIFEST.in
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)     2323 2023-06-29 16:14:53.334240 pygments-rzk-0.1.0/PKG-INFO
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)     1659 2023-06-29 16:12:34.000000 pygments-rzk-0.1.0/README.md
-drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:14:53.331045 pygments-rzk-0.1.0/pygments_rzk/
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)     2666 2023-06-29 14:16:01.000000 pygments-rzk-0.1.0/pygments_rzk/__init__.py
-drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:14:53.333652 pygments-rzk-0.1.0/pygments_rzk.egg-info/
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)     2323 2023-06-29 16:14:53.000000 pygments-rzk-0.1.0/pygments_rzk.egg-info/PKG-INFO
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)      281 2023-06-29 16:14:53.000000 pygments-rzk-0.1.0/pygments_rzk.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)        1 2023-06-29 16:14:53.000000 pygments-rzk-0.1.0/pygments_rzk.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)       51 2023-06-29 16:14:53.000000 pygments-rzk-0.1.0/pygments_rzk.egg-info/entry_points.txt
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)       14 2023-06-29 16:14:53.000000 pygments-rzk-0.1.0/pygments_rzk.egg-info/requires.txt
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)       13 2023-06-29 16:14:53.000000 pygments-rzk-0.1.0/pygments_rzk.egg-info/top_level.txt
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)       38 2023-06-29 16:14:53.334648 pygments-rzk-0.1.0/setup.cfg
--rw-r--r--   0 nikolaikudasov   (501) staff       (20)      985 2023-06-29 16:14:45.000000 pygments-rzk-0.1.0/setup.py
+drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:18:39.798878 pygments-rzk-0.1.1/
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)     1502 2023-06-29 14:06:43.000000 pygments-rzk-0.1.1/LICENSE
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)       63 2023-06-29 16:16:25.000000 pygments-rzk-0.1.1/MANIFEST.in
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)     2323 2023-06-29 16:18:39.798317 pygments-rzk-0.1.1/PKG-INFO
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)     1659 2023-06-29 16:12:34.000000 pygments-rzk-0.1.1/README.md
+drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:18:39.780788 pygments-rzk-0.1.1/images/
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)   449381 2023-06-29 14:07:04.000000 pygments-rzk-0.1.1/images/latex-highlighting-demo.png
+drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:18:39.782936 pygments-rzk-0.1.1/pygments_rzk/
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)     2666 2023-06-29 14:16:01.000000 pygments-rzk-0.1.1/pygments_rzk/__init__.py
+drwxr-xr-x   0 nikolaikudasov   (501) staff       (20)        0 2023-06-29 16:18:39.797442 pygments-rzk-0.1.1/pygments_rzk.egg-info/
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)     2323 2023-06-29 16:18:39.000000 pygments-rzk-0.1.1/pygments_rzk.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)      316 2023-06-29 16:18:39.000000 pygments-rzk-0.1.1/pygments_rzk.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)        1 2023-06-29 16:18:39.000000 pygments-rzk-0.1.1/pygments_rzk.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)       51 2023-06-29 16:18:39.000000 pygments-rzk-0.1.1/pygments_rzk.egg-info/entry_points.txt
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)       14 2023-06-29 16:18:39.000000 pygments-rzk-0.1.1/pygments_rzk.egg-info/requires.txt
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)       13 2023-06-29 16:18:39.000000 pygments-rzk-0.1.1/pygments_rzk.egg-info/top_level.txt
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)       38 2023-06-29 16:18:39.798997 pygments-rzk-0.1.1/setup.cfg
+-rw-r--r--   0 nikolaikudasov   (501) staff       (20)      985 2023-06-29 16:17:08.000000 pygments-rzk-0.1.1/setup.py
```

### Comparing `pygments-rzk-0.1.0/LICENSE` & `pygments-rzk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments-rzk-0.1.0/PKG-INFO` & `pygments-rzk-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-rzk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pygments lexer for Rzk language (of proof assistant for synthetic ∞-categories).
 Home-page: https://github.com/fizruk/pygments-rzk
 Author: Nikolai Kudasov
 Author-email: nickolay.kudasov@gmail.com
 License: BSD 3
 Keywords: pygments rzk lexer
 Classifier: Environment :: Plugins
```

### Comparing `pygments-rzk-0.1.0/README.md` & `pygments-rzk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pygments-rzk-0.1.0/pygments_rzk/__init__.py` & `pygments-rzk-0.1.1/pygments_rzk/__init__.py`

 * *Files identical despite different names*

### Comparing `pygments-rzk-0.1.0/pygments_rzk.egg-info/PKG-INFO` & `pygments-rzk-0.1.1/pygments_rzk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-rzk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pygments lexer for Rzk language (of proof assistant for synthetic ∞-categories).
 Home-page: https://github.com/fizruk/pygments-rzk
 Author: Nikolai Kudasov
 Author-email: nickolay.kudasov@gmail.com
 License: BSD 3
 Keywords: pygments rzk lexer
 Classifier: Environment :: Plugins
```

### Comparing `pygments-rzk-0.1.0/setup.py` & `pygments-rzk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pygments-rzk',
-    version='0.1.0',
+    version='0.1.1',
     description='Pygments lexer for Rzk language (of proof assistant for synthetic ∞-categories).',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords='pygments rzk lexer',
     license='BSD 3',
 
     author='Nikolai Kudasov',
```

