# Comparing `tmp/cloci-0.0.8.tar.gz` & `tmp/cloci-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloci-0.0.8.tar", last modified: Wed Jun 28 22:59:37 2023, max compression
+gzip compressed data, was "cloci-0.0.9.tar", last modified: Wed Jun 28 23:00:12 2023, max compression
```

## Comparing `cloci-0.0.8.tar` & `cloci-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 22:59:37.603814 cloci-0.0.8/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    34207 2023-06-21 18:37:49.000000 cloci-0.0.8/LICENSE
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     4367 2023-06-28 22:59:37.601820 cloci-0.0.8/PKG-INFO
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3894 2023-06-21 18:37:25.000000 cloci-0.0.8/README.md
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      696 2023-06-21 18:37:25.000000 cloci-0.0.8/TODO.md
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 22:59:37.485820 cloci-0.0.8/cloci/
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 22:59:37.526821 cloci-0.0.8/cloci/cloci.egg-info/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     4367 2023-06-28 22:59:37.000000 cloci-0.0.8/cloci/cloci.egg-info/PKG-INFO
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      532 2023-06-28 22:59:37.000000 cloci-0.0.8/cloci/cloci.egg-info/SOURCES.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2023-06-28 22:59:37.000000 cloci-0.0.8/cloci/cloci.egg-info/dependency_links.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      107 2023-06-28 22:59:37.000000 cloci-0.0.8/cloci/cloci.egg-info/requires.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       10 2023-06-28 22:59:37.000000 cloci-0.0.8/cloci/cloci.egg-info/top_level.txt
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 22:59:37.554816 cloci-0.0.8/cloci/lib/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:01.000000 cloci-0.0.8/cloci/lib/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    27794 2023-06-28 00:57:46.000000 cloci-0.0.8/cloci/lib/evo_conco.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    18698 2023-06-28 00:57:46.000000 cloci-0.0.8/cloci/lib/generate_nulls.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16702 2023-06-28 00:57:46.000000 cloci-0.0.8/cloci/lib/hgp2hgx.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74109 2023-06-28 00:57:46.000000 cloci-0.0.8/cloci/lib/hgx2hlgs.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    36251 2023-05-30 17:06:24.000000 cloci-0.0.8/cloci/lib/input_parsing.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    39842 2023-06-28 00:57:46.000000 cloci-0.0.8/cloci/lib/output_data.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     7114 2023-05-30 17:03:59.000000 cloci-0.0.8/cloci/lib/treecalcs.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 22:59:37.585817 cloci-0.0.8/cloci/tools/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:06.000000 cloci-0.0.8/cloci/tools/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23144 2023-05-04 18:14:28.000000 cloci-0.0.8/cloci/tools/cloci2enrich.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13698 2023-06-28 00:57:46.000000 cloci-0.0.8/cloci/tools/cloci2stats.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     9802 2023-06-16 22:09:29.000000 cloci-0.0.8/cloci/tools/hlg2biofile.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17241 2023-06-16 22:09:33.000000 cloci-0.0.8/cloci/tools/hlg2hlg_net.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2023-06-28 22:59:37.603821 cloci-0.0.8/setup.cfg
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1272 2023-06-28 22:59:36.000000 cloci-0.0.8/setup.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.821971 cloci-0.0.9/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    34207 2023-06-21 18:37:49.000000 cloci-0.0.9/LICENSE
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     4367 2023-06-28 23:00:12.819971 cloci-0.0.9/PKG-INFO
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3894 2023-06-21 18:37:25.000000 cloci-0.0.9/README.md
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      696 2023-06-21 18:37:25.000000 cloci-0.0.9/TODO.md
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.696979 cloci-0.0.9/cloci/
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.732017 cloci-0.0.9/cloci/cloci.egg-info/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     4367 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/PKG-INFO
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      532 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/SOURCES.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/dependency_links.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      107 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/requires.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       10 2023-06-28 23:00:12.000000 cloci-0.0.9/cloci/cloci.egg-info/top_level.txt
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.777976 cloci-0.0.9/cloci/lib/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:01.000000 cloci-0.0.9/cloci/lib/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    27794 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/evo_conco.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    18698 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/generate_nulls.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16702 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/hgp2hgx.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74109 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/hgx2hlgs.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    36251 2023-05-30 17:06:24.000000 cloci-0.0.9/cloci/lib/input_parsing.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    39842 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/lib/output_data.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     7114 2023-05-30 17:03:59.000000 cloci-0.0.9/cloci/lib/treecalcs.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-06-28 23:00:12.815973 cloci-0.0.9/cloci/tools/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:06.000000 cloci-0.0.9/cloci/tools/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23144 2023-05-04 18:14:28.000000 cloci-0.0.9/cloci/tools/cloci2enrich.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13698 2023-06-28 00:57:46.000000 cloci-0.0.9/cloci/tools/cloci2stats.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     9802 2023-06-16 22:09:29.000000 cloci-0.0.9/cloci/tools/hlg2biofile.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17241 2023-06-16 22:09:33.000000 cloci-0.0.9/cloci/tools/hlg2hlg_net.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2023-06-28 23:00:12.822974 cloci-0.0.9/setup.cfg
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1249 2023-06-28 23:00:11.000000 cloci-0.0.9/setup.py
```

### Comparing `cloci-0.0.8/LICENSE` & `cloci-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/PKG-INFO` & `cloci-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Function-agnostic gene cluster detection
 Home-page: https://github.com/xonq/cloci/
 Author: xonq
 Author-email: konkelzach@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cloci-0.0.8/README.md` & `cloci-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/TODO.md` & `cloci-0.0.9/TODO.md`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/cloci.egg-info/PKG-INFO` & `cloci-0.0.9/cloci/cloci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Function-agnostic gene cluster detection
 Home-page: https://github.com/xonq/cloci/
 Author: xonq
 Author-email: konkelzach@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cloci-0.0.8/cloci/cloci.egg-info/SOURCES.txt` & `cloci-0.0.9/cloci/cloci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/evo_conco.py` & `cloci-0.0.9/cloci/lib/evo_conco.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/generate_nulls.py` & `cloci-0.0.9/cloci/lib/generate_nulls.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/hgp2hgx.py` & `cloci-0.0.9/cloci/lib/hgp2hgx.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/hgx2hlgs.py` & `cloci-0.0.9/cloci/lib/hgx2hlgs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/input_parsing.py` & `cloci-0.0.9/cloci/lib/input_parsing.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/output_data.py` & `cloci-0.0.9/cloci/lib/output_data.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/lib/treecalcs.py` & `cloci-0.0.9/cloci/lib/treecalcs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/tools/cloci2enrich.py` & `cloci-0.0.9/cloci/tools/cloci2enrich.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/tools/cloci2stats.py` & `cloci-0.0.9/cloci/tools/cloci2stats.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/tools/hlg2biofile.py` & `cloci-0.0.9/cloci/tools/hlg2biofile.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/cloci/tools/hlg2hlg_net.py` & `cloci-0.0.9/cloci/tools/hlg2hlg_net.py`

 * *Files identical despite different names*

