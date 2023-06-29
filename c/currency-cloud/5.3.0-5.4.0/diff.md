# Comparing `tmp/currency_cloud-5.3.0.tar.gz` & `tmp/currency_cloud-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currency_cloud-5.3.0.tar", last modified: Tue Apr  4 08:48:15 2023, max compression
+gzip compressed data, was "currency_cloud-5.4.0.tar", last modified: Thu Jun 29 15:00:15 2023, max compression
```

## Comparing `currency_cloud-5.3.0.tar` & `currency_cloud-5.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.861354 currency_cloud-5.3.0/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1085 2019-02-08 12:30:25.000000 currency_cloud-5.3.0/LICENSE.md
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      878 2023-04-04 08:48:15.860870 currency_cloud-5.3.0/PKG-INFO
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)    10427 2023-04-04 08:46:18.000000 currency_cloud-5.3.0/README.md
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)       38 2023-04-04 08:48:15.861493 currency_cloud-5.3.0/setup.cfg
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1465 2023-04-04 08:44:49.000000 currency_cloud-5.3.0/setup.py
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.818462 currency_cloud-5.3.0/src/
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.823657 currency_cloud-5.3.0/src/currency_cloud.egg-info/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      878 2023-04-04 08:48:15.000000 currency_cloud-5.3.0/src/currency_cloud.egg-info/PKG-INFO
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2164 2023-04-04 08:48:15.000000 currency_cloud-5.3.0/src/currency_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)        1 2023-04-04 08:48:15.000000 currency_cloud-5.3.0/src/currency_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)       28 2023-04-04 08:48:15.000000 currency_cloud-5.3.0/src/currency_cloud.egg-info/requires.txt
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)       14 2023-04-04 08:48:15.000000 currency_cloud-5.3.0/src/currency_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.827478 currency_cloud-5.3.0/src/currencycloud/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      578 2019-05-22 10:48:57.000000 currency_cloud-5.3.0/src/currencycloud/__init__.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     5834 2023-03-20 12:40:39.000000 currency_cloud-5.3.0/src/currencycloud/client.py
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.842589 currency_cloud-5.3.0/src/currencycloud/clients/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1041 2020-12-01 17:38:55.000000 currency_cloud-5.3.0/src/currencycloud/clients/__init__.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2382 2019-05-22 10:48:57.000000 currency_cloud-5.3.0/src/currencycloud/clients/accounts.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      646 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/auth.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1295 2020-03-16 17:07:49.000000 currency_cloud-5.3.0/src/currencycloud/clients/balances.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3189 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/beneficiaries.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1745 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/contacts.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3531 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/conversions.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      751 2020-01-23 09:52:25.000000 currency_cloud-5.3.0/src/currencycloud/clients/funding.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      602 2019-02-08 12:30:25.000000 currency_cloud-5.3.0/src/currencycloud/clients/ibans.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      454 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/payers.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3954 2023-03-20 12:40:39.000000 currency_cloud-5.3.0/src/currencycloud/clients/payments.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1296 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/rates.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2780 2020-01-02 14:59:27.000000 currency_cloud-5.3.0/src/currencycloud/clients/reference.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1294 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/reports.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      358 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/senders.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      940 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/clients/transactions.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1425 2022-07-12 14:24:53.000000 currency_cloud-5.3.0/src/currencycloud/clients/transfers.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      719 2019-05-22 10:48:57.000000 currency_cloud-5.3.0/src/currencycloud/clients/vans.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1081 2020-09-25 12:49:10.000000 currency_cloud-5.3.0/src/currencycloud/clients/withdrawal_accounts.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2553 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/config.py
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.844193 currency_cloud-5.3.0/src/currencycloud/errors/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      199 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/errors/__init__.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3698 2023-04-04 08:28:58.000000 currency_cloud-5.3.0/src/currencycloud/errors/api.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     4224 2023-03-20 12:40:39.000000 currency_cloud-5.3.0/src/currencycloud/http.py
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.858147 currency_cloud-5.3.0/src/currencycloud/resources/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1281 2020-12-01 17:38:55.000000 currency_cloud-5.3.0/src/currencycloud/resources/__init__.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      347 2019-05-22 10:48:57.000000 currency_cloud-5.3.0/src/currencycloud/resources/account.py
-drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-04-04 08:48:15.860138 currency_cloud-5.3.0/src/currencycloud/resources/actions/
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      197 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/actions/__init__.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      286 2023-03-20 12:40:39.000000 currency_cloud-5.3.0/src/currencycloud/resources/actions/delete.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      352 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/actions/update.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      342 2020-03-16 17:07:49.000000 currency_cloud-5.3.0/src/currencycloud/resources/balance.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      334 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/beneficiary.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      296 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/contact.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      236 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/conversion.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      242 2020-01-23 09:52:25.000000 currency_cloud-5.3.0/src/currencycloud/resources/funding.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      290 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/iban.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      612 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/paginated_collection.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)       93 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/pagination.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      221 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/payer.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      565 2023-03-20 12:40:39.000000 currency_cloud-5.3.0/src/currencycloud/resources/payment.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      305 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/rate.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      416 2019-10-22 13:04:25.000000 currency_cloud-5.3.0/src/currencycloud/resources/reference.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      146 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/report.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1660 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/resource.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      145 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/sender.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      239 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/transaction.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      230 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/transfer.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      288 2018-11-21 11:19:56.000000 currency_cloud-5.3.0/src/currencycloud/resources/van.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)      400 2020-09-25 12:49:10.000000 currency_cloud-5.3.0/src/currencycloud/resources/withdrawal_account.py
--rw-r--r--   0 jonathan.couchman   (502) staff       (20)       18 2023-04-04 08:46:18.000000 currency_cloud-5.3.0/src/currencycloud/version.py
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.738544 currency_cloud-5.4.0/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1085 2019-02-08 12:30:25.000000 currency_cloud-5.4.0/LICENSE.md
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      878 2023-06-29 15:00:15.737606 currency_cloud-5.4.0/PKG-INFO
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)    10753 2023-06-29 14:55:49.000000 currency_cloud-5.4.0/README.md
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)       38 2023-06-29 15:00:15.738812 currency_cloud-5.4.0/setup.cfg
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1465 2023-06-29 14:52:12.000000 currency_cloud-5.4.0/setup.py
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.641957 currency_cloud-5.4.0/src/
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.647319 currency_cloud-5.4.0/src/currency_cloud.egg-info/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      878 2023-06-29 15:00:15.000000 currency_cloud-5.4.0/src/currency_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2164 2023-06-29 15:00:15.000000 currency_cloud-5.4.0/src/currency_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)        1 2023-06-29 15:00:15.000000 currency_cloud-5.4.0/src/currency_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)       28 2023-06-29 15:00:15.000000 currency_cloud-5.4.0/src/currency_cloud.egg-info/requires.txt
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)       14 2023-06-29 15:00:15.000000 currency_cloud-5.4.0/src/currency_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.650720 currency_cloud-5.4.0/src/currencycloud/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      578 2019-05-22 10:48:57.000000 currency_cloud-5.4.0/src/currencycloud/__init__.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     5834 2023-03-20 12:40:39.000000 currency_cloud-5.4.0/src/currencycloud/client.py
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.690044 currency_cloud-5.4.0/src/currencycloud/clients/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1041 2020-12-01 17:38:55.000000 currency_cloud-5.4.0/src/currencycloud/clients/__init__.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2377 2023-06-29 14:52:12.000000 currency_cloud-5.4.0/src/currencycloud/clients/accounts.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      646 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/auth.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1295 2020-03-16 17:07:49.000000 currency_cloud-5.4.0/src/currencycloud/clients/balances.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3184 2023-06-29 14:52:12.000000 currency_cloud-5.4.0/src/currencycloud/clients/beneficiaries.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1740 2023-06-29 14:52:12.000000 currency_cloud-5.4.0/src/currencycloud/clients/contacts.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3531 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/conversions.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      751 2020-01-23 09:52:25.000000 currency_cloud-5.4.0/src/currencycloud/clients/funding.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      602 2019-02-08 12:30:25.000000 currency_cloud-5.4.0/src/currencycloud/clients/ibans.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      454 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/payers.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3954 2023-03-20 12:40:39.000000 currency_cloud-5.4.0/src/currencycloud/clients/payments.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1296 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/rates.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2780 2023-06-29 14:52:12.000000 currency_cloud-5.4.0/src/currencycloud/clients/reference.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1294 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/reports.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      358 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/senders.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      940 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/clients/transactions.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1425 2022-07-12 14:24:53.000000 currency_cloud-5.4.0/src/currencycloud/clients/transfers.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      719 2019-05-22 10:48:57.000000 currency_cloud-5.4.0/src/currencycloud/clients/vans.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1081 2020-09-25 12:49:10.000000 currency_cloud-5.4.0/src/currencycloud/clients/withdrawal_accounts.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     2553 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/config.py
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.692580 currency_cloud-5.4.0/src/currencycloud/errors/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      199 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/errors/__init__.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     3698 2023-04-04 08:28:58.000000 currency_cloud-5.4.0/src/currencycloud/errors/api.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     4224 2023-03-20 12:40:39.000000 currency_cloud-5.4.0/src/currencycloud/http.py
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.727425 currency_cloud-5.4.0/src/currencycloud/resources/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1281 2020-12-01 17:38:55.000000 currency_cloud-5.4.0/src/currencycloud/resources/__init__.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      347 2019-05-22 10:48:57.000000 currency_cloud-5.4.0/src/currencycloud/resources/account.py
+drwxr-xr-x   0 jonathan.couchman   (502) staff       (20)        0 2023-06-29 15:00:15.735262 currency_cloud-5.4.0/src/currencycloud/resources/actions/
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      197 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/actions/__init__.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      286 2023-03-20 12:40:39.000000 currency_cloud-5.4.0/src/currencycloud/resources/actions/delete.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      352 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/actions/update.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      342 2020-03-16 17:07:49.000000 currency_cloud-5.4.0/src/currencycloud/resources/balance.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      334 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/beneficiary.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      296 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/contact.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      236 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/conversion.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      242 2020-01-23 09:52:25.000000 currency_cloud-5.4.0/src/currencycloud/resources/funding.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      290 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/iban.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      612 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/paginated_collection.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)       93 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/pagination.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      221 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/payer.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      565 2023-03-20 12:40:39.000000 currency_cloud-5.4.0/src/currencycloud/resources/payment.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      305 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/rate.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      416 2019-10-22 13:04:25.000000 currency_cloud-5.4.0/src/currencycloud/resources/reference.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      146 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/report.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)     1660 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/resource.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      145 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/sender.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      239 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/transaction.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      230 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/transfer.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      288 2018-11-21 11:19:56.000000 currency_cloud-5.4.0/src/currencycloud/resources/van.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)      400 2020-09-25 12:49:10.000000 currency_cloud-5.4.0/src/currencycloud/resources/withdrawal_account.py
+-rw-r--r--   0 jonathan.couchman   (502) staff       (20)       18 2023-06-29 14:54:31.000000 currency_cloud-5.4.0/src/currencycloud/version.py
```

### Comparing `currency_cloud-5.3.0/LICENSE.md` & `currency_cloud-5.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/PKG-INFO` & `currency_cloud-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currency_cloud
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python SDK for the Currencycloud API.
 Home-page: https://github.com/CurrencyCloud/currencycloud-python
 Author: Currencycloud
 Author-email: sdk@currencycloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `currency_cloud-5.3.0/README.md` & `currency_cloud-5.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -217,14 +217,23 @@
 
 ### List of features being deprecated
 ```
 (No features are currently being deprecated)
 ```
 
 # Release History
+* [5.4.0]
+    * Add POST accounts/find 
+    * Deprecate GET accounts/find     
+    * Add POST beneficiaries/find     
+    * Deprecate GET beneficiaries/find     
+    * Add POST contacts/find     
+    * Deprecate GET contacts/find     
+    * Add POST reference/bank_details/find     
+    * Deprecate GET reference/bank_details
 * [5.3.0]
     * Redact sensitive data in error logs
     * Fix handling of malformed error responses
 * [5.2.0]
     * Fixes User-Agent header for authenticated calls
     * Adds support for transfers/{id}/cancel
 * [5.1.2]
```

