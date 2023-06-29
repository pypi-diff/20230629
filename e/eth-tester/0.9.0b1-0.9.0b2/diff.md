# Comparing `tmp/eth-tester-0.9.0b1.tar.gz` & `tmp/eth-tester-0.9.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-tester-0.9.0b1.tar", last modified: Fri May 12 17:13:15 2023, max compression
+gzip compressed data, was "eth-tester-0.9.0b2.tar", last modified: Thu Jun 29 16:33:27 2023, max compression
```

## Comparing `eth-tester-0.9.0b1.tar` & `eth-tester-0.9.0b2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.097611 eth-tester-0.9.0b1/
--rw-r--r--   0 fselmo     (501) staff       (20)     1080 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/LICENSE
--rw-r--r--   0 fselmo     (501) staff       (20)      121 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/MANIFEST.in
--rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-05-12 17:13:15.097258 eth-tester-0.9.0b1/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)    34123 2023-04-27 17:15:42.000000 eth-tester-0.9.0b1/README.md
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.067687 eth-tester-0.9.0b1/eth_tester/
--rw-r--r--   0 fselmo     (501) staff       (20)      331 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.072724 eth-tester-0.9.0b1/eth_tester/backends/
--rw-r--r--   0 fselmo     (501) staff       (20)     1652 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/backends/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2889 2023-02-01 17:33:56.000000 eth-tester-0.9.0b1/eth_tester/backends/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/backends/common.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.076943 eth-tester-0.9.0b1/eth_tester/backends/mock/
--rw-r--r--   0 fselmo     (501) staff       (20)       53 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      304 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)    13229 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/factory.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9480 2023-05-11 22:08:22.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/serializers.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.080301 eth-tester-0.9.0b1/eth_tester/backends/pyevm/
--rw-r--r--   0 fselmo     (501) staff       (20)      173 2021-11-18 21:01:41.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    26621 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8556 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/serializers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      515 2021-11-18 21:01:41.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1725 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      413 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)    29630 2023-02-01 17:33:56.000000 eth-tester-0.9.0b1/eth_tester/main.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.084919 eth-tester-0.9.0b1/eth_tester/normalization/
--rw-r--r--   0 fselmo     (501) staff       (20)      702 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/normalization/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3297 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/normalization/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      636 2023-05-01 23:05:21.000000 eth-tester-0.9.0b1/eth_tester/normalization/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2665 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/normalization/default.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3171 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/normalization/inbound.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5366 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/normalization/outbound.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/rpc.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.086025 eth-tester-0.9.0b1/eth_tester/tools/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-10 20:58:14.000000 eth-tester-0.9.0b1/eth_tester/tools/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2235 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/tools/gas_burner_contract.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.093400 eth-tester-0.9.0b1/eth_tester/utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      152 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/utils/accounts.py
--rw-r--r--   0 fselmo     (501) staff       (20)      243 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/utils/address.py
--rw-r--r--   0 fselmo     (501) staff       (20)    64238 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/utils/backend_testing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9633 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/emitter_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)      323 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/encoding.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5244 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/filters.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4324 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/math_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)      906 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/module_loading.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5035 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/throws_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1191 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.096555 eth-tester-0.9.0b1/eth_tester/validation/
--rw-r--r--   0 fselmo     (501) staff       (20)      658 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/validation/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2949 2021-11-04 23:39:22.000000 eth-tester-0.9.0b1/eth_tester/validation/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5833 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/validation/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2903 2021-10-06 21:26:28.000000 eth-tester-0.9.0b1/eth_tester/validation/default.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11059 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/validation/inbound.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9124 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/validation/outbound.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.070441 eth-tester-0.9.0b1/eth_tester.egg-info/
--rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     1616 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/SOURCES.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/dependency_links.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2022-11-21 22:09:50.000000 eth-tester-0.9.0b1/eth_tester.egg-info/not-zip-safe
--rw-r--r--   0 fselmo     (501) staff       (20)      994 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/requires.txt
--rw-r--r--   0 fselmo     (501) staff       (20)       11 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/top_level.txt
--rw-r--r--   0 fselmo     (501) staff       (20)     1055 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/pyproject.toml
--rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-05-12 17:13:15.097705 eth-tester-0.9.0b1/setup.cfg
--rw-r--r--   0 fselmo     (501) staff       (20)     2532 2023-05-12 17:10:30.000000 eth-tester-0.9.0b1/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.569672 eth-tester-0.9.0b2/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1080 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/LICENSE
+-rw-r--r--   0 fselmo     (501) staff       (20)      121 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/MANIFEST.in
+-rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-06-29 16:33:27.569154 eth-tester-0.9.0b2/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)    34123 2023-04-27 17:15:42.000000 eth-tester-0.9.0b2/README.md
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.531983 eth-tester-0.9.0b2/eth_tester/
+-rw-r--r--   0 fselmo     (501) staff       (20)      331 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.537466 eth-tester-0.9.0b2/eth_tester/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1652 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/backends/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2889 2023-06-28 15:53:58.000000 eth-tester-0.9.0b2/eth_tester/backends/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/backends/common.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.541611 eth-tester-0.9.0b2/eth_tester/backends/mock/
+-rw-r--r--   0 fselmo     (501) staff       (20)       53 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      304 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    13229 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/factory.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9480 2023-06-28 15:53:58.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/serializers.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.545902 eth-tester-0.9.0b2/eth_tester/backends/pyevm/
+-rw-r--r--   0 fselmo     (501) staff       (20)      173 2021-11-18 21:01:41.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    26856 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8556 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/serializers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      515 2021-11-18 21:01:41.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1725 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      413 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    30564 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/main.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.551534 eth-tester-0.9.0b2/eth_tester/normalization/
+-rw-r--r--   0 fselmo     (501) staff       (20)      702 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/normalization/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3429 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/normalization/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      924 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/normalization/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2869 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/normalization/default.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3171 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/normalization/inbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5748 2023-06-26 21:57:05.000000 eth-tester-0.9.0b2/eth_tester/normalization/outbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/rpc.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.553273 eth-tester-0.9.0b2/eth_tester/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-10 20:58:14.000000 eth-tester-0.9.0b2/eth_tester/tools/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2235 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/tools/gas_burner_contract.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.563598 eth-tester-0.9.0b2/eth_tester/utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      152 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/utils/accounts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      243 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/utils/address.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    64238 2023-06-28 15:53:58.000000 eth-tester-0.9.0b2/eth_tester/utils/backend_testing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9633 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/emitter_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      323 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/encoding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5244 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/filters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4324 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/math_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      906 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/module_loading.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5035 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/throws_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1191 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.568182 eth-tester-0.9.0b2/eth_tester/validation/
+-rw-r--r--   0 fselmo     (501) staff       (20)      658 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/validation/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3075 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/validation/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5833 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/validation/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3114 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/validation/default.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11442 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/validation/inbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9124 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/validation/outbound.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.535329 eth-tester-0.9.0b2/eth_tester.egg-info/
+-rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     1616 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2022-11-21 22:09:50.000000 eth-tester-0.9.0b2/eth_tester.egg-info/not-zip-safe
+-rw-r--r--   0 fselmo     (501) staff       (20)      988 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/requires.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       11 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/top_level.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)     1055 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/pyproject.toml
+-rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-06-29 16:33:27.569839 eth-tester-0.9.0b2/setup.cfg
+-rw-r--r--   0 fselmo     (501) staff       (20)     2529 2023-06-29 16:32:33.000000 eth-tester-0.9.0b2/setup.py
```

### Comparing `eth-tester-0.9.0b1/LICENSE` & `eth-tester-0.9.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/PKG-INFO` & `eth-tester-0.9.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `eth-tester-0.9.0b1/README.md` & `eth-tester-0.9.0b2/README.md`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/__init__.py` & `eth-tester-0.9.0b2/eth_tester/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/base.py` & `eth-tester-0.9.0b2/eth_tester/backends/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/common.py` & `eth-tester-0.9.0b2/eth_tester/backends/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/mock/factory.py` & `eth-tester-0.9.0b2/eth_tester/backends/mock/factory.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/mock/main.py` & `eth-tester-0.9.0b2/eth_tester/backends/mock/main.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/mock/serializers.py` & `eth-tester-0.9.0b2/eth_tester/backends/mock/serializers.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/pyevm/main.py` & `eth-tester-0.9.0b2/eth_tester/backends/pyevm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from typing import Dict, List, Union
 
 from eth_abi import abi
 from eth_abi.exceptions import DecodingError
 
 from eth_account.hdaccount import HDPath, seed_from_mnemonic
