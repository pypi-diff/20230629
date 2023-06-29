# Comparing `tmp/kernml-0.0.4.tar.gz` & `tmp/kernml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernml-0.0.4.tar", last modified: Thu Jun 29 19:01:06 2023, max compression
+gzip compressed data, was "kernml-0.0.5.tar", last modified: Thu Jun 29 19:52:26 2023, max compression
```

## Comparing `kernml-0.0.4.tar` & `kernml-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.661566 kernml-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-06-23 01:54:01.000000 kernml-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      417 2023-06-29 19:01:06.661566 kernml-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-06-23 01:52:37.000000 kernml-0.0.4/README.md
--rw-rw-rw-   0        0        0      447 2023-06-29 18:56:28.000000 kernml-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 19:01:06.661566 kernml-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.630317 kernml-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.645943 kernml-0.0.4/src/kernml/
--rw-rw-rw-   0        0        0        0 2023-06-23 05:13:51.000000 kernml-0.0.4/src/kernml/__init__.py
--rw-rw-rw-   0        0        0    26194 2023-06-29 18:59:34.000000 kernml-0.0.4/src/kernml/prg.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:01:06.661566 kernml-0.0.4/src/kernml.egg-info/
--rw-rw-rw-   0        0        0      417 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 19:01:06.000000 kernml-0.0.4/src/kernml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 19:52:26.491865 kernml-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 01:54:01.000000 kernml-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      417 2023-06-29 19:52:26.489868 kernml-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-06-23 01:52:37.000000 kernml-0.0.5/README.md
+-rw-rw-rw-   0        0        0      447 2023-06-29 19:51:46.000000 kernml-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 19:52:26.491865 kernml-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 19:52:26.463938 kernml-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 19:52:26.476903 kernml-0.0.5/src/kernml/
+-rw-rw-rw-   0        0        0        0 2023-06-23 05:13:51.000000 kernml-0.0.5/src/kernml/__init__.py
+-rw-rw-rw-   0        0        0    26194 2023-06-29 19:51:07.000000 kernml-0.0.5/src/kernml/prg.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:52:26.487873 kernml-0.0.5/src/kernml.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-06-29 19:52:26.000000 kernml-0.0.5/src/kernml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-06-29 19:52:26.000000 kernml-0.0.5/src/kernml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 19:52:26.000000 kernml-0.0.5/src/kernml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 19:52:26.000000 kernml-0.0.5/src/kernml.egg-info/top_level.txt
```

### Comparing `kernml-0.0.4/LICENSE` & `kernml-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kernml-0.0.4/src/kernml/prg.py` & `kernml-0.0.5/src/kernml/prg.py`

 * *Files identical despite different names*

