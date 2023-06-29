# Comparing `tmp/fair_async_rlock-1.0.3.tar.gz` & `tmp/fair_async_rlock-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_async_rlock-1.0.3.tar", last modified: Thu Jun 15 23:39:56 2023, max compression
+gzip compressed data, was "fair_async_rlock-1.0.4.tar", last modified: Thu Jun 29 11:55:48 2023, max compression
```

## Comparing `fair_async_rlock-1.0.3.tar` & `fair_async_rlock-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.3/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.3/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.609452 fair_async_rlock-1.0.3/fair_async_rlock/
--rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.3/fair_async_rlock/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2043 2023-06-15 23:07:46.000000 fair_async_rlock-1.0.3/fair_async_rlock/fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/fair_async_rlock/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.3/fair_async_rlock/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15990 2023-06-15 23:27:05.000000 fair_async_rlock-1.0.3/fair_async_rlock/tests/test_fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.3/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-15 23:33:49.000000 fair_async_rlock-1.0.3/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.4/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.4/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.186770 fair_async_rlock-1.0.4/fair_async_rlock/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.4/fair_async_rlock/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2364 2023-06-29 11:49:51.000000 fair_async_rlock-1.0.4/fair_async_rlock/fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/fair_async_rlock/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.4/fair_async_rlock/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17446 2023-06-29 11:43:58.000000 fair_async_rlock-1.0.4/fair_async_rlock/tests/test_fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.4/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-29 11:50:29.000000 fair_async_rlock-1.0.4/setup.py
```

### Comparing `fair_async_rlock-1.0.3/LICENSE` & `fair_async_rlock-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.3/PKG-INFO` & `fair_async_rlock-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_async_rlock
-Version: 1.0.3
+Version: 1.0.4
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fair_async_rlock-1.0.3/README.md` & `fair_async_rlock-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.3/fair_async_rlock/fair_async_rlock.py` & `fair_async_rlock-1.0.4/fair_async_rlock/fair_async_rlock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from collections import deque
 
 __all__ = ['FairAsyncRLock']
 
+
 class FairAsyncRLock:
     """
     A fair reentrant lock for async programming. Fair means that it respects the order of acquisition.
     """
 
     def __init__(self):
         self._owner: asyncio.Task | None = None
@@ -42,31 +43,40 @@
             await event.wait()
             self._owner = me
             self._count = 1
         except asyncio.CancelledError:
             self._queue.remove(event)
             raise
 
-    async def release(self):
+    def _current_task_release(self):
+        self._count -= 1
+        if self._count == 0:
+            self._owner = None
+            if self._queue:
+                # Wake up the next task in the queue
+                event = self._queue.popleft()
+                event.set()
+
+    def release(self):
         """Release the lock"""
         me = asyncio.current_task()
 
         if self._owner is None:
             raise RuntimeError(f"Cannot release un-acquired lock. {me} tried to release.")
 
         if not self.is_owner(task=me):
             raise RuntimeError(f"Cannot release foreign lock. {me} tried to unlock {self._owner}.")
 
-        self._count -= 1
-        if self._count == 0:
-            self._owner = None
-            if self._queue:
-                # Wake up the next task in the queue
-                event = self._queue.popleft()
-                event.set()
+        self._current_task_release()
 
     async def __aenter__(self):
         await self.acquire()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
-        await self.release()
+        try:
+            self.release()
+        except asyncio.CancelledError as e:
+            if self.is_owner():
+                # If a cancellation happened during release, we force the current task to release.
+                self._current_task_release()
+            raise e
```

### Comparing `fair_async_rlock-1.0.3/fair_async_rlock/tests/test_fair_async_rlock.py` & `fair_async_rlock-1.0.4/fair_async_rlock/tests/test_fair_async_rlock.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,19 +57,19 @@
 
 
 @pytest.mark.asyncio
 async def test_unowned_release():
     lock = FairAsyncRLock()
 
     with pytest.raises(RuntimeError, match="Cannot release un-acquired lock."):
-        await lock.release()
+        lock.release()
 
     async def worker():
         with pytest.raises(RuntimeError, match="Cannot release un-acquired lock."):
-            await lock.release()
+            lock.release()
 
     await asyncio.gather(worker())
 
 
 @pytest.mark.asyncio
 async def test_performance():
     # This test is useful for measuring the overhead of the locking mechanism and can help determine whether it's
@@ -210,15 +210,15 @@
     lock = FairAsyncRLock()
     result = []
 
     async def worker(n):
         await lock.acquire()  # This will block until the lock can be acquired
         result.append(n)
         await asyncio.sleep(0)  # Yield control
