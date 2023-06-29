# Comparing `tmp/joserfc-0.2.0.tar.gz` & `tmp/joserfc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joserfc-0.2.0.tar", last modified: Sun Jun 25 09:39:52 2023, max compression
+gzip compressed data, was "joserfc-0.3.0.tar", last modified: Thu Jun 29 13:07:28 2023, max compression
```

## Comparing `joserfc-0.2.0.tar` & `joserfc-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.151733 joserfc-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 09:39:43.000000 joserfc-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-25 09:39:52.151733 joserfc-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-25 09:39:43.000000 joserfc-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-25 09:39:43.000000 joserfc-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:39:52.151733 joserfc-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 09:39:43.000000 joserfc-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/joserfc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/joserfc/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/drafts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/drafts/jwe_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/drafts/jwe_ecdh_1pu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jwe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jwk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7515/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7515/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7516/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7516/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7517/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/keygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/keyset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7517/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7518/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/derive_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/ec_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jwe_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jwe_encs.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jwe_zips.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/jws_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/oct_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/rsa_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7518/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7519/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7519/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7519/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7519/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc7638/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc7638/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc8037/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8037/jws_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8037/okp_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.147734 joserfc-0.2.0/src/joserfc/rfc8812/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/rfc8812/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-25 09:39:43.000000 joserfc-0.2.0/src/joserfc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:39:52.143734 joserfc-0.2.0/src/joserfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:39:52.000000 joserfc-0.2.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-29 13:07:03.000000 joserfc-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 13:07:28.495389 joserfc-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-29 13:07:03.000000 joserfc-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 13:07:03.000000 joserfc-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:07:28.495389 joserfc-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 13:07:03.000000 joserfc-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.487389 joserfc-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/drafts/jwe_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/drafts/jwe_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/rfc7515/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/rfc7516/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7517/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7518/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/derive_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jwe_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jwe_encs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jwe_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jws_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/rsa_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7519/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7519/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7519/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7519/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7638/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7638/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc8037/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8037/jws_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8037/okp_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc8812/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8812/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/top_level.txt
```

### Comparing `joserfc-0.2.0/LICENSE` & `joserfc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/PKG-INFO` & `joserfc-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.2.0
+Version: 0.3.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `joserfc-0.2.0/README.rst` & `joserfc-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/pyproject.toml` & `joserfc-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/drafts/jwe_chacha20.py` & `joserfc-0.3.0/src/joserfc/drafts/jwe_chacha20.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from Crypto.Cipher import ChaCha20_Poly1305
+from ..rfc7516.registry import JWERegistry
 from ..rfc7516.models import JWEEncModel
 
+__all__ = ["ChaCha20EncModel", "JWE_ENC_MODELS", "register_chaha20_poly1305"]
+
 
 class ChaCha20EncModel(JWEEncModel):
     # https://datatracker.ietf.org/doc/html/draft-amringer-jose-chacha-02#section-4
     cek_size = 256
-    recommended: bool = False
+    recommended = False
 
     def __init__(self, name: str, description: str, iv_size: int):
         self.name = name
         self.description = description
         self.iv_size = iv_size
 
     def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
@@ -27,7 +30,12 @@
         return chacha.decrypt_and_verify(ciphertext, tag)
 
 
 C20P = ChaCha20EncModel("C20P", "ChaCha20-Poly1305", 96)
 XC20P = ChaCha20EncModel("XC20P", "XChaCha20-Poly1305", 192)
 
 JWE_ENC_MODELS = [C20P, XC20P]
+
+
+def register_chaha20_poly1305():
+    for model in JWE_ENC_MODELS:
+        JWERegistry.register(model)
```

### Comparing `joserfc-0.2.0/src/joserfc/drafts/jwe_ecdh_1pu.py` & `joserfc-0.3.0/src/joserfc/drafts/jwe_ecdh_1pu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as t
+from ..rfc7516.registry import JWERegistry
 from ..rfc7516.models import (
     Recipient,
     JWEKeyAgreement,
     JWEKeyWrapping,
     JWEEncModel
 )
 from ..rfc7517.models import CurveKey
@@ -15,16 +16,19 @@
     derive_key_for_concat_kdf,
 )
 from ..rfc7518.jwe_encs import CBCHS2EncModel
 from ..registry import HeaderParameter
 from ..errors import InvalidEncryptionAlgorithmError
 
 
+__all__ = ['ECDH1PUAlgModel', 'register_ecdh_1pu', 'JWE_ALG_MODELS']
+
+
 class ECDH1PUAlgModel(JWEKeyAgreement):
