# Comparing `tmp/neo4j-5.8.1.tar.gz` & `tmp/neo4j-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j-5.8.1.tar", last modified: Wed May 17 11:00:24 2023, max compression
+gzip compressed data, was "neo4j-5.9.0.tar", last modified: Fri May 26 10:29:56 2023, max compression
```

## Comparing `neo4j-5.8.1.tar` & `neo4j-5.9.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.630422 neo4j-5.8.1/
--rw-r--r--   0 root         (0) root         (0)    11360 2023-05-17 10:59:04.000000 neo4j-5.8.1/LICENSE.APACHE2.txt
--rw-r--r--   0 root         (0) root         (0)     2762 2023-05-17 10:59:04.000000 neo4j-5.8.1/LICENSE.PYTHON.txt
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-17 10:59:04.000000 neo4j-5.8.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-17 10:59:04.000000 neo4j-5.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-17 10:59:04.000000 neo4j-5.8.1/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     5946 2023-05-17 11:00:24.630422 neo4j-5.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5035 2023-05-17 10:59:04.000000 neo4j-5.8.1/README.rst
--rw-r--r--   0 root         (0) root         (0)     2905 2023-05-17 11:00:24.000000 neo4j-5.8.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 11:00:24.630422 neo4j-5.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2442 2023-05-17 10:59:04.000000 neo4j-5.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.610422 neo4j-5.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.618422 neo4j-5.8.1/src/neo4j/
--rw-r--r--   0 root         (0) root         (0)     4635 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6648 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.618422 neo4j-5.8.1/src/neo4j/_async/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6561 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/auth_management.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/bookmark_manager.py
--rw-r--r--   0 root         (0) root         (0)    50031 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_async/io/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35983 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/_bolt.py
--rw-r--r--   0 root         (0) root         (0)    16740 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/_bolt3.py
--rw-r--r--   0 root         (0) root         (0)    23378 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/_bolt4.py
--rw-r--r--   0 root         (0) root         (0)    24676 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/_bolt5.py
--rw-r--r--   0 root         (0) root         (0)    10670 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/_common.py
--rw-r--r--   0 root         (0) root         (0)    38631 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/io/_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_async/work/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27782 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/work/result.py
--rw-r--r--   0 root         (0) root         (0)    27600 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/work/session.py
--rw-r--r--   0 root         (0) root         (0)    11289 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/work/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7448 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async/work/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_async_compat/
--rw-r--r--   0 root         (0) root         (0)      755 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14870 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_async_compat/network/
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/network/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25841 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/network/_bolt_socket.py
--rw-r--r--   0 root         (0) root         (0)     6223 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/network/_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_async_compat/shims/
--rw-r--r--   0 root         (0) root         (0)     4939 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/shims/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_async_compat/util.py
--rw-r--r--   0 root         (0) root         (0)     4628 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_auth_management.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_codec/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_codec/hydration/
--rw-r--r--   0 root         (0) root         (0)      898 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.622422 neo4j-5.8.1/src/neo4j/_codec/hydration/_interface/
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/_interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_codec/hydration/v1/
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v1/hydration_handler.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v1/spatial.py
--rw-r--r--   0 root         (0) root         (0)     8870 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v1/temporal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_codec/hydration/v2/
--rw-r--r--   0 root         (0) root         (0)      730 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v2/hydration_handler.py
--rw-r--r--   0 root         (0) root         (0)     5002 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/hydration/v2/temporal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_codec/packstream/
--rw-r--r--   0 root         (0) root         (0)      707 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/packstream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/packstream/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_codec/packstream/v1/
--rw-r--r--   0 root         (0) root         (0)    16696 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_codec/packstream/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18295 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_conf.py
--rw-r--r--   0 root         (0) root         (0)    11673 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_data.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_deadline.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5539 2023-05-17 11:00:23.000000 neo4j-5.8.1/src/neo4j/_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_optional_deps/
--rw-r--r--   0 root         (0) root         (0)      261 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_optional_deps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_spatial/
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_spatial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_sync/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6377 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/auth_management.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/bookmark_manager.py
--rw-r--r--   0 root         (0) root         (0)    49135 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_sync/io/
--rw-r--r--   0 root         (0) root         (0)     1190 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35506 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/_bolt.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/_bolt3.py
--rw-r--r--   0 root         (0) root         (0)    23173 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/_bolt4.py
--rw-r--r--   0 root         (0) root         (0)    24509 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/_bolt5.py
--rw-r--r--   0 root         (0) root         (0)    10393 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/_common.py
--rw-r--r--   0 root         (0) root         (0)    37987 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/io/_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.626422 neo4j-5.8.1/src/neo4j/_sync/work/
--rw-r--r--   0 root         (0) root         (0)      988 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27291 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/work/result.py
--rw-r--r--   0 root         (0) root         (0)    26864 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/work/session.py
--rw-r--r--   0 root         (0) root         (0)    10873 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/work/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_sync/work/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.630422 neo4j-5.8.1/src/neo4j/_work/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_work/eager_result.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_work/query.py
--rw-r--r--   0 root         (0) root         (0)    10365 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/_work/summary.py
--rw-r--r--   0 root         (0) root         (0)    10985 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/addressing.py
--rw-r--r--   0 root         (0) root         (0)    18240 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/api.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/auth_management.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/conf.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/data.py
--rw-r--r--   0 root         (0) root         (0)     7802 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/debug.py
--rw-r--r--   0 root         (0) root         (0)    17262 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.630422 neo4j-5.8.1/src/neo4j/graph/
--rw-r--r--   0 root         (0) root         (0)    11098 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/meta.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/packstream.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/py.typed
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.630422 neo4j-5.8.1/src/neo4j/spatial/
--rw-r--r--   0 root         (0) root         (0)     2081 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/spatial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.630422 neo4j-5.8.1/src/neo4j/time/
--rw-r--r--   0 root         (0) root         (0)    95454 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/_arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/_clock_implementations.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/_metaclasses.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/clock_implementations.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/hydration.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/time/metaclasses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.630422 neo4j-5.8.1/src/neo4j/work/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/work/query.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-17 10:59:04.000000 neo4j-5.8.1/src/neo4j/work/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:24.618422 neo4j-5.8.1/src/neo4j.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5946 2023-05-17 11:00:24.000000 neo4j-5.8.1/src/neo4j.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3175 2023-05-17 11:00:24.000000 neo4j-5.8.1/src/neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 11:00:24.000000 neo4j-5.8.1/src/neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-17 11:00:24.000000 neo4j-5.8.1/src/neo4j.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-17 11:00:24.000000 neo4j-5.8.1/src/neo4j.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.508140 neo4j-5.9.0/
+-rw-r--r--   0 root         (0) root         (0)    11360 2023-05-26 10:28:11.000000 neo4j-5.9.0/LICENSE.APACHE2.txt
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-05-26 10:28:11.000000 neo4j-5.9.0/LICENSE.PYTHON.txt
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-26 10:28:11.000000 neo4j-5.9.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-26 10:28:11.000000 neo4j-5.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-26 10:28:11.000000 neo4j-5.9.0/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-05-26 10:29:56.508140 neo4j-5.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-05-26 10:28:11.000000 neo4j-5.9.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-05-26 10:29:56.000000 neo4j-5.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 10:29:56.508140 neo4j-5.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-05-26 10:28:11.000000 neo4j-5.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.488140 neo4j-5.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.496140 neo4j-5.9.0/src/neo4j/
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6648 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.496140 neo4j-5.9.0/src/neo4j/_async/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6334 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/bookmark_manager.py
+-rw-r--r--   0 root         (0) root         (0)    50031 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.496140 neo4j-5.9.0/src/neo4j/_async/io/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36179 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/_bolt.py
+-rw-r--r--   0 root         (0) root         (0)    16740 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/_bolt3.py
+-rw-r--r--   0 root         (0) root         (0)    23378 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/_bolt4.py
+-rw-r--r--   0 root         (0) root         (0)    24936 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/_bolt5.py
+-rw-r--r--   0 root         (0) root         (0)    10670 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/_common.py
+-rw-r--r--   0 root         (0) root         (0)    38631 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/io/_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_async/work/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27782 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/work/result.py
+-rw-r--r--   0 root         (0) root         (0)    27600 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/work/session.py
+-rw-r--r--   0 root         (0) root         (0)    11289 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/work/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async/work/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_async_compat/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14870 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_async_compat/network/
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25841 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/network/_bolt_socket.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/network/_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_async_compat/shims/
+-rw-r--r--   0 root         (0) root         (0)     4939 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/shims/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_async_compat/util.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_auth_management.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/hydration/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/hydration/_interface/
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/_interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/hydration/v1/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v1/hydration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v1/spatial.py
+-rw-r--r--   0 root         (0) root         (0)     8870 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v1/temporal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/hydration/v2/
+-rw-r--r--   0 root         (0) root         (0)      730 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v2/hydration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/hydration/v2/temporal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/packstream/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/packstream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/packstream/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_codec/packstream/v1/
+-rw-r--r--   0 root         (0) root         (0)    16696 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_codec/packstream/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18263 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_conf.py
+-rw-r--r--   0 root         (0) root         (0)    11673 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_data.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_deadline.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6378 2023-05-26 10:29:54.000000 neo4j-5.9.0/src/neo4j/_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_optional_deps/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_optional_deps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.500140 neo4j-5.9.0/src/neo4j/_spatial/
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_spatial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.504140 neo4j-5.9.0/src/neo4j/_sync/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6150 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/bookmark_manager.py
+-rw-r--r--   0 root         (0) root         (0)    49135 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.504140 neo4j-5.9.0/src/neo4j/_sync/io/
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35677 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/_bolt.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/_bolt3.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/_bolt4.py
+-rw-r--r--   0 root         (0) root         (0)    24759 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/_bolt5.py
+-rw-r--r--   0 root         (0) root         (0)    10393 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/_common.py
+-rw-r--r--   0 root         (0) root         (0)    37987 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/io/_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.504140 neo4j-5.9.0/src/neo4j/_sync/work/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27291 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/work/result.py
+-rw-r--r--   0 root         (0) root         (0)    26864 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/work/session.py
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/work/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_sync/work/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.504140 neo4j-5.9.0/src/neo4j/_work/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_work/eager_result.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_work/query.py
+-rw-r--r--   0 root         (0) root         (0)    10365 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/_work/summary.py
+-rw-r--r--   0 root         (0) root         (0)    10985 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/addressing.py
+-rw-r--r--   0 root         (0) root         (0)    18240 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/api.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/data.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/debug.py
+-rw-r--r--   0 root         (0) root         (0)    17262 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.504140 neo4j-5.9.0/src/neo4j/graph/
+-rw-r--r--   0 root         (0) root         (0)    11098 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/meta.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/packstream.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.504140 neo4j-5.9.0/src/neo4j/spatial/
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/spatial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.508140 neo4j-5.9.0/src/neo4j/time/
+-rw-r--r--   0 root         (0) root         (0)    95454 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/_arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/_clock_implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/_metaclasses.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/clock_implementations.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/hydration.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/time/metaclasses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.508140 neo4j-5.9.0/src/neo4j/work/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/work/query.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-26 10:28:11.000000 neo4j-5.9.0/src/neo4j/work/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:29:56.496140 neo4j-5.9.0/src/neo4j.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-05-26 10:29:56.000000 neo4j-5.9.0/src/neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-05-26 10:29:56.000000 neo4j-5.9.0/src/neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 10:29:56.000000 neo4j-5.9.0/src/neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 10:29:56.000000 neo4j-5.9.0/src/neo4j.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-26 10:29:56.000000 neo4j-5.9.0/src/neo4j.egg-info/top_level.txt
```

### Comparing `neo4j-5.8.1/LICENSE.APACHE2.txt` & `neo4j-5.9.0/LICENSE.APACHE2.txt`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/LICENSE.PYTHON.txt` & `neo4j-5.9.0/LICENSE.PYTHON.txt`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/PKG-INFO` & `neo4j-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j
-Version: 5.8.1
+Version: 5.9.0
 Summary: Neo4j Bolt driver for Python
 Author-email: "Neo4j, Inc." <drivers@neo4j.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/neo4j/neo4j-python-driver
 Keywords: neo4j,graph,database
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neo4j-5.8.1/README.rst` & `neo4j-5.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/pyproject.toml` & `neo4j-5.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/setup.py` & `neo4j-5.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/__init__.py` & `neo4j-5.9.0/src/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_api.py` & `neo4j-5.9.0/src/neo4j/_api.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/__init__.py` & `neo4j-5.9.0/src/neo4j/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/auth_management.py` & `neo4j-5.9.0/src/neo4j/_async/auth_management.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import time
 import typing as t
 from logging import getLogger
 
 from .._async_compat.concurrency import AsyncLock
 from .._auth_management import (
     AsyncAuthManager,
+    expiring_auth_has_expired,
     ExpiringAuth,
 )
 from .._meta import preview
 
 # work around for https://github.com/sphinx-doc/sphinx/pull/10880
 # make sure TAuth is resolved in the docs, else they're pretty useless
 # if t.TYPE_CHECKING:
