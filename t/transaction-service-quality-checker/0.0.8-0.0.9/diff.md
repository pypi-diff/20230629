# Comparing `tmp/transaction_service_quality_checker-0.0.8.tar.gz` & `tmp/transaction_service_quality_checker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction_service_quality_checker-0.0.8.tar", last modified: Wed Jun 28 15:18:12 2023, max compression
+gzip compressed data, was "transaction_service_quality_checker-0.0.9.tar", last modified: Wed Jun 28 15:33:12 2023, max compression
```

## Comparing `transaction_service_quality_checker-0.0.8.tar` & `transaction_service_quality_checker-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:18:12.217212 transaction_service_quality_checker-0.0.8/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-06-28 15:18:12.216469 transaction_service_quality_checker-0.0.8/PKG-INFO
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1601 2023-05-10 16:34:46.000000 transaction_service_quality_checker-0.0.8/README.md
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)       38 2023-06-28 15:18:12.217441 transaction_service_quality_checker-0.0.8/setup.cfg
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      383 2023-06-28 14:58:17.000000 transaction_service_quality_checker-0.0.8/setup.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:18:12.198075 transaction_service_quality_checker-0.0.8/tests/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:08.000000 transaction_service_quality_checker-0.0.8/tests/__init__.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:18:12.199536 transaction_service_quality_checker-0.0.8/tests/api/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:10.000000 transaction_service_quality_checker-0.0.8/tests/api/__init__.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      960 2023-05-25 12:23:42.000000 transaction_service_quality_checker-0.0.8/tests/api/test_config_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2317 2023-05-25 12:26:21.000000 transaction_service_quality_checker-0.0.8/tests/api/test_transaction_api_interface.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:18:12.207002 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-25 12:19:38.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/__init__.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      513 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/addresses_map.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:18:12.215157 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:25:46.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/__init__.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      425 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      651 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/config_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     3717 2023-06-28 12:53:28.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/etherscan_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1828 2023-05-03 11:00:35.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/transaction_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1374 2023-05-23 18:18:38.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/app.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      525 2023-05-08 10:47:32.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/app_block_creation.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2494 2023-05-29 15:40:49.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/app_by_list.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1422 2023-05-31 18:44:42.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/block_creation.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)    15144 2023-06-28 15:16:46.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/comparer.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2077 2023-06-28 14:59:32.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/metrics.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     6320 2023-05-24 09:08:26.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/reindex_operator.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:18:12.209893 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker.egg-info/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-06-28 15:18:12.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker.egg-info/PKG-INFO
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1144 2023-06-28 15:18:12.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker.egg-info/SOURCES.txt
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        1 2023-06-28 15:18:12.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker.egg-info/dependency_links.txt
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)       42 2023-06-28 15:18:12.000000 transaction_service_quality_checker-0.0.8/transaction_service_quality_checker.egg-info/top_level.txt
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:33:12.054830 transaction_service_quality_checker-0.0.9/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-06-28 15:33:12.054214 transaction_service_quality_checker-0.0.9/PKG-INFO
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1601 2023-05-10 16:34:46.000000 transaction_service_quality_checker-0.0.9/README.md
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)       38 2023-06-28 15:33:12.055019 transaction_service_quality_checker-0.0.9/setup.cfg
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      383 2023-06-28 15:33:10.000000 transaction_service_quality_checker-0.0.9/setup.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:33:12.038021 transaction_service_quality_checker-0.0.9/tests/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:08.000000 transaction_service_quality_checker-0.0.9/tests/__init__.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:33:12.039346 transaction_service_quality_checker-0.0.9/tests/api/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:10.000000 transaction_service_quality_checker-0.0.9/tests/api/__init__.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      960 2023-05-25 12:23:42.000000 transaction_service_quality_checker-0.0.9/tests/api/test_config_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2317 2023-05-25 12:26:21.000000 transaction_service_quality_checker-0.0.9/tests/api/test_transaction_api_interface.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:33:12.046032 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-25 12:19:38.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/__init__.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      513 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/addresses_map.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:33:12.052948 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:25:46.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/__init__.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      425 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      651 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/config_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     3717 2023-06-28 12:53:28.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/etherscan_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1828 2023-05-03 11:00:35.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/transaction_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1374 2023-05-23 18:18:38.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/app.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      525 2023-05-08 10:47:32.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/app_block_creation.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2494 2023-05-29 15:40:49.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/app_by_list.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1422 2023-05-31 18:44:42.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/block_creation.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)    15144 2023-06-28 15:16:46.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/comparer.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2077 2023-06-28 14:59:32.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/metrics.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-06-28 15:33:12.048554 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker.egg-info/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-06-28 15:33:11.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker.egg-info/PKG-INFO
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1088 2023-06-28 15:33:11.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        1 2023-06-28 15:33:11.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)       42 2023-06-28 15:33:11.000000 transaction_service_quality_checker-0.0.9/transaction_service_quality_checker.egg-info/top_level.txt
```

### Comparing `transaction_service_quality_checker-0.0.8/README.md` & `transaction_service_quality_checker-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/tests/api/test_config_api_interface.py` & `transaction_service_quality_checker-0.0.9/tests/api/test_config_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/tests/api/test_transaction_api_interface.py` & `transaction_service_quality_checker-0.0.9/tests/api/test_transaction_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/addresses_map.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/addresses_map.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/config_api_interface.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/config_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/etherscan_api_interface.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/etherscan_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/api/transaction_api_interface.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/api/transaction_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/app.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/app.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/app_block_creation.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/app_block_creation.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/app_by_list.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/app_by_list.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/block_creation.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/block_creation.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/comparer.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/comparer.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker/metrics.py` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker/metrics.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.8/transaction_service_quality_checker.egg-info/SOURCES.txt` & `transaction_service_quality_checker-0.0.9/transaction_service_quality_checker.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 transaction_service_quality_checker/addresses_map.py
 transaction_service_quality_checker/app.py
 transaction_service_quality_checker/app_block_creation.py
 transaction_service_quality_checker/app_by_list.py
 transaction_service_quality_checker/block_creation.py
 transaction_service_quality_checker/comparer.py
 transaction_service_quality_checker/metrics.py
-transaction_service_quality_checker/reindex_operator.py
 transaction_service_quality_checker.egg-info/PKG-INFO
 transaction_service_quality_checker.egg-info/SOURCES.txt
 transaction_service_quality_checker.egg-info/dependency_links.txt
 transaction_service_quality_checker.egg-info/top_level.txt
 transaction_service_quality_checker/api/__init__.py
 transaction_service_quality_checker/api/api_interface.py
 transaction_service_quality_checker/api/config_api_interface.py
```