-    """ Key Agreement with Elliptic Curve Diffie-Hellman One-Pass Unified Model (ECDH-1PU)
+    """Key Agreement with Elliptic Curve Diffie-Hellman One-Pass Unified Model (ECDH-1PU)
 
     https://datatracker.ietf.org/doc/html/draft-madden-jose-ecdh-1pu-04
     """
     more_header_registry = {
         "epk": HeaderParameter("Ephemeral Public Key", "jwk", True),
         "apu": HeaderParameter("Agreement PartyUInfo", "str"),
         "apv": HeaderParameter("Agreement PartyVInfo", "str"),
@@ -68,35 +72,40 @@
 
     def __encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient, tag: t.Optional[bytes]) -> bytes:
         sender_key: CurveKey = recipient.sender_key
         recipient_pubkey = recipient.recipient_key.get_op_key("deriveKey")
         sender_shared_key = sender_key.exchange_shared_key(recipient_pubkey)
         ephemeral_shared_key = recipient.ephemeral_key.exchange_shared_key(recipient_pubkey)
         shared_key = ephemeral_shared_key + sender_shared_key
-        header = recipient.headers()
-        return derive_key_for_concat_kdf(shared_key, header, enc.cek_size, self.key_size, tag)
+        headers = recipient.headers()
+        return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size, tag)
 
     def __decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient, tag: t.Optional[bytes]) -> bytes:
         self._check_enc(enc)
 
-        header = recipient.headers()
-        assert "epk" in header
+        headers = recipient.headers()
+        assert "epk" in headers
 
         recipient_key: CurveKey = recipient.recipient_key
         sender_key: CurveKey = recipient.sender_key
 
-        ephemeral_key = recipient_key.import_key(header["epk"])
+        ephemeral_key = recipient_key.import_key(headers["epk"])
         ephemeral_pubkey = ephemeral_key.get_op_key("deriveKey")
         sender_pubkey = sender_key.get_op_key("deriveKey")
 
         sender_shared_key = recipient_key.exchange_shared_key(sender_pubkey)
         ephemeral_shared_key = recipient_key.exchange_shared_key(ephemeral_pubkey)
         shared_key = ephemeral_shared_key + sender_shared_key
-        return derive_key_for_concat_kdf(shared_key, header, enc.cek_size, self.key_size, tag)
+        return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size, tag)
 
 
 JWE_ALG_MODELS = [
     ECDH1PUAlgModel(None),    # ECDH-1PU
     ECDH1PUAlgModel(A128KW),  # ECDH-1PU+A128KW
     ECDH1PUAlgModel(A192KW),  # ECDH-1PU+A192KW
     ECDH1PUAlgModel(A256KW),  # ECDH-1PU+A256KW
 ]
+
+
+def register_ecdh_1pu():
+    for model in JWE_ALG_MODELS:
+        JWERegistry.register(model)
```

### Comparing `joserfc-0.2.0/src/joserfc/errors.py` & `joserfc-0.3.0/src/joserfc/errors.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/jwe.py` & `joserfc-0.3.0/src/joserfc/jwe.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     "JWEEncModel",
     "JWEZipModel",
     "Recipient",
     "CompactEncryption",
     "JSONEncryption",
     "encrypt_compact",
     "decrypt_compact",
-    "extract_compact",
-    "validate_compact",
     "encrypt_json",
     "decrypt_json",
     "default_registry",
 ]
 
 
 def __register():
@@ -52,19 +50,19 @@
 
 
 __register()
 
 
 def encrypt_compact(
         protected: Header,
-        plaintext: bytes,
+        plaintext: t.AnyStr,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
-        sender_key: t.Optional[CurveKey] = None) -> bytes:
+        sender_key: t.Optional[CurveKey] = None) -> str:
     """Generate a JWE Compact Serialization. The JWE Compact Serialization represents
     encrypted content as a compact, URL-safe string.  This string is::
 
         BASE64URL(UTF8(JWE Protected Header)) || '.' ||
         BASE64URL(JWE Encrypted Key) || '.' ||
         BASE64URL(JWE Initialization Vector) || '.' ||
         BASE64URL(JWE Ciphertext) || '.' ||
@@ -80,22 +78,23 @@
     """
 
     if algorithms:
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
-    obj = CompactEncryption(protected, plaintext)
+    obj = CompactEncryption(protected, to_bytes(plaintext))
     recipient = Recipient(obj)
     key = guess_key(public_key, recipient)
     recipient.recipient_key = key
     recipient.sender_key = sender_key
     obj.recipient = recipient
     perform_encrypt(obj, registry)
-    return represent_compact(obj)
+    out = represent_compact(obj)
+    return out.decode("utf-8")
 
 
 def decrypt_compact(
         value: t.AnyStr,
         private_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
@@ -117,33 +116,14 @@
     :param private_key: a flexible private key to decrypt the serialization
     :param algorithms: a list of allowed algorithms
     :param registry: a JWERegistry to use
     :param sender_key: only required when using ECDH-1PU
     :return: object of the ``CompactEncryption``
     """
     obj = extract_compact(to_bytes(value))
-    return validate_compact(obj, private_key, algorithms, registry, sender_key)
-
-
-def validate_compact(
-        obj: CompactEncryption,
-        private_key: KeyFlexible,
-        algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[JWERegistry] = None,
-        sender_key: t.Optional[CurveKey] = None) -> CompactEncryption:
-    """Validate the JWE Compact Serialization with the given key.
-    This method is usually used together with ``extract_compact``.
-
-    :param obj: object of the JWE Compact Serialization
-    :param private_key: a flexible private key to decrypt the serialization
-    :param algorithms: a list of allowed algorithms
-    :param registry: a JWERegistry to use
-    :param sender_key: only required when using ECDH-1PU
-    :return: object of the ``CompactEncryption``
-    """
     if algorithms:
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
     recipient = obj.recipient
     recipient.recipient_key = guess_key(private_key, recipient)
@@ -167,17 +147,17 @@
         from joserfc.jwe import JSONEncryption
 
         protected = {"enc": "A128CBC-HS256"}
         plaintext = b"hello world"
         header = {"jku": "https://server.example.com/keys.jwks"}  # optional shared header
         obj = JSONEncryption(protected, plaintext, header)
         # add the recipients
-        obj.add_recipient(None, {"kid": "alice", "alg": "RSA1_5"})  # not configured a key
+        obj.add_recipient({"kid": "alice", "alg": "RSA1_5"})  # not configured a key
         bob_key = OctKey.import_key("bob secret")
