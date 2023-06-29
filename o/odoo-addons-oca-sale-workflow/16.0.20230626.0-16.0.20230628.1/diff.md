# Comparing `tmp/odoo_addons_oca_sale_workflow-16.0.20230626.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_sale_workflow-16.0.20230628.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1769 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2991 b- defN 23-Jun-27 05:13 odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 05:13 odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 05:13 odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      425 b- defN 23-Jun-27 05:13 odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/RECORD
-4 files, 3509 bytes uncompressed, 931 bytes compressed:  73.5%
+Zip file size: 1786 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3133 b- defN 23-Jun-29 06:10 odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 06:10 odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-29 06:10 odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      425 b- defN 23-Jun-29 06:10 odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/RECORD
+4 files, 3651 bytes uncompressed, 948 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/METADATA
+Filename: odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/WHEEL
+Filename: odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/RECORD
+Filename: odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_sale_workflow-16.0.20230626.0.dist-info/METADATA` & `odoo_addons_oca_sale_workflow-16.0.20230628.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-sale-workflow
-Version: 16.0.20230626.0
+Version: 16.0.20230628.1
 Summary: Meta package for oca-sale-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -24,26 +24,28 @@
 Requires-Dist: odoo-addon-sale-force-invoiced (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-invoice-policy (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-mrp-bom (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-archive (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-general-discount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-general-discount-triple (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-invoice-amount (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-sale-order-line-date (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-line-menu (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-line-price-history (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-lot-generator (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-lot-selection (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-product-availability-inline (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-product-recommendation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-qty-change-no-recompute (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-revision (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-type (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-partner-incoterm (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-partner-selectable-option (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-procurement-group-by-line (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-sale-product-category-menu (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-stock-cancel-restriction (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-stock-picking-blocking (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-substate (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-tier-validation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-triple-discount (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

