# Comparing `tmp/gyver-2.3.0.tar.gz` & `tmp/gyver-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-2.3.0.tar", max compression
+gzip compressed data, was "gyver-2.3.1.tar", max compression
```

## Comparing `gyver-2.3.0.tar` & `gyver-2.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.3.0/LICENSE
--rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.3.0/README.md
--rw-r--r--   0        0        0      158 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/__init__.py
--rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/__init__.py
--rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/asyncio.py
--rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/config.py
--rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/interface.py
--rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/mapper.py
--rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/mock.py
--rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/redis.py
--rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/sync.py
--rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/utils.py
--rw-r--r--   0        0        0      597 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     5940 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0     3459 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/config.py
--rw-r--r--   0        0        0     2690 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/envconfig.py
--rw-r--r--   0        0        0     1016 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/interface.py
--rw-r--r--   0        0        0     5534 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/lazy.py
--rw-r--r--   0        0        0      627 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/typedef.py
--rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/utils.py
--rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/context.py
--rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/typedef.py
--rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/__init__.py
--rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/config.py
--rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/fernet.py
--rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/rsa.py
--rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/database/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/database/adapter.py
--rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/config.py
--rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/context/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/context/asyncio.py
--rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/context/sync.py
--rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/__init__.py
--rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/dialect.py
--rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/interface.py
--rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/utils.py
--rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/entity.py
--rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/entity.pyi
--rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/metadata.py
--rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/query/__init__.py
--rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/query/_helpers.py
--rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/comp.py
--rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/exc.py
--rw-r--r--   0        0        0     1353 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/interface.py
--rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/null.py
--rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/order_by.py
--rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/paginate.py
--rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/utils.py
--rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/where.py
--rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/typedef.py
--rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/utils.py
--rw-r--r--   0        0        0     2272 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/exc.py
--rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.3.0/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3107 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2503 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2808 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/model.py
--rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/py.typed
--rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/url/__init__.py
--rw-r--r--   0        0        0     4663 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/core.py
--rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/url/encode.py
--rw-r--r--   0        0        0     1285 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/fragment.py
--rw-r--r--   0        0        0     5566 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/netloc.py
--rw-r--r--   0        0        0     4307 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/path.py
--rw-r--r--   0        0        0     3592 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/query.py
--rw-r--r--   0        0        0     1186 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/utils.py
--rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/__init__.py
--rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/exc.py
--rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/finder.py
--rw-r--r--   0        0        0     4262 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/utils/helpers.py
--rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/json.py
--rw-r--r--   0        0        0     2574 2023-06-27 06:41:36.154386 gyver-2.3.0/gyver/utils/lazy.py
--rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/singleton.py
--rw-r--r--   0        0        0     2224 2023-06-27 06:41:36.154386 gyver-2.3.0/gyver/utils/strings.py
--rw-r--r--   0        0        0      134 2023-06-27 06:41:36.154386 gyver-2.3.0/gyver/utils/timezone.py
--rw-r--r--   0        0        0     2449 2023-06-27 06:41:36.154386 gyver-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 gyver-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.3.1/LICENSE
+-rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.3.1/README.md
+-rw-r--r--   0        0        0      158 2023-06-29 12:54:08.234272 gyver-2.3.1/gyver/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/__init__.py
+-rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/asyncio.py
+-rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/config.py
+-rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/interface.py
+-rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/mapper.py
+-rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/mock.py
+-rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/redis.py
+-rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/sync.py
+-rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/cache/utils.py
+-rw-r--r--   0        0        0      597 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.3.1/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     5940 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0     3459 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/config.py
+-rw-r--r--   0        0        0     2690 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/envconfig.py
+-rw-r--r--   0        0        0     1016 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/interface.py
+-rw-r--r--   0        0        0     5534 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/lazy.py
+-rw-r--r--   0        0        0      627 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/config/typedef.py
+-rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/config/utils.py
+-rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.3.1/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/context/typedef.py
+-rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/crypto/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/crypto/config.py
+-rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/crypto/fernet.py
+-rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/crypto/rsa.py
+-rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/database/__init__.py
+-rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.3.1/gyver/database/adapter.py
+-rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/config.py
+-rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/context/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/context/asyncio.py
+-rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/context/sync.py
+-rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/drivers/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/drivers/dialect.py
+-rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/drivers/interface.py
+-rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/drivers/utils.py
+-rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/entity.py
+-rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/entity.pyi
+-rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/metadata.py
+-rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/query/__init__.py
+-rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.3.1/gyver/database/query/_helpers.py
+-rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/comp.py
+-rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/exc.py
+-rw-r--r--   0        0        0     1353 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/interface.py
+-rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/null.py
+-rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/order_by.py
+-rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/paginate.py
+-rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/utils.py
+-rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/query/where.py
+-rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/typedef.py
+-rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/database/utils.py
+-rw-r--r--   0        0        0     2272 2023-06-27 06:41:36.152386 gyver-2.3.1/gyver/exc.py
+-rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.3.1/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3107 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2503 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.3.1/gyver/model.py
+-rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/py.typed
+-rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/url/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.3.1/gyver/url/encode.py
+-rw-r--r--   0        0        0     1285 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5566 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4307 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/url/path.py
+-rw-r--r--   0        0        0     3592 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/url/utils.py
+-rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.3.1/gyver/utils/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.3.1/gyver/utils/exc.py
+-rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.3.1/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4262 2023-06-27 06:41:36.153386 gyver-2.3.1/gyver/utils/helpers.py
+-rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.3.1/gyver/utils/json.py
+-rw-r--r--   0        0        0     2574 2023-06-27 06:41:36.154386 gyver-2.3.1/gyver/utils/lazy.py
+-rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.3.1/gyver/utils/singleton.py
+-rw-r--r--   0        0        0     2224 2023-06-27 06:41:36.154386 gyver-2.3.1/gyver/utils/strings.py
+-rw-r--r--   0        0        0      134 2023-06-27 06:41:36.154386 gyver-2.3.1/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     2456 2023-06-29 12:54:08.232272 gyver-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 gyver-2.3.1/PKG-INFO
```

### Comparing `gyver-2.3.0/LICENSE` & `gyver-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/README.md` & `gyver-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/asyncio.py` & `gyver-2.3.1/gyver/cache/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/interface.py` & `gyver-2.3.1/gyver/cache/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/mapper.py` & `gyver-2.3.1/gyver/cache/mapper.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/mock.py` & `gyver-2.3.1/gyver/cache/mock.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/redis.py` & `gyver-2.3.1/gyver/cache/redis.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/sync.py` & `gyver-2.3.1/gyver/cache/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/cache/utils.py` & `gyver-2.3.1/gyver/cache/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/__init__.py` & `gyver-2.3.1/gyver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/attrs.py` & `gyver-2.3.1/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/dataclass.py` & `gyver-2.3.1/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/factory.py` & `gyver-2.3.1/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/gattrs.py` & `gyver-2.3.1/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/interface.py` & `gyver-2.3.1/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/mark.py` & `gyver-2.3.1/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/adapter/pydantic.py` & `gyver-2.3.1/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/config.py` & `gyver-2.3.1/gyver/config/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/envconfig.py` & `gyver-2.3.1/gyver/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/interface.py` & `gyver-2.3.1/gyver/config/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/lazy.py` & `gyver-2.3.1/gyver/config/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/config/typedef.py` & `gyver-2.3.1/gyver/config/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/context/atomic_/bound.py` & `gyver-2.3.1/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/context/atomic_/core.py` & `gyver-2.3.1/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/context/atomic_/resolver.py` & `gyver-2.3.1/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/context/context.py` & `gyver-2.3.1/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/context/interfaces/adapter.py` & `gyver-2.3.1/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/crypto/fernet.py` & `gyver-2.3.1/gyver/crypto/fernet.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/crypto/rsa.py` & `gyver-2.3.1/gyver/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/__init__.py` & `gyver-2.3.1/gyver/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/adapter.py` & `gyver-2.3.1/gyver/database/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/config.py` & `gyver-2.3.1/gyver/database/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/context/asyncio.py` & `gyver-2.3.1/gyver/database/context/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/context/sync.py` & `gyver-2.3.1/gyver/database/context/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/drivers/utils.py` & `gyver-2.3.1/gyver/database/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/entity.py` & `gyver-2.3.1/gyver/database/entity.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/__init__.py` & `gyver-2.3.1/gyver/database/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/_helpers.py` & `gyver-2.3.1/gyver/database/query/_helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/comp.py` & `gyver-2.3.1/gyver/database/query/comp.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/interface.py` & `gyver-2.3.1/gyver/database/query/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/order_by.py` & `gyver-2.3.1/gyver/database/query/order_by.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/paginate.py` & `gyver-2.3.1/gyver/database/query/paginate.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/utils.py` & `gyver-2.3.1/gyver/database/query/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/query/where.py` & `gyver-2.3.1/gyver/database/query/where.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/database/utils.py` & `gyver-2.3.1/gyver/database/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/exc.py` & `gyver-2.3.1/gyver/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/filetree/filetree.py` & `gyver-2.3.1/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/filetree/interface.py` & `gyver-2.3.1/gyver/filetree/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/filetree/typedef.py` & `gyver-2.3.1/gyver/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/filetree/virtual.py` & `gyver-2.3.1/gyver/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/model.py` & `gyver-2.3.1/gyver/model.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/pools/asyncio.py` & `gyver-2.3.1/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/pools/resource.py` & `gyver-2.3.1/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/pools/thread.py` & `gyver-2.3.1/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/url/core.py` & `gyver-2.3.1/gyver/url/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/url/fragment.py` & `gyver-2.3.1/gyver/url/fragment.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/url/netloc.py` & `gyver-2.3.1/gyver/url/netloc.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/url/path.py` & `gyver-2.3.1/gyver/url/path.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/url/query.py` & `gyver-2.3.1/gyver/url/query.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/url/utils.py` & `gyver-2.3.1/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/utils/__init__.py` & `gyver-2.3.1/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/utils/finder.py` & `gyver-2.3.1/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/utils/helpers.py` & `gyver-2.3.1/gyver/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/utils/lazy.py` & `gyver-2.3.1/gyver/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/utils/singleton.py` & `gyver-2.3.1/gyver/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/gyver/utils/strings.py` & `gyver-2.3.1/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.0/pyproject.toml` & `gyver-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "2.3.0"
+version = "2.3.1"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -17,15 +17,15 @@
 pymysql = { version = "^1.0.2", optional = true }
 aiosqlite = { version = "^0.18.0", optional = true }
 tzdata = { markers = "sys_platform != \"linux\"", version = "^2022.6" }
 sqlalchemy = { version = "^2.0.4", optional = true }
 cryptography = "^41.0.0"
 redis = { version = "^4.5.5", optional = true }
 gyver-attrs = "^0.5.2"