-        await lock.release()
+        lock.release()
 
     # Start several tasks concurrently
     tasks = [asyncio.create_task(worker(i)) for i in range(5)]
 
     await asyncio.gather(*tasks)
 
     # All tasks should have been able to acquire the lock, but only one at a time
@@ -275,15 +275,15 @@
     async def task1():
         async with lock:
             await asyncio.sleep(0.1)  # Sleep to ensure that task2 gets to the point where it's waiting for the lock
 
     async def task2():
         # Wait for both tasks to complete
         try:
-            await lock.release()
+            lock.release()
         except RuntimeError as e:
             assert str(e).startswith("Cannot release foreign lock.")
             return
 
     # Create the tasks and schedule them
     task1_handle = asyncio.create_task(task1())
     task2_handle = asyncio.create_task(task2())
@@ -335,20 +335,20 @@
     lock = FairAsyncRLock()
 
     async def failing_task():
         try:
             await lock.acquire()
             raise RuntimeError("Simulated exception during acquire")
         except:
-            await lock.release()
+            lock.release()
             raise
 
     async def succeeding_task():
         await lock.acquire()
-        await lock.release()
+        lock.release()
 
     task1 = asyncio.create_task(failing_task())
     task2 = asyncio.create_task(succeeding_task())
     with pytest.raises(RuntimeError, match="Simulated exception during acquire"):
         await asyncio.gather(task1, task2)
 
     # Ensure that lock is not owned and queue is empty after exception
@@ -360,15 +360,15 @@
 async def test_task_cancellation():
     # We need to verify that if a task is cancelled while waiting for the lock, it gets removed from the queue.
     lock = FairAsyncRLock()
 
     async def task1():
         await lock.acquire()
         await asyncio.sleep(0.1)  # Let's ensure the lock is held for a bit
-        await lock.release()
+        lock.release()
 
     async def task2():
         await lock.acquire()
 
     task1 = asyncio.create_task(task1())
     task2 = asyncio.create_task(task2())
     await asyncio.sleep(0)  # Yield control to allow tasks to start
@@ -484,7 +484,57 @@
     # Wait for all tasks to complete or be cancelled
     await asyncio.gather(*tasks, return_exceptions=True)
 
     await monitor_task
 
     # At least one cancellation should have occurred
     assert cancellation_occurred.is_set()
+
+
+class DelayedFairAsyncRLock(FairAsyncRLock):
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        """Release the lock"""
+        await asyncio.sleep(0.1)
+        await super().__aexit__(exc_type, exc_val, exc_tb)
+
+
+class ExceptionFairAsyncRLock(FairAsyncRLock):
+    def release(self):
+        """Release the lock"""
+        raise asyncio.CancelledError()
+        super().release()
+
+
+@pytest.mark.asyncio
+async def test_delayed_release():
+    lock = DelayedFairAsyncRLock()
+
+    async def first_task():
+        async with lock:
+            await asyncio.sleep(0.1)  # hold lock for a moment
+
+    async def second_task():
+        await asyncio.sleep(0.05)  # wait until first task has lock
+        await lock.acquire()
+        got_lock = lock.is_owner()
+        lock.release()
+        return got_lock
+
+    t1 = asyncio.create_task(first_task())
+    t2 = asyncio.create_task(second_task())
+    await asyncio.gather(t1, t2)
+
+    assert t2.result() is True, "Second task should acquire the lock after the first task has released it"
+
+
+@pytest.mark.asyncio
+async def test_exception_on_release_gh7():
+    lock = ExceptionFairAsyncRLock()
+
+    async def task():
+        with pytest.raises(asyncio.CancelledError):
+            async with lock:
+                pass  # no action needed inside
+
+    await asyncio.create_task(task())
+    assert lock._owner is None, "Lock owner should be None after an exception"
+    assert len(lock._queue) == 0, "Lock queue should be empty after an exception"
```

### Comparing `fair_async_rlock-1.0.3/fair_async_rlock.egg-info/PKG-INFO` & `fair_async_rlock-1.0.4/fair_async_rlock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-async-rlock
-Version: 1.0.3
+Version: 1.0.4
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fair_async_rlock-1.0.3/setup.py` & `fair_async_rlock-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='fair_async_rlock',
-      version='1.0.3',
+      version='1.0.4',
       description='A well-tested implementation of a fair asynchronous RLock for concurrent programming.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/Joshuaalbert/FairAsyncRLock",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=[],
```

