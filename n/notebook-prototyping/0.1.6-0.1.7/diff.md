# Comparing `tmp/notebook_prototyping-0.1.6.tar.gz` & `tmp/notebook_prototyping-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_prototyping-0.1.6.tar", last modified: Thu Jun 29 12:22:35 2023, max compression
+gzip compressed data, was "notebook_prototyping-0.1.7.tar", last modified: Thu Jun 29 12:42:37 2023, max compression
```

## Comparing `notebook_prototyping-0.1.6.tar` & `notebook_prototyping-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:35.105357 notebook_prototyping-0.1.6/
--rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3055 2023-06-29 12:22:35.106368 notebook_prototyping-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-06-29 12:22:35.107385 notebook_prototyping-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      681 2023-06-29 12:22:33.000000 notebook_prototyping-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:35.080356 notebook_prototyping-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 12:22:35.104358 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:22:35.000000 notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 12:42:37.329831 notebook_prototyping-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3055 2023-06-29 12:42:37.330831 notebook_prototyping-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-06-29 12:42:37.332831 notebook_prototyping-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-06-29 12:42:34.000000 notebook_prototyping-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:42:37.310888 notebook_prototyping-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 12:42:37.329831 notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-29 12:42:37.000000 notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-29 12:42:37.000000 notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:42:37.000000 notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-29 12:42:37.000000 notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:42:37.000000 notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/top_level.txt
```

### Comparing `notebook_prototyping-0.1.6/LICENSE` & `notebook_prototyping-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_prototyping-0.1.6/PKG-INFO` & `notebook_prototyping-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook_prototyping
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `notebook_prototyping-0.1.6/setup.py` & `notebook_prototyping-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 from pathlib import Path
 long_description = Path("readme.md").read_text()
 
 
 setup(
     name='notebook_prototyping',
-    version='0.1.6',
+    version='0.1.7',
     license='MIT',
     author="Reitze Jansen",
     author_email='rlh.jansen@outlook.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=find_packages('src'),
     # package_dir={'': 'src'},
     url='https://github.com/rlhjansen/nbprototyping',
     keywords='jupyter notebook tooling',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
+    include_package_data=True,
     install_requires=['jupyter', 'ipynbname', 'ast-comments']
 )
```

### Comparing `notebook_prototyping-0.1.6/src/notebook_prototyping.egg-info/PKG-INFO` & `notebook_prototyping-0.1.7/src/notebook_prototyping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-prototyping
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

