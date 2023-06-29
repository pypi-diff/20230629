# Comparing `tmp/PALs-0.3.4.tar.gz` & `tmp/PALs-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PALs-0.3.4.tar", last modified: Mon Mar  6 17:24:06 2023, max compression
+gzip compressed data, was "PALs-0.3.5.tar", last modified: Thu Jun 29 12:20:46 2023, max compression
```

## Comparing `PALs-0.3.4.tar` & `PALs-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.246585 PALs-0.3.4/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.242585 PALs-0.3.4/.ci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      104 2021-02-01 16:04:04.000000 PALs-0.3.4/.ci/pytest.ini
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.242585 PALs-0.3.4/.circleci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1094 2023-01-06 19:39:01.000000 PALs-0.3.4/.circleci/config.yml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      313 2021-02-01 16:04:04.000000 PALs-0.3.4/.coveragerc
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      204 2023-01-06 19:39:01.000000 PALs-0.3.4/MANIFEST.in
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.242585 PALs-0.3.4/PALs.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9651 2023-03-06 17:24:05.000000 PALs-0.3.4/PALs.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      449 2023-03-06 17:24:06.000000 PALs-0.3.4/PALs.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-03-06 17:24:05.000000 PALs-0.3.4/PALs.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2021-02-01 16:06:26.000000 PALs-0.3.4/PALs.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       54 2023-03-06 17:24:06.000000 PALs-0.3.4/PALs.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        5 2023-03-06 17:24:06.000000 PALs-0.3.4/PALs.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9651 2023-03-06 17:24:06.246585 PALs-0.3.4/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4013 2023-03-06 17:23:48.000000 PALs-0.3.4/changelog.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      256 2023-01-06 19:39:01.000000 PALs-0.3.4/docker-compose.yaml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1549 2021-02-01 16:04:04.000000 PALs-0.3.4/license.txt
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.242585 PALs-0.3.4/pals/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       32 2021-02-01 16:04:04.000000 PALs-0.3.4/pals/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6417 2023-03-06 17:23:08.000000 PALs-0.3.4/pals/core.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.242585 PALs-0.3.4/pals/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6376 2023-01-06 19:39:01.000000 PALs-0.3.4/pals/tests/test_core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-03-06 17:23:34.000000 PALs-0.3.4/pals/version.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       24 2021-02-01 16:04:04.000000 PALs-0.3.4/pyp.ini
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4883 2023-01-06 19:39:01.000000 PALs-0.3.4/readme.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-06 17:24:06.246585 PALs-0.3.4/scripts/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      941 2021-02-01 16:04:04.000000 PALs-0.3.4/scripts/hang.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      410 2023-01-06 19:39:01.000000 PALs-0.3.4/scripts/setup-codecov
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      172 2023-03-06 17:24:06.246585 PALs-0.3.4/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1469 2023-01-06 19:39:01.000000 PALs-0.3.4/setup.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      219 2023-01-06 19:39:01.000000 PALs-0.3.4/stable-requirements.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1151 2023-03-06 17:23:08.000000 PALs-0.3.4/tox.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.583046 PALs-0.3.5/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/.ci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      104 2021-02-01 16:04:04.000000 PALs-0.3.5/.ci/pytest.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/.circleci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1094 2023-01-06 19:39:01.000000 PALs-0.3.5/.circleci/config.yml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      313 2021-02-01 16:04:04.000000 PALs-0.3.5/.coveragerc
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      204 2023-01-06 19:39:01.000000 PALs-0.3.5/MANIFEST.in
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/PALs.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9839 2023-06-29 12:20:45.000000 PALs-0.3.5/PALs.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      449 2023-06-29 12:20:46.000000 PALs-0.3.5/PALs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-06-29 12:20:45.000000 PALs-0.3.5/PALs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2021-02-01 16:06:26.000000 PALs-0.3.5/PALs.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       54 2023-06-29 12:20:46.000000 PALs-0.3.5/PALs.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        5 2023-06-29 12:20:46.000000 PALs-0.3.5/PALs.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9839 2023-06-29 12:20:46.583046 PALs-0.3.5/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4201 2023-06-29 12:20:25.000000 PALs-0.3.5/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      256 2023-01-06 19:39:01.000000 PALs-0.3.5/docker-compose.yaml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1549 2021-02-01 16:04:04.000000 PALs-0.3.5/license.txt
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/pals/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       32 2021-02-01 16:04:04.000000 PALs-0.3.5/pals/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6459 2023-06-29 12:18:47.000000 PALs-0.3.5/pals/core.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/pals/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7437 2023-06-29 12:18:47.000000 PALs-0.3.5/pals/tests/test_core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-06-29 12:19:04.000000 PALs-0.3.5/pals/version.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       24 2021-02-01 16:04:04.000000 PALs-0.3.5/pyp.ini
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4883 2023-01-06 19:39:01.000000 PALs-0.3.5/readme.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/scripts/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      941 2021-02-01 16:04:04.000000 PALs-0.3.5/scripts/hang.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      410 2023-01-06 19:39:01.000000 PALs-0.3.5/scripts/setup-codecov
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      172 2023-06-29 12:20:46.583046 PALs-0.3.5/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1469 2023-01-06 19:39:01.000000 PALs-0.3.5/setup.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      219 2023-01-06 19:39:01.000000 PALs-0.3.5/stable-requirements.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1151 2023-03-06 17:23:08.000000 PALs-0.3.5/tox.ini
```

### Comparing `PALs-0.3.4/.circleci/config.yml` & `PALs-0.3.5/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `PALs-0.3.4/PALs.egg-info/PKG-INFO` & `PALs-0.3.5/PALs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PALs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Easy distributed locking using PostgreSQL Advisory Locks.
 Home-page: https://github.com/level12/pals
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -176,14 +176,22 @@
 * https://github.com/Xof/django-pglocks
 
 
 
 Changelog
 =========
 
+0.3.5 released 2023-06-29
+-------------------------
+
+- fix cursor usage after connection close (thanks to @moser) (ded88e7_)
+
+.. _ded88e7: https://github.com/level12/pals/commit/ded88e7
+
+
 0.3.4 released 2023-03-06
 -------------------------
 
 - support SQLAlchemy 2.0 (6879081_)
 
 .. _6879081: https://github.com/level12/pals/commit/6879081
```