-        obj.add_recipient(bob_key, {"kid": "bob", "alg": "A128KW"})
+        obj.add_recipient({"kid": "bob", "alg": "A128KW"}, bob_key)
 
     :param obj: an instance of ``JSONEncryption``
     :param public_key: a public key used to encrypt the CEK
     :param algorithms: a list of allowed algorithms
     :param registry: a JWERegistry to use
     :param sender_key: only required when using ECDH-1PU
     :return: JWE JSON Serialization in dict
@@ -226,13 +206,13 @@
             recipient.sender_key = _guess_sender_key(recipient, sender_key)
 
     return perform_decrypt(obj, registry)
 
 
 def _guess_sender_key(recipient, key: t.Union[CurveKey, KeySet]):
     if isinstance(key, KeySet):
-        header = recipient.headers()
-        skid = header.get('skid')
+        headers = recipient.headers()
+        skid = headers.get('skid')
         if skid:
             return key.get_by_kid(skid)
         return None
     return key
```

### Comparing `joserfc-0.2.0/src/joserfc/jwt.py` & `joserfc-0.3.0/src/joserfc/jwt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,27 @@
+import json
 import typing as t
 from .rfc7519.claims import Claims, convert_claims, check_sensitive_data
 from .rfc7519.registry import ClaimsOption, JWTClaimsRegistry
 from .jws import (
     JWSRegistry,
-    CompactSignature,
     serialize_compact,
-    validate_compact as validate_jws,
-    extract_compact as extract_jws,
+    deserialize_compact,
 )
 from .jwe import (
     JWERegistry,
-    CompactEncryption,
     encrypt_compact,
-    validate_compact as validate_jwe,
-    extract_compact as extract_jwe,
+    decrypt_compact,
 )
 from .jwk import KeyFlexible
 from .errors import InvalidTypeError, InvalidPayloadError
 from .util import to_bytes
 from .registry import Header
 
 __all__ = [
-    "Header",
     "Claims",
     "Token",
     "ClaimsOption",
     "JWTClaimsRegistry",
     "encode",
     "decode",
     "check_sensitive_data",
@@ -37,20 +33,19 @@
 class Token:
     """The extracted token object, which contains ``header`` and ``claims``.
 
     :param header: the header part of the JWT
     :param claims: the payload part of the JWT
     """
     def __init__(self, header: Header, claims: Claims):
+        #: header in dict
         self.header = header
+        #: payload claims in dict
         self.claims = claims
 
-    def __repr__(self):
-        return str(self.claims)
-
 
 def encode(
         header: Header,
         claims: Claims,
         key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWTRegistry] = None) -> str:
@@ -65,60 +60,44 @@
     # add ``typ`` in header
     header["typ"] = "JWT"
     payload = convert_claims(claims)
     if "enc" in header:
         result = encrypt_compact(header, payload, key, algorithms, registry)
     else:
         result = serialize_compact(header, payload, key, algorithms, registry)
-    return result.decode("utf-8")
-
-
-def extract(value: t.AnyStr) -> Token:
-    """Extract the JSON Web Token string, without validating with the key,
-    without validating the header and claims."""
-    obj = _extract_segment(value)
-    return Token(obj.headers(), obj.claims)
+    return result
 
 
 def decode(
         value: t.AnyStr,
         key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWTRegistry] = None) -> Token:
     """Decode the JSON Web Token string with the given key, and validate
-    it with the claims requests. This method is a combination of the
-    :function:`extract` and :function:`validate`.
+    it with the claims requests.
 
     :param value: text of the JWT
     :param key: key used to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a ``JWSRegistry`` or ``JWERegistry`` to use
     :raise: BadSignatureError
     """
-    obj = _extract_segment(value)
+    value = to_bytes(value)
+    if value.count(b".") == 4:
+        obj = decrypt_compact(value, key, algorithms, registry)
+        payload = obj.plaintext
+    else:
+        obj = deserialize_compact(value, key, algorithms, registry)
+        payload = obj.payload
 
-    token = Token(obj.headers(), obj.claims)
+    try:
+        claims: Claims = json.loads(payload)
+    except (TypeError, ValueError):
+        raise InvalidPayloadError()
+
+    token = Token(obj.headers(), claims)
     typ = token.header.get("typ")
     # https://www.rfc-editor.org/rfc/rfc7519#section-5.1
     # If present, it is RECOMMENDED that its value be "JWT".
     if typ and typ != "JWT":
         raise InvalidTypeError()
-
-    if isinstance(obj, CompactSignature):
-        validate_jws(obj, key, algorithms=algorithms, registry=registry)
-    else:
-        validate_jwe(obj, key, algorithms=algorithms, registry=registry)
     return token
-
-
-def _extract_segment(value: t.AnyStr) -> t.Union[CompactSignature, CompactEncryption]:
-    segment = to_bytes(value)
-    if segment.count(b".") == 4:
-        obj = extract_jwe(segment)
-    else:
-        obj = extract_jws(segment)
-
-    try:
-        assert isinstance(obj.claims, dict)
-    except (ValueError, TypeError):
-        raise InvalidPayloadError("Payload should be a JSON dict")
-    return obj
```

### Comparing `joserfc-0.2.0/src/joserfc/registry.py` & `joserfc-0.3.0/src/joserfc/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7515/compact.py` & `joserfc-0.3.0/src/joserfc/rfc7515/compact.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,7 +51,14 @@
 
 
 def verify_compact(obj: CompactSignature, alg: JWSAlgModel, key) -> bool:
     key.check_use("sig")
     signing_input = obj.segments["header"] + b"." + obj.segments["payload"]
     sig = urlsafe_b64decode(obj.segments["signature"])
     return alg.verify(signing_input, sig, key)
