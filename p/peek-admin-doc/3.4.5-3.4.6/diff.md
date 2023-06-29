# Comparing `tmp/peek-admin-doc-3.4.5.tar.gz` & `tmp/peek-admin-doc-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-admin-doc-3.4.5.tar", last modified: Wed Jun 28 07:26:01 2023, max compression
+gzip compressed data, was "peek-admin-doc-3.4.6.tar", last modified: Thu Jun 29 10:19:50 2023, max compression
```

## Comparing `peek-admin-doc-3.4.5.tar` & `peek-admin-doc-3.4.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:01.132066 peek-admin-doc-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-28 07:26:01.131066 peek-admin-doc-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:01.131066 peek-admin-doc-3.4.5/peek_admin_doc/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:26:00.000000 peek-admin-doc-3.4.5/peek_admin_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:01.131066 peek-admin-doc-3.4.5/peek_admin_doc/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:01.131066 peek-admin-doc-3.4.5/peek_admin_doc/_static/fonts/
--rw-r--r--   0 root         (0) root         (0)    77160 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)      556 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/build_html_docs.sh
--rw-r--r--   0 root         (0) root         (0)      545 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/build_latex_docs.sh
--rw-r--r--   0 root         (0) root         (0)    11240 2023-06-28 07:26:00.000000 peek-admin-doc-3.4.5/peek_admin_doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/watch_docs.sh
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-28 07:25:22.000000 peek-admin-doc-3.4.5/peek_admin_doc/welcome.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:01.131066 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-28 07:26:01.000000 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-28 07:26:01.000000 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:01.000000 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:01.000000 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-28 07:26:01.000000 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-28 07:26:01.000000 peek-admin-doc-3.4.5/peek_admin_doc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:01.132066 peek-admin-doc-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3077 2023-06-28 07:26:00.000000 peek-admin-doc-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:50.868344 peek-admin-doc-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-29 10:19:50.868344 peek-admin-doc-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:50.867344 peek-admin-doc-3.4.6/peek_admin_doc/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:50.868344 peek-admin-doc-3.4.6/peek_admin_doc/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:50.868344 peek-admin-doc-3.4.6/peek_admin_doc/_static/fonts/
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/build_html_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/build_latex_docs.sh
+-rw-r--r--   0 root         (0) root         (0)    11240 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/watch_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-29 10:19:13.000000 peek-admin-doc-3.4.6/peek_admin_doc/welcome.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:50.868344 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/peek_admin_doc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:19:50.868344 peek-admin-doc-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-29 10:19:50.000000 peek-admin-doc-3.4.6/setup.py
```

### Comparing `peek-admin-doc-3.4.5/README.rst` & `peek-admin-doc-3.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.5/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2` & `peek-admin-doc-3.4.6/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.5/peek_admin_doc/build_html_docs.sh` & `peek-admin-doc-3.4.6/peek_admin_doc/build_html_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.5/peek_admin_doc/build_latex_docs.sh` & `peek-admin-doc-3.4.6/peek_admin_doc/build_latex_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.5/peek_admin_doc/conf.py` & `peek-admin-doc-3.4.6/peek_admin_doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # sys.path.insert(0, os.path.abspath('.'))
 from sphinx.ext.apidoc import create_modules_toc_file, recurse_tree
 
 title = "Synerty Peek - Administration Documentation"
 __project__ = "SynertyPeek-AdminDocs"
 __copyright__ = "2021, Synerty"
 __author__ = "Synerty"
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 import sphinx_rtd_theme
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
```

### Comparing `peek-admin-doc-3.4.5/peek_admin_doc/watch_docs.sh` & `peek-admin-doc-3.4.6/peek_admin_doc/watch_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.5/peek_admin_doc.egg-info/SOURCES.txt` & `peek-admin-doc-3.4.6/peek_admin_doc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.5/setup.py` & `peek-admin-doc-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_admin_doc"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Admin Docs."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

