# Comparing `tmp/dauth-0.4.tar.gz` & `tmp/dauth-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauth-0.4.tar", last modified: Thu Jun 29 11:42:46 2023, max compression
+gzip compressed data, was "dauth-0.5.tar", last modified: Thu Jun 29 19:46:24 2023, max compression
```

## Comparing `dauth-0.4.tar` & `dauth-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:42:46.633360 dauth-0.4/
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 11:42:46.633360 dauth-0.4/PKG-INFO
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2569 2023-06-21 07:35:06.000000 dauth-0.4/README.md
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)       38 2023-06-29 11:42:46.633360 dauth-0.4/setup.cfg
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      570 2023-06-29 11:42:30.000000 dauth-0.4/setup.py
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:42:46.633360 dauth-0.4/src/
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:42:46.633360 dauth-0.4/src/dauth/
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      187 2023-06-21 07:35:08.000000 dauth-0.4/src/dauth/__init__.py
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      890 2023-06-21 07:35:08.000000 dauth-0.4/src/dauth/auth.py
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 11:42:46.633360 dauth-0.4/src/dauth.egg-info/
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 11:42:46.000000 dauth-0.4/src/dauth.egg-info/PKG-INFO
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      190 2023-06-29 11:42:46.000000 dauth-0.4/src/dauth.egg-info/SOURCES.txt
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)        1 2023-06-29 11:42:46.000000 dauth-0.4/src/dauth.egg-info/dependency_links.txt
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)        6 2023-06-29 11:42:46.000000 dauth-0.4/src/dauth.egg-info/top_level.txt
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 19:46:24.090052 dauth-0.5/PKG-INFO
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2569 2023-06-21 07:35:06.000000 dauth-0.5/README.md
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)       38 2023-06-29 19:46:24.090052 dauth-0.5/setup.cfg
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      570 2023-06-29 19:38:55.000000 dauth-0.5/setup.py
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/src/
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/src/dauth/
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      187 2023-06-21 07:35:08.000000 dauth-0.5/src/dauth/__init__.py
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      903 2023-06-29 19:38:49.000000 dauth-0.5/src/dauth/auth.py
+drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/src/dauth.egg-info/
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/PKG-INFO
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)      190 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/SOURCES.txt
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)        1 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/dependency_links.txt
+-rw-r--r--   0 denvilk   (1000) denvilk   (1000)        6 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/top_level.txt
```

### Comparing `dauth-0.4/PKG-INFO` & `dauth-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.4
+Version: 0.5
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
```

### Comparing `dauth-0.4/README.md` & `dauth-0.5/README.md`

 * *Files identical despite different names*

### Comparing `dauth-0.4/setup.py` & `dauth-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 print(long_description)
 
 if __name__ == '__main__':
     setup(
         name='dauth',
-        version="0.4",
+        version="0.5",
         package_dir={'': 'src'},
         packages=find_packages('src', include=[
             'dauth*'
         ]),
         description='FastAPI ABAC authorization realization',
         long_description=long_description,
         long_description_content_type='text/markdown',
```

### Comparing `dauth-0.4/src/dauth.egg-info/PKG-INFO` & `dauth-0.5/src/dauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.4
+Version: 0.5
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
```