+
+
+def detach_compact_content(value: str) -> str:
+    # https://www.rfc-editor.org/rfc/rfc7515#appendix-F
+    parts = value.split(".")
+    parts[1] = ""
+    return ".".join(parts)
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7515/json.py` & `joserfc-0.3.0/src/joserfc/rfc7515/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 import binascii
 from .model import JWSAlgModel, HeaderMember, JSONSignature
 from .types import (
     JSONSignatureDict,
     JSONSerialization,
-    CompleteJSONSerialization,
-    FlattenJSONSerialization,
+    GeneralJSONSerialization,
+    FlattenedJSONSerialization,
 )
 from ..util import (
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
@@ -19,38 +19,41 @@
 
 
 def sign_json(obj: JSONSignature, find_alg: FindAlgorithm, find_key) -> JSONSerialization:
     signatures: t.List[JSONSignatureDict] = []
 
     payload_segment = obj.segments["payload"]
     for member in obj.members:
-        alg = find_alg(member.protected["alg"])
+        headers = member.headers()
+        alg = find_alg(headers["alg"])
         key = find_key(member)
         key.check_use("sig")
         signature = _sign_member(payload_segment, member, alg, key)
         signatures.append(signature)
 
     rv = {"payload": payload_segment.decode("utf-8")}
-    if obj.flatten and len(signatures) == 1:
+    if obj.flattened and len(signatures) == 1:
         rv.update(dict(signatures[0]))
     else:
         rv["signatures"] = signatures
 
     obj.signatures = signatures
     return rv
 
 
 def _sign_member(payload_segment, member: HeaderMember, alg: JWSAlgModel, key) -> JSONSignatureDict:
-    protected_segment = json_b64encode(member.protected)
+    if member.protected:
+        protected_segment = json_b64encode(member.protected)
+    else:
+        protected_segment = b""
     signing_input = b".".join([protected_segment, payload_segment])
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
-    rv = {
-        "protected": protected_segment.decode("utf-8"),
-        "signature": signature.decode("utf-8"),
-    }
+    rv: JSONSignatureDict = {"signature": signature.decode("utf-8")}
+    if member.protected:
+        rv["protected"] = protected_segment.decode("utf-8")
     if member.header:
         rv["header"] = member.header
     return rv
 
 
 def extract_json(value: JSONSerialization) -> JSONSignature:
     """Extract the JWS JSON Serialization from dict to object.
@@ -62,19 +65,19 @@
     try:
         payload = urlsafe_b64decode(payload_segment)
     except (TypeError, ValueError, binascii.Error):
         raise DecodeError("Invalid payload")
 
     if "signatures" in value:
         flatten = False
-        value: CompleteJSONSerialization
+        value: GeneralJSONSerialization
         signatures: t.List[JSONSignatureDict] = value["signatures"]
     else:
         flatten = True
-        value: FlattenJSONSerialization
+        value: FlattenedJSONSerialization
         _sig: JSONSignatureDict = {
             "protected": value["protected"],
             "signature": value["signature"],
         }
         if "header" in value:
             _sig["header"] = value["header"]
         signatures = [_sig]
@@ -86,15 +89,15 @@
         member = HeaderMember(protected)
         if "header" in sig:
             member.header = sig["header"]
         members.append(member)
 
     obj = JSONSignature(members, payload)
     obj.segments.update({"payload": payload_segment})
-    obj.flatten = flatten
+    obj.flattened = flatten
     obj.signatures = signatures
     return obj
 
 
 def verify_json(obj: JSONSignature, find_alg: FindAlgorithm, find_key) -> bool:
     """Verify the signature of this JSON serialization with the given
     algorithm and key.
@@ -102,20 +105,29 @@
     :param obj: instance of the SignatureData
     :param find_alg: a function to return "alg" model
     :param find_key: a function to return public key
     """
     payload_segment = obj.segments["payload"]
     for index, signature in enumerate(obj.signatures):
         member = obj.members[index]
-        alg = find_alg(member.protected["alg"])
+        headers = member.headers()
+        alg = find_alg(headers["alg"])
         key = find_key(member)
         key.check_use("sig")
         if not _verify_signature(signature, payload_segment, alg, key):
             return False
     return True
 
 
 def _verify_signature(signature: JSONSignatureDict, payload_segment, alg: JWSAlgModel, key) -> bool:
     protected_segment = signature["protected"].encode("utf-8")
     sig = urlsafe_b64decode(signature["signature"].encode("utf-8"))
     signing_input = b".".join([protected_segment, payload_segment])
     return alg.verify(signing_input, sig, key)
+
+
+def detach_json_content(value: JSONSerialization) -> JSONSerialization:
+    # https://www.rfc-editor.org/rfc/rfc7515#appendix-F
+    rv = value.copy()  # don't alter original value
+    if "payload" in rv:
+        del rv["payload"]
+    return rv
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7515/model.py` & `joserfc-0.3.0/src/joserfc/rfc7515/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,63 @@
-import json
 import typing as t
 from abc import ABCMeta, abstractmethod
-from functools import cached_property
 from .types import SegmentsDict, JSONSignatureDict
 from ..registry import Header
 
 
 class HeaderMember:
-    def __init__(self, protected: Header, header: t.Optional[Header] = None):
+    def __init__(self, protected: t.Optional[Header] = None, header: t.Optional[Header] = None):
         self.protected = protected
         self.header = header
 
     def headers(self) -> Header:
-        rv = {}
-        rv.update(self.protected)
+        rv: Header = {}
+        if self.protected:
+            rv.update(self.protected)
         if self.header:
             rv.update(self.header)
         return rv
 
     def set_kid(self, kid: str):
         if self.header is None:
             self.header = {}
         self.header["kid"] = kid
 
 
 class CompactSignature:
     """JSON Web Signature object for compact mode. This object is used to
     represent the JWS instance.
     """
-    def __init__(self, protect: Header, payload: bytes):
-        self.protect = protect
+    def __init__(self, protected: Header, payload: bytes):
+        self.protected = protected
         self.payload = payload
         self.segments: SegmentsDict = {}
 
     def headers(self) -> Header:
-        return self.protect
+        return self.protected
 
     def set_kid(self, kid: str):
-        self.protect["kid"] = kid
-
-    @cached_property
-    def claims(self) -> t.Dict[str, t.Any]:
-        return json.loads(self.payload)
+        self.protected["kid"] = kid
 
 
 class JSONSignature:
+    """JSON Web Signature object for JSON mode. This object is used to
+    represent the JWS instance.
+    """
     def __init__(self, members: t.List[HeaderMember], payload: bytes):
         self.members = members
         self.payload = payload
         self.signatures: t.List[JSONSignatureDict] = []
-        self.flatten: bool = False
+        self.flattened: bool = False
         self.segments: SegmentsDict = {}
 
     def headers(self) -> Header:
-        if self.flatten and len(self.members) == 1:
+        if self.flattened and len(self.members) == 1:
             return self.members[0].headers()
-        raise ValueError("Only compact or flatten data has .headers() method.")
+        raise ValueError("Only flattened JSON Serialization has .headers() method.")
 
 
 class JWSAlgModel(object, metaclass=ABCMeta):
     """Interface for JWS algorithm. JWA specification (RFC7518) SHOULD
     implement the algorithms for JWS with this base implementation.
     """
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7515/registry.py` & `joserfc-0.3.0/src/joserfc/rfc7515/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7515/types.py` & `joserfc-0.3.0/src/joserfc/rfc7515/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing as t
 from ..registry import Header
 
 __all__ = [
     "SegmentsDict",
     "HeaderDict",
     "JSONSignatureDict",
-    "CompleteJSONSerialization",
-    "FlattenJSONSerialization",
+    "GeneralJSONSerialization",
+    "FlattenedJSONSerialization",
     "JSONSerialization",
 ]
 
 SegmentsDict = t.TypedDict("SegmentsDict", {
     "header": bytes,
     "payload": bytes,
     "signature": bytes,
@@ -25,20 +25,20 @@
 JSONSignatureDict = t.TypedDict("JSONSignatureDict", {
     "protected": str,
     "header": Header,
     "signature": str,
 }, total=False)
 
 
-CompleteJSONSerialization = t.TypedDict("CompleteJSONSerialization", {
+GeneralJSONSerialization = t.TypedDict("GeneralJSONSerialization", {
     "payload": str,
     "signatures": t.List[JSONSignatureDict],
 })
 
-FlattenJSONSerialization = t.TypedDict("FlattenJSONSerialization", {
+FlattenedJSONSerialization = t.TypedDict("FlattenedJSONSerialization", {
     "payload": str,
     "protected": str,
     "header": Header,
     "signature": str,
 }, total=False)
 
-JSONSerialization = t.Union[CompleteJSONSerialization, FlattenJSONSerialization]
+JSONSerialization = t.Union[GeneralJSONSerialization, FlattenedJSONSerialization]
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7516/compact.py` & `joserfc-0.3.0/src/joserfc/rfc7516/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7516/json.py` & `joserfc-0.3.0/src/joserfc/rfc7516/json.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7516/message.py` & `joserfc-0.3.0/src/joserfc/rfc7516/message.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7516/models.py` & `joserfc-0.3.0/src/joserfc/rfc7516/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.recipient: t.Optional[Recipient] = None
         self.bytes_segments: t.Dict[str, bytes] = {}  # store the decoded segments
         self.base64_segments: t.Dict[str, bytes] = {}  # store the encoded segments
 
     def headers(self):
         return self.protected
 
-    def add_recipient(self, key: Key, header: t.Optional[Header] = None):
+    def attach_recipient(self, key: Key, header: t.Optional[Header] = None):
         """Add a recipient to the JWE Compact Serialization. Please add a key that
         comply with the given "alg" value.
 
         :param key: an instance of a key, e.g. (OctKey, RSAKey, ECKey, and etc)
         :param header: extra header in dict
         """
         recipient = Recipient(self, None, key)
@@ -72,55 +72,65 @@
 
     @property
     def recipients(self) -> t.List[Recipient]:
         return [self.recipient]
 
 
 class JSONEncryption:
-    """An object to represent the JWE JSON Serialization. It is usually returned by
-    ``decrypt_json`` method.
+    """An object to represent the JWE JSON Serialization. It is used by
+    ``encrypt_json``, and it is usually returned by ``decrypt_json`` method.
+
+    To construct an object of ``JSONEncryption``:
+
+    .. code-block:: python
+
+        protected = {"enc": "A128CBC-HS256"}
+        plaintext = b"hello world"
+        obj = JSONEncryption(protected, plaintext)
+        # then add each recipient
+        obj.add_recipient({"alg": "A128KW"})
     """
     def __init__(
             self,
             protected: Header,
             plaintext: t.Optional[bytes] = None,
             unprotected: t.Optional[Header] = None,
             aad: t.Optional[bytes] = None,
             flatten: bool=False):
         #: protected header in dict
-        self.protected = protected
+        self.protected: Header = protected
         #: the plaintext in bytes
-        self.plaintext = plaintext
+        self.plaintext: bytes = plaintext
         #: unprotected header in dict
-        self.unprotected = unprotected
+        self.unprotected: t.Optional[Header] = unprotected
         #: an optional additional authenticated data
         self.aad: t.Optional[bytes] = aad
         #: represents if the object is in flatten syntax
         self.flatten: bool = flatten
         #: a list of recipients
         self.recipients: t.List[Recipient] = []
 
         self.bytes_segments: t.Dict[str, bytes] = {}  # store the decoded segments
         self.base64_segments: t.Dict[str, bytes] = {}  # store the encoded segments
 
-    def add_recipient(self, key: Key, header: t.Optional[Header] = None):
+    def add_recipient(self, header: t.Optional[Header] = None, key: t.Optional[Key] = None):
         """Add a recipient to the JWE JSON Serialization. Please add a key that
         comply with the "alg" to this recipient.
 
-        :param key: an instance of a key, e.g. (OctKey, RSAKey, ECKey, and etc)
         :param header: recipient's own (unprotected) header
+        :param key: an instance of a key, e.g. (OctKey, RSAKey, ECKey, and etc)
         """
         recipient = Recipient(self, header, key)
         self.recipients.append(recipient)
 
 
 class JWEEncModel(object, metaclass=ABCMeta):
     name: str
     description: str
-    recommended: bool = True
+    recommended: bool = False
     algorithm_type = "JWE"
     algorithm_location = "enc"
 
     iv_size: int
     cek_size: int
 
     def generate_cek(self) -> bytes:
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7516/registry.py` & `joserfc-0.3.0/src/joserfc/rfc7516/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,20 @@
         cls.algorithms[location][model.name] = model
         if model.recommended:
             cls.recommended.append(model.name)
 
     def check_header(self, header: Header, check_more=False):
         check_crit_header(header)
         check_registry_header(self.header_registry, header)
-        if check_more:
-            alg = self.get_alg(header["alg"])
-            if alg.more_header_registry:
+
+        alg = self.get_alg(header["alg"])
+        if alg.more_header_registry:
+            if check_more:
                 check_registry_header(alg.more_header_registry, header)
+
             if self.strict_check_header:
                 allowed_registry = self.header_registry.copy()
                 allowed_registry.update(alg.more_header_registry)
                 check_supported_header(allowed_registry, header)
         elif self.strict_check_header:
             check_supported_header(self.header_registry, header)
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7516/types.py` & `joserfc-0.3.0/src/joserfc/rfc7516/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7517/models.py` & `joserfc-0.3.0/src/joserfc/rfc7517/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,28 +164,38 @@
             if k in self.value_registry and self.value_registry[k].private:
                 del data[k]
 
         data.update(params)
         return data
 
     def check_use(self, use: str):
+        """Check if this key supports the given "use".
+
+        :param use: this key is used for, e.g. "sig", "enc"
+        :raise: UnsupportedKeyUseError
+        """
         designed_use = self.get("use")
         if designed_use and designed_use != use:
             raise UnsupportedKeyUseError(f'This key is designed to be used for "{designed_use}"')
 
     def check_alg(self, alg: str):
+        """Check if this key supports the given "alg".
+
+        :param alg: the algorithm this key is intended to be used, e.g. "HS256", "ECDH-EC"
+        :raise: UnsupportedKeyAlgorithmError
+        """
         designed_alg = self.get("alg")
         if designed_alg and designed_alg != alg:
             raise UnsupportedKeyAlgorithmError(f'This key is designed for algorithm "{designed_alg}"')
 
     def check_key_op(self, operation: str):
         """Check if the given key_op is supported by this key.
 
         :param operation: key operation value, such as "sign", "encrypt".
-        :raise: ValueError
+        :raise: UnsupportedKeyOperationError
         """
         key_ops = self.get("key_ops")
         if key_ops is not None and operation not in key_ops:
             raise UnsupportedKeyOperationError(f'Unsupported key_op "{operation}"')
 
         assert operation in self.operation_registry
         reg = self.operation_registry[operation]
@@ -219,26 +229,30 @@
     def generate_key(cls, size_or_crv, options: KeyOptions = None, private: bool = True) -> "BaseKey":
         raise NotImplementedError()
 
 
 class SymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
     @property
     def raw_value(self) -> bytes:
+        """The raw key in bytes."""
         return self._raw_value
 
     @property
     def is_private(self) -> bool:
+        """A symmetric key will always be private."""
         return True
 
     @property
     def public_key(self) -> bytes:
+        """Returns the ``raw_value`` as the public key."""
         return self.raw_value
 
     @property
     def private_key(self) -> bytes:
+        """Returns the ``raw_value`` as the private key."""
         return self.raw_value
 
 
 class AsymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
     @property
     def raw_value(self) -> t.Union[NativePublicKey, NativePrivateKey]:
         return self._raw_value
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7517/pem.py` & `joserfc-0.3.0/src/joserfc/rfc7517/pem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,67 @@
+import typing as t
 from abc import ABCMeta, abstractmethod
-
 from cryptography.x509 import load_pem_x509_certificate
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
     load_pem_public_key,
     load_ssh_public_key,
+    load_ssh_private_key,
     Encoding,
     PrivateFormat,
     PublicFormat,
     BestAvailableEncryption,
     NoEncryption,
 )
 from cryptography.hazmat.backends import default_backend
 from .models import NativeKeyBinding
 from .types import KeyDict
 from ..util import to_bytes
 
 
