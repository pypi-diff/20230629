# Comparing `tmp/kuut-0.0.2.tar.gz` & `tmp/kuut-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuut-0.0.2.tar", last modified: Sat Jun 24 12:17:53 2023, max compression
+gzip compressed data, was "kuut-0.0.3.tar", last modified: Thu Jun 29 16:19:10 2023, max compression
```

## Comparing `kuut-0.0.2.tar` & `kuut-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-24 12:17:53.780960 kuut-0.0.2/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 kuut-0.0.2/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 kuut-0.0.2/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1090 2023-06-24 12:17:53.780828 kuut-0.0.2/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      293 2023-06-21 20:04:04.000000 kuut-0.0.2/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-24 12:17:53.779484 kuut-0.0.2/kuut/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-24 12:17:46.000000 kuut-0.0.2/kuut/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     3601 2023-06-24 12:17:46.000000 kuut-0.0.2/kuut/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     6257 2023-06-24 12:17:46.000000 kuut-0.0.2/kuut/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-24 12:17:53.780611 kuut-0.0.2/kuut.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1090 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      294 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-22 12:35:10.000000 kuut-0.0.2/kuut.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      828 2023-06-24 12:17:46.000000 kuut-0.0.2/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-24 12:17:53.781001 kuut-0.0.2/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 kuut-0.0.2/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-29 16:19:10.416785 kuut-0.0.3/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 kuut-0.0.3/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 kuut-0.0.3/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2208 2023-06-29 16:19:10.416632 kuut-0.0.3/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-29 16:17:53.000000 kuut-0.0.3/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-29 16:19:10.415375 kuut-0.0.3/kuut/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-29 16:19:06.000000 kuut-0.0.3/kuut/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     3601 2023-06-29 16:19:06.000000 kuut-0.0.3/kuut/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     9798 2023-06-29 16:19:06.000000 kuut-0.0.3/kuut/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-29 16:19:10.416429 kuut-0.0.3/kuut.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2208 2023-06-29 16:19:10.000000 kuut-0.0.3/kuut.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      294 2023-06-29 16:19:10.000000 kuut-0.0.3/kuut.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-29 16:19:10.000000 kuut-0.0.3/kuut.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-29 16:19:10.000000 kuut-0.0.3/kuut.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-22 12:35:10.000000 kuut-0.0.3/kuut.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-29 16:19:10.000000 kuut-0.0.3/kuut.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-29 16:19:10.000000 kuut-0.0.3/kuut.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      875 2023-06-29 16:19:06.000000 kuut-0.0.3/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-29 16:19:10.416835 kuut-0.0.3/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 kuut-0.0.3/setup.py
```

### Comparing `kuut-0.0.2/LICENSE` & `kuut-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kuut-0.0.2/kuut/_modidx.py` & `kuut-0.0.3/kuut/_modidx.py`

 * *Files identical despite different names*

### Comparing `kuut-0.0.2/settings.ini` & `kuut-0.0.3/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = kuut
 lib_name = kuut
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = kuut
 nbs_path = nbs
 recursive = True
@@ -18,15 +18,15 @@
 git_url = https://github.com/dsm-72/kuut
 title = kuut
 audience = Developers
 author = dsm-72
 author_email = sumner.magruder@yale.edu
 copyright = 2023 onwards, dsm-72
 description = taqadum: arabic for progress (tqdm). khutuat: arabic for steps (kuut)
-keywords = nbdev jupyter notebook python
+keywords = tqdm kuut progress step stepper interation iter substep notebook interactive
 language = English
 status = 3
 user = dsm-72
 conda_user = dsm-72
 requirements = tqdm
 readme_nb = index.ipynb
 allowed_metadata_keys =
```

### Comparing `kuut-0.0.2/setup.py` & `kuut-0.0.3/setup.py`

 * *Files identical despite different names*