### Comparing `PALs-0.3.4/PKG-INFO` & `PALs-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PALs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Easy distributed locking using PostgreSQL Advisory Locks.
 Home-page: https://github.com/level12/pals
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -176,14 +176,22 @@
 * https://github.com/Xof/django-pglocks
 
 
 
 Changelog
 =========
 
+0.3.5 released 2023-06-29
+-------------------------
+
+- fix cursor usage after connection close (thanks to @moser) (ded88e7_)
+
+.. _ded88e7: https://github.com/level12/pals/commit/ded88e7
+
+
 0.3.4 released 2023-03-06
 -------------------------
 
 - support SQLAlchemy 2.0 (6879081_)
 
 .. _6879081: https://github.com/level12/pals/commit/6879081
```

### Comparing `PALs-0.3.4/changelog.rst` & `PALs-0.3.5/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.3.5 released 2023-06-29
+-------------------------
+
+- fix cursor usage after connection close (thanks to @moser) (ded88e7_)
+
+.. _ded88e7: https://github.com/level12/pals/commit/ded88e7
+
+
 0.3.4 released 2023-03-06
 -------------------------
 
 - support SQLAlchemy 2.0 (6879081_)
 
 .. _6879081: https://github.com/level12/pals/commit/6879081
```

### Comparing `PALs-0.3.4/license.txt` & `PALs-0.3.5/license.txt`

 * *Files identical despite different names*

### Comparing `PALs-0.3.4/pals/core.py` & `PALs-0.3.5/pals/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,19 @@
     def release(self):
         if self.conn is None:
             return False
 
         sql = sa.text(f'select pg_advisory_unlock{self.shared_suffix}(:lock_num)')
         with self.conn.begin():
             result = self.conn.execute(sql, {'lock_num': self.lock_num})
-        self.conn.close()
-        self.conn = None
-        return result.scalar()
+        try:
+            return result.scalar()
+        finally:
+            self.conn.close()
+            self.conn = None
 
     def __enter__(self):
         self._acquire()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.release()
```

### Comparing `PALs-0.3.4/pals/tests/test_core.py` & `PALs-0.3.5/pals/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime as dt
 import gc
 import os
 import random
 import string
+import threading
+import time
 
 import pytest
 
 import pals
 
 # Default URL will work for CI tests
 db_url = os.environ.get('PALS_DB_URL', 'postgresql://postgres:password@localhost/postgres')
@@ -185,7 +187,39 @@
     def test_gc_lock_release(self):
         lock1 = self.locker.lock('test_it')
         lock1.acquire()
         del lock1
         gc.collect()
 
         assert self.locker.lock('test_it', blocking=False).acquire()
+
+    def test_contention_on_connection_pool(self):
+        """
+        Given N = size of connection pool, run N + 1 threads that all try to
+        acquire locks (different ones) at the same time.
+
+        The first N threads should all acquire a lock. The last thread should
+        wait until one of the first N threads releases their lock, then acquire
+        it normally.
+
+        This test demonstrates issue #40.
+        """
+        set_size = self.locker.engine.pool.size() + 1
+        results = [None] * set_size
+
+        def target(n):
+            try:
+                with self.locker.lock(f"example-{n}"):
+                    time.sleep(0.05)
+                results[n] = True
+            except Exception as e:
+                results[n] = e
+
+        threads = [threading.Thread(target=target, args=(n,)) for n in range(set_size)]
+
+        for thread in threads:
+            thread.start()
+        for thread in threads:
+            thread.join()
+
+        assert [r for r in results if isinstance(r, Exception)] == []
+
```

### Comparing `PALs-0.3.4/readme.rst` & `PALs-0.3.5/readme.rst`

 * *Files identical despite different names*

### Comparing `PALs-0.3.4/scripts/hang.py` & `PALs-0.3.5/scripts/hang.py`

 * *Files identical despite different names*

### Comparing `PALs-0.3.4/setup.py` & `PALs-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `PALs-0.3.4/tox.ini` & `PALs-0.3.5/tox.ini`

 * *Files identical despite different names*