-def load_pem_key(raw: bytes, ssh_type=None, key_type=None, password=None):
+def load_pem_key(
+        raw: bytes,
+        ssh_type: t.Optional[bytes]=None,
+        key_type: t.Optional[str]=None,
+        password: t.Optional[bytes]=None):
     if ssh_type and raw.startswith(ssh_type):
         return load_ssh_public_key(raw, backend=default_backend())
 
     if key_type == "public":
         return load_pem_public_key(raw, backend=default_backend())
 
     if key_type == "private" or password is not None:
-        return load_pem_private_key(raw, password=password, backend=default_backend())
+        return __load_private_key(raw, password=password)
 
     if b"PUBLIC" in raw:
         return load_pem_public_key(raw, backend=default_backend())
 
+    if b"OPENSSH PRIVATE" in raw:
+        return load_ssh_private_key(raw, password=password, backend=default_backend())
+
     if b"PRIVATE" in raw:
-        return load_pem_private_key(raw, password=password, backend=default_backend())
+        return __load_private_key(raw, password=password)
 
     if b"CERTIFICATE" in raw:
         cert = load_pem_x509_certificate(raw, default_backend())
         return cert.public_key()
 
     try:
-        return load_pem_private_key(raw, password=password, backend=default_backend())
+        return __load_private_key(raw, password=password)
     except ValueError:
         return load_pem_public_key(raw, backend=default_backend())
 
 
