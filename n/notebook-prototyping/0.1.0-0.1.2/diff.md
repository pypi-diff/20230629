# Comparing `tmp/notebook_prototyping-0.1.0.tar.gz` & `tmp/notebook_prototyping-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_prototyping-0.1.0.tar", last modified: Thu Jun 29 10:43:51 2023, max compression
+gzip compressed data, was "notebook_prototyping-0.1.2.tar", last modified: Thu Jun 29 11:13:23 2023, max compression
```

## Comparing `notebook_prototyping-0.1.0.tar` & `notebook_prototyping-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:51.992020 notebook_prototyping-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      257 2023-06-29 10:43:51.992020 notebook_prototyping-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:51.979026 notebook_prototyping-0.1.0/nested/
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:51.984021 notebook_prototyping-0.1.0/nested/directory/
--rw-rw-rw-   0        0        0      111 2023-06-18 08:27:53.000000 notebook_prototyping-0.1.0/nested/directory/third_example.py
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:51.991020 notebook_prototyping-0.1.0/notebook_prototyping.egg-info/
--rw-rw-rw-   0        0        0      257 2023-06-29 10:43:51.000000 notebook_prototyping-0.1.0/notebook_prototyping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-29 10:43:51.000000 notebook_prototyping-0.1.0/notebook_prototyping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 10:43:51.000000 notebook_prototyping-0.1.0/notebook_prototyping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 10:43:51.000000 notebook_prototyping-0.1.0/notebook_prototyping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-29 10:43:51.993020 notebook_prototyping-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-06-29 10:43:17.000000 notebook_prototyping-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:13:23.371659 notebook_prototyping-0.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-18 09:21:31.000000 notebook_prototyping-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      256 2023-06-29 11:13:23.372666 notebook_prototyping-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 11:13:23.355659 notebook_prototyping-0.1.2/nested/
+drwxrwxrwx   0        0        0        0 2023-06-29 11:13:23.361659 notebook_prototyping-0.1.2/nested/directory/
+-rw-rw-rw-   0        0        0      111 2023-06-18 08:27:53.000000 notebook_prototyping-0.1.2/nested/directory/third_example.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:13:23.370659 notebook_prototyping-0.1.2/notebook_prototyping.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-06-29 11:13:23.000000 notebook_prototyping-0.1.2/notebook_prototyping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-29 11:13:23.000000 notebook_prototyping-0.1.2/notebook_prototyping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:13:23.000000 notebook_prototyping-0.1.2/notebook_prototyping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 11:13:23.000000 notebook_prototyping-0.1.2/notebook_prototyping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-29 11:13:23.373659 notebook_prototyping-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      374 2023-06-29 11:13:17.000000 notebook_prototyping-0.1.2/setup.py
```

### Comparing `notebook_prototyping-0.1.0/LICENSE` & `notebook_prototyping-0.1.2/LICENSE`

 * *Files identical despite different names*