### Comparing `currency_cloud-5.3.0/setup.py` & `currency_cloud-5.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os.path import splitext
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='currency_cloud',
-    version='5.3.0',
+    version='5.4.0',
     license='MIT',
     description="Python SDK for the Currencycloud API.",
     long_description='',
 
     author='Currencycloud',
     author_email='sdk@currencycloud.com',
     url='https://github.com/CurrencyCloud/currencycloud-python',
```

### Comparing `currency_cloud-5.3.0/src/currency_cloud.egg-info/PKG-INFO` & `currency_cloud-5.4.0/src/currency_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currency-cloud
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python SDK for the Currencycloud API.
 Home-page: https://github.com/CurrencyCloud/currencycloud-python
 Author: Currencycloud
 Author-email: sdk@currencycloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `currency_cloud-5.3.0/src/currency_cloud.egg-info/SOURCES.txt` & `currency_cloud-5.4.0/src/currency_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/__init__.py` & `currency_cloud-5.4.0/src/currencycloud/__init__.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/client.py` & `currency_cloud-5.4.0/src/currencycloud/client.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/__init__.py` & `currency_cloud-5.4.0/src/currencycloud/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/accounts.py` & `currency_cloud-5.4.0/src/currencycloud/clients/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         return Account(self, **self.get('/v2/accounts/current'))
 
     def find(self, **kwargs):
         '''
         Return an array containing json structures of details of the accounts matching the
         search criteria for the logged in user.
         '''
-        response = self.get('/v2/accounts/find', query=kwargs)
+        response = self.post('/v2/accounts/find', kwargs)
         data = [Account(self, **fields) for fields in response['accounts']]
         return PaginatedCollection(data, response['pagination'])
 
     def first(self, **params):
         params['per_page'] = 1
         return self.find(**params)[0]
```

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/auth.py` & `currency_cloud-5.4.0/src/currencycloud/clients/auth.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/balances.py` & `currency_cloud-5.4.0/src/currencycloud/clients/balances.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/beneficiaries.py` & `currency_cloud-5.4.0/src/currencycloud/clients/beneficiaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return Beneficiary(self, **self.post('/v2/beneficiaries/' + resource_id + '/delete', kwargs))
 
     def find(self, **kwargs):
         '''
         Return an array containing json structures of details of the accounts matching the search
         criteria for the logged in user.
         '''
