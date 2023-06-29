# Comparing `tmp/recon_lw-2.0.0.dev5398854918.tar.gz` & `tmp/recon_lw-2.0.0.dev5410797159.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5398854918.tar", last modified: Wed Jun 28 08:21:42 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5410797159.tar", last modified: Thu Jun 29 09:46:39 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5398854918.tar` & `recon_lw-2.0.0.dev5410797159.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-28 08:21:16.000000 recon_lw-2.0.0.dev5398854918/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33734 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 08:21:42.000000 recon_lw-2.0.0.dev5398854918/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-28 08:20:49.000000 recon_lw-2.0.0.dev5398854918/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-29 09:46:12.000000 recon_lw-2.0.0.dev5410797159/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34338 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:46:39.000000 recon_lw-2.0.0.dev5410797159/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-29 09:45:46.000000 recon_lw-2.0.0.dev5410797159/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob.py`

 * *Files 4% similar despite different names*

```diff
@@ -598,21 +598,22 @@
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     errors = {}
     if "max_price" not in order_book or order_book["max_price"] is None:
-        errors["trade_book_max_price_eror"] = "max_price not initialized"
         order_book["max_price"] = trade_price
 
     if "min_price" not in order_book or order_book["min_price"] is None:
-        errors["trade_book_min_price_eror"] = "min_price not initialized"
         order_book["min_price"] = trade_price
 
+    if "open_price" not in order_book or order_book["open_price"] is None:
+        order_book["open_price"] = trade_price
+
 
     order_book["last_price"] = trade_price
     if trade_price > order_book["max_price"]:
         order_book["max_price"] = trade_price
     if trade_price < order_book["min_price"]:
         order_book["min_price"] = trade_price
     if "total_n_trades" not in order_book:
@@ -623,28 +624,33 @@
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 0
     order_book["aggr_seq"]["limit_delta"] = 0
 
     return errors, [copy.deepcopy(order_book)]
 
 
-def ob_indicative_open_price(opening_price: float, str_time_of_event, order_book: dict):
+def ob_indicative_open_price(open_price: float, open_size: int, 
+                             open_mid_price: float, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
-    order_book["open_price"] = opening_price
-    order_book["last_price"] = opening_price
-    order_book["max_price"] = opening_price
-    order_book["min_price"] = opening_price
+    #order_book["open_price"] = opening_price
+    #order_book["last_price"] = opening_price
+    #order_book["max_price"] = opening_price
+    #order_book["min_price"] = opening_price
+    order_book["ind_open_price"] = open_price
+    order_book["ind_open_size"] = open_size
+    order_book["ind_open_mid_price"] = open_mid_price
+
 
     update_time_and_version(str_time_of_event, order_book)
-    order_book["aggr_seq"]["top_delta"] = 0
-    order_book["aggr_seq"]["limit_delta"] = 0
+    order_book["aggr_seq"]["top_delta"] = 1
+    order_book["aggr_seq"]["limit_delta"] = 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
 def is_side_unchanged(side, new_price, new_real_qty, new_impl_qty, new_real_n_orders, new_impl_n_orders, book):
     if new_price is None:
         return book[side+"_price"] is None
@@ -717,26 +723,37 @@
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
 
     return {}, [copy.deepcopy(order_book)]
 
+def display_summary(order_book):
+       header = ["open_price",
+                 "last_price",
+                 "max_price",
+                 "min_price",
+                 "ind_open_size",
+                 "ind_open_price",
+                 "ind_open_mid_price"]
+       data = [None if k not in order_book else order_book[k] for k in header]
+       return [header, data]
+       
 
 def display_l1(order_book):
     header = ["bid_price", "bid_real_qty", "bid_impl_qty", "bid_real_n_orders", "bid_impl_n_orders",
               "ask_price", "ask_real_qty", "ask_impl_qty", "ask_real_n_orders", "ask_impl_n_orders"]
     data = [order_book[col] for col in header]
     return [header, data]
 
 
 def display_l2(order_book):
-    header = ["bid_price", "bid_real_qty", "bid_impl_qty", "bid_real_num_orders", "bid_impl_num_orders",
-              "ask_price", "ask_real_qty", "ask_impl_qty", "ask_real_num_orders", "ask_impl_num_orders"]
-    result = [header]
+    header = ["price", "real_qty", "impl_qty", "real_num_orders", "impl_num_orders",
+              "price", "real_qty", "impl_qty", "real_num_orders", "impl_num_orders"]
+    result = [[f'bid_{header[i]}' if i < 5 else f'ask_{header[i]}' for i in range(len(header))]]
     levels = max(len(order_book["bid_aggr"]), len(order_book["ask_aggr"]))
     keys = ["bid_aggr","bid_aggr"]
     shifts = [0,5]
     for i in range(levels):
         line = []
         for key, shift in zip(keys, shifts):
             if i < len(order_book[key]):
```

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_cross_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,28 @@
         syn += "p"
     if not num_orders_condition:
         syn += "n"
     if not size_condition:
         syn += "s"
     return syn
 
