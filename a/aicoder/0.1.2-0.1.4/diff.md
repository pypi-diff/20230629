# Comparing `tmp/aicoder-0.1.2.tar.gz` & `tmp/aicoder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicoder-0.1.2.tar", last modified: Thu Jun 29 11:02:58 2023, max compression
+gzip compressed data, was "aicoder-0.1.4.tar", last modified: Thu Jun 29 11:17:11 2023, max compression
```

## Comparing `aicoder-0.1.2.tar` & `aicoder-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:02:58.419856 aicoder-0.1.2/
--rw-r--r--   0 carlospolop   (501) staff       (20)    18809 2023-06-29 00:13:10.000000 aicoder-0.1.2/LICENSE
--rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 11:02:58.419707 aicoder-0.1.2/PKG-INFO
--rw-r--r--   0 carlospolop   (501) staff       (20)      507 2023-06-29 00:52:18.000000 aicoder-0.1.2/README.md
-drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:02:58.418267 aicoder-0.1.2/aicoder/
--rw-r--r--   0 carlospolop   (501) staff       (20)    12624 2023-06-28 23:41:03.000000 aicoder-0.1.2/aicoder/AICoder.py
--rw-r--r--   0 carlospolop   (501) staff       (20)     8120 2023-06-28 17:08:14.000000 aicoder-0.1.2/aicoder/AICoderFull.py
--rw-r--r--   0 carlospolop   (501) staff       (20)     4803 2023-06-28 17:02:35.000000 aicoder-0.1.2/aicoder/AICoderPartial.py
--rw-r--r--   0 carlospolop   (501) staff       (20)     3481 2023-06-28 23:49:28.000000 aicoder-0.1.2/aicoder/AICoderPrompts.py
--rw-r--r--   0 carlospolop   (501) staff       (20)        0 2023-06-28 23:57:06.000000 aicoder-0.1.2/aicoder/__init__.py
-drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:02:58.419457 aicoder-0.1.2/aicoder.egg-info/
--rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/PKG-INFO
--rw-r--r--   0 carlospolop   (501) staff       (20)      328 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/SOURCES.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)        1 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/dependency_links.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)       41 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/entry_points.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)       39 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/requires.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)        8 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/top_level.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)       38 2023-06-29 11:02:58.419909 aicoder-0.1.2/setup.cfg
--rw-r--r--   0 carlospolop   (501) staff       (20)      731 2023-06-29 11:02:52.000000 aicoder-0.1.2/setup.py
+drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:17:11.126525 aicoder-0.1.4/
+-rw-r--r--   0 carlospolop   (501) staff       (20)    18809 2023-06-29 00:13:10.000000 aicoder-0.1.4/LICENSE
+-rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 11:17:11.126373 aicoder-0.1.4/PKG-INFO
+-rw-r--r--   0 carlospolop   (501) staff       (20)      507 2023-06-29 00:52:18.000000 aicoder-0.1.4/README.md
+drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:17:11.124830 aicoder-0.1.4/aicoder/
+-rw-r--r--   0 carlospolop   (501) staff       (20)    12624 2023-06-28 23:41:03.000000 aicoder-0.1.4/aicoder/AICoder.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     8120 2023-06-28 17:08:14.000000 aicoder-0.1.4/aicoder/AICoderFull.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     4803 2023-06-28 17:02:35.000000 aicoder-0.1.4/aicoder/AICoderPartial.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     3481 2023-06-28 23:49:28.000000 aicoder-0.1.4/aicoder/AICoderPrompts.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:14:56.000000 aicoder-0.1.4/aicoder/__init__.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     5302 2023-06-29 11:14:54.000000 aicoder-0.1.4/aicoder/main.py
+drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:17:11.126157 aicoder-0.1.4/aicoder.egg-info/
+-rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 11:17:11.000000 aicoder-0.1.4/aicoder.egg-info/PKG-INFO
+-rw-r--r--   0 carlospolop   (501) staff       (20)      344 2023-06-29 11:17:11.000000 aicoder-0.1.4/aicoder.egg-info/SOURCES.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)        1 2023-06-29 11:17:11.000000 aicoder-0.1.4/aicoder.egg-info/dependency_links.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)       46 2023-06-29 11:17:11.000000 aicoder-0.1.4/aicoder.egg-info/entry_points.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)       39 2023-06-29 11:17:11.000000 aicoder-0.1.4/aicoder.egg-info/requires.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)        8 2023-06-29 11:17:11.000000 aicoder-0.1.4/aicoder.egg-info/top_level.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)       38 2023-06-29 11:17:11.126574 aicoder-0.1.4/setup.cfg
+-rw-r--r--   0 carlospolop   (501) staff       (20)      768 2023-06-29 11:16:59.000000 aicoder-0.1.4/setup.py
```

### Comparing `aicoder-0.1.2/LICENSE` & `aicoder-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.2/aicoder/AICoder.py` & `aicoder-0.1.4/aicoder/AICoder.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.2/aicoder/AICoderFull.py` & `aicoder-0.1.4/aicoder/AICoderFull.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.2/aicoder/AICoderPartial.py` & `aicoder-0.1.4/aicoder/AICoderPartial.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.2/aicoder/AICoderPrompts.py` & `aicoder-0.1.4/aicoder/AICoderPrompts.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.2/setup.py` & `aicoder-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 #python3 setup.py sdist
 #twine upload dist/*
 
 
 setup(
     name='aicoder',
-    version='0.1.2',
+    version='0.1.4',
     url='https://github.com/carlospolop/AICoder',
     author='Carlos Polop',
     author_email='carlospolop@gmail.com',
     description='This is a tool to generate code using OpenAI api.',
-    packages=find_packages(),    
+    packages=find_packages(include=["aicoder", "aicoder.*"]),    
     install_requires=[
         'requests',
         'colorlog',
         'openai',
         'tqdm',
         'PyGithub'
     ],
     entry_points={
         'console_scripts': [
-            'aicoder=aicoder:main',
+            'aicoder=aicoder.main:main',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License (GPL)',
     ],
 )
```

