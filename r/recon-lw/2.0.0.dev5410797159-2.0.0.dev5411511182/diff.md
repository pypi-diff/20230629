# Comparing `tmp/recon_lw-2.0.0.dev5410797159.tar.gz` & `tmp/recon_lw-2.0.0.dev5411511182.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5410797159.tar", last modified: Thu Jun 29 09:46:39 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5411511182.tar", last modified: Thu Jun 29 11:09:38 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5410797159.tar` & `recon_lw-2.0.0.dev5411511182.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-29 09:46:12.000000 recon_lw-2.0.0.dev5410797159/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    34338 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-29 11:09:14.000000 recon_lw-2.0.0.dev5411511182/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34334 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,22 +747,22 @@
 
 
 def display_l2(order_book):
     header = ["price", "real_qty", "impl_qty", "real_num_orders", "impl_num_orders",
               "price", "real_qty", "impl_qty", "real_num_orders", "impl_num_orders"]
     result = [[f'bid_{header[i]}' if i < 5 else f'ask_{header[i]}' for i in range(len(header))]]
     levels = max(len(order_book["bid_aggr"]), len(order_book["ask_aggr"]))
-    keys = ["bid_aggr","bid_aggr"]
+    keys = ["bid_aggr","ask_aggr"]
     shifts = [0,5]
     for i in range(levels):
         line = []
         for key, shift in zip(keys, shifts):
             if i < len(order_book[key]):
                 for j in range(5):
-                    line.append(order_book[key][i].get(header[j+shift]))
+                    line.append(order_book[key][i][header[j+shift]])
             else:
                 line.extend([None]*5)
         result.append(line)
     return result
 
 
 def display_l3(order_book):
```

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/setup.py` & `recon_lw-2.0.0.dev5411511182/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5410797159/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5411511182/test/test_recon_ob.py`

 * *Files identical despite different names*