+def __load_private_key(raw: bytes, password: t.Optional[bytes]=None):
+    try:
+        return load_pem_private_key(raw, password=password, backend=default_backend())
+    except ValueError:
+        return load_ssh_private_key(raw, password=password, backend=default_backend())
+
+
 def dump_pem_key(key, encoding=None, private=False, password=None) -> bytes:
     """Export key into PEM/DER format bytes.
 
     :param key: native cryptography key
     :param encoding: "PEM" or "DER"
     :param private: export private key or public key
     :param password: encrypt private key with password
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7517/types.py` & `joserfc-0.3.0/src/joserfc/rfc7517/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/derive_key.py` & `joserfc-0.3.0/src/joserfc/rfc7518/derive_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/ec_key.py` & `joserfc-0.3.0/src/joserfc/rfc7518/ec_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/jwe_algs.py` & `joserfc-0.3.0/src/joserfc/rfc7518/jwe_algs.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,26 +193,26 @@
         self.key_wrapping = key_wrapping
 
     def encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient):
         recipient_key: CurveKey = recipient.recipient_key
         ephemeral_key: CurveKey = recipient.ephemeral_key
         pubkey = recipient_key.get_op_key("deriveKey")
         shared_key = ephemeral_key.exchange_shared_key(pubkey)
-        header = recipient.headers()
-        return derive_key_for_concat_kdf(shared_key, header, enc.cek_size, self.key_size)
+        headers = recipient.headers()
+        return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size)
 
     def decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
-        header = recipient.headers()
-        assert "epk" in header
+        headers = recipient.headers()
+        assert "epk" in headers
 
         recipient_key: CurveKey = self.check_recipient_key(recipient.recipient_key)
-        epk = recipient_key.import_key(header["epk"])
+        epk = recipient_key.import_key(headers["epk"])
         pubkey = epk.get_op_key("deriveKey")
         shared_key = recipient_key.exchange_shared_key(pubkey)
-        return derive_key_for_concat_kdf(shared_key, header, enc.cek_size, self.key_size)
+        return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size)
 
 
 class PBES2HSAlgModel(JWEKeyEncryption):
     # https://www.rfc-editor.org/rfc/rfc7518#section-4.8
     more_header_registry = {
         "p2s": HeaderParameter("PBES2 Salt Input", "str", True),
         "p2c": HeaderParameter("PBES2 Count", "int", True),
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/jwe_encs.py` & `joserfc-0.3.0/src/joserfc/rfc7518/jwe_encs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .util import encode_int
 
 
 class CBCHS2EncModel(JWEEncModel):
     # The IV used is a 128-bit value generated randomly or
     # pseudo-randomly for use in the cipher.
     iv_size = 128
+    recommended = True
 
     def __init__(self, key_size: int, hash_type: int):
         self.name = f"A{key_size}CBC-HS{hash_type}"
         self.description = (
             f"AES_{key_size}_CBC_HMAC_SHA_{hash_type} authenticated encryption algorithm"
         )
 
@@ -73,14 +74,15 @@
         return unpad.update(data) + unpad.finalize()
 
 
 class GCMEncModel(JWEEncModel):
     # Use of an IV of size 96 bits is REQUIRED with this algorithm.
     # https://tools.ietf.org/html/rfc7518#section-5.3
     iv_size = 96
+    recommended = True
 
     def __init__(self, key_size: int):
         self.name = f"A{key_size}GCM"
         self.description = f"AES GCM using {key_size}-bit key"
         self.key_size = key_size
         self.cek_size = key_size
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/jwe_zips.py` & `joserfc-0.3.0/src/joserfc/rfc7518/jwe_zips.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/jws_algs.py` & `joserfc-0.3.0/src/joserfc/rfc7518/jws_algs.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,21 +73,21 @@
     - RS384: RSASSA-PKCS1-v1_5 using SHA-384
     - RS512: RSASSA-PKCS1-v1_5 using SHA-512
     """
 
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
+    padding = padding.PKCS1v15()
 
     def __init__(self, sha_type: int, recommended: bool = False):
         self.name = f"RS{sha_type}"
         self.description = f"RSASSA-PKCS1-v1_5 using SHA-{sha_type}"
         self.recommended = recommended
         self.hash_alg = getattr(self, f"SHA{sha_type}")
