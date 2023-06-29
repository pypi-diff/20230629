# Comparing `tmp/datalibro_utils-1.0.1.tar.gz` & `tmp/datalibro_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_utils-1.0.1.tar", last modified: Wed Jun 28 06:23:41 2023, max compression
+gzip compressed data, was "datalibro_utils-1.0.2.tar", last modified: Thu Jun 29 10:03:27 2023, max compression
```

## Comparing `datalibro_utils-1.0.1.tar` & `datalibro_utils-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-28 06:23:41.665716 datalibro_utils-1.0.1/
--rw-r--r--   0 livid      (501) staff       (20)      194 2023-06-28 06:23:41.665572 datalibro_utils-1.0.1/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      431 2023-06-21 03:09:04.000000 datalibro_utils-1.0.1/README.md
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-28 06:23:41.664641 datalibro_utils-1.0.1/datalibro_utils/
--rw-r--r--   0 livid      (501) staff       (20)       69 2023-06-28 06:17:23.000000 datalibro_utils-1.0.1/datalibro_utils/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     2828 2023-06-21 02:19:56.000000 datalibro_utils-1.0.1/datalibro_utils/mapping.py
--rw-r--r--   0 livid      (501) staff       (20)       80 2023-06-28 06:14:01.000000 datalibro_utils-1.0.1/datalibro_utils/test.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-28 06:23:41.665398 datalibro_utils-1.0.1/datalibro_utils.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      194 2023-06-28 06:23:41.000000 datalibro_utils-1.0.1/datalibro_utils.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      291 2023-06-28 06:23:41.000000 datalibro_utils-1.0.1/datalibro_utils.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2023-06-28 06:23:41.000000 datalibro_utils-1.0.1/datalibro_utils.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)       19 2023-06-28 06:23:41.000000 datalibro_utils-1.0.1/datalibro_utils.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       16 2023-06-28 06:23:41.000000 datalibro_utils-1.0.1/datalibro_utils.egg-info/top_level.txt
--rw-r--r--   0 livid      (501) staff       (20)       38 2023-06-28 06:23:41.665776 datalibro_utils-1.0.1/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      358 2023-06-28 06:22:59.000000 datalibro_utils-1.0.1/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-29 10:03:27.769456 datalibro_utils-1.0.2/
+-rw-r--r--   0 livid      (501) staff       (20)      194 2023-06-29 10:03:27.769304 datalibro_utils-1.0.2/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      431 2023-06-21 03:09:04.000000 datalibro_utils-1.0.2/README.md
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-29 10:03:27.768348 datalibro_utils-1.0.2/datalibro_utils/
+-rw-r--r--   0 livid      (501) staff       (20)       69 2023-06-28 06:17:23.000000 datalibro_utils-1.0.2/datalibro_utils/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     3389 2023-06-29 09:23:50.000000 datalibro_utils-1.0.2/datalibro_utils/mapping.py
+-rw-r--r--   0 livid      (501) staff       (20)       80 2023-06-28 06:14:01.000000 datalibro_utils-1.0.2/datalibro_utils/test.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-29 10:03:27.769138 datalibro_utils-1.0.2/datalibro_utils.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      194 2023-06-29 10:03:27.000000 datalibro_utils-1.0.2/datalibro_utils.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      291 2023-06-29 10:03:27.000000 datalibro_utils-1.0.2/datalibro_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2023-06-29 10:03:27.000000 datalibro_utils-1.0.2/datalibro_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)       19 2023-06-29 10:03:27.000000 datalibro_utils-1.0.2/datalibro_utils.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       16 2023-06-29 10:03:27.000000 datalibro_utils-1.0.2/datalibro_utils.egg-info/top_level.txt
+-rw-r--r--   0 livid      (501) staff       (20)       38 2023-06-29 10:03:27.769497 datalibro_utils-1.0.2/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      358 2023-06-29 10:02:56.000000 datalibro_utils-1.0.2/setup.py
```