+def compare_keys(keys_collection, book1, book2):
+    problems = []
+    for k in keys_collection:
+        if k not in book1 or book1[k] is None:
+            if k in book2 and book2[k] is not None:
+                problems.append({"mismatch_key": k, "1": None, "2": book2[k]})
+                continue
+        if k not in book2 or book2[k] is None:
+            problems.append({"mismatch_key": k, "1": book1[k], "2": None})
+            continue
+        if book1[k] != book2[k]:
+            problems.append({"mismatch_key": k, "1": book1[k], "2": None})
+    return problems
+
 
 def compare_full_vs_aggr(full_book: dict, aggr_book: dict) -> list:
     problems = []
     for side in ["ask", "bid"]:
         full_levels = list(full_book[side].keys())
         if side == "ask":
             full_levels.sort()
@@ -40,15 +54,22 @@
                                      "level": i + 1})
             elif i >= len(full_levels) and i >= len(aggr_levels):
                 break
             elif i >= len(full_levels):
                 problems.append({"synopsys": " full_miss_level", "side": side, "level": i + 1})
             elif i >= len(aggr_levels):
                 problems.append({"synopsys": " aggr_miss_level", "side": side, "level": i + 1})
-
+    problems.extend(compare_keys(["open_price",
+                                  "last_price",
+                                  "max_price",
+                                  "min_price",
+                                  "ind_open_price",
+                                  "ind_open_size",
+                                  "ind_open_mid_price"]))
+    
     return problems
 
 
 def compare_aggr_vs_top(aggr_book: dict, top_book: dict):
     problems = []
     if len(aggr_book["ask_aggr"]) > 0:
         if top_book["ask_real_qty"] == 0 and top_book["ask_impl_qty"] == 0:
@@ -87,14 +108,21 @@
                 problems.append({"synopsys": synopsys(price_condition,
                                                       num_orders_condition1 and num_orders_condition2,
                                                       size_condition1 and size_condition2),
                                  "side": "bid"})
     else:
         if top_book["bid_real_qty"] != 0 or top_book["bid_impl_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
+    problems.extend(compare_keys(["open_price",
+                                  "last_price",
+                                  "max_price",
+                                  "min_price",
+                                  "ind_open_price",
+                                  "ind_open_size",
+                                  "ind_open_mid_price"]))
     return problems
 
 
 def compare_full_vs_top(full_book: dict, top_book: dict):
     problems = []
     if top_book["ask_real_n_orders"] == 0 and top_book["ask_impl_n_orders"] != 0:
         problems = []
@@ -127,14 +155,21 @@
             size_condition = sum(full_book["bid"][top_p].values()) == (top_book["bid_real_qty"])
             if not (price_condition and num_orders_condition and size_condition):
                 problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                  "side": "bid"})
     else:
         if top_book["bid_real_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
+    problems.extend(compare_keys(["open_price",
+                                  "last_price",
+                                  "max_price",
+                                  "min_price",
+                                  "ind_open_price",
+                                  "ind_open_size",
+                                  "ind_open_mid_price"]))
     return problems
 
 
 def ob_compare_get_timestamp_key1_key2_aggr(o, custom_settings):
     if o["body"]["aggr_seq"]["limit_delta"] not in [1, 2]:
         return None, None, None
     if o["body"]["sessionId"] == custom_settings["full_session"]:
```

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5410797159/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5410797159/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/setup.py` & `recon_lw-2.0.0.dev5410797159/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5398854918/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5410797159/test/test_recon_ob.py`

 * *Files identical despite different names*

