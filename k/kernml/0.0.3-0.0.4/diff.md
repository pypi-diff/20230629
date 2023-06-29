# Comparing `tmp/kernml-0.0.3.tar.gz` & `tmp/kernml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernml-0.0.3.tar", last modified: Mon Jun 26 07:51:35 2023, max compression
+gzip compressed data, was "kernml-0.0.4.tar", last modified: Thu Jun 29 19:01:06 2023, max compression
```

## Comparing `kernml-0.0.3.tar` & `kernml-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.826195 kernml-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-23 01:54:01.000000 kernml-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      417 2023-06-26 07:51:35.825238 kernml-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-06-23 01:52:37.000000 kernml-0.0.3/README.md
--rw-rw-rw-   0        0        0      447 2023-06-26 07:38:49.000000 kernml-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 07:51:35.826195 kernml-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.803256 kernml-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.815225 kernml-0.0.3/src/kernml/
--rw-rw-rw-   0        0        0        0 2023-06-23 05:13:51.000000 kernml-0.0.3/src/kernml/__init__.py
--rw-rw-rw-   0        0        0    26033 2023-06-26 07:51:11.000000 kernml-0.0.3/src/kernml/prg.py
-drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.823202 kernml-0.0.3/src/kernml.egg-info/
--rw-rw-rw-   0        0        0      417 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.661566 kernml-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 01:54:01.000000 kernml-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      417 2023-06-29 19:01:06.661566 kernml-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-06-23 01:52:37.000000 kernml-0.0.4/README.md
+-rw-rw-rw-   0        0        0      447 2023-06-29 18:56:28.000000 kernml-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 19:01:06.661566 kernml-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.630317 kernml-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.645943 kernml-0.0.4/src/kernml/
+-rw-rw-rw-   0        0        0        0 2023-06-23 05:13:51.000000 kernml-0.0.4/src/kernml/__init__.py
+-rw-rw-rw-   0        0        0    26194 2023-06-29 18:59:34.000000 kernml-0.0.4/src/kernml/prg.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.661566 kernml-0.0.4/src/kernml.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/top_level.txt
```

### Comparing `kernml-0.0.3/LICENSE` & `kernml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kernml-0.0.3/src/kernml/prg.py` & `kernml-0.0.4/src/kernml/prg.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 # pr_2()
 # pr_3()
 # pr_4()
 # pr_4_algo()
 # pr_4_nb()
 # pr_5()
 # pr_6()
+# pr_7()
+# pr_8()
+# pr_9()
 # pr_10()
 
 def pr_1_algo():
     p1 = '''
 import pandas as pd
 import itertools
 
@@ -829,14 +832,22 @@
     annot=True, 
     fmt = "d", 
     xticklabels=newsgroups_train.target_names,
     yticklabels=newsgroups_train.target_names)
 plt.xlabel("Actual Category")
 plt.ylabel("Predicted Category")
 plt.show() 
+
+#
+print(
+    classification_report(
+    newsgroups_test.target,
+    predicted_categories, 
+    target_names=categories)
+)
 '''
     p7 = print(p7)
     return p7
 
 def pr_8():
     p8 = '''
 import pandas as pd
```

