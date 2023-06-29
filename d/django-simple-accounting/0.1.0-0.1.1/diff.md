# Comparing `tmp/django_simple_accounting-0.1.0.tar.gz` & `tmp/django_simple_accounting-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_accounting-0.1.0.tar", max compression
+gzip compressed data, was "django_simple_accounting-0.1.1.tar", max compression
```

## Comparing `django_simple_accounting-0.1.0.tar` & `django_simple_accounting-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/LICENSE
--rw-r--r--   0        0        0       73 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/README.md
--rw-r--r--   0        0        0      510 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/simple_accounting/__init__.py
--rw-r--r--   0        0        0      599 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/simple_accounting/admin.py
--rw-r--r--   0        0        0     3302 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/simple_accounting/models.py
--rw-r--r--   0        0        0      525 2023-06-29 20:58:46.400923 django_simple_accounting-0.1.0/simple_accounting/utils.py
--rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 django_simple_accounting-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/LICENSE
+-rw-r--r--   0        0        0      738 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/README.md
+-rw-r--r--   0        0        0      510 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/simple_accounting/__init__.py
+-rw-r--r--   0        0        0      606 2023-06-29 21:19:59.028801 django_simple_accounting-0.1.1/simple_accounting/admin.py
+-rw-r--r--   0        0        0     3302 2023-06-29 21:19:59.028801 django_simple_accounting-0.1.1/simple_accounting/models.py
+-rw-r--r--   0        0        0      603 2023-06-29 21:19:59.028801 django_simple_accounting-0.1.1/simple_accounting/utils.py
+-rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 django_simple_accounting-0.1.1/PKG-INFO
```

### Comparing `django_simple_accounting-0.1.0/LICENSE` & `django_simple_accounting-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.0/simple_accounting/admin.py` & `django_simple_accounting-0.1.1/simple_accounting/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib import admin
 
-from accounting.models import *
+from simple_accounting.models import *
 
 
 class LedgerAdmin(admin.ModelAdmin):
     list_display = ("name", "ledger_type")
 
 
 class TransactionAdmin(admin.ModelAdmin):
```

### Comparing `django_simple_accounting-0.1.0/simple_accounting/models.py` & `django_simple_accounting-0.1.1/simple_accounting/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.0/simple_accounting/utils.py` & `django_simple_accounting-0.1.1/simple_accounting/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,7 +13,9 @@
         return Signs(debit=-1, credit=1)
     elif ledger_type == 2:  # LIABILITIES
         return Signs(debit=-1, credit=1)
     elif ledger_type == 3:  # REVENUE
         return Signs(debit=-1, credit=1)
     elif ledger_type == 4:  # EXPENSES
         return Signs(debit=1, credit=-1)
+    else:
+        raise RuntimeError(f"Unhandled ledger_type: {ledger_type}")
```

