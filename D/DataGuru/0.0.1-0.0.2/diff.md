# Comparing `tmp/DataGuru-0.0.1.tar.gz` & `tmp/DataGuru-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataGuru-0.0.1.tar", last modified: Mon Jun 12 17:33:18 2023, max compression
+gzip compressed data, was "DataGuru-0.0.2.tar", last modified: Thu Jun 29 08:31:38 2023, max compression
```

## Comparing `DataGuru-0.0.1.tar` & `DataGuru-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:33:18.485000 DataGuru-0.0.1/
--rw-rw-rw-   0        0        0      160 2023-06-12 17:19:47.000000 DataGuru-0.0.1/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 17:33:18.348000 DataGuru-0.0.1/DataGuru/
--rw-rw-rw-   0        0        0     4405 2023-06-12 16:58:21.000000 DataGuru-0.0.1/DataGuru/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:33:18.456000 DataGuru-0.0.1/DataGuru.egg-info/
--rw-rw-rw-   0        0        0     3421 2023-06-12 17:33:17.000000 DataGuru-0.0.1/DataGuru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-12 17:33:18.000000 DataGuru-0.0.1/DataGuru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:33:17.000000 DataGuru-0.0.1/DataGuru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 17:33:17.000000 DataGuru-0.0.1/DataGuru.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 17:33:17.000000 DataGuru-0.0.1/DataGuru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1059 2023-06-12 16:06:42.000000 DataGuru-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 16:03:00.000000 DataGuru-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3421 2023-06-12 17:33:18.472000 DataGuru-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-06-12 17:31:26.000000 DataGuru-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 17:33:18.482000 DataGuru-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-06-12 17:31:18.000000 DataGuru-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:31:38.431825 DataGuru-0.0.2/
+-rw-rw-rw-   0        0        0      262 2023-06-29 08:30:04.000000 DataGuru-0.0.2/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 08:31:38.385772 DataGuru-0.0.2/DataGuru/
+-rw-rw-rw-   0        0        0     5144 2023-06-29 08:30:13.000000 DataGuru-0.0.2/DataGuru/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:31:38.427688 DataGuru-0.0.2/DataGuru.egg-info/
+-rw-rw-rw-   0        0        0     3523 2023-06-29 08:31:38.000000 DataGuru-0.0.2/DataGuru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-29 08:31:38.000000 DataGuru-0.0.2/DataGuru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:31:38.000000 DataGuru-0.0.2/DataGuru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 08:31:38.000000 DataGuru-0.0.2/DataGuru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 08:31:38.000000 DataGuru-0.0.2/DataGuru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1059 2023-06-29 08:27:25.000000 DataGuru-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 08:27:25.000000 DataGuru-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3523 2023-06-29 08:31:38.430694 DataGuru-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2455 2023-06-29 08:27:25.000000 DataGuru-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:31:38.431825 DataGuru-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-06-29 08:28:01.000000 DataGuru-0.0.2/setup.py
```

### Comparing `DataGuru-0.0.1/DataGuru.egg-info/PKG-INFO` & `DataGuru-0.0.2/DataGuru.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataGuru
-Version: 0.0.1
+Version: 0.0.2
 Summary: The "DataGuru" library is a comprehensive Python toolkit designed to simplify common data analysis tasks for data science students and practitioners. With a focus on ease of use and efficiency, this library provides a range of functions to streamline your data analysis workflow.
 Home-page: 
 Author: Guna M
 Author-email: guna0professional@gmail.com
 License: MIT
 Keywords: data analysis
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,8 +38,14 @@
 0.0.1 (12/06/2023)
 -------------------
 - First Release
 - features
 --- 1. missingValues
 --- 2. findOutliers
 --- 3. analyzeData
+
+=======================
+
+0.0.2 (29/06/2023)
+-------------------
+fixed the bugs in the features
```

### Comparing `DataGuru-0.0.1/LICENCE.txt` & `DataGuru-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `DataGuru-0.0.1/PKG-INFO` & `DataGuru-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataGuru
-Version: 0.0.1
+Version: 0.0.2
 Summary: The "DataGuru" library is a comprehensive Python toolkit designed to simplify common data analysis tasks for data science students and practitioners. With a focus on ease of use and efficiency, this library provides a range of functions to streamline your data analysis workflow.
 Home-page: 
 Author: Guna M
 Author-email: guna0professional@gmail.com
 License: MIT
 Keywords: data analysis
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,8 +38,14 @@
 0.0.1 (12/06/2023)
 -------------------
 - First Release
 - features
 --- 1. missingValues
 --- 2. findOutliers
 --- 3. analyzeData
+
+=======================
+
+0.0.2 (29/06/2023)
+-------------------
+fixed the bugs in the features
```

### Comparing `DataGuru-0.0.1/README.txt` & `DataGuru-0.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `DataGuru-0.0.1/setup.py` & `DataGuru-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='DataGuru',
-    version='0.0.1',
+    version='0.0.2',
     description='The "DataGuru" library is a comprehensive Python toolkit designed to simplify common data analysis tasks for data science students and practitioners. With a focus on ease of use and efficiency, this library provides a range of functions to streamline your data analysis workflow.',
     long_description=open('README.txt').read() + '\n\n' +
     open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Guna M',
     author_email='guna0professional@gmail.com',
```

