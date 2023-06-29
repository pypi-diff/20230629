# Comparing `tmp/peek-office-doc-3.4.5.tar.gz` & `tmp/peek-office-doc-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-office-doc-3.4.5.tar", last modified: Wed Jun 28 07:27:04 2023, max compression
+gzip compressed data, was "peek-office-doc-3.4.6.tar", last modified: Thu Jun 29 10:20:52 2023, max compression
```

## Comparing `peek-office-doc-3.4.5.tar` & `peek-office-doc-3.4.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:04.637087 peek-office-doc-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-28 07:27:04.636087 peek-office-doc-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:04.636087 peek-office-doc-3.4.5/peek_office_doc/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:04.636087 peek-office-doc-3.4.5/peek_office_doc/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:04.636087 peek-office-doc-3.4.5/peek_office_doc/_static/fonts/
--rw-r--r--   0 root         (0) root         (0)    77160 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)      556 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/build_html_docs.sh
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/build_latex_docs.sh
--rw-r--r--   0 root         (0) root         (0)    10786 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/watch_docs.sh
--rw-r--r--   0 root         (0) root         (0)      233 2023-06-28 07:25:24.000000 peek-office-doc-3.4.5/peek_office_doc/welcome.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:04.636087 peek-office-doc-3.4.5/peek_office_doc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/peek_office_doc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:27:04.637087 peek-office-doc-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3091 2023-06-28 07:27:04.000000 peek-office-doc-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:52.355463 peek-office-doc-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-29 10:20:52.354462 peek-office-doc-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:52.354462 peek-office-doc-3.4.6/peek_office_doc/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:52.354462 peek-office-doc-3.4.6/peek_office_doc/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:52.354462 peek-office-doc-3.4.6/peek_office_doc/_static/fonts/
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/build_html_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/build_latex_docs.sh
+-rw-r--r--   0 root         (0) root         (0)    10786 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/watch_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-29 10:19:15.000000 peek-office-doc-3.4.6/peek_office_doc/welcome.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:52.354462 peek-office-doc-3.4.6/peek_office_doc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/peek_office_doc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:52.355463 peek-office-doc-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3091 2023-06-29 10:20:52.000000 peek-office-doc-3.4.6/setup.py
```

### Comparing `peek-office-doc-3.4.5/README.rst` & `peek-office-doc-3.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `peek-office-doc-3.4.5/peek_office_doc/_static/fonts/fontawesome-webfont.woff2` & `peek-office-doc-3.4.6/peek_office_doc/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `peek-office-doc-3.4.5/peek_office_doc/build_html_docs.sh` & `peek-office-doc-3.4.6/peek_office_doc/build_html_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-office-doc-3.4.5/peek_office_doc/build_latex_docs.sh` & `peek-office-doc-3.4.6/peek_office_doc/build_latex_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-office-doc-3.4.5/peek_office_doc/conf.py` & `peek-office-doc-3.4.6/peek_office_doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 title = "Synerty Peek - Office App Documentation"
 __project__ = "SynertyPeek-OfficeAppDocs"
 __copyright__ = "2019, Synerty"
 __author__ = "Synerty"
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 import sphinx_rtd_theme
 
 # -- General configuration ------------------------------------------------
 
 #
 # needs_sphinx = '1.0'
```

### Comparing `peek-office-doc-3.4.5/peek_office_doc/watch_docs.sh` & `peek-office-doc-3.4.6/peek_office_doc/watch_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-office-doc-3.4.5/peek_office_doc.egg-info/SOURCES.txt` & `peek-office-doc-3.4.6/peek_office_doc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-office-doc-3.4.5/setup.py` & `peek-office-doc-3.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_office_doc"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Developer Documentation."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

