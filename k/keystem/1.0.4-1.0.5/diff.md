# Comparing `tmp/keystem-1.0.4.tar.gz` & `tmp/keystem-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/naga/Documents/projects/mine/keyroot/dist/.tmp-jk980k96/keystem-1.0.4.tar", last modified: Fri May 26 14:05:24 2023, max compression
+gzip compressed data, was "keystem-1.0.5.tar", last modified: Thu Jun 29 19:42:10 2023, max compression
```

## Comparing `keystem-1.0.4.tar` & `keystem-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-26 14:05:24.000000 keystem-1.0.4/
--rw-r--r--   0 naga       (501) staff       (20)     9077 2023-05-26 14:05:24.000000 keystem-1.0.4/PKG-INFO
--rwxrwxrwx   0 naga       (501) staff       (20)     8499 2023-05-26 11:09:18.000000 keystem-1.0.4/README.md
-drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem/
--rwxrwxrwx   0 naga       (501) staff       (20)       22 2023-05-18 19:25:08.000000 keystem-1.0.4/keystem/__init__.py
--rwxrwxrwx   0 naga       (501) staff       (20)     1735 2023-05-26 11:09:18.000000 keystem-1.0.4/keystem/_kmeans.py
--rwxrwxrwx   0 naga       (501) staff       (20)     3674 2023-05-26 14:04:16.000000 keystem-1.0.4/keystem/keystem.py
-drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/
--rwxrwxrwx   0 naga       (501) staff       (20)     9077 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/PKG-INFO
--rwxrwxrwx   0 naga       (501) staff       (20)      290 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/SOURCES.txt
--rwxrwxrwx   0 naga       (501) staff       (20)        1 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/dependency_links.txt
--rwxrwxrwx   0 naga       (501) staff       (20)       55 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/entry_points.txt
--rwxrwxrwx   0 naga       (501) staff       (20)      144 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/requires.txt
--rwxrwxrwx   0 naga       (501) staff       (20)        8 2023-05-26 14:05:24.000000 keystem-1.0.4/keystem.egg-info/top_level.txt
--rwxrwxrwx   0 naga       (501) staff       (20)     3674 2023-05-26 14:04:20.000000 keystem-1.0.4/keystem.py
--rwxrwxrwx   0 naga       (501) staff       (20)     1356 2023-05-26 14:04:39.000000 keystem-1.0.4/pyproject.toml
--rw-r--r--   0 naga       (501) staff       (20)       38 2023-05-26 14:05:24.000000 keystem-1.0.4/setup.cfg
--rwxrwxrwx   0 naga       (501) staff       (20)     1123 2023-05-26 14:04:34.000000 keystem-1.0.4/setup.py
+drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-06-29 19:42:10.995588 keystem-1.0.5/
+-rw-r--r--   0 naga       (501) staff       (20)     9077 2023-06-29 19:42:10.995333 keystem-1.0.5/PKG-INFO
+-rwxrwxrwx   0 naga       (501) staff       (20)     8499 2023-05-26 11:09:18.000000 keystem-1.0.5/README.md
+drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-06-29 19:42:10.994072 keystem-1.0.5/keystem/
+-rwxrwxrwx   0 naga       (501) staff       (20)       22 2023-05-18 19:25:08.000000 keystem-1.0.5/keystem/__init__.py
+-rwxrwxrwx   0 naga       (501) staff       (20)     1735 2023-05-26 11:09:18.000000 keystem-1.0.5/keystem/_kmeans.py
+-rwxrwxrwx   0 naga       (501) staff       (20)     3745 2023-06-29 19:36:58.000000 keystem-1.0.5/keystem/keystem.py
+drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-06-29 19:42:10.995074 keystem-1.0.5/keystem.egg-info/
+-rwxrwxrwx   0 naga       (501) staff       (20)     9077 2023-06-29 19:42:10.000000 keystem-1.0.5/keystem.egg-info/PKG-INFO
+-rwxrwxrwx   0 naga       (501) staff       (20)      290 2023-06-29 19:42:10.000000 keystem-1.0.5/keystem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)        1 2023-06-29 19:42:10.000000 keystem-1.0.5/keystem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)       55 2023-06-29 19:42:10.000000 keystem-1.0.5/keystem.egg-info/entry_points.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)      144 2023-06-29 19:42:10.000000 keystem-1.0.5/keystem.egg-info/requires.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)        8 2023-06-29 19:42:10.000000 keystem-1.0.5/keystem.egg-info/top_level.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)     3674 2023-05-26 14:04:20.000000 keystem-1.0.5/keystem.py
+-rwxrwxrwx   0 naga       (501) staff       (20)     1356 2023-06-29 19:39:00.000000 keystem-1.0.5/pyproject.toml
+-rw-r--r--   0 naga       (501) staff       (20)       38 2023-06-29 19:42:10.995645 keystem-1.0.5/setup.cfg
+-rwxrwxrwx   0 naga       (501) staff       (20)     1123 2023-06-29 19:39:14.000000 keystem-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `keystem-1.0.4/PKG-INFO` & `keystem-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystem
-Version: 1.0.4
+Version: 1.0.5
 Summary: Extract the keywords from the given text and assign root of the key for each cluster keys
 Home-page: https://github.com/Nagakiran1/keystem.git
 Author: Naga
 Author-email: Naga <naga@caspai.in>
 Project-URL: Homepage, https://github.com/Nagakiran1/keystem
 Keywords: text,keywords,bert,keybert
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keystem-1.0.4/README.md` & `keystem-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `keystem-1.0.4/keystem/_kmeans.py` & `keystem-1.0.5/keystem/_kmeans.py`

 * *Files identical despite different names*

### Comparing `keystem-1.0.4/keystem/keystem.py` & `keystem-1.0.5/keystem.py`

 * *Files identical despite different names*

### Comparing `keystem-1.0.4/keystem.egg-info/PKG-INFO` & `keystem-1.0.5/keystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystem
-Version: 1.0.4
+Version: 1.0.5
 Summary: Extract the keywords from the given text and assign root of the key for each cluster keys
 Home-page: https://github.com/Nagakiran1/keystem.git
 Author: Naga
 Author-email: Naga <naga@caspai.in>
 Project-URL: Homepage, https://github.com/Nagakiran1/keystem
 Keywords: text,keywords,bert,keybert
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keystem-1.0.4/keystem.py` & `keystem-1.0.5/keystem/keystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 
         return tags 
 
     def get_keygroups(
         self,
         text,
         by_sents=False,
-        pos=True,
+        pos=False,
         keyword_thresh = 0.3
     ):
         if isinstance(text, list) and text:
             keywords = text
             keywords = [(k, 1) for k in keywords]
         else:
             if by_sents:    
