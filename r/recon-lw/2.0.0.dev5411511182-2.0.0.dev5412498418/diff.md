# Comparing `tmp/recon_lw-2.0.0.dev5411511182.tar.gz` & `tmp/recon_lw-2.0.0.dev5412498418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5411511182.tar", last modified: Thu Jun 29 11:09:38 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5412498418.tar", last modified: Thu Jun 29 13:03:07 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5411511182.tar` & `recon_lw-2.0.0.dev5412498418.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-29 11:09:14.000000 recon_lw-2.0.0.dev5411511182/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    34334 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 11:09:38.000000 recon_lw-2.0.0.dev5411511182/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-29 11:08:51.000000 recon_lw-2.0.0.dev5411511182/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-29 13:02:37.000000 recon_lw-2.0.0.dev5412498418/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34334 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23832 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:03:07.000000 recon_lw-2.0.0.dev5412498418/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-29 13:02:05.000000 recon_lw-2.0.0.dev5412498418/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/recon_ob_cross_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     problems = []
     for k in keys_collection:
         if k not in book1 or book1[k] is None:
             if k in book2 and book2[k] is not None:
                 problems.append({"mismatch_key": k, "1": None, "2": book2[k]})
                 continue
         if k not in book2 or book2[k] is None:
-            problems.append({"mismatch_key": k, "1": book1[k], "2": None})
+            problems.append({"mismatch_key": k, "1": None, "2": None})
             continue
         if book1[k] != book2[k]:
             problems.append({"mismatch_key": k, "1": book1[k], "2": None})
     return problems
 
 
 def compare_full_vs_aggr(full_book: dict, aggr_book: dict) -> list:
@@ -60,15 +60,15 @@
                 problems.append({"synopsys": " aggr_miss_level", "side": side, "level": i + 1})
     problems.extend(compare_keys(["open_price",
                                   "last_price",
                                   "max_price",
                                   "min_price",
                                   "ind_open_price",
                                   "ind_open_size",
-                                  "ind_open_mid_price"]))
+                                  "ind_open_mid_price"], full_book, aggr_book))
     
     return problems
 
 
 def compare_aggr_vs_top(aggr_book: dict, top_book: dict):
     problems = []
     if len(aggr_book["ask_aggr"]) > 0:
@@ -114,15 +114,15 @@
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
     problems.extend(compare_keys(["open_price",
                                   "last_price",
                                   "max_price",
                                   "min_price",
                                   "ind_open_price",
                                   "ind_open_size",
-                                  "ind_open_mid_price"]))
+                                  "ind_open_mid_price"], aggr_book, top_book))
     return problems
 
 
 def compare_full_vs_top(full_book: dict, top_book: dict):
     problems = []
     if top_book["ask_real_n_orders"] == 0 and top_book["ask_impl_n_orders"] != 0:
         problems = []
@@ -161,15 +161,15 @@
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
     problems.extend(compare_keys(["open_price",
                                   "last_price",
                                   "max_price",
                                   "min_price",
                                   "ind_open_price",
                                   "ind_open_size",
-                                  "ind_open_mid_price"]))
+                                  "ind_open_mid_price"], full_book, top_book))
     return problems
 
 
 def ob_compare_get_timestamp_key1_key2_aggr(o, custom_settings):
     if o["body"]["aggr_seq"]["limit_delta"] not in [1, 2]:
         return None, None, None
     if o["body"]["sessionId"] == custom_settings["full_session"]:
```

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5412498418/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5412498418/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/setup.py` & `recon_lw-2.0.0.dev5412498418/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5411511182/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5412498418/test/test_recon_ob.py`

 * *Files identical despite different names*

