# Comparing `tmp/sentry-redis-tools-0.1.6.tar.gz` & `tmp/sentry-redis-tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-redis-tools-0.1.6.tar", last modified: Wed May 17 17:01:26 2023, max compression
+gzip compressed data, was "sentry-redis-tools-0.1.7.tar", last modified: Thu Jun 29 14:35:27 2023, max compression
```

## Comparing `sentry-redis-tools-0.1.6.tar` & `sentry-redis-tools-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:26.646076 sentry-redis-tools-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-17 17:01:26.642076 sentry-redis-tools-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:26.642076 sentry-redis-tools-0.1.6/sentry_redis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/cardinality_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/failover_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/retrying_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/sliding_windows_rate_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:26.642076 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:01:26.646076 sentry-redis-tools-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:35:27.566506 sentry-redis-tools-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 14:35:27.566506 sentry-redis-tools-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:35:27.566506 sentry-redis-tools-0.1.7/sentry_redis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/cardinality_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/failover_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/retrying_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/sentry_redis_tools/sliding_windows_rate_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:35:27.566506 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 14:35:27.000000 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 14:35:27.000000 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:35:27.000000 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:35:27.000000 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 14:35:27.000000 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 14:35:27.000000 sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:35:27.566506 sentry-redis-tools-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-29 14:35:22.000000 sentry-redis-tools-0.1.7/setup.py
```

### Comparing `sentry-redis-tools-0.1.6/LICENSE` & `sentry-redis-tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.6/sentry_redis_tools/cardinality_limiter.py` & `sentry-redis-tools-0.1.7/sentry_redis_tools/cardinality_limiter.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.6/sentry_redis_tools/failover_redis.py` & `sentry-redis-tools-0.1.7/sentry_redis_tools/failover_redis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,62 @@
+from __future__ import annotations
+
 import random
 import time
-from typing import Any
+from typing import Any, Callable, Optional
 
 from sentry_redis_tools.clients import StrictRedis
 from redis.exceptions import (
     ConnectionError,
     ReadOnlyError,
     TimeoutError,
 )
 
 
+def _sentry_wrap_with_retry(
+    get_wrapped_fn: Callable[[], Any], client_self: Optional[FailoverRedis] = None
+) -> Any:
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
+        nonlocal client_self
+        slf = client_self
+        if slf is None:
+            slf = args[0]
+        assert slf is not None
+
+        retries = 0
+        while True:
+            try:
+                return get_wrapped_fn()(*args, **kwargs)
+            except (
+                # Caught during the inital phase of failver when writes are
+                # paused on primary
+                ReadOnlyError,
+                # When the connection to primary is dropped and the one to the
+                # replica is not ready yet.
+                # ConnectionError with the errno ETIMEDOUT = 110
+                ConnectionError,
+                # When the client is initiated with socket_timeout or
+                # socket_connect_timeout, during the reconnect it throws
+                # redis.exceptions.TimeoutError instead of ConnectionError
+                TimeoutError,
+            ):
+                if retries >= slf._retries:
+                    raise
+                time.sleep(
+                    min(
+                        slf._backoff_max,
+                        (slf._backoff_min * (slf._backoff_multiplier**retries))
+                        * (1 + random.random()),
+                    )
+                )
+                retries += 1
+
+    return wrapper
+
+
 class FailoverRedis(StrictRedis):  # type: ignore
     """
     Single host redis client implementation with retry logic intended to
     survive failover events. Retry logic uses capped exponential backoff with
     jitter.
 
     https://redis.io/commands/failover
@@ -82,35 +125,14 @@
         if _backoff_multiplier <= 0:
             raise ValueError(
                 f"Backoff multiplier must be positive number: _backoff_multiplier={_backoff_multiplier}"
             )
         self._backoff_multiplier = _backoff_multiplier
         super().__init__(*args, **kwargs)
 
-    def execute_command(self, *args: Any, **kwargs: Any) -> Any:
-        retries = 0
-        while True:
-            try:
-                return super().execute_command(*args, **kwargs)
-            except (
-                # Caught during the inital phase of failver when writes are
-                # paused on primary
-                ReadOnlyError,
-                # When the connection to primary is dropped and the one to the
-                # replica is not ready yet.
-                # ConnectionError with the errno ETIMEDOUT = 110
-                ConnectionError,
-                # When the client is initiated with socket_timeout or
-                # socket_connect_timeout, during the reconnect it throws
-                # redis.exceptions.TimeoutError instead of ConnectionError
-                TimeoutError,
-            ):
-                if retries >= self._retries:
-                    raise
-                time.sleep(
-                    min(
-                        self._backoff_max,
-                        (self._backoff_min * (self._backoff_multiplier**retries))
-                        * (1 + random.random()),
-                    )
-                )
-                retries += 1
+    execute_command = _sentry_wrap_with_retry(lambda: StrictRedis.execute_command)
+
+    def pipeline(self, *args: Any, **kwargs: Any) -> Any:
+        rv = StrictRedis.pipeline(self, *args, **kwargs)
+        old_execute = rv.execute
+        rv.execute = _sentry_wrap_with_retry(lambda: old_execute, client_self=self)
+        return rv
```

### Comparing `sentry-redis-tools-0.1.6/sentry_redis_tools/metrics.py` & `sentry-redis-tools-0.1.7/sentry_redis_tools/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.6/sentry_redis_tools/retrying_cluster.py` & `sentry-redis-tools-0.1.7/sentry_redis_tools/retrying_cluster.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.6/sentry_redis_tools/sliding_windows_rate_limiter.py` & `sentry-redis-tools-0.1.7/sentry_redis_tools/sliding_windows_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/SOURCES.txt` & `sentry-redis-tools-0.1.7/sentry_redis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.6/setup.py` & `sentry-redis-tools-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 from typing import Sequence
 
 
 setup(
     name="sentry-redis-tools",
-    version="0.1.6",
+    version="0.1.7",
     author="Sentry",
     author_email="oss@sentry.io",
     license="Apache-2.0",
     url="https://github.com/getsentry/sentry-redis-tools",
     description="Common utilities related to how Sentry uses Redis",
     zip_safe=False,
     install_requires=['redis>=3.0'],
```