@@ -50,56 +51,45 @@
     async def get_auth(self) -> _TAuth:
         return self._auth
 
     async def on_auth_expired(self, auth: _TAuth) -> None:
         pass
 
 
-class _ExpiringAuthHolder:
-    def __init__(self, auth: ExpiringAuth) -> None:
-        self._auth = auth
-        self._expiry = None
-        if auth.expires_in is not None:
-            self._expiry = time.monotonic() + auth.expires_in
-
-    @property
-    def auth(self) -> _TAuth:
-        return self._auth.auth
-
-    def expired(self) -> bool:
-        if self._expiry is None:
-            return False
-        return time.monotonic() > self._expiry
-
 class AsyncExpirationBasedAuthManager(AsyncAuthManager):
-    _current_auth: t.Optional[_ExpiringAuthHolder]
+    _current_auth: t.Optional[ExpiringAuth]
     _provider: t.Callable[[], t.Awaitable[ExpiringAuth]]
     _lock: AsyncLock
 
 
     def __init__(
         self,
         provider: t.Callable[[], t.Awaitable[ExpiringAuth]]
     ) -> None:
         self._provider = provider
         self._current_auth = None
         self._lock = AsyncLock()
 
     async def _refresh_auth(self):
-        self._current_auth = _ExpiringAuthHolder(await self._provider())
+        self._current_auth = await self._provider()
+        if self._current_auth is None:
+            raise TypeError(
+                "Auth provider function passed to expiration_based "
+                "AuthManager returned None, expected ExpiringAuth"
+            )
 
     async def get_auth(self) -> _TAuth:
         async with self._lock:
             auth = self._current_auth