-cchardet = "^2.1.7"
+faust-cchardet = "^2.1.18"
 
 [tool.poetry.group.lint.dependencies]
 black = "^22.10.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 autoflake = "^1.7.7"
```

### Comparing `gyver-2.3.0/PKG-INFO` & `gyver-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 2.3.0
+Version: 2.3.1
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,16 +14,16 @@
 Provides-Extra: db-mariadb
 Provides-Extra: db-mysql
 Provides-Extra: db-pg
 Provides-Extra: db-sqlite
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0) ; extra == "db-mysql" or extra == "db-mariadb"
 Requires-Dist: aiosqlite (>=0.18.0,<0.19.0) ; extra == "db-sqlite"
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "db-pg"
-Requires-Dist: cchardet (>=2.1.7,<3.0.0)
 Requires-Dist: cryptography (>=41.0.0,<42.0.0)
+Requires-Dist: faust-cchardet (>=2.1.18,<3.0.0)
 Requires-Dist: gyver-attrs (>=0.5.2,<0.6.0)
 Requires-Dist: orjson (>=3.8.1,<4.0.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "db-pg"
 Requires-Dist: pydantic[email] (>=1.10.2,<2.0.0)
 Requires-Dist: pymysql (>=1.0.2,<2.0.0) ; extra == "db-mysql" or extra == "db-mariadb"
 Requires-Dist: redis (>=4.5.5,<5.0.0) ; extra == "cache"
 Requires-Dist: sqlalchemy (>=2.0.4,<3.0.0) ; extra == "db-mysql" or extra == "db-mariadb" or extra == "db-pg" or extra == "db-sqlite"
```

