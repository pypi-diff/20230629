# Comparing `tmp/fnapy-1.3.0.tar.gz` & `tmp/fnapy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fnapy-1.3.0.tar", last modified: Thu Jan  7 17:07:38 2021, max compression
+gzip compressed data, was "dist/fnapy-1.4.0.tar", last modified: Thu Jun 29 16:25:19 2023, max compression
```

## Comparing `fnapy-1.3.0.tar` & `fnapy-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2021-01-07 17:07:38.990842 fnapy-1.3.0/
--rw-r--r--   0 damien    (1000) damien    (1000)      135 2020-09-11 15:49:23.000000 fnapy-1.3.0/AUTHORS.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     1067 2020-09-11 15:49:23.000000 fnapy-1.3.0/LICENSE.txt
--rw-r--r--   0 damien    (1000) damien    (1000)      243 2020-09-11 15:49:23.000000 fnapy-1.3.0/MANIFEST.in
--rw-r--r--   0 damien    (1000) damien    (1000)     7696 2021-01-07 17:07:38.990842 fnapy-1.3.0/PKG-INFO
--rw-r--r--   0 damien    (1000) damien    (1000)      585 2020-09-11 15:49:23.000000 fnapy-1.3.0/README.rst
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2021-01-07 17:07:38.987508 fnapy-1.3.0/docs/
--rw-r--r--   0 damien    (1000) damien    (1000)     4420 2021-01-07 17:02:17.000000 fnapy-1.3.0/docs/CHANGELOG.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     6758 2020-09-11 15:49:23.000000 fnapy-1.3.0/docs/Makefile
--rw-r--r--   0 damien    (1000) damien    (1000)      553 2020-09-11 15:49:23.000000 fnapy-1.3.0/docs/api.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     5320 2020-09-11 15:49:23.000000 fnapy-1.3.0/docs/conf.py
--rw-r--r--   0 damien    (1000) damien    (1000)      474 2020-09-11 15:49:23.000000 fnapy-1.3.0/docs/index.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     6699 2020-09-11 15:49:23.000000 fnapy-1.3.0/docs/make.bat
--rw-r--r--   0 damien    (1000) damien    (1000)     6814 2021-01-07 16:59:44.000000 fnapy-1.3.0/docs/quickstart.rst
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2021-01-07 17:07:38.987508 fnapy-1.3.0/fnapy/
--rw-r--r--   0 damien    (1000) damien    (1000)       22 2021-01-07 17:03:06.000000 fnapy-1.3.0/fnapy/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)     2311 2020-09-11 15:49:23.000000 fnapy-1.3.0/fnapy/compat.py
--rw-r--r--   0 damien    (1000) damien    (1000)     8199 2021-01-07 09:45:21.000000 fnapy-1.3.0/fnapy/config.py
--rw-r--r--   0 damien    (1000) damien    (1000)     2627 2020-09-11 15:49:23.000000 fnapy-1.3.0/fnapy/connection.py
--rw-r--r--   0 damien    (1000) damien    (1000)      740 2020-09-11 15:49:23.000000 fnapy-1.3.0/fnapy/exceptions.py
--rw-r--r--   0 damien    (1000) damien    (1000)    24093 2021-01-07 15:49:20.000000 fnapy-1.3.0/fnapy/fnapy_manager.py
--rw-r--r--   0 damien    (1000) damien    (1000)    16496 2021-01-07 13:51:33.000000 fnapy-1.3.0/fnapy/utils.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2021-01-07 17:07:38.990842 fnapy-1.3.0/fnapy.egg-info/
--rw-r--r--   0 damien    (1000) damien    (1000)     7696 2021-01-07 17:07:38.000000 fnapy-1.3.0/fnapy.egg-info/PKG-INFO
--rw-r--r--   0 damien    (1000) damien    (1000)      469 2021-01-07 17:07:38.000000 fnapy-1.3.0/fnapy.egg-info/SOURCES.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        1 2021-01-07 17:07:38.000000 fnapy-1.3.0/fnapy.egg-info/dependency_links.txt
--rw-r--r--   0 damien    (1000) damien    (1000)       24 2021-01-07 17:07:38.000000 fnapy-1.3.0/fnapy.egg-info/requires.txt
--rw-r--r--   0 damien    (1000) damien    (1000)       12 2021-01-07 17:07:38.000000 fnapy-1.3.0/fnapy.egg-info/top_level.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        1 2021-01-07 14:00:10.000000 fnapy-1.3.0/fnapy.egg-info/zip-safe
--rw-r--r--   0 damien    (1000) damien    (1000)      398 2021-01-07 17:07:38.990842 fnapy-1.3.0/setup.cfg
--rw-r--r--   0 damien    (1000) damien    (1000)     1687 2020-09-11 15:49:23.000000 fnapy-1.3.0/setup.py
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/
+-rw-rw-r--   0 damien    (1000) damien    (1000)      135 2023-05-29 09:36:13.000000 fnapy-1.4.0/AUTHORS.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     1067 2023-05-29 09:36:13.000000 fnapy-1.4.0/LICENSE.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)      243 2023-05-29 09:36:13.000000 fnapy-1.4.0/MANIFEST.in
+-rw-rw-r--   0 damien    (1000) damien    (1000)     5811 2023-06-29 16:25:19.000000 fnapy-1.4.0/PKG-INFO
+-rw-rw-r--   0 damien    (1000) damien    (1000)      585 2023-05-29 09:36:13.000000 fnapy-1.4.0/README.rst
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/docs/
+-rw-rw-r--   0 damien    (1000) damien    (1000)     4554 2023-06-29 15:19:05.000000 fnapy-1.4.0/docs/CHANGELOG.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     6758 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/Makefile
+-rw-rw-r--   0 damien    (1000) damien    (1000)      553 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/api.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     5320 2023-06-29 15:06:59.000000 fnapy-1.4.0/docs/conf.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)      474 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/index.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     6699 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/make.bat
+-rw-rw-r--   0 damien    (1000) damien    (1000)     8417 2023-06-29 15:15:40.000000 fnapy-1.4.0/docs/quickstart.rst
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy/
+-rw-rw-r--   0 damien    (1000) damien    (1000)       22 2023-06-29 15:20:03.000000 fnapy-1.4.0/fnapy/__init__.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)     2311 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/compat.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)     8092 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/config.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)     2627 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/connection.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)      740 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/exceptions.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)    24093 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/fnapy_manager.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)    16862 2023-06-29 14:54:57.000000 fnapy-1.4.0/fnapy/utils.py
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/
+-rw-rw-r--   0 damien    (1000) damien    (1000)     5811 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/PKG-INFO
+-rw-rw-r--   0 damien    (1000) damien    (1000)      469 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)        1 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)       24 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/requires.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)       12 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/top_level.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)        1 2023-06-29 14:18:54.000000 fnapy-1.4.0/fnapy.egg-info/zip-safe
+-rw-rw-r--   0 damien    (1000) damien    (1000)      398 2023-06-29 16:25:19.000000 fnapy-1.4.0/setup.cfg
+-rw-rw-r--   0 damien    (1000) damien    (1000)     1687 2023-05-29 09:36:13.000000 fnapy-1.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fnapy-1.3.0/LICENSE.txt` & `fnapy-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/README.rst` & `fnapy-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/docs/CHANGELOG.rst` & `fnapy-1.4.0/docs/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 Change log
 ==========
 
 All notable changes to this project will be documented in this file.
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
+[1.4.0] - 2023-06-29
+--------------------
+Changed
+*******
+* Allow `update_offers` to accept more code types when passing a dictionary
 
 [1.3.0] - 2021-01-07
 --------------------
 Changed
 *******
 * Change the argument for `query_pricing` to allow to specify any combination of code types
   and keep compatibility with the old version (a list of EANs when the code type is not specified)
