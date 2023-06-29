# Comparing `tmp/pdbplus-1.4.1.tar.gz` & `tmp/pdbplus-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.4.1.tar", last modified: Thu Jun 22 15:56:45 2023, max compression
+gzip compressed data, was "pdbplus-1.4.2.tar", last modified: Thu Jun 29 21:50:09 2023, max compression
```

## Comparing `pdbplus-1.4.1.tar` & `pdbplus-1.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:56:45.974635 pdbplus-1.4.1/
--rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-22 15:56:45.974538 pdbplus-1.4.1/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     5099 2023-06-22 14:53:13.000000 pdbplus-1.4.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:56:45.974405 pdbplus-1.4.1/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-22 15:56:45.974664 pdbplus-1.4.1/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5032 2023-06-22 15:22:19.000000 pdbplus-1.4.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:50:09.367777 pdbplus-1.4.2/
+-rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-29 21:50:09.367681 pdbplus-1.4.2/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     5099 2023-06-22 14:53:13.000000 pdbplus-1.4.2/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:50:09.367539 pdbplus-1.4.2/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-29 21:50:09.367808 pdbplus-1.4.2/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5032 2023-06-29 21:49:47.000000 pdbplus-1.4.2/setup.py
```

### Comparing `pdbplus-1.4.1/PKG-INFO` & `pdbplus-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.1
+Version: 1.4.2
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
```

### Comparing `pdbplus-1.4.1/README.md` & `pdbplus-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pdbplus-1.4.1/pdbplus.egg-info/PKG-INFO` & `pdbplus-1.4.2/pdbplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.1
+Version: 1.4.2
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
```

### Comparing `pdbplus-1.4.1/setup.py` & `pdbplus-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.4.1',
+    version='1.4.2',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -103,14 +103,14 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pdbp>=1.4.1',
+        'pdbp>=1.4.2',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```

