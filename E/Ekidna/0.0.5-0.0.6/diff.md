# Comparing `tmp/Ekidna-0.0.5.tar.gz` & `tmp/Ekidna-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ekidna-0.0.5.tar", last modified: Wed May 31 23:52:13 2023, max compression
+gzip compressed data, was "Ekidna-0.0.6.tar", last modified: Thu Jun 29 21:13:23 2023, max compression
```

## Comparing `Ekidna-0.0.5.tar` & `Ekidna-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:13.948625 Ekidna-0.0.5/
--rw-rw-rw-   0        0        0      466 2023-05-31 23:49:16.000000 Ekidna-0.0.5/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:13.920670 Ekidna-0.0.5/Ekidna/
--rw-rw-rw-   0        0        0    11395 2023-05-31 23:46:41.000000 Ekidna-0.0.5/Ekidna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:13.946630 Ekidna-0.0.5/Ekidna.egg-info/
--rw-rw-rw-   0        0        0     1347 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1059 2023-05-31 23:45:24.000000 Ekidna-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-31 23:45:24.000000 Ekidna-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6657 2023-05-31 23:49:51.000000 Ekidna-0.0.5/Module Contents.txt
--rw-rw-rw-   0        0        0     1347 2023-05-31 23:52:13.948625 Ekidna-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-05-31 23:45:24.000000 Ekidna-0.0.5/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 23:52:13.949620 Ekidna-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-05-31 23:50:24.000000 Ekidna-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:13:23.861999 Ekidna-0.0.6/
+-rw-rw-rw-   0        0        0      630 2023-06-29 19:54:15.000000 Ekidna-0.0.6/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 21:13:23.823647 Ekidna-0.0.6/Ekidna/
+-rw-rw-rw-   0        0        0    33166 2023-06-29 21:11:59.000000 Ekidna-0.0.6/Ekidna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:13:23.859009 Ekidna-0.0.6/Ekidna.egg-info/
+-rw-rw-rw-   0        0        0     1523 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1059 2023-06-29 21:10:14.000000 Ekidna-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:41:11.000000 Ekidna-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    13206 2023-06-29 21:10:17.000000 Ekidna-0.0.6/Module Contents.txt
+-rw-rw-rw-   0        0        0     1523 2023-06-29 21:13:23.861020 Ekidna-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-29 21:10:51.000000 Ekidna-0.0.6/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:13:23.862998 Ekidna-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-06-29 21:11:55.000000 Ekidna-0.0.6/setup.py
```

### Comparing `Ekidna-0.0.5/LICENSE.txt` & `Ekidna-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ekidna-0.0.5/setup.py` & `Ekidna-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Ekidna',
-    version='0.0.5',
+    version='0.0.6',
     description='Electrochemistry data analysis tools',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='OzymandiasTheDead',
     author_email='jacob@ekidnasensing.com',
     license='MIT',
     classifiers=classifiers,
```