-            if auth is not None and not auth.expired():
-                return auth.auth
-            log.debug("[     ]  _: <TEMPORAL AUTH> refreshing (time out)")
-            await self._refresh_auth()
-            assert self._current_auth is not None
-            return self._current_auth.auth
+            if auth is None or expiring_auth_has_expired(auth):
+                log.debug("[     ]  _: <TEMPORAL AUTH> refreshing (time out)")
+                await self._refresh_auth()
+                auth = self._current_auth
+                assert auth is not None
+            return auth.auth
 
     async def on_auth_expired(self, auth: _TAuth) -> None:
         async with self._lock:
             cur_auth = self._current_auth
             if cur_auth is not None and cur_auth.auth == auth:
                 log.debug("[     ]  _: <TEMPORAL AUTH> refreshing (error)")
                 await self._refresh_auth()
```

### Comparing `neo4j-5.8.1/src/neo4j/_async/bookmark_manager.py` & `neo4j-5.9.0/src/neo4j/_async/bookmark_manager.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/driver.py` & `neo4j-5.9.0/src/neo4j/_async/driver.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/__init__.py` & `neo4j-5.9.0/src/neo4j/_async/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/_bolt.py` & `neo4j-5.9.0/src/neo4j/_async/io/_bolt.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from ..._codec.packstream import v1 as packstream_v1
 from ..._conf import PoolConfig
 from ..._deadline import Deadline
 from ..._exceptions import (
     BoltError,
     BoltHandshakeError,
 )