-        self.padding = padding.PKCS1v15()
 
     def sign(self, msg: bytes, key: RSAKey) -> bytes:
         op_key = key.get_op_key("sign")
         return op_key.sign(msg, self.padding, self.hash_alg())
 
     def verify(self, msg: bytes, sig: bytes, key: RSAKey) -> bool:
         op_key = key.get_op_key("verify")
@@ -162,25 +162,24 @@
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
 
     def __init__(self, sha_type: int):
         self.name = f"PS{sha_type}"
         self.description = f"RSASSA-PSS using SHA-{sha_type} and MGF1 with SHA-{sha_type}"
         self.hash_alg = getattr(self, f"SHA{sha_type}")
+        self.padding = padding.PSS(mgf=padding.MGF1(self.hash_alg()), salt_length=self.hash_alg.digest_size)
 
     def sign(self, msg: bytes, key: RSAKey) -> bytes:
         op_key = key.get_op_key("sign")
-        pad = padding.PSS(mgf=padding.MGF1(self.hash_alg()), salt_length=self.hash_alg.digest_size)
-        return op_key.sign(msg, pad, self.hash_alg())
+        return op_key.sign(msg, self.padding, self.hash_alg())
 
     def verify(self, msg: bytes, sig: bytes, key: RSAKey) -> bool:
         op_key = key.get_op_key("verify")