```

### Comparing `fnapy-1.3.0/docs/Makefile` & `fnapy-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/docs/api.rst` & `fnapy-1.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/docs/conf.py` & `fnapy-1.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # -- Project information -----------------------------------------------------
 
 project = u'fnapy'
 copyright = u'2019, Taurus Olson'
 author = u'Taurus Olson'
 
 # The short X.Y version
-version = u'1.1.8'
+version = u'1.4.0'
 # The full version, including alpha/beta/rc tags
-release = u'1.1.8'
+release = u'1.4.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `fnapy-1.3.0/docs/make.bat` & `fnapy-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/docs/quickstart.rst` & `fnapy-1.4.0/docs/quickstart.rst`

 * *Files 16% similar despite different names*

```diff
@@ -31,16 +31,32 @@
             'offer_reference':'B76A-CD5-153',
             'price':15, 'product_state':11, 'quantity':10, 
             'description': 'New product - 2-3 days shipping, from France'}
     offer_data2 = {'product_reference':'5030917077418',
             'offer_reference':'B067-F0D-75E',
             'price':20, 'product_state':11, 'quantity':16, 
             'description': 'New product - 2-3 days shipping, from France'}
+    offer_data3 = {'product_reference':{'value': '9780262510875', 'type': 'Ean'},
+            'offer_reference':'B76A-CD5-444',
+            'price':80.0, 'product_state':11, 'quantity':10,
+            'description': 'New product - 2-3 days shipping, from France'}
+    offer_data4 = {'product_reference': {'value': '1593275919', 'type': 'Isbn'},
+        'offer_reference': 'A31F-B6C-95F',
+        'price': 30.0, 'product_state': 11, 'quantity': 1,
+        'description': 'New product - 2-3 days shipping, from France'
+    }
+
+    response = manager.update_offers([offers_data1, offer_data2, offer_data3, offer_data4])
+
 
-    response = manager.update_offers([offers_data1, offer_data2])
+.. note::
+   Note that the `product_reference` key can be a string (by default an EAN) or 
+   a dictionary which allows you to specify the code value and its type.
+   (cf https://partners-test.mp.fnacdarty.com/docs/api/2.6/services/type/state.html#product-reference-type
+   for a detailed list)
 
 Behind the scene, the manager sent an XML request to the `offers_update`
 service. We can have a look at this request with the attribute `offers_update_request`::
 
     >>> request = manager.offers_update_request
     >>> print request.xml
     <?xml version='1.0' encoding='utf-8'?>
@@ -57,14 +73,30 @@
         <product_reference type="Ean">5030917077418</product_reference>
         <offer_reference type="SellerSku"><![CDATA[B067-F0D-75E]]></offer_reference>
         <price>20</price>
         <product_state>11</product_state>
         <quantity>16</quantity>
         <description><![CDATA[New product - 2-3 days shipping, from France]]></description>
       </offer>
+      <offer>
+        <product_reference type="Ean">9780262510875</product_reference>
+        <offer_reference type="SellerSku"><![CDATA[B76A-CD5-444]]></offer_reference>
+        <price>80.0</price>
+        <product_state>11</product_state>
+        <quantity>10</quantity>
+        <description><![CDATA[New product - 2-3 days shipping, from France]]></description>
+      </offer>
+      <offer>
+        <product_reference type="Isbn">1593275919</product_reference>
+        <offer_reference type="SellerSku"><![CDATA[A31F-B6C-95F]]></offer_reference>
+        <price>30.0</price>
+        <product_state>11</product_state>
+        <quantity>1</quantity>
+        <description><![CDATA[New product - 2-3 days shipping, from France]]></description>
+      </offer>
     </offers_update>
 
 Actually this request is an instance of the :class:`Request <Request>` class.
 We'll talk about it later. For now, let's see what we've got in our response::
 
     >>> print response.xml
     <?xml version="1.0" encoding="utf-8"?>
```

