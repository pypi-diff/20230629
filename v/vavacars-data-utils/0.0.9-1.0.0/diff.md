# Comparing `tmp/vavacars_data_utils-0.0.9.tar.gz` & `tmp/vavacars_data_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/acg/repositories/Data.Utils/dist/tmpp9_thcst/vavacars_data_utils-0.0.9.tar", last modified: Tue Dec 21 14:50:33 2021, max compression
+gzip compressed data, was "vavacars_data_utils-1.0.0.tar", last modified: Thu Jun 29 09:18:45 2023, max compression
```

## Comparing `vavacars_data_utils-0.0.9.tar` & `vavacars_data_utils-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,52 @@
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/
--rw-r--r--   0 acg       (1000) acg       (1000)     1297 2021-12-21 14:42:35.000000 vavacars_data_utils-0.0.9/README.md
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/turkey/
--rw-r--r--   0 acg       (1000) acg       (1000)      888 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/turkey/dates.py
--rw-r--r--   0 acg       (1000) acg       (1000)      148 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/turkey/__init__.py
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/smartiq/
--rw-r--r--   0 acg       (1000) acg       (1000)     4759 2021-12-21 14:49:56.000000 vavacars_data_utils-0.0.9/vava_utils/smartiq/smartiq_helper.py
--rw-r--r--   0 acg       (1000) acg       (1000)       85 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/smartiq/__init__.py
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vava_utils/utils/
--rw-r--r--   0 acg       (1000) acg       (1000)     1277 2021-12-21 14:42:35.000000 vavacars_data_utils-0.0.9/vava_utils/utils/comparisons.py
--rw-r--r--   0 acg       (1000) acg       (1000)       81 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/utils/__init__.py
--rw-r--r--   0 acg       (1000) acg       (1000)        0 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/vava_utils/__init__.py
--rw-r--r--   0 acg       (1000) acg       (1000)      104 2021-12-17 08:47:50.000000 vavacars_data_utils-0.0.9/pyproject.toml
-drwxr-xr-x   0 acg       (1000) acg       (1000)        0 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/
--rw-r--r--   0 acg       (1000) acg       (1000)       11 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/top_level.txt
--rw-r--r--   0 acg       (1000) acg       (1000)        1 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/dependency_links.txt
--rw-r--r--   0 acg       (1000) acg       (1000)      471 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/SOURCES.txt
--rw-r--r--   0 acg       (1000) acg       (1000)        7 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/requires.txt
--rw-r--r--   0 acg       (1000) acg       (1000)     1803 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/vavacars_data_utils.egg-info/PKG-INFO
--rw-r--r--   0 acg       (1000) acg       (1000)      673 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/setup.cfg
--rw-r--r--   0 acg       (1000) acg       (1000)     1803 2021-12-21 14:50:33.000000 vavacars_data_utils-0.0.9/PKG-INFO
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.922788 vavacars_data_utils-1.0.0/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-06-29 09:18:45.922788 vavacars_data_utils-1.0.0/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/README.md
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/pyproject.toml
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      799 2023-06-29 09:18:45.941556 vavacars_data_utils-1.0.0/setup.cfg
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.434080 vavacars_data_utils-1.0.0/test/
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.639239 vavacars_data_utils-1.0.0/test/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/test/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/test/utils/test_strings.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.670570 vavacars_data_utils-1.0.0/vava_utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/__init__.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.733876 vavacars_data_utils-1.0.0/vava_utils/azure/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.0.0/vava_utils/azure/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    10180 2023-03-06 06:57:28.000000 vavacars_data_utils-1.0.0/vava_utils/azure/az_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.814763 vavacars_data_utils-1.0.0/vava_utils/bigquery/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/bigquery/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/bigquery/bigquery_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.891846 vavacars_data_utils-1.0.0/vava_utils/camunda/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/camunda/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.0.0/vava_utils/camunda/camunda_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.972228 vavacars_data_utils-1.0.0/vava_utils/email/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.0.0/vava_utils/email/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2023-06-29 09:16:49.000000 vavacars_data_utils-1.0.0/vava_utils/email/email_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.052187 vavacars_data_utils-1.0.0/vava_utils/salesforce/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.0.0/vava_utils/salesforce/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2136 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/salesforce/salesforce_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.193542 vavacars_data_utils-1.0.0/vava_utils/smartiq/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.0/vava_utils/smartiq/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.0/vava_utils/smartiq/smartiq_helper.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.0.0/vava_utils/smartiq/smartiq_helper_v2.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.286701 vavacars_data_utils-1.0.0/vava_utils/sql/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.0.0/vava_utils/sql/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    12971 2023-06-19 15:21:04.000000 vavacars_data_utils-1.0.0/vava_utils/sql/sql_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.381572 vavacars_data_utils-1.0.0/vava_utils/turkey/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/turkey/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/turkey/dates.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.635387 vavacars_data_utils-1.0.0/vava_utils/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      288 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/utils/callables.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.0.0/vava_utils/utils/comparisons.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/utils/naming.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.0/vava_utils/utils/singleton.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/utils/strings.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.730404 vavacars_data_utils-1.0.0/vava_utils/vavaprice/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.0.0/vava_utils/vavaprice/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.0.0/vava_utils/vavaprice/vavaprice_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.891842 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1185 2023-06-29 09:18:44.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       97 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/requires.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vavacars_data_utils-0.0.9/vava_utils/turkey/dates.py` & `vavacars_data_utils-1.0.0/vava_utils/turkey/dates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import datetime
 
 months_translation = {'Ocak': 1,
-                      'Çubat': 2,
+                      'Şubat': 2,
                       'Mart': 3,
                       'Nisan': 4,
-                      'Mayis': 5,
+                      'Mayıs': 5,
                       'Haziran': 6,
                       'Temmuz': 7,
                       'Ağustos': 8,
                       'Eylül': 9,
                       'Ekim': 10,
                       'Kasım': 11,
                       'Aralık': 12}
 
 
 def turkish_to_datetime(s):
-    '''
+    """
     Converts a string containing a turkish date into a datetime object.
 
     Input format of the date as 'dd turkish_month year': 08 Aralık 2021
 
     Parameters:
         s (str): String with turkish date
-    '''
+    """
     try:
         (day, month, year) = s.split()
         return datetime.datetime(int(year), months_translation[month], int(day))
     except Exception as e:
         return datetime.datetime(1900, 1, 1)
```