-from ..._meta import get_user_agent
+from ..._meta import USER_AGENT
 from ...addressing import ResolvedAddress
 from ...api import (
     ServerInfo,
     Version,
 )
 from ...exceptions import (
     AuthError,
@@ -150,15 +150,15 @@
         self.routing_context = routing_context
         self.idle_since = perf_counter()
 
         # Determine the user agent
         if user_agent:
             self.user_agent = user_agent
         else:
-            self.user_agent = get_user_agent()
+            self.user_agent = USER_AGENT
 
         self.auth = auth
         self.auth_dict = self._to_auth_dict(auth)
         self.auth_manager = auth_manager
 
         self.notifications_min_severity = notifications_min_severity
         self.notifications_disabled_categories = \
@@ -259,26 +259,28 @@
             AsyncBolt4x3,
             AsyncBolt4x4,
         )
         from ._bolt5 import (
             AsyncBolt5x0,
             AsyncBolt5x1,
             AsyncBolt5x2,
+            AsyncBolt5x3,
         )
 
         handlers = {
             AsyncBolt3.PROTOCOL_VERSION: AsyncBolt3,
             # 4.0 unsupported because no space left in the handshake
             AsyncBolt4x1.PROTOCOL_VERSION: AsyncBolt4x1,
             AsyncBolt4x2.PROTOCOL_VERSION: AsyncBolt4x2,
             AsyncBolt4x3.PROTOCOL_VERSION: AsyncBolt4x3,
             AsyncBolt4x4.PROTOCOL_VERSION: AsyncBolt4x4,
             AsyncBolt5x0.PROTOCOL_VERSION: AsyncBolt5x0,
             AsyncBolt5x1.PROTOCOL_VERSION: AsyncBolt5x1,
             AsyncBolt5x2.PROTOCOL_VERSION: AsyncBolt5x2,
+            AsyncBolt5x3.PROTOCOL_VERSION: AsyncBolt5x3,
         }
 
         if protocol_version is None:
             return handlers
 
         if not isinstance(protocol_version, tuple):
             raise TypeError("Protocol version must be specified as a tuple")
@@ -385,15 +387,18 @@
                 keep_alive=pool_config.keep_alive,
             )
 
         pool_config.protocol_version = protocol_version
 
         # Carry out Bolt subclass imports locally to avoid circular dependency
         # issues.
-        if protocol_version == (5, 2):
+        if protocol_version == (5, 3):
+            from ._bolt5 import AsyncBolt5x3
+            bolt_cls = AsyncBolt5x3
+        elif protocol_version == (5, 2):
             from ._bolt5 import AsyncBolt5x2
             bolt_cls = AsyncBolt5x2
         elif protocol_version == (5, 1):
             from ._bolt5 import AsyncBolt5x1
             bolt_cls = AsyncBolt5x1
         elif protocol_version == (5, 0):
             from ._bolt5 import AsyncBolt5x0
@@ -833,15 +838,15 @@
 
     async def _set_defunct(self, message, error=None, silent=False):
         from ._pool import AsyncBoltPool
         direct_driver = isinstance(self.pool, AsyncBoltPool)
         user_cancelled = isinstance(error, asyncio.CancelledError)
 
         if error:
-            log.debug("[#%04X] _: <CONNECTION> error: %r", self.local_port,
+            log.debug("[#%04X]  _: <CONNECTION> error: %r", self.local_port,
                       error)
         if not user_cancelled:
             log.error(message)
         # We were attempting to receive data but the connection
         # has unexpectedly terminated. So, we need to close the
         # connection from the client side, and remove the address
         # from the connection pool.
```

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/_bolt3.py` & `neo4j-5.9.0/src/neo4j/_async/io/_bolt3.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/_bolt4.py` & `neo4j-5.9.0/src/neo4j/_async/io/_bolt4.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/_bolt5.py` & `neo4j-5.9.0/src/neo4j/_async/io/_bolt5.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import typing as t
 from enum import Enum
 from logging import getLogger
 from ssl import SSLSocket
 
 from ..._codec.hydration import v2 as hydration_v2
 from ..._exceptions import BoltProtocolError
+from ..._meta import BOLT_AGENT_DICT
 from ...api import (
     READ_ACCESS,
     Version,
 )
 from ...exceptions import (
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
@@ -614,7 +615,17 @@
         if notifications_disabled_categories is not None:
             extra["notifications_disabled_categories"] = \
                 notifications_disabled_categories
         log.debug("[#%04X]  C: BEGIN %r", self.local_port, extra)
         self._append(b"\x11", (extra,),
                      Response(self, "begin", hydration_hooks, **handlers),
                      dehydration_hooks=dehydration_hooks)
+
+
+class AsyncBolt5x3(AsyncBolt5x2):
+
+    PROTOCOL_VERSION = Version(5, 3)
+
+    def get_base_headers(self):
+        headers = super().get_base_headers()
+        headers["bolt_agent"] = BOLT_AGENT_DICT
+        return headers
```

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/_common.py` & `neo4j-5.9.0/src/neo4j/_async/io/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/io/_pool.py` & `neo4j-5.9.0/src/neo4j/_async/io/_pool.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/work/__init__.py` & `neo4j-5.9.0/src/neo4j/_async/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/work/result.py` & `neo4j-5.9.0/src/neo4j/_async/work/result.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/work/session.py` & `neo4j-5.9.0/src/neo4j/_async/work/session.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/work/transaction.py` & `neo4j-5.9.0/src/neo4j/_async/work/transaction.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async/work/workspace.py` & `neo4j-5.9.0/src/neo4j/_async/work/workspace.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/__init__.py` & `neo4j-5.9.0/src/neo4j/_async_compat/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/concurrency.py` & `neo4j-5.9.0/src/neo4j/_async_compat/concurrency.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/network/__init__.py` & `neo4j-5.9.0/src/neo4j/_async_compat/network/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/network/_bolt_socket.py` & `neo4j-5.9.0/src/neo4j/_async_compat/network/_bolt_socket.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/network/_util.py` & `neo4j-5.9.0/src/neo4j/_async_compat/network/_util.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/shims/__init__.py` & `neo4j-5.9.0/src/neo4j/_async_compat/shims/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_async_compat/util.py` & `neo4j-5.9.0/src/neo4j/_async_compat/util.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_auth_management.py` & `neo4j-5.9.0/src/neo4j/_auth_management.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,46 +18,82 @@
 
 # from __future__ import annotations
 # work around for https://github.com/sphinx-doc/sphinx/pull/10880
 # make sure TAuth is resolved in the docs, else they're pretty useless
 
 
 import abc
+import time
 import typing as t
+import warnings
 from dataclasses import dataclass
 
-from ._meta import preview
+from ._meta import (
+    preview,
+    PreviewWarning,
+)
 from .api import _TAuth
 
 
 @preview("Auth managers are a preview feature.")
 @dataclass
 class ExpiringAuth:
     """Represents potentially expiring authentication information.
 
     This class is used with :meth:`.AuthManagers.expiration_based` and
     :meth:`.AsyncAuthManagers.expiration_based`.
 
     :param auth: The authentication information.
-    :param expires_in: The number of seconds until the authentication
-        information expires. If :data:`None`, the authentication information
-        is considered to not expire until the server explicitly indicates so.
+    :param expires_at:
+        Unix timestamp (seconds since 1970-01-01 00:00:00 UTC)
+        indicating when the authentication information expires.
+        If :data:`None`, the authentication information is considered to not
+        expire until the server explicitly indicates so.
 
     **This is a preview** (see :ref:`filter-warnings-ref`).
     It might be changed without following the deprecation policy.
     See also https://github.com/neo4j/neo4j-python-driver/wiki/preview-features
 
     .. seealso::
         :meth:`.AuthManagers.expiration_based`,
         :meth:`.AsyncAuthManagers.expiration_based`
 
     .. versionadded:: 5.8
     """
-    auth: _TAuth
-    expires_in: t.Optional[float] = None
+    auth: "_TAuth"
+    expires_at: t.Optional[float] = None
+
+    def expires_in(self, seconds: float) -> "ExpiringAuth":
+        """Return a copy of this object with a new expiration time.
+
+        This is a convenience method for creating an :class:`.ExpiringAuth`
+        for a relative expiration time ("expires in" instead of "expires at").
+
+            >>> import time, freezegun
+            >>> with freezegun.freeze_time("1970-01-01 00:00:40"):
+            ...     ExpiringAuth(("user", "pass")).expires_in(2)
+            ExpiringAuth(auth=('user', 'pass'), expires_at=42.0)
+            >>> with freezegun.freeze_time("1970-01-01 00:00:40"):
+            ...     ExpiringAuth(("user", "pass"), time.time() + 2)
+            ExpiringAuth(auth=('user', 'pass'), expires_at=42.0)
+
+        :param seconds:
+            The number of seconds from now until the authentication information
+            expires.
+        """
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore",
+                                    message=r"^Auth managers\b.*",
+                                    category=PreviewWarning)
+            return ExpiringAuth(self.auth, time.time() + seconds)
+
+
+def expiring_auth_has_expired(auth: ExpiringAuth) -> bool:
+    expires_at = auth.expires_at
+    return expires_at is not None and expires_at < time.time()
 
 
 class AuthManager(metaclass=abc.ABCMeta):
     """Baseclass for authentication information managers.
 
     The driver provides some default implementations of this class in
     :class:`.AuthManagers` for convenience.
```

### Comparing `neo4j-5.8.1/src/neo4j/_codec/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/_common.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/_interface/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v1/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v1/hydration_handler.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v1/hydration_handler.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v1/spatial.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v1/spatial.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v1/temporal.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v1/temporal.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v2/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v2/hydration_handler.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v2/hydration_handler.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/hydration/v2/temporal.py` & `neo4j-5.9.0/src/neo4j/_codec/hydration/v2/temporal.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/packstream/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/packstream/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/packstream/_common.py` & `neo4j-5.9.0/src/neo4j/_codec/packstream/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_codec/packstream/v1/__init__.py` & `neo4j-5.9.0/src/neo4j/_codec/packstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_conf.py` & `neo4j-5.9.0/src/neo4j/_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from abc import ABCMeta
 from collections.abc import Mapping
 
 from ._meta import (
     deprecation_warn,
     experimental_warn,
     ExperimentalWarning,
-    get_user_agent,
 )
 from .api import (
     DEFAULT_DATABASE,
     TRUST_ALL_CERTIFICATES,
     TRUST_SYSTEM_CA_SIGNED_CERTIFICATES,
     WRITE_ACCESS,
 )
@@ -396,15 +395,15 @@
     #: Custom SSL context to use for wrapping sockets
     ssl_context = None
     # Use any custom SSL context to wrap sockets.
     # Overwrites `trusted_certificates` and `encrypted`.
     # The use of this option is strongly discouraged.
 
     #: User Agent (Python Driver Specific)
-    user_agent = get_user_agent()
+    user_agent = None
     # Specify the client agent name.
 
     #: Socket Keep Alive (Python and .NET Driver Specific)
     keep_alive = True
     # Specify whether TCP keep-alive should be enabled.
 
     #: Authentication provider
```

### Comparing `neo4j-5.8.1/src/neo4j/_data.py` & `neo4j-5.9.0/src/neo4j/_data.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_deadline.py` & `neo4j-5.9.0/src/neo4j/_deadline.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_exceptions.py` & `neo4j-5.9.0/src/neo4j/_exceptions.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_meta.py` & `neo4j-5.9.0/src/neo4j/_meta.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,41 +15,69 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import asyncio
+import platform
+import sys
 import tracemalloc
 import typing as t
 from functools import wraps
 from inspect import isclass
 from warnings import warn
 
 
 _FuncT = t.TypeVar("_FuncT", bound=t.Callable)
 
 
 # Can be automatically overridden in builds
 package = "neo4j"
-version = "5.8.1"
+version = "5.9.0"
 deprecated_package = False
 
 
+def _compute_bolt_agent() -> t.Dict[str, str]:
+    def format_version_info(version_info):
+        return "{}.{}.{}-{}-{}".format(*version_info)
+
+    return {
+        "product": f"neo4j-python/{version}",
+        "platform":
+            f"{platform.system() or 'Unknown'} "
+            f"{platform.release() or 'unknown'}; "
+            f"{platform.machine() or 'unknown'}",
+        "language": f"Python/{format_version_info(sys.version_info)}",
+        "language_details":
+            f"{platform.python_implementation()}; "
+            f"{format_version_info(sys.implementation.version)} "
+            f"({', '.join(platform.python_build())}) "
+            f"[{platform.python_compiler()}]"
+    }
+
+
+BOLT_AGENT_DICT = _compute_bolt_agent()
+
+
+def _compute_user_agent() -> str:
+    template = "neo4j-python/{} Python/{}.{}.{}-{}-{} ({})"
+    fields = (version,) + tuple(sys.version_info) + (sys.platform,)
+    return template.format(*fields)
+
+
+USER_AGENT = _compute_user_agent()
+
+
+# TODO: 6.0 - remove this function
 def get_user_agent():
     """ Obtain the default user agent string sent to the server after
     a successful handshake.
     """
-    from sys import (
-        platform,
-        version_info,
-    )
-    template = "neo4j-python/{} Python/{}.{}.{}-{}-{} ({})"
-    fields = (version,) + tuple(version_info) + (platform,)
-    return template.format(*fields)
+    return USER_AGENT
 
 
 def _id(x):
     return x
 
 
 def copy_signature(_: _FuncT) -> t.Callable[[t.Callable], _FuncT]:
```

### Comparing `neo4j-5.8.1/src/neo4j/_routing.py` & `neo4j-5.9.0/src/neo4j/_routing.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_spatial/__init__.py` & `neo4j-5.9.0/src/neo4j/_spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/__init__.py` & `neo4j-5.9.0/src/neo4j/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/auth_management.py` & `neo4j-5.9.0/src/neo4j/_sync/auth_management.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import time
 import typing as t
 from logging import getLogger
 
 from .._async_compat.concurrency import Lock
 from .._auth_management import (
     AuthManager,
+    expiring_auth_has_expired,
     ExpiringAuth,
 )
 from .._meta import preview
 
 # work around for https://github.com/sphinx-doc/sphinx/pull/10880
 # make sure TAuth is resolved in the docs, else they're pretty useless
 # if t.TYPE_CHECKING:
@@ -50,56 +51,45 @@
     def get_auth(self) -> _TAuth:
         return self._auth
 
     def on_auth_expired(self, auth: _TAuth) -> None:
         pass
 
 
-class _ExpiringAuthHolder:
-    def __init__(self, auth: ExpiringAuth) -> None:
-        self._auth = auth
-        self._expiry = None
-        if auth.expires_in is not None:
-            self._expiry = time.monotonic() + auth.expires_in
-
-    @property
-    def auth(self) -> _TAuth:
-        return self._auth.auth
-
-    def expired(self) -> bool:
-        if self._expiry is None:
-            return False
-        return time.monotonic() > self._expiry
-
 class ExpirationBasedAuthManager(AuthManager):
-    _current_auth: t.Optional[_ExpiringAuthHolder]
+    _current_auth: t.Optional[ExpiringAuth]
     _provider: t.Callable[[], t.Union[ExpiringAuth]]
     _lock: Lock
 
 
     def __init__(
         self,
         provider: t.Callable[[], t.Union[ExpiringAuth]]
     ) -> None:
         self._provider = provider
         self._current_auth = None
         self._lock = Lock()
 
     def _refresh_auth(self):
-        self._current_auth = _ExpiringAuthHolder(self._provider())
+        self._current_auth = self._provider()
+        if self._current_auth is None:
+            raise TypeError(
+                "Auth provider function passed to expiration_based "
+                "AuthManager returned None, expected ExpiringAuth"
+            )
 
     def get_auth(self) -> _TAuth:
         with self._lock:
             auth = self._current_auth
-            if auth is not None and not auth.expired():
-                return auth.auth
-            log.debug("[     ]  _: <TEMPORAL AUTH> refreshing (time out)")
-            self._refresh_auth()
-            assert self._current_auth is not None
-            return self._current_auth.auth
+            if auth is None or expiring_auth_has_expired(auth):
+                log.debug("[     ]  _: <TEMPORAL AUTH> refreshing (time out)")
+                self._refresh_auth()
+                auth = self._current_auth
+                assert auth is not None
+            return auth.auth
 
     def on_auth_expired(self, auth: _TAuth) -> None:
         with self._lock:
             cur_auth = self._current_auth
             if cur_auth is not None and cur_auth.auth == auth:
                 log.debug("[     ]  _: <TEMPORAL AUTH> refreshing (error)")
                 self._refresh_auth()
```

### Comparing `neo4j-5.8.1/src/neo4j/_sync/bookmark_manager.py` & `neo4j-5.9.0/src/neo4j/_sync/bookmark_manager.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/driver.py` & `neo4j-5.9.0/src/neo4j/_sync/driver.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/__init__.py` & `neo4j-5.9.0/src/neo4j/_sync/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/_bolt.py` & `neo4j-5.9.0/src/neo4j/_sync/io/_bolt.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from ..._codec.packstream import v1 as packstream_v1
 from ..._conf import PoolConfig
 from ..._deadline import Deadline
 from ..._exceptions import (
     BoltError,
     BoltHandshakeError,
 )
-from ..._meta import get_user_agent
+from ..._meta import USER_AGENT
 from ...addressing import ResolvedAddress
 from ...api import (
     ServerInfo,
     Version,
 )
 from ...exceptions import (
     AuthError,
@@ -150,15 +150,15 @@
         self.routing_context = routing_context
         self.idle_since = perf_counter()
 
         # Determine the user agent
         if user_agent:
             self.user_agent = user_agent
         else:
-            self.user_agent = get_user_agent()
+            self.user_agent = USER_AGENT
 
         self.auth = auth
         self.auth_dict = self._to_auth_dict(auth)
         self.auth_manager = auth_manager
 
         self.notifications_min_severity = notifications_min_severity
         self.notifications_disabled_categories = \
@@ -259,26 +259,28 @@
             Bolt4x3,
             Bolt4x4,
         )
         from ._bolt5 import (
             Bolt5x0,
             Bolt5x1,
             Bolt5x2,
+            Bolt5x3,
         )
 
         handlers = {
             Bolt3.PROTOCOL_VERSION: Bolt3,
             # 4.0 unsupported because no space left in the handshake
             Bolt4x1.PROTOCOL_VERSION: Bolt4x1,
             Bolt4x2.PROTOCOL_VERSION: Bolt4x2,
             Bolt4x3.PROTOCOL_VERSION: Bolt4x3,
             Bolt4x4.PROTOCOL_VERSION: Bolt4x4,
             Bolt5x0.PROTOCOL_VERSION: Bolt5x0,
             Bolt5x1.PROTOCOL_VERSION: Bolt5x1,
             Bolt5x2.PROTOCOL_VERSION: Bolt5x2,
+            Bolt5x3.PROTOCOL_VERSION: Bolt5x3,
         }
 
         if protocol_version is None:
             return handlers
 
         if not isinstance(protocol_version, tuple):
             raise TypeError("Protocol version must be specified as a tuple")
@@ -385,15 +387,18 @@
                 keep_alive=pool_config.keep_alive,
             )
 
         pool_config.protocol_version = protocol_version
 
         # Carry out Bolt subclass imports locally to avoid circular dependency
         # issues.
-        if protocol_version == (5, 2):
+        if protocol_version == (5, 3):
+            from ._bolt5 import Bolt5x3
+            bolt_cls = Bolt5x3
+        elif protocol_version == (5, 2):
             from ._bolt5 import Bolt5x2
             bolt_cls = Bolt5x2
         elif protocol_version == (5, 1):
             from ._bolt5 import Bolt5x1
             bolt_cls = Bolt5x1
         elif protocol_version == (5, 0):
             from ._bolt5 import Bolt5x0
@@ -833,15 +838,15 @@
 
     def _set_defunct(self, message, error=None, silent=False):
         from ._pool import BoltPool
         direct_driver = isinstance(self.pool, BoltPool)
         user_cancelled = isinstance(error, asyncio.CancelledError)
 
         if error:
-            log.debug("[#%04X] _: <CONNECTION> error: %r", self.local_port,
+            log.debug("[#%04X]  _: <CONNECTION> error: %r", self.local_port,
                       error)
         if not user_cancelled:
             log.error(message)
         # We were attempting to receive data but the connection
         # has unexpectedly terminated. So, we need to close the
         # connection from the client side, and remove the address
         # from the connection pool.
```

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/_bolt3.py` & `neo4j-5.9.0/src/neo4j/_sync/io/_bolt3.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/_bolt4.py` & `neo4j-5.9.0/src/neo4j/_sync/io/_bolt4.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/_bolt5.py` & `neo4j-5.9.0/src/neo4j/_sync/io/_bolt5.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import typing as t
 from enum import Enum
 from logging import getLogger
 from ssl import SSLSocket
 
 from ..._codec.hydration import v2 as hydration_v2
 from ..._exceptions import BoltProtocolError
+from ..._meta import BOLT_AGENT_DICT
 from ...api import (
     READ_ACCESS,
     Version,
 )
 from ...exceptions import (
     DatabaseUnavailable,
     ForbiddenOnReadOnlyDatabase,
@@ -614,7 +615,17 @@
         if notifications_disabled_categories is not None:
             extra["notifications_disabled_categories"] = \
                 notifications_disabled_categories
         log.debug("[#%04X]  C: BEGIN %r", self.local_port, extra)
         self._append(b"\x11", (extra,),
                      Response(self, "begin", hydration_hooks, **handlers),
                      dehydration_hooks=dehydration_hooks)
+
+
+class Bolt5x3(Bolt5x2):
+
+    PROTOCOL_VERSION = Version(5, 3)
+
+    def get_base_headers(self):
+        headers = super().get_base_headers()
+        headers["bolt_agent"] = BOLT_AGENT_DICT
+        return headers
```

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/_common.py` & `neo4j-5.9.0/src/neo4j/_sync/io/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/io/_pool.py` & `neo4j-5.9.0/src/neo4j/_sync/io/_pool.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/work/__init__.py` & `neo4j-5.9.0/src/neo4j/_sync/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/work/result.py` & `neo4j-5.9.0/src/neo4j/_sync/work/result.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/work/session.py` & `neo4j-5.9.0/src/neo4j/_sync/work/session.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/work/transaction.py` & `neo4j-5.9.0/src/neo4j/_sync/work/transaction.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_sync/work/workspace.py` & `neo4j-5.9.0/src/neo4j/_sync/work/workspace.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_work/__init__.py` & `neo4j-5.9.0/src/neo4j/_work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_work/eager_result.py` & `neo4j-5.9.0/src/neo4j/_work/eager_result.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_work/query.py` & `neo4j-5.9.0/src/neo4j/_work/query.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/_work/summary.py` & `neo4j-5.9.0/src/neo4j/_work/summary.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/addressing.py` & `neo4j-5.9.0/src/neo4j/addressing.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/api.py` & `neo4j-5.9.0/src/neo4j/api.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/auth_management.py` & `neo4j-5.9.0/src/neo4j/auth_management.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/conf.py` & `neo4j-5.9.0/src/neo4j/conf.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/data.py` & `neo4j-5.9.0/src/neo4j/data.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/debug.py` & `neo4j-5.9.0/src/neo4j/debug.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/exceptions.py` & `neo4j-5.9.0/src/neo4j/exceptions.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/graph/__init__.py` & `neo4j-5.9.0/src/neo4j/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/meta.py` & `neo4j-5.9.0/src/neo4j/meta.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/packstream.py` & `neo4j-5.9.0/src/neo4j/packstream.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/routing.py` & `neo4j-5.9.0/src/neo4j/routing.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/spatial/__init__.py` & `neo4j-5.9.0/src/neo4j/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/__init__.py` & `neo4j-5.9.0/src/neo4j/time/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/__main__.py` & `neo4j-5.9.0/src/neo4j/time/__main__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/_arithmetic.py` & `neo4j-5.9.0/src/neo4j/time/_arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/_clock_implementations.py` & `neo4j-5.9.0/src/neo4j/time/_clock_implementations.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/_metaclasses.py` & `neo4j-5.9.0/src/neo4j/time/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/arithmetic.py` & `neo4j-5.9.0/src/neo4j/time/arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/clock_implementations.py` & `neo4j-5.9.0/src/neo4j/time/clock_implementations.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/hydration.py` & `neo4j-5.9.0/src/neo4j/time/hydration.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/time/metaclasses.py` & `neo4j-5.9.0/src/neo4j/time/metaclasses.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/work/__init__.py` & `neo4j-5.9.0/src/neo4j/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/work/query.py` & `neo4j-5.9.0/src/neo4j/work/query.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j/work/summary.py` & `neo4j-5.9.0/src/neo4j/work/summary.py`

 * *Files identical despite different names*

### Comparing `neo4j-5.8.1/src/neo4j.egg-info/PKG-INFO` & `neo4j-5.9.0/src/neo4j.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j
-Version: 5.8.1
+Version: 5.9.0
 Summary: Neo4j Bolt driver for Python
 Author-email: "Neo4j, Inc." <drivers@neo4j.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/neo4j/neo4j-python-driver
 Keywords: neo4j,graph,database
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neo4j-5.8.1/src/neo4j.egg-info/SOURCES.txt` & `neo4j-5.9.0/src/neo4j.egg-info/SOURCES.txt`

 * *Files identical despite different names*