+from eth_typing import Address
 
 from eth_utils import (
     encode_hex,
     int_to_big_endian,
     to_bytes,
     to_checksum_address,
     to_dict,
@@ -534,14 +535,18 @@
         vm = _get_vm_for_block_number(self.chain, block_number)
         return vm.state.get_balance(account)
 
     def get_code(self, account, block_number="latest"):
         vm = _get_vm_for_block_number(self.chain, block_number)
         return vm.state.get_code(account)
 
+    def get_storage(self, account: Address, slot: int, block_number="latest") -> bytes:
+        vm = _get_vm_for_block_number(self.chain, block_number)
+        return vm.state.get_storage(account, slot)
+
     def get_base_fee(self, block_number="latest"):
         vm = _get_vm_for_block_number(self.chain, block_number)
         return vm.state.base_fee
 
     #
     # Transactions
     #
```

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/pyevm/serializers.py` & `eth-tester-0.9.0b2/eth_tester/backends/pyevm/serializers.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/backends/pyevm/utils.py` & `eth-tester-0.9.0b2/eth_tester/backends/pyevm/utils.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/constants.py` & `eth-tester-0.9.0b2/eth_tester/constants.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/main.py` & `eth-tester-0.9.0b2/eth_tester/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 import collections
 import itertools
 import operator
 import time
 import functools
 
+from eth_typing import (
+    HexAddress,
+    HexStr,
+)
 from eth_utils import (
     is_integer,
     is_same_address,
     to_list,
     to_tuple,
 )
 
@@ -250,14 +254,32 @@
         raw_account = self.normalizer.normalize_inbound_account(account)
         raw_block_number = self.normalizer.normalize_inbound_block_number(block_number)
         raw_code = self.backend.get_code(raw_account, raw_block_number)
         self.validator.validate_outbound_code(raw_code)
         code = self.normalizer.normalize_outbound_code(raw_code)
         return code
 
+    def get_storage_at(
+        self,
+        account: HexAddress,
+        slot: HexStr,
+        # properly type hint once eth-typing brings in updated `BlockIdentifier`
+        block_number="latest",
+    ) -> int:
+        self.validator.validate_inbound_account(account)
+        self.validator.validate_inbound_storage_slot(slot)
+        self.validator.validate_inbound_block_number(block_number)
+        raw_account = self.normalizer.normalize_inbound_account(account)
+        raw_slot = self.normalizer.normalize_inbound_storage_slot(slot)
+        raw_block_number = self.normalizer.normalize_inbound_block_number(block_number)
+        raw_storage = self.backend.get_storage(raw_account, raw_slot, raw_block_number)
+        self.validator.validate_outbound_storage(raw_storage)
+        storage = self.normalizer.normalize_outbound_storage(raw_storage)
+        return storage
+
     def get_nonce(self, account, block_number="latest"):
         self.validator.validate_inbound_account(account)
         self.validator.validate_inbound_block_number(block_number)
         raw_account = self.normalizer.normalize_inbound_account(account)
         raw_block_number = self.normalizer.normalize_inbound_block_number(block_number)
         raw_nonce = self.backend.get_nonce(raw_account, raw_block_number)
         self.validator.validate_outbound_nonce(raw_nonce)
```

### Comparing `eth-tester-0.9.0b1/eth_tester/normalization/__init__.py` & `eth-tester-0.9.0b2/eth_tester/normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/normalization/base.py` & `eth-tester-0.9.0b2/eth_tester/normalization/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
     def normalize_inbound_private_key(self, private_key):
         raise NotImplementedError("must be implemented by subclasses")
 
     def normalize_inbound_raw_transaction(self, raw_transaction_hex):
         raise NotImplementedError("must be implemented by subclasses")
 
+    def normalize_inbound_storage_slot(self, storage_slot):
+        raise NotImplementedError("must be implemented by subclasses")
+
     def normalize_inbound_timestamp(self, timestamp):
         raise NotImplementedError("must be implemented by subclasses")
 
     def normalize_inbound_transaction(self, transaction):
         raise NotImplementedError("must be implemented by subclasses")
 
     def normalize_inbound_transaction_hash(self, transaction_hash):
```

### Comparing `eth-tester-0.9.0b1/eth_tester/normalization/default.py` & `eth-tester-0.9.0b2/eth_tester/normalization/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from eth_utils.toolz import (
     identity,
 )
 
 from .base import (
     BaseNormalizer,
 )
+from .common import (
+    int_to_32byte_hex,
+    to_integer_if_hex,
+)
 from .inbound import (
     normalize_filter_params as normalize_inbound_filter_params,
     normalize_log_entry as normalize_inbound_log_entry,
     normalize_private_key as normalize_inbound_private_key,
     normalize_raw_transaction as normalize_inbound_raw_transaction,
     normalize_transaction as normalize_inbound_transaction,
 )
@@ -36,14 +40,15 @@
     normalize_inbound_block_hash = staticmethod(decode_hex)
     normalize_inbound_block_number = staticmethod(identity)
     normalize_inbound_filter_id = staticmethod(identity)
     normalize_inbound_filter_params = staticmethod(normalize_inbound_filter_params)
     normalize_inbound_log_entry = staticmethod(normalize_inbound_log_entry)
     normalize_inbound_private_key = staticmethod(normalize_inbound_private_key)
     normalize_inbound_raw_transaction = staticmethod(normalize_inbound_raw_transaction)
+    normalize_inbound_storage_slot = staticmethod(to_integer_if_hex)
     normalize_inbound_timestamp = staticmethod(identity)
     normalize_inbound_transaction = staticmethod(normalize_inbound_transaction)
     normalize_inbound_transaction_hash = staticmethod(decode_hex)
 
     # Outbound
     normalize_outbound_account = staticmethod(normalize_outbound_account)
     normalize_outbound_account_list = staticmethod(normalize_outbound_account_list)
@@ -53,9 +58,10 @@
     normalize_outbound_code = staticmethod(encode_hex)
     normalize_outbound_filter_id = staticmethod(identity)
     normalize_outbound_log_entry = staticmethod(normalize_outbound_log_entry)
     normalize_outbound_gas_estimate = staticmethod(identity)
     normalize_outbound_nonce = staticmethod(identity)
     normalize_outbound_receipt = staticmethod(normalize_outbound_receipt)
     normalize_outbound_return_data = staticmethod(encode_hex)
+    normalize_outbound_storage = staticmethod(int_to_32byte_hex)
     normalize_outbound_transaction = staticmethod(normalize_outbound_transaction)
     normalize_outbound_transaction_hash = staticmethod(encode_hex)
```

### Comparing `eth-tester-0.9.0b1/eth_tester/normalization/inbound.py` & `eth-tester-0.9.0b2/eth_tester/normalization/inbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/normalization/outbound.py` & `eth-tester-0.9.0b2/eth_tester/normalization/outbound.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import absolute_import
 
-from toolz import dissoc
+from toolz import (
+    assoc,
+    dissoc,
+)
 
 from eth_utils.curried import (
     apply_one_of_formatters,
     to_checksum_address,
     encode_hex,
     is_address,
     is_bytes,
@@ -164,33 +167,45 @@
     "address": to_checksum_address,
     "data": encode_hex,
     "topics": partial(normalize_array, normalizer=encode_hex),
 }
 normalize_log_entry = partial(normalize_dict, normalizers=LOG_ENTRY_NORMALIZERS)
 
 
+def _normalize_contract_address(receipt):
+    if receipt["status"] == 0:
+        return assoc(receipt, "contract_address", None)
+    elif is_address(receipt["contract_address"]):
+        return assoc(
+            receipt,
+            "contract_address",
+            to_checksum_address(receipt["contract_address"]),
+        )
+    else:
+        return receipt
+
+
 RECEIPT_NORMALIZERS = {
     "transaction_hash": encode_hex,
     "transaction_index": identity,
     "block_number": identity,
     "block_hash": partial(
         normalize_if,
         conditional_fn=is_bytes,
         normalizer=encode_hex,
     ),
     "cumulative_gas_used": identity,
     "effective_gas_price": identity,
     "from": to_checksum_address,
     "gas_used": identity,
-    "contract_address": partial(
-        normalize_if,
-        conditional_fn=is_address,
-        normalizer=to_checksum_address,
-    ),
+    "contract_address": identity,  # special case, see ``_normalize_contract_address()``
     "logs": partial(normalize_array, normalizer=normalize_log_entry),
     "state_root": identity,
     "status": identity,
     "to": to_empty_or_checksum_address,
     "type": identity,
     "base_fee_per_gas": identity,
 }
-normalize_receipt = partial(normalize_dict, normalizers=RECEIPT_NORMALIZERS)
+normalize_receipt = compose(
+    partial(normalize_dict, normalizers=RECEIPT_NORMALIZERS),
+    _normalize_contract_address,
+)
```

### Comparing `eth-tester-0.9.0b1/eth_tester/tools/gas_burner_contract.py` & `eth-tester-0.9.0b2/eth_tester/tools/gas_burner_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/backend_testing.py` & `eth-tester-0.9.0b2/eth_tester/utils/backend_testing.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/emitter_contract.py` & `eth-tester-0.9.0b2/eth_tester/utils/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/filters.py` & `eth-tester-0.9.0b2/eth_tester/utils/filters.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/math_contract.py` & `eth-tester-0.9.0b2/eth_tester/utils/math_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/module_loading.py` & `eth-tester-0.9.0b2/eth_tester/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/throws_contract.py` & `eth-tester-0.9.0b2/eth_tester/utils/throws_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/utils/transactions.py` & `eth-tester-0.9.0b2/eth_tester/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/validation/__init__.py` & `eth-tester-0.9.0b2/eth_tester/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/validation/base.py` & `eth-tester-0.9.0b2/eth_tester/validation/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 class BaseValidator:
     #
     # Inbound
     #
     def validate_inbound_account(self, account):
         raise NotImplementedError("must be implemented by subclasses")
 
+    def validate_inbound_storage_slot(self, account):
+        raise NotImplementedError("must be implemented by subclasses")
+
     def validate_inbound_block_hash(self, block_hash):
         raise NotImplementedError("must be implemented by subclasses")
 
     def validate_inbound_block_number(self, block_number):
         raise NotImplementedError("must be implemented by subclasses")
 
     def validate_inbound_filter_id(self, filter_id):
```

### Comparing `eth-tester-0.9.0b1/eth_tester/validation/common.py` & `eth-tester-0.9.0b2/eth_tester/validation/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester/validation/default.py` & `eth-tester-0.9.0b2/eth_tester/validation/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     validate_account as validate_inbound_account,
     validate_block_hash as validate_inbound_block_hash,
     validate_block_number as validate_inbound_block_number,
     validate_filter_id as validate_inbound_filter_id,
     validate_filter_params as validate_inbound_filter_params,
     validate_private_key as validate_inbound_private_key,
     validate_raw_transaction as validate_inbound_raw_transaction,
+    validate_inbound_storage_slot as validate_inbound_storage_slot,
     validate_timestamp as validate_inbound_timestamp,
     validate_transaction as validate_inbound_transaction,
     validate_transaction_hash as validate_inbound_transaction_hash,
 )
 from .outbound import (
     validate_32_byte_string,
     validate_accounts as validate_outbound_accounts,
@@ -37,14 +38,15 @@
     validate_inbound_account = staticmethod(validate_inbound_account)
     validate_inbound_block_hash = staticmethod(validate_inbound_block_hash)
     validate_inbound_block_number = staticmethod(validate_inbound_block_number)
     validate_inbound_filter_id = staticmethod(validate_inbound_filter_id)
     validate_inbound_filter_params = staticmethod(validate_inbound_filter_params)
     validate_inbound_private_key = staticmethod(validate_inbound_private_key)
     validate_inbound_raw_transaction = staticmethod(validate_inbound_raw_transaction)
+    validate_inbound_storage_slot = staticmethod(validate_inbound_storage_slot)
     validate_inbound_timestamp = staticmethod(validate_inbound_timestamp)
     validate_inbound_transaction = staticmethod(validate_inbound_transaction)
     validate_inbound_transaction_hash = staticmethod(validate_inbound_transaction_hash)
 
     #
     # Outbound
     #
@@ -54,9 +56,10 @@
     validate_outbound_block_hash = staticmethod(validate_outbound_block_hash)
     validate_outbound_code = staticmethod(validate_outbound_bytes)
     validate_outbound_gas_estimate = staticmethod(validate_uint256)
     validate_outbound_nonce = staticmethod(validate_uint256)
     validate_outbound_log_entry = staticmethod(validate_outbound_log_entry)
     validate_outbound_receipt = staticmethod(validate_outbound_receipt)
     validate_outbound_return_data = staticmethod(validate_outbound_bytes)
+    validate_outbound_storage = staticmethod(validate_uint256)
     validate_outbound_transaction = staticmethod(validate_outbound_transaction)
     validate_outbound_transaction_hash = staticmethod(validate_32_byte_string)
```

### Comparing `eth-tester-0.9.0b1/eth_tester/validation/inbound.py` & `eth-tester-0.9.0b2/eth_tester/validation/inbound.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from eth_utils import (
     is_boolean,
     is_checksum_address,
     is_checksum_formatted_address,
     is_dict,
     is_hex,
     is_hex_address,
+    is_hexstr,
     is_integer,
     is_list_like,
     is_string,
     is_text,
     remove_0x_prefix,
     decode_hex,
 )
@@ -95,22 +96,38 @@
 
 validate_block_hash = partial(validate_32_byte_hex_value, name="Block hash")
 validate_transaction_hash = partial(validate_32_byte_hex_value, name="Transaction hash")
 validate_filter_id = partial(validate_positive_integer)
 
 
 def validate_account(value):
-    if not is_text(value):
-        raise ValidationError("Address must be 20 bytes encoded as hexadecimal")
-    elif not is_hex_address(value):
-        raise ValidationError("Address must be 20 bytes encoded as hexadecimal")
+    if not is_text(value) or not is_hex_address(value):
+        raise ValidationError(
+            f"Address must be 20 bytes encoded as hexadecimal - address: {value}"
+        )
     elif is_checksum_formatted_address(value) and not is_checksum_address(value):
         raise ValidationError("Address does not validate EIP55 checksum")
 
 
+def validate_inbound_storage_slot(value):
+    error_msg = (
+        "Storage slot must be a hex string representation of a positive integer - "
+        f"slot: {value}"
+    )
+    if not (is_hexstr(value) and value.startswith("0x")):
+        raise ValidationError(error_msg)
+
+    try:
+        int_val = int(value, 16)
+    except ValueError:
+        raise ValidationError(error_msg)
+
+    validate_uint256(int_val)
+
+
 def is_valid_topic_array(value):
     if not is_list_like(value):
         return False
     return all(
         is_valid_topic_array(item) if is_list_like(item) else is_topic(item)
         for item in value
     )
```

### Comparing `eth-tester-0.9.0b1/eth_tester/validation/outbound.py` & `eth-tester-0.9.0b2/eth_tester/validation/outbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester.egg-info/PKG-INFO` & `eth-tester-0.9.0b2/eth_tester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `eth-tester-0.9.0b1/eth_tester.egg-info/SOURCES.txt` & `eth-tester-0.9.0b2/eth_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/eth_tester.egg-info/requires.txt` & `eth-tester-0.9.0b2/eth_tester.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 rlp<4,>=3.0.0
 semantic_version<3.0.0,>=2.6.0
 
 [dev]
 bumpversion<1.0.0,>=0.5.3
 tox<3.0.0,>=2.9.1
 wheel<1.0.0,>=0.30.0
-pytest<7,>=6.2.5
+pytest>=7.0.0
 pytest-xdist<3,>=2.0.0
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
 py-evm==0.7.0a2
 black<23,>=22
 flake8<4.0.0,>=3.5.0
 towncrier<22,>=21
 
@@ -45,10 +45,10 @@
 [pyevm:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
 [pyevm:implementation_name == "pypy"]
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
 
 [test]
-pytest<7,>=6.2.5
+pytest>=7.0.0
 pytest-xdist<3,>=2.0.0
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
```

### Comparing `eth-tester-0.9.0b1/pyproject.toml` & `eth-tester-0.9.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b1/setup.py` & `eth-tester-0.9.0b2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 extras_require = {
     "lint": [
         "black>=22,<23",
         "flake8>=3.5.0,<4.0.0",
     ],
     "test": [
-        "pytest>=6.2.5,<7",
+        "pytest>=7.0.0",
         "pytest-xdist>=2.0.0,<3",
         "eth-hash[pycryptodome]>=0.1.4,<1.0.0",
     ],
     "dev": [
         "bumpversion>=0.5.3,<1.0.0",
         "tox>=2.9.1,<3.0.0",
         "wheel>=0.30.0,<1.0.0",
@@ -45,15 +45,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="eth-tester",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.9.0-beta.1",
+    version="0.9.0-beta.2",
     description="""Tools for testing Ethereum applications.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/eth-tester",
     include_package_data=True,
```

