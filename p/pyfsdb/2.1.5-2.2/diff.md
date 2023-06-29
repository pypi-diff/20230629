# Comparing `tmp/pyfsdb-2.1.5.tar.gz` & `tmp/pyfsdb-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsdb-2.1.5.tar", last modified: Tue May 23 21:00:24 2023, max compression
+gzip compressed data, was "pyfsdb-2.2.tar", last modified: Thu Jun 29 21:16:45 2023, max compression
```

## Comparing `pyfsdb-2.1.5.tar` & `pyfsdb-2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-04-12 16:27:12.000000 pyfsdb-2.1.5/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-11 15:10:15.000000 pyfsdb-2.1.5/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.815670 pyfsdb-2.1.5/mod/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2020-10-09 02:50:07.000000 pyfsdb-2.1.5/mod/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       21 2020-10-09 02:49:47.000000 pyfsdb-2.1.5/mod/ick.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.815670 pyfsdb-2.1.5/pyfsdb/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/__init__.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35299 2023-05-23 20:58:56.000000 pyfsdb-2.1.5/pyfsdb/fsdb.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.817669 pyfsdb-2.1.5/pyfsdb/obsolete/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/db2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbensure.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbformat.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbfullpivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbheatmap.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbnormalize.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbreescape.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbreversepivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbsplitter.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbtopn.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/pyfsdb/tools/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/__init__.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/bro2fsdb.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/fsdb2json.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/fsdb2many.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/json2fsdb.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-10-25 20:28:42.000000 pyfsdb-2.1.5/pyfsdb/tools/pdb2sql.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-10 17:33:49.000000 pyfsdb-2.1.5/pyfsdb/tools/pdb2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdb2to1.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbaddtypes.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbcdf.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     3430 2023-01-10 19:40:21.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbdatetoepoch.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-10 17:33:49.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbensure.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbepochtodate.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2023-01-11 16:18:55.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbformat.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbfullpivot.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbheatmap.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-23 22:31:04.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbjinja.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbnormalize.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbreescape.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2023-01-27 16:33:47.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbreversepivot.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-15 21:23:13.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbroc.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3230 2023-05-23 20:59:33.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbrow.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3524 2023-05-23 20:59:33.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbroweval.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbsplitter.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbtopn.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-05-03 15:01:57.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.816670 pyfsdb-2.1.5/pyfsdb.egg-info/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1532 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/entry_points.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       11 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3323 2023-05-23 20:59:58.000000 pyfsdb-2.1.5/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:16:45.600122 pyfsdb-2.2/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-04-12 16:27:12.000000 pyfsdb-2.2/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6052 2023-06-29 21:16:45.600122 pyfsdb-2.2/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-11 15:10:15.000000 pyfsdb-2.2/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:16:45.596122 pyfsdb-2.2/mod/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2020-10-09 02:50:07.000000 pyfsdb-2.2/mod/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       21 2020-10-09 02:49:47.000000 pyfsdb-2.2/mod/ick.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:16:45.596122 pyfsdb-2.2/pyfsdb/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/__init__.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    38466 2023-06-29 21:14:33.000000 pyfsdb-2.2/pyfsdb/fsdb.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:16:45.597122 pyfsdb-2.2/pyfsdb/obsolete/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/db2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbdatetoepoch.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbensure.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbformat.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbfullpivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbheatmap.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbnormalize.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbreescape.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbreversepivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbsplitter.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbtopn.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/obsolete/dbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:16:45.600122 pyfsdb-2.2/pyfsdb/tools/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/__init__.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/bro2fsdb.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/fsdb2json.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/fsdb2many.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/json2fsdb.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-10-25 20:28:42.000000 pyfsdb-2.2/pyfsdb/tools/pdb2sql.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-10 17:33:49.000000 pyfsdb-2.2/pyfsdb/tools/pdb2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdb2to1.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbaddtypes.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbcdf.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     3451 2023-06-29 20:04:45.000000 pyfsdb-2.2/pyfsdb/tools/pdbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbdatetoepoch.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-10 17:33:49.000000 pyfsdb-2.2/pyfsdb/tools/pdbensure.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbepochtodate.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2023-01-11 16:18:55.000000 pyfsdb-2.2/pyfsdb/tools/pdbformat.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbfullpivot.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbheatmap.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-23 22:31:04.000000 pyfsdb-2.2/pyfsdb/tools/pdbjinja.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbnormalize.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbreescape.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2678 2023-06-29 20:04:45.000000 pyfsdb-2.2/pyfsdb/tools/pdbreversepivot.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-15 21:23:13.000000 pyfsdb-2.2/pyfsdb/tools/pdbroc.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3251 2023-06-29 20:04:45.000000 pyfsdb-2.2/pyfsdb/tools/pdbrow.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3545 2023-06-29 20:04:45.000000 pyfsdb-2.2/pyfsdb/tools/pdbroweval.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbsplitter.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-07-13 23:54:39.000000 pyfsdb-2.2/pyfsdb/tools/pdbtopn.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-05-03 15:01:57.000000 pyfsdb-2.2/pyfsdb/tools/pdbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:16:45.596122 pyfsdb-2.2/pyfsdb.egg-info/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6052 2023-06-29 21:16:45.000000 pyfsdb-2.2/pyfsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1532 2023-06-29 21:16:45.000000 pyfsdb-2.2/pyfsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-06-29 21:16:45.000000 pyfsdb-2.2/pyfsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-06-29 21:16:45.000000 pyfsdb-2.2/pyfsdb.egg-info/entry_points.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       11 2023-06-29 21:16:45.000000 pyfsdb-2.2/pyfsdb.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-06-29 21:16:45.600122 pyfsdb-2.2/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3321 2023-06-29 21:16:04.000000 pyfsdb-2.2/setup.py
```

### Comparing `pyfsdb-2.1.5/LICENSE` & `pyfsdb-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/PKG-INFO` & `pyfsdb-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.5
+Version: 2.2
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-2.1.5/README.md` & `pyfsdb-2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/fsdb.py` & `pyfsdb-2.2/pyfsdb/fsdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 f = pyfsdb.Fsdb("data.fsdb", out_file="output.fsdb")
 results = f.filter(myfilt)
 
 """
 
 import sys
+import os
+import io
 
 if sys.version_info[0] < 3:
     raise Exception("Must be using Python 3")
 
 RETURN_AS_ARRAY = 1
 RETURN_AS_DICTIONARY = 2
 
@@ -104,14 +106,15 @@
     _out_column_names_set = False
     _out_separator = "\t"
     _out_separator_token = "t"
     _out_command_line = "____BROKEN____"  # ick, magic
     _save_command_history = True
     _handle_compressed = True
     _compression_checked = False
+    _commands = False
 
     def __init__(
         self,
         filename=None,
         file_handle=None,
         return_type=RETURN_AS_ARRAY,
         out_file=None,
@@ -128,23 +131,27 @@
     ):
         """Returns a Fsdb class that can be used as an iterator.
 
         return_type can be pyfsdb.RETURN_AS_ARRAY (default) or
         RETURN_AS_DICTIONARY to return dictionary based rows with
         indexes as columns (this is slower).
 