### Comparing `fnapy-1.3.0/fnapy/compat.py` & `fnapy-1.4.0/fnapy/compat.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/fnapy/config.py` & `fnapy-1.4.0/fnapy/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,14 @@
 description = Parameter("description", "Product description")
 internal_comment = Parameter(
     "internal_comment", "Offer internal comment for personal use"
 )
 showcase = Parameter("showcase", "Offer position in shop’s showcase")
 treatment = Parameter("treatment", "Treatment to do on offer")
 pictures = Parameter("pictures", "Add pictures to offer")
-time_to_ship = Parameter("time_to_ship", "Add a specific time to ship (if is activate)")
 
 # The elements for the requests
 REQUEST_ELEMENTS = {}
 REQUEST_ELEMENTS["offers_query"] = (
     paging,
     date,
     quantity,
@@ -149,15 +148,14 @@
     product_state,
     quantity.change_desc("Offer quantity"),
     description,
     internal_comment,
     showcase,
     treatment,
     pictures,
-    time_to_ship,
 )
 REQUEST_ELEMENTS["orders_query"] = (
     paging,
     date,
     sort_by,
     product_fnac_id,
     offer_fnac_id,
```

### Comparing `fnapy-1.3.0/fnapy/connection.py` & `fnapy-1.4.0/fnapy/connection.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/fnapy/exceptions.py` & `fnapy-1.4.0/fnapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/fnapy/fnapy_manager.py` & `fnapy-1.4.0/fnapy/fnapy_manager.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.3.0/fnapy/utils.py` & `fnapy-1.4.0/fnapy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,22 @@
     etree.SubElement(offer, "offer_reference", type="SellerSku").text = etree.CDATA(
         offer_reference
     )
     offer_data_items = [(k, v) for k, v in offer_data.items() if k != "offer_reference"]
 
     for key, value in offer_data_items:
         if key == "product_reference":
-            etree.SubElement(offer, "product_reference", type="Ean").text = str(value)
+            # Form: {"value": code_value, "type": code_type}
+            # Example: {"value": "9781462055517", "type": "Ean"}
+            if isinstance(value, dict):
+                etree.SubElement(offer, "product_reference", type=value["type"]).text = str(value["value"])
+            # Form: code_value
+            # Example: "9781462055517"
+            else:
+                etree.SubElement(offer, "product_reference", type="Ean").text = str(value)
         elif key == "description":
             etree.SubElement(offer, "description").text = etree.CDATA(value)
         else:
             etree.SubElement(offer, key).text = str(value)
     return offer
```

### Comparing `fnapy-1.3.0/setup.py` & `fnapy-1.4.0/setup.py`

 * *Files identical despite different names*

