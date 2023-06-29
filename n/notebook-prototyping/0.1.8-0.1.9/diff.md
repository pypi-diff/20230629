# Comparing `tmp/notebook_prototyping-0.1.8.tar.gz` & `tmp/notebook_prototyping-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_prototyping-0.1.8.tar", last modified: Thu Jun 29 13:25:55 2023, max compression
+gzip compressed data, was "notebook_prototyping-0.1.9.tar", last modified: Thu Jun 29 16:42:04 2023, max compression
```

## Comparing `notebook_prototyping-0.1.8.tar` & `notebook_prototyping-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:25:55.607373 notebook_prototyping-0.1.8/
--rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       17 2023-06-29 12:41:06.000000 notebook_prototyping-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3055 2023-06-29 13:25:55.607373 notebook_prototyping-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2756 2023-06-18 09:14:46.000000 notebook_prototyping-0.1.8/readme.md
--rw-rw-rw-   0        0        0      111 2023-06-29 13:25:55.609372 notebook_prototyping-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-06-29 13:25:52.000000 notebook_prototyping-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:25:55.580370 notebook_prototyping-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 13:25:55.606372 notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-29 13:25:55.000000 notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-29 13:25:55.000000 notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:25:55.000000 notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-29 13:25:55.000000 notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:25:55.000000 notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 16:42:04.941551 notebook_prototyping-0.1.9/
+-rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-06-29 12:41:06.000000 notebook_prototyping-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3055 2023-06-29 16:42:04.941551 notebook_prototyping-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2756 2023-06-18 09:14:46.000000 notebook_prototyping-0.1.9/readme.md
+-rw-rw-rw-   0        0        0      111 2023-06-29 16:42:04.946577 notebook_prototyping-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-06-29 16:37:45.000000 notebook_prototyping-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:42:04.899551 notebook_prototyping-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 16:42:04.919558 notebook_prototyping-0.1.9/src/notebook_prototyping/
+-rw-rw-rw-   0        0        0        0 2023-06-29 11:55:03.000000 notebook_prototyping-0.1.9/src/notebook_prototyping/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-06-18 08:27:53.000000 notebook_prototyping-0.1.9/src/notebook_prototyping/example.py
+-rw-rw-rw-   0        0        0     8716 2023-06-29 12:05:55.000000 notebook_prototyping-0.1.9/src/notebook_prototyping/notebook_import.py
+-rw-rw-rw-   0        0        0      213 2023-06-18 08:27:53.000000 notebook_prototyping-0.1.9/src/notebook_prototyping/second_example.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:42:04.940559 notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-29 16:42:04.000000 notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-06-29 16:42:04.000000 notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:42:04.000000 notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-29 16:42:04.000000 notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-29 16:42:04.000000 notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/top_level.txt
```

### Comparing `notebook_prototyping-0.1.8/LICENSE` & `notebook_prototyping-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_prototyping-0.1.8/PKG-INFO` & `notebook_prototyping-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook_prototyping
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `notebook_prototyping-0.1.8/readme.md` & `notebook_prototyping-0.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `notebook_prototyping-0.1.8/setup.py` & `notebook_prototyping-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 
 setup(
     name='notebook_prototyping',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     author="Reitze Jansen",
     author_email='rlh.jansen@outlook.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=find_packages('src'),
     # package_dir={'': 'src'},
```

### Comparing `notebook_prototyping-0.1.8/src/notebook_prototyping.egg-info/PKG-INFO` & `notebook_prototyping-0.1.9/src/notebook_prototyping.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-prototyping
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

