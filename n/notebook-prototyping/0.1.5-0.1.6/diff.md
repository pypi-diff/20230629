# Comparing `tmp/notebook_prototyping-0.1.5.tar.gz` & `tmp/notebook_prototyping-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_prototyping-0.1.5.tar", last modified: Thu Jun 29 12:12:40 2023, max compression
+gzip compressed data, was "notebook_prototyping-0.1.6.tar", last modified: Thu Jun 29 12:22:35 2023, max compression
```

## Comparing `notebook_prototyping-0.1.5.tar` & `notebook_prototyping-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:12:40.034873 notebook_prototyping-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3055 2023-06-29 12:12:40.035855 notebook_prototyping-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-06-29 12:12:40.036855 notebook_prototyping-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      732 2023-06-29 12:12:04.000000 notebook_prototyping-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:12:40.011859 notebook_prototyping-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 12:12:40.033855 notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-29 12:12:39.000000 notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-29 12:12:39.000000 notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:12:39.000000 notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-29 12:12:39.000000 notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:12:39.000000 notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 12:22:35.105357 notebook_prototyping-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3055 2023-06-29 12:22:35.106368 notebook_prototyping-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-06-29 12:22:35.107385 notebook_prototyping-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-06-29 12:22:33.000000 notebook_prototyping-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:22:35.080356 notebook_prototyping-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 12:22:35.104358 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/top_level.txt
```

### Comparing `notebook_prototyping-0.1.5/LICENSE` & `notebook_prototyping-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_prototyping-0.1.5/PKG-INFO` & `notebook_prototyping-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook_prototyping
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `notebook_prototyping-0.1.5/src/notebook_prototyping.egg-info/PKG-INFO` & `notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-prototyping
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