-        response = self.get('/v2/beneficiaries/find', query=kwargs)
+        response = self.post('/v2/beneficiaries/find', kwargs)
         data = [Beneficiary(self, **fields) for fields in response['beneficiaries']]
         return PaginatedCollection(data, response['pagination'])
 
     def first(self, **params):
         params['per_page'] = 1
         return self.find(**params)[0]
```

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/contacts.py` & `currency_cloud-5.4.0/src/currencycloud/clients/contacts.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         return Contact(self, **self.get('/v2/contacts/current'))
 
     def find(self, **kwargs):
         '''
         A paged response of an array containing hashes of details of the contacts matching the
         search criteria for the active user.
         '''
-        response = self.get('/v2/contacts/find', query=kwargs)
+        response = self.post('/v2/contacts/find', kwargs)
         data = [Contact(self, **fields) for fields in response['contacts']]
         return PaginatedCollection(data, response['pagination'])
 
     def first(self, **params):
         params['per_page'] = 1
         return self.find(**params)[0]
```

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/conversions.py` & `currency_cloud-5.4.0/src/currencycloud/clients/conversions.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/funding.py` & `currency_cloud-5.4.0/src/currencycloud/clients/funding.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/ibans.py` & `currency_cloud-5.4.0/src/currencycloud/clients/ibans.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/payments.py` & `currency_cloud-5.4.0/src/currencycloud/clients/payments.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/rates.py` & `currency_cloud-5.4.0/src/currencycloud/clients/rates.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/reference.py` & `currency_cloud-5.4.0/src/currencycloud/clients/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
     def payment_purpose_codes(self, **kwargs):
         '''Returns a list of valid purpose codes for the specified currency.'''
         response = self.get('/v2/reference/payment_purpose_codes', query=kwargs)['purpose_codes']
         return [PaymentPurposeCode(self, **c) for c in response]
 
     def bank_details(self, **kwargs):
         '''Returns the details of the bank related to the specified identifier.'''
