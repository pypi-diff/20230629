# Comparing `tmp/pyrdp-0.1.4.tar.gz` & `tmp/pyrdp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdp-0.1.4.tar", last modified: Mon Jun  5 12:16:22 2023, max compression
+gzip compressed data, was "pyrdp-0.1.5.tar", last modified: Thu Jun 29 07:16:04 2023, max compression
```

## Comparing `pyrdp-0.1.4.tar` & `pyrdp-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1064 2023-04-30 09:47:21.216851 pyrdp-0.1.4/LICENSE
--rw-r--r--   0        0        0      445 2023-04-30 10:22:49.318096 pyrdp-0.1.4/README.md
--rw-r--r--   0        0        0      455 2023-06-05 12:16:22.980137 pyrdp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2210 2023-06-05 12:13:11.510555 pyrdp-0.1.4/pyrdp/__init__.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 pyrdp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 09:47:21.216851 pyrdp-0.1.5/LICENSE
+-rw-r--r--   0        0        0      445 2023-04-30 10:22:49.318096 pyrdp-0.1.5/README.md
+-rw-r--r--   0        0        0      455 2023-06-29 07:16:04.076036 pyrdp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2210 2023-06-05 12:13:11.510555 pyrdp-0.1.5/pyrdp/__init__.py
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 pyrdp-0.1.5/PKG-INFO
```

### Comparing `pyrdp-0.1.4/LICENSE` & `pyrdp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdp-0.1.4/pyrdp/__init__.py` & `pyrdp-0.1.5/pyrdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrdp-0.1.4/PKG-INFO` & `pyrdp-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrdp
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple Rammer-Douglas-Peuker algorithm implementation.
 Author-Email: Florian Stasse <f.stasse@skipperndt.com>
 License: MIT
 Requires-Python: >=3.8
-Requires-Dist: numpy>=1.24.3
+Requires-Dist: numpy>=1.23.4
 Description-Content-Type: text/markdown
 
 # Ramer-Douglas-Peucker
 
 Ramer-Douglas-Peucker python implementation.
 
 ## Installation
```

