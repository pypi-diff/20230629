# Comparing `tmp/teamanchorhello-0.0.3.tar.gz` & `tmp/teamanchorhello-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamanchorhello-0.0.3.tar", last modified: Thu Jun 29 18:39:40 2023, max compression
+gzip compressed data, was "teamanchorhello-0.0.4.tar", last modified: Thu Jun 29 18:44:26 2023, max compression
```

## Comparing `teamanchorhello-0.0.3.tar` & `teamanchorhello-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.3/LICENSE
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1329 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      729 2023-06-29 18:37:56.000000 teamanchorhello-0.0.3/README.md
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/setup.cfg
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-29 18:32:06.000000 teamanchorhello-0.0.3/setup.py
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/teamanchorhello/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/teamanchorhello/src/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:39:40.893660 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1329 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-29 18:39:40.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-29 18:32:01.000000 teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.4/LICENSE
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1857 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1161 2023-06-29 18:43:23.000000 teamanchorhello-0.0.4/README.md
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/setup.cfg
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-29 18:43:38.000000 teamanchorhello-0.0.4/setup.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/teamanchorhello/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/teamanchorhello/src/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1857 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-29 18:43:40.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.py
```

### Comparing `teamanchorhello-0.0.3/PKG-INFO` & `teamanchorhello-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.3
+Version: 0.0.4
 Summary: teamanchor say hello using Pypi package.
 Home-page: UNKNOWN
 Author: fanis
 License: UNKNOWN
 Description: ## TEAMANCHORHELLO
         
         Team Anchor say hello using Pypi package.
@@ -21,19 +21,31 @@
         5. pyhon3
             * import teamanchorhello
             * teamanchorhello.hello()
         6. Upload to testpypi:
             * python3 -m twine upload --repository testpypi dist/*
                 * Enter user & password (register if you didn't have).
         7. Upload to pypi:
-            * python3 -m t
+            * python3 -m twine upload dist/*
         
+        ## FASTEST WAY
+        1. $vim teamanchorhello\src\teamanchorhello.py
+            * print('Team Anchor say hello <UPDATE>')
+        2. $vim setup.py
+            * version: <UPDATE>
+        3. Delete file in dist/*
+            * rm -rf dist/*
+        4. Upload to Pypi:
+            * python3 -m twine upload dist/*
         ## PYPI
         TESTPYPI: https://test.pypi.org/project/teamanchorhello/
         PYPI: https://pypi.org/project/teamanchorhello/
         
+        ## CERTIFICATE ISSUE
+        * Can't use venv, exit venv & upload to Pypi.
+        * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamanchorhello-0.0.3/README.md` & `teamanchorhello-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,12 +14,25 @@
 5. pyhon3
     * import teamanchorhello
     * teamanchorhello.hello()
 6. Upload to testpypi:
     * python3 -m twine upload --repository testpypi dist/*
         * Enter user & password (register if you didn't have).
 7. Upload to pypi:
-    * python3 -m t
+    * python3 -m twine upload dist/*
 
+## FASTEST WAY
+1. $vim teamanchorhello\src\teamanchorhello.py
+    * print('Team Anchor say hello <UPDATE>')
+2. $vim setup.py
+    * version: <UPDATE>
+3. Delete file in dist/*
+    * rm -rf dist/*
+4. Upload to Pypi:
+    * python3 -m twine upload dist/*
 ## PYPI
 TESTPYPI: https://test.pypi.org/project/teamanchorhello/
 PYPI: https://pypi.org/project/teamanchorhello/
+
+## CERTIFICATE ISSUE
+* Can't use venv, exit venv & upload to Pypi.
+* If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
```

### Comparing `teamanchorhello-0.0.3/setup.py` & `teamanchorhello-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="teamanchorhello",
-    version="0.0.3",
+    version="0.0.4",
     author="fanis",
     description="teamanchor say hello using Pypi package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `teamanchorhello-0.0.3/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO` & `teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.3
+Version: 0.0.4
 Summary: teamanchor say hello using Pypi package.
 Home-page: UNKNOWN
 Author: fanis
 License: UNKNOWN
 Description: ## TEAMANCHORHELLO
         
         Team Anchor say hello using Pypi package.
@@ -21,19 +21,31 @@
         5. pyhon3
             * import teamanchorhello
             * teamanchorhello.hello()
         6. Upload to testpypi:
             * python3 -m twine upload --repository testpypi dist/*
                 * Enter user & password (register if you didn't have).
         7. Upload to pypi:
-            * python3 -m t
+            * python3 -m twine upload dist/*
         
+        ## FASTEST WAY
+        1. $vim teamanchorhello\src\teamanchorhello.py
+            * print('Team Anchor say hello <UPDATE>')
+        2. $vim setup.py
+            * version: <UPDATE>
+        3. Delete file in dist/*
+            * rm -rf dist/*
+        4. Upload to Pypi:
+            * python3 -m twine upload dist/*
         ## PYPI
         TESTPYPI: https://test.pypi.org/project/teamanchorhello/
         PYPI: https://pypi.org/project/teamanchorhello/
         
+        ## CERTIFICATE ISSUE
+        * Can't use venv, exit venv & upload to Pypi.
+        * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

