# Comparing `tmp/notebook_prototyping-0.1.3.tar.gz` & `tmp/notebook_prototyping-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_prototyping-0.1.3.tar", last modified: Thu Jun 29 11:29:31 2023, max compression
+gzip compressed data, was "notebook_prototyping-0.1.4.tar", last modified: Thu Jun 29 12:06:34 2023, max compression
```

## Comparing `notebook_prototyping-0.1.3.tar` & `notebook_prototyping-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 11:29:31.530113 notebook_prototyping-0.1.3/
--rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3055 2023-06-29 11:29:31.530113 notebook_prototyping-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 11:29:31.512112 notebook_prototyping-0.1.3/nested/
-drwxrwxrwx   0        0        0        0 2023-06-29 11:29:31.517112 notebook_prototyping-0.1.3/nested/directory/
--rw-rw-rw-   0        0        0      111 2023-06-18 08:27:53.000000 notebook_prototyping-0.1.3/nested/directory/third_example.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:29:31.529112 notebook_prototyping-0.1.3/notebook_prototyping.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-29 11:29:31.000000 notebook_prototyping-0.1.3/notebook_prototyping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-29 11:29:31.000000 notebook_prototyping-0.1.3/notebook_prototyping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 11:29:31.000000 notebook_prototyping-0.1.3/notebook_prototyping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 11:29:31.000000 notebook_prototyping-0.1.3/notebook_prototyping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-29 11:29:31.531113 notebook_prototyping-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      597 2023-06-29 11:29:15.000000 notebook_prototyping-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:06:34.270661 notebook_prototyping-0.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3055 2023-06-29 12:06:34.270661 notebook_prototyping-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-06-29 12:06:34.272660 notebook_prototyping-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      732 2023-06-29 12:06:28.000000 notebook_prototyping-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:06:34.252660 notebook_prototyping-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 12:06:34.269661 notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-29 12:06:34.000000 notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-29 12:06:34.000000 notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:06:34.000000 notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-29 12:06:34.000000 notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:06:34.000000 notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/top_level.txt
```

### Comparing `notebook_prototyping-0.1.3/LICENSE` & `notebook_prototyping-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_prototyping-0.1.3/PKG-INFO` & `notebook_prototyping-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook_prototyping
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `notebook_prototyping-0.1.3/notebook_prototyping.egg-info/PKG-INFO` & `notebook_prototyping-0.1.4/src/notebook_prototyping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-prototyping
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/rlhjansen/nbprototyping
 Author: Reitze Jansen
 Author-email: rlh.jansen@outlook.com
 License: MIT
 Keywords: jupyter notebook tooling
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `notebook_prototyping-0.1.3/setup.py` & `notebook_prototyping-0.1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='notebook_prototyping',
-    version='0.1.3',
+    version='0.1.4',
     license='MIT',
     author="Reitze Jansen",
     author_email='rlh.jansen@outlook.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=find_packages('src'),
     # package_dir={'': 'src'},
     url='https://github.com/rlhjansen/nbprototyping',
     keywords='jupyter notebook tooling',
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
+    install_requires=['jupyter', 'ipynbname', 'ast-comments']
 )
```