-        response = self.get('/v2/reference/bank_details', query=kwargs)
+        response = self.post('/v2/reference/bank_details/find', kwargs)
         return BankDetails(self, **response)
 
     def payment_fee_rules(self, **kwargs):
         '''Returns a list of payment fee rules.'''
         response = self.get('/v2/reference/payment_fee_rules', query=kwargs)['payment_fee_rules']
         return [PaymentFeeRule(self, **c) for c in response]
```

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/reports.py` & `currency_cloud-5.4.0/src/currencycloud/clients/reports.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/transactions.py` & `currency_cloud-5.4.0/src/currencycloud/clients/transactions.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/transfers.py` & `currency_cloud-5.4.0/src/currencycloud/clients/transfers.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/vans.py` & `currency_cloud-5.4.0/src/currencycloud/clients/vans.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/clients/withdrawal_accounts.py` & `currency_cloud-5.4.0/src/currencycloud/clients/withdrawal_accounts.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/config.py` & `currency_cloud-5.4.0/src/currencycloud/config.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/errors/api.py` & `currency_cloud-5.4.0/src/currencycloud/errors/api.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/http.py` & `currency_cloud-5.4.0/src/currencycloud/http.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/resources/__init__.py` & `currency_cloud-5.4.0/src/currencycloud/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/resources/paginated_collection.py` & `currency_cloud-5.4.0/src/currencycloud/resources/paginated_collection.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/resources/payment.py` & `currency_cloud-5.4.0/src/currencycloud/resources/payment.py`

 * *Files identical despite different names*

### Comparing `currency_cloud-5.3.0/src/currencycloud/resources/resource.py` & `currency_cloud-5.4.0/src/currencycloud/resources/resource.py`

 * *Files identical despite different names*

