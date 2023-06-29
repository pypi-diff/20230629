# Comparing `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.3.tar.gz` & `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.3.tar", last modified: Fri Jun  9 08:03:50 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.4.tar", last modified: Thu Jun 29 07:23:29 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3.tar` & `odoo13-addon-photovoltaic_api-13.0.1.1.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.011019 odoo13-addon-photovoltaic_api-13.0.1.1.3/
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-09 08:03:50.010019 odoo13-addon-photovoltaic_api-13.0.1.1.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.003019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.003019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.004019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.005019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/controllers/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.005019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/data/
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.005019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/models/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.007019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/contract.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/info.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.007019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/security/
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.008019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4683 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/account.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/allocations.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/contracts.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/info.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/powerstation.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.009019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/tests/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/tests/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6052 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/tests/test_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:03:50.010019 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-09 08:03:49.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-09 08:03:49.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 08:03:49.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 08:03:49.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      212 2023-06-09 08:03:49.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 08:03:49.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 08:03:50.011019 odoo13-addon-photovoltaic_api-13.0.1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-09 08:03:33.000000 odoo13-addon-photovoltaic_api-13.0.1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.231580 odoo13-addon-photovoltaic_api-13.0.1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-29 07:23:29.230580 odoo13-addon-photovoltaic_api-13.0.1.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.220581 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.220581 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.222581 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.223580 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/controllers/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.223580 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.224581 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.226580 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.226580 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.228581 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4683 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/contracts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/powerstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.229580 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/tests/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/tests/test_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:23:29.230580 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-29 07:23:29.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-29 07:23:29.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:23:29.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:23:29.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2023-06-29 07:23:29.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-29 07:23:29.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:23:29.231580 odoo13-addon-photovoltaic_api-13.0.1.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-29 07:23:11.000000 odoo13-addon-photovoltaic_api-13.0.1.1.4/setup.py
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/CHANGELOG.md` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file. (from version 13.0.1.1.0 onwards)
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [13.0.1.1.4] - 29-06-2023
+
+### Fixed
+- Promotions policy endpoint to allow both subscription and unsubscription
+
 ## [13.0.1.1.3] - 09-06-2023
 
 ### Added
 - Endpoint to update promotions policy of a contact
 
 ### Fixed
 - Comparator of vat in login and signup to be case insensitive
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/__manifest__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/__manifest__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic API',
-    'version': '13.0.1.1.3',
+    'version': '13.0.1.1.4',
     'depends': [
         'base_rest',
         'auth_api_key',
         'auth_jwt',
         'base_rest_pydantic',
         'pydantic',
         'photovoltaic_mgmt',
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/data/data.xml` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/data/data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/__init__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/contract.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/power_station.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/pydantic_models/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/pydantic_models/user.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/allocations.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/allocations.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/bank_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/bank_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/contracts.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/contracts.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/info.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/info.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/powerstation.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/powerstation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/services/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/services/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,17 @@
         input_param=restapi.CerberusValidator('_validator_promotions'),
         auth='api_key'
     )
     def allow_promotions(self, **params):
         user = self.env['res.partner'].browse([params.get('id')])
         if len(user) < 1:
             raise MissingError('No user with provided id')
-        user[0].write({ 'promotions': True })
-        return True
+        user[0].write({ 'promotions': params.get('allow_promotions') })
+        return user[0].email
+
 
     #Private methods
     def _to_pydantic(self, user):
 
         representative = None
         if (user.company_type == 'company' and user.child_ids):
             representative = UserShort.from_orm(user.child_ids[0])
@@ -95,9 +96,10 @@
             'representative': representative,
             'about_us': false_to_none(user, 'about_us'),
             'interests': user.interest_ids.mapped(lambda i: i.name) if user.interest_ids else []
         })
 
     def _validator_promotions(self):
         return {
-            'id':{'type': 'integer'}
+            'id':{'type': 'integer'},
+            'allow_promotions': {'type': 'boolean'}
         }
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/tests/common.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo/addons/photovoltaic_api/tests/test_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo/addons/photovoltaic_api/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.3/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_api-13.0.1.1.4/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