-        pad = padding.PSS(mgf=padding.MGF1(self.hash_alg()), salt_length=self.hash_alg.digest_size)
         try:
-            op_key.verify(sig, msg, pad, self.hash_alg())
+            op_key.verify(sig, msg, self.padding, self.hash_alg())
             return True
         except InvalidSignature:
             return False
 
 
 JWS_ALGORITHMS = [
     NoneAlgModel(),  # none
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/oct_key.py` & `joserfc-0.3.0/src/joserfc/rfc7518/oct_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,22 +33,30 @@
         # security check
         if value.startswith(POSSIBLE_UNSAFE_KEYS):
             raise ValueError("This key may not be safe to import")
         return value
 
 
 class OctKey(SymmetricKey[bytes, bytes]):
+    """OctKey is a symmetric key, defined by RFC7518 Section 6.4.
+    """
     key_type: str = "oct"
     binding = OctBinding
+
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.4
     value_registry = {"k": KeyParameter("Key Value", "str", True, True)}
 
     @classmethod
     def generate_key(cls, key_size=256, options: KeyOptions = None, private: bool = True) -> "OctKey":
-        """Generate a ``OctKey`` with the given bit size."""
+        """Generate a ``OctKey`` with the given bit size (not bytes).
+
+        :param key_size: size in bit
+        :param options: extra parameter in JWK
+        :param private: must be True
+        """
         if not private:
             raise ValueError("oct key can not be generated as public")
 
         if key_size % 8 != 0:
             raise ValueError("Invalid bit size for oct key")
 
         length = key_size // 8
```

### Comparing `joserfc-0.2.0/src/joserfc/rfc7518/rsa_key.py` & `joserfc-0.3.0/src/joserfc/rfc7518/rsa_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7519/claims.py` & `joserfc-0.3.0/src/joserfc/rfc7519/claims.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc7519/registry.py` & `joserfc-0.3.0/src/joserfc/rfc7519/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc8037/jws_eddsa.py` & `joserfc-0.3.0/src/joserfc/rfc8037/jws_eddsa.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/rfc8037/okp_key.py` & `joserfc-0.3.0/src/joserfc/rfc8037/okp_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.2.0/src/joserfc/util.py` & `joserfc-0.3.0/src/joserfc/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import base64
-import string
 import struct
 import json
-import random
 
 
 def to_bytes(x, charset="utf-8", errors="strict"):
     if isinstance(x, bytes):
         return x
     if isinstance(x, str):
         return x.encode(charset, errors)
@@ -52,13 +50,7 @@
     if isinstance(text, dict):
         text = json_dumps(text)
     return urlsafe_b64encode(to_bytes(text, charset))
 
 
 def json_b64decode(text, charset="utf-8") -> dict:
     return json.loads(urlsafe_b64decode(to_bytes(text, charset)))
-
-
-def generate_token(length=30):
-    rand = random.SystemRandom()
-    chars = string.ascii_letters + string.digits
-    return "".join(rand.choice(chars) for _ in range(length))
```

### Comparing `joserfc-0.2.0/src/joserfc.egg-info/PKG-INFO` & `joserfc-0.3.0/src/joserfc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.2.0
+Version: 0.3.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `joserfc-0.2.0/src/joserfc.egg-info/SOURCES.txt` & `joserfc-0.3.0/src/joserfc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,17 @@
 src/joserfc/rfc7516/compact.py
 src/joserfc/rfc7516/json.py
 src/joserfc/rfc7516/message.py
 src/joserfc/rfc7516/models.py
 src/joserfc/rfc7516/registry.py
 src/joserfc/rfc7516/types.py
 src/joserfc/rfc7517/__init__.py
-src/joserfc/rfc7517/keygen.py
-src/joserfc/rfc7517/keyset.py
 src/joserfc/rfc7517/models.py
 src/joserfc/rfc7517/pem.py
+src/joserfc/rfc7517/registry.py
 src/joserfc/rfc7517/types.py
 src/joserfc/rfc7518/__init__.py
 src/joserfc/rfc7518/derive_key.py
 src/joserfc/rfc7518/ec_key.py
 src/joserfc/rfc7518/jwe_algs.py
 src/joserfc/rfc7518/jwe_encs.py
 src/joserfc/rfc7518/jwe_zips.py
```