### Comparing `cloci-0.0.8/setup.py` & `cloci-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open( "README.md", "r" ) as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "cloci",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "xonq",
     author_email = "konkelzach@protonmail.com",
     description = "Function-agnostic gene cluster detection",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/xonq/cloci/",
     package_dir={"": "cloci"},
     packages = setuptools.find_packages( where="cloci" ),
-    scripts = ['README.md', 'TODO.md', 'cloci/prepUpdate.py', 'cloci/setup.py', 'cloci/lib/output_data.py', 'cloci/lib/evo_conco.py', 'cloci/lib/generate_nulls.py', 'cloci/lib/hgp2hgx.py', 'cloci/lib/hgx2hlgs.py', 'cloci/lib/input_parsing.py', 'cloci/lib/treecalcs.py', 'README.md', 'TODO.md'],
+    scripts = ['README.md', 'TODO.md', 'cloci/setup.py', 'cloci/lib/output_data.py', 'cloci/lib/evo_conco.py', 'cloci/lib/generate_nulls.py', 'cloci/lib/hgp2hgx.py', 'cloci/lib/hgx2hlgs.py', 'cloci/lib/input_parsing.py', 'cloci/lib/treecalcs.py', 'README.md', 'TODO.md'],
     install_requires = ['mycotools', 'numpy', 'scipy', 'graph-tools', 'cogent3'
                         'sniffio', 'pydantic', 'PyYAML', 'SQLAlchemy', 'packaging',
                         'pydantic', 'anyio', 'attrs'],
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: POSIX :: Linux",
```

