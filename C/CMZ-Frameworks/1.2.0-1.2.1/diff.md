# Comparing `tmp/CMZ_Frameworks-1.2.0.tar.gz` & `tmp/CMZ_Frameworks-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMZ_Frameworks-1.2.0.tar", last modified: Thu Jun 29 08:33:29 2023, max compression
+gzip compressed data, was "CMZ_Frameworks-1.2.1.tar", last modified: Thu Jun 29 08:38:56 2023, max compression
```

## Comparing `CMZ_Frameworks-1.2.0.tar` & `CMZ_Frameworks-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 08:33:29.136150 CMZ_Frameworks-1.2.0/
-drwxrwxrwx   0        0        0        0 2023-06-29 08:33:29.130835 CMZ_Frameworks-1.2.0/CMZ_Frameworks.egg-info/
--rw-rw-rw-   0        0        0      293 2023-06-29 08:33:29.000000 CMZ_Frameworks-1.2.0/CMZ_Frameworks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-06-29 08:33:29.000000 CMZ_Frameworks-1.2.0/CMZ_Frameworks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:33:29.000000 CMZ_Frameworks-1.2.0/CMZ_Frameworks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 08:33:29.000000 CMZ_Frameworks-1.2.0/CMZ_Frameworks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:33:29.000000 CMZ_Frameworks-1.2.0/CMZ_Frameworks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      293 2023-06-29 08:33:29.135226 CMZ_Frameworks-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-29 08:33:29.137148 CMZ_Frameworks-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      421 2023-06-29 08:33:24.000000 CMZ_Frameworks-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:38:56.203033 CMZ_Frameworks-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:38:56.198043 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/
+-rw-rw-rw-   0        0        0      293 2023-06-29 08:38:56.000000 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-29 08:38:56.000000 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:38:56.000000 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 08:38:56.000000 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 08:38:56.000000 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:38:56.000000 CMZ_Frameworks-1.2.1/CMZ_Frameworks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      293 2023-06-29 08:38:56.201047 CMZ_Frameworks-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:38:56.205027 CMZ_Frameworks-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      550 2023-06-29 08:38:52.000000 CMZ_Frameworks-1.2.1/setup.py
```