@@ -90,14 +90,15 @@
 
         res['features'] = res['text'].apply(lambda x: self.preprocess(x, pos=pos))
         res = res.reset_index(drop=True)
         word_frame = res#[['features','keywords']]
         word_frame = word_frame.explode('features')
         word_frame = word_frame.reset_index()
         # word_frame['frame_index'] = word_frame.reset_index
+        word_frame = word_frame.loc[word_frame['features'].notnull()]
         features = np.vstack([i.vector for i in word_frame['features']])
 
 
         clusters, centroids = self.kmeans.predict(features)
 
 
         for c_id, cluster in enumerate(clusters):
```

### Comparing `keystem-1.0.4/pyproject.toml` & `keystem-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keystem"
-version = "1.0.4"
+version = "1.0.5"
 description = "Extract the keywords from the given text and assign root of the key for each cluster keys"
 readme = "README.md"
 authors = [{ name = "Naga", email = "naga@caspai.in" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `keystem-1.0.4/setup.py` & `keystem-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # +
 from setuptools import find_packages, setup
 
 setup(
     name = "keystem",
-    version = "1.0.4",
+    version = "1.0.5",
     author = "Naga",
     author_email = "naga@caspai.in",
     description = "This project helps to have git version for S3 buckets."  ,
     url = "https://github.com/Nagakiran1/keystem.git",
     py_modules=['keystem.keyroots', 'keystem'],
     include_package_data=True,
     classifiers=[
```