-        If `pass_comments` is True and both an input and output file
+        If `pass_comments` is "y" and both an input and output file
         handle are available, any comments read in while reading
         are printed to the output.
 
+        If `save_command_history` is True, then comments will be saved
+        to the comments attribute.
+
         `converters` may be passed in as an array or dict of
         converters to call (such as int, float, etc)
 
         If `handle_compressed` is True (the default), the class will
         do its best to handle compressed formats: bz2, gzip, and xz (lzma).
+
         """
 
         self.return_type = return_type
         self.filename = filename
         self.fileh = file_handle
         self._column_names = column_names
         self._pass_comments = pass_comments
@@ -414,14 +421,18 @@
         return self._out_column_names
 
     @property
     def comments(self):
         """Returns a list of comments seen in the document"""
         return self._comments
 
+    @property
+    def commands(self):
+        return self.parse_commands()
+
     @out_column_names.setter
     def out_column_names(self, values):
         mapping = self.__create_column_name_mapping__(values)
 
     # support functions
 
     def create_header_line(self, columns=None, separator_token=None, init_row=None):
@@ -665,15 +676,15 @@
 
                 self._write_header_line()
 
             if self._pass_comments == "y":
                 self._out_file_handle.write(line)
             else:
                 self._comments.append(line)
-        elif self._save_command_history:
+        elif self._pass_comments == "y":
             self._comments.append(line)
 
         return next(self.fileh)
 
     def _convert_array_values(self, row):
         for (n, converter) in enumerate(self._converters):
             if row[n] == "-" or row[n] == "":
@@ -1032,20 +1043,113 @@
     # backwards compatible ... don't use
     def write_row(self, row=None):
         self.append(row)
 
     def write_finish(self):
         self.close()
 
-    def close(self):
+    def import_comments(self, from_fsdb):
+        for comment in from_fsdb._comments:
+            self._comments.append(comment)
+
+    def get_file_size(self):
+        return os.stat(self.fileh.name).st_size
+
+    def read_commands_ahead(self):
+        """reads the command list at the bottom of the input stream if the input stream can seek.
+
+        returns a list of commands found in comments in the input stream
+        returns None when the input is not seekable"""
+
+        self.maybe_open_filehandle()
+
+        if not self.file_handle.seekable():
+            return None
+
+        guess_length = 10
+
+        # save our spot
+        position = self.file_handle.tell()
+
+        # get the file size
+        file_size = self.get_file_size()
+        multiplier = 1
+
+        # move to the bottom minus the guess length
+        self.file_handle.seek(file_size - guess_length)
+
+        # poor man's search from the back
+        while True:
+            data = self.file_handle.read(guess_length * multiplier)
+            first_newline = data.find("\n")
+
+            if first_newline != -1 and (
+                first_newline == len(data) - 1 or data[first_newline + 1] == "#"
+            ):
+                # keep rewinding (x2 since we read x1 in already)
+                multiplier += 1
+                if file_size - guess_length * multiplier < 0:
+                    return None
+
+                self.file_handle.seek(file_size - guess_length * multiplier)
+                continue
+
+            break
+
+        # now extract all the commands from where we've found things
+        commands = []
+        iowrapper = io.StringIO(data)
+        for line in iowrapper:
+            if line.startswith("#  | "):
+                commands.append(line[5:].strip())
+
+        self.file_handle.seek(position)
+        return commands
+
+    def parse_commands(self):
+        """parses the list of stored comments for any saved commands
+
+        Note: Assumes saved commands will be prefixed with '#  |' per convention
+
+        Returns a list of strings when commands can be found.
+
+        Returns None when we don't have the information yet, such as when
+        we have a non-seekable stream input.
+        """
+
+        self.maybe_open_filehandle()
+
+        # we already have some stored
+        if self._commands:
+            return self._commands
+
+        # see if we can read them from the end of the file
+        if not self._comments:
+            if self.file_handle.seekable():
+                self._commands = self.read_commands_ahead()
+                return self._commands
+            return None
+
+        # parse them from the comments
+        self._commands = []
+        for comment in self._comments:
+            if comment.startswith("#  | "):
+                self._commands.append(comment[5:].strip())
+
+        return self._commands
+
+    def close(self, copy_comments_from=None):
         """Writes final processing command comment to the output file and closes it."""
         if self.fileh:
             self.fileh.close()
             self.fileh = None
 
+        if copy_comments_from:
+            self.import_comments(copy_comments_from)
+
         if self._out_file_handle:
             # ignore closing errors
             try:
                 if not self._header_written:
                     self._write_header_line()
                 if self._save_command_history and self.out_command_line:
                     for comment_line in self._comments:
```

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/bro2fsdb.py` & `pyfsdb-2.2/pyfsdb/tools/bro2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/fsdb2json.py` & `pyfsdb-2.2/pyfsdb/tools/fsdb2json.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/fsdb2many.py` & `pyfsdb-2.2/pyfsdb/tools/fsdb2many.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/json2fsdb.py` & `pyfsdb-2.2/pyfsdb/tools/json2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdb2sql.py` & `pyfsdb-2.2/pyfsdb/tools/pdb2sql.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdb2tex.py` & `pyfsdb-2.2/pyfsdb/tools/pdb2tex.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdb2to1.py` & `pyfsdb-2.2/pyfsdb/tools/pdb2to1.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbaddtypes.py` & `pyfsdb-2.2/pyfsdb/tools/pdbaddtypes.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbaugment.py` & `pyfsdb-2.2/pyfsdb/tools/pdbaugment.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbcdf.py` & `pyfsdb-2.2/pyfsdb/tools/pdbcdf.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbcoluniq.py` & `pyfsdb-2.2/pyfsdb/tools/pdbcoluniq.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             else:
                 pointer[this_value][final_value] += 1
 
     # output the results, with optional counts
     # (if statement at outer tier for speed)
     output_results(ofh, [], counters, count)
 
-    ofh.close()
+    ofh.close(copy_comments_from=fh)
 
 
 def main():
     args = parse_args()
 
     filter_unique_columns(
         args.input_file,
```

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbdatetoepoch.py` & `pyfsdb-2.2/pyfsdb/tools/pdbdatetoepoch.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbensure.py` & `pyfsdb-2.2/pyfsdb/tools/pdbensure.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbepochtodate.py` & `pyfsdb-2.2/pyfsdb/tools/pdbepochtodate.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbformat.py` & `pyfsdb-2.2/pyfsdb/tools/pdbformat.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbfullpivot.py` & `pyfsdb-2.2/pyfsdb/tools/pdbfullpivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbheatmap.py` & `pyfsdb-2.2/pyfsdb/tools/pdbheatmap.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbjinja.py` & `pyfsdb-2.2/pyfsdb/tools/pdbjinja.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbkeyedsort.py` & `pyfsdb-2.2/pyfsdb/tools/pdbkeyedsort.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbnormalize.py` & `pyfsdb-2.2/pyfsdb/tools/pdbnormalize.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbreescape.py` & `pyfsdb-2.2/pyfsdb/tools/pdbreescape.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbreversepivot.py` & `pyfsdb-2.2/pyfsdb/tools/pdbreversepivot.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,26 +90,26 @@
     # from the input, get extract column numbers/names
     key_column = args.key_column
     value_column = args.value_column
     other_columns = args.other_columns
     columns = args.columns
 
     # open the input file stream
-    input = pyfsdb.Fsdb(
+    fh = pyfsdb.Fsdb(
         file_handle=args.input_file, return_type=pyfsdb.RETURN_AS_DICTIONARY
     )
     output = pyfsdb.Fsdb(out_file_handle=args.output_file)
     output.out_column_names = [key_column, value_column] + other_columns
 
     # for each row, remember each value based on time and key
-    for row in input:
+    for row in fh:
         for column in columns:
             out_row = [column, row[column]]
             for other in other_columns:
                 out_row.append(row[other])
             output.append(out_row)
 
-    output.close()
+    output.close(copy_comments_from=fh)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbroc.py` & `pyfsdb-2.2/pyfsdb/tools/pdbroc.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbrow.py` & `pyfsdb-2.2/pyfsdb/tools/pdbrow.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         else:
             result = eval(compiled_expression, globals, row)
 
         if result:
             oh.append(row)
 
-    oh.close()
+    oh.close(copy_comments_from=fh)
 
 
 def main():
     args = parse_args()
 
     process_pdbrow(
         args.input_file,
```

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbroweval.py` & `pyfsdb-2.2/pyfsdb/tools/pdbroweval.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         # execute the expression and check its result
         exec(compiled_expression, globals, row)
         if use_underbars:
             row = {k[1:]: v for k, v in row.items()}
         oh.append(row)
 
-    oh.close()
+    oh.close(copy_comments_from=fh)
 
 
 def main():
     args = parse_args()
 
     process_pdbroweval(
         args.input_file,
```

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbsplitter.py` & `pyfsdb-2.2/pyfsdb/tools/pdbsplitter.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbsum.py` & `pyfsdb-2.2/pyfsdb/tools/pdbsum.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbtopn.py` & `pyfsdb-2.2/pyfsdb/tools/pdbtopn.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb/tools/pdbzerofill.py` & `pyfsdb-2.2/pyfsdb/tools/pdbzerofill.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb.egg-info/PKG-INFO` & `pyfsdb-2.2/pyfsdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.5
+Version: 2.2
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-2.1.5/pyfsdb.egg-info/SOURCES.txt` & `pyfsdb-2.2/pyfsdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/pyfsdb.egg-info/entry_points.txt` & `pyfsdb-2.2/pyfsdb.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.5/setup.py` & `pyfsdb-2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfsdb",
-    version="2.1.5",
+    version="2.2",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A python implementation of the flat-file streaming database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/pyfsdb",
     packages=setuptools.find_packages(),
```

