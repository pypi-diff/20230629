# Comparing `tmp/spinneroo-0.0.0.tar.gz` & `tmp/spinneroo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinneroo-0.0.0.tar", last modified: Thu Jun 15 21:58:12 2023, max compression
+gzip compressed data, was "spinneroo-1.0.0.tar", last modified: Thu Jun 29 13:55:28 2023, max compression
```

## Comparing `spinneroo-0.0.0.tar` & `spinneroo-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:58:12.314418 spinneroo-0.0.0/
--rw-rw-rw-   0        0        0       98 2023-06-15 21:58:12.000000 spinneroo-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2032 2023-06-15 21:58:12.313440 spinneroo-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1240 2023-06-15 21:54:41.000000 spinneroo-0.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-0.0.0/build.py
--rw-rw-rw-   0        0        0      630 2023-06-15 21:55:26.000000 spinneroo-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       30 2023-06-15 21:50:53.000000 spinneroo-0.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 21:58:12.314418 spinneroo-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1546 2023-06-15 21:54:41.000000 spinneroo-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:58:12.295419 spinneroo-0.0.0/spinneroo/
--rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-0.0.0/spinneroo/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 spinneroo-0.0.0/spinneroo/base.py
--rw-rw-rw-   0        0        0      284 2023-06-15 21:53:26.000000 spinneroo-0.0.0/spinneroo/document.py
--rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-0.0.0/spinneroo/elements.py
--rw-rw-rw-   0        0        0     8236 2023-06-15 21:42:21.000000 spinneroo-0.0.0/spinneroo/progress.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:58:12.312450 spinneroo-0.0.0/spinneroo.egg-info/
--rw-rw-rw-   0        0        0     2032 2023-06-15 21:58:12.000000 spinneroo-0.0.0/spinneroo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-15 21:58:12.000000 spinneroo-0.0.0/spinneroo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:58:12.000000 spinneroo-0.0.0/spinneroo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-15 21:58:12.000000 spinneroo-0.0.0/spinneroo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 21:58:12.000000 spinneroo-0.0.0/spinneroo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 13:55:28.512052 spinneroo-1.0.0/
+-rw-rw-rw-   0        0        0       98 2023-06-29 13:55:28.000000 spinneroo-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2032 2023-06-29 13:55:28.511053 spinneroo-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1240 2023-06-15 21:54:41.000000 spinneroo-1.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.0.0/build.py
+-rw-rw-rw-   0        0        0      630 2023-06-29 13:55:28.000000 spinneroo-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:55:28.512052 spinneroo-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2023-06-29 13:55:15.000000 spinneroo-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:55:28.495082 spinneroo-1.0.0/spinneroo/
+-rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.0.0/spinneroo/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 spinneroo-1.0.0/spinneroo/base.py
+-rw-rw-rw-   0        0        0      284 2023-06-15 21:53:26.000000 spinneroo-1.0.0/spinneroo/document.py
+-rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.0.0/spinneroo/elements.py
+-rw-rw-rw-   0        0        0     9908 2023-06-29 13:54:53.000000 spinneroo-1.0.0/spinneroo/progress.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:55:28.510053 spinneroo-1.0.0/spinneroo.egg-info/
+-rw-rw-rw-   0        0        0     2032 2023-06-29 13:55:28.000000 spinneroo-1.0.0/spinneroo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-29 13:55:28.000000 spinneroo-1.0.0/spinneroo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:55:28.000000 spinneroo-1.0.0/spinneroo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-29 13:55:28.000000 spinneroo-1.0.0/spinneroo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-29 13:55:28.000000 spinneroo-1.0.0/spinneroo.egg-info/top_level.txt
```

### Comparing `spinneroo-0.0.0/PKG-INFO` & `spinneroo-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 0.0.0
+Version: 1.0.0
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spinneroo-0.0.0/README.md` & `spinneroo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `spinneroo-0.0.0/build.py` & `spinneroo-1.0.0/build.py`

 * *Files identical despite different names*

### Comparing `spinneroo-0.0.0/pyproject.toml` & `spinneroo-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'spinneroo'
-version = '0.0.0'
+version = '1.0.0'
 description = 'A module for displaying progress messages and timers with spinners in the command line.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `spinneroo-0.0.0/setup.py` & `spinneroo-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='spinneroo',
-        version='0.0.0',
+        version='1.0.0',
         description=(
             "A module for displaying progress messages and "
             "timers with spinners in the command line."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `spinneroo-0.0.0/spinneroo/base.py` & `spinneroo-1.0.0/spinneroo/base.py`

 * *Files identical despite different names*

### Comparing `spinneroo-0.0.0/spinneroo/progress.py` & `spinneroo-1.0.0/spinneroo/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # progress.py
 
 import sys
 import datetime as dt
 import time
+import warnings
 from time import strftime
 from time import gmtime
 
 import threading
 from typing import (
     Optional, Type, Generator, Iterable,
     Union, Any, Callable, Literal
@@ -135,33 +136,40 @@
 
         if elements is None:
             elements = self.ELEMENTS
         # end if
 
         self.message = message
         self.complete = complete
-        self.title = title or ""
-        self.delay = delay or self.DELAY
         self.silence = silence
         self.stay = stay
         self.counter = counter
         self.clean = clean
         self.elements = elements
 
-        self.spinner_generator = self.spinning_cursor()
+        self.title = title or ""
+        self.delay = delay or self.DELAY
+
+        self._paused = False
+
+        self._spinner_generator = self._spinning_cursor()
 
-        self.running = False
+        self._running = False
 
-        self.start = None
-        self.time = None
-        self.output = None
+        self.start: Optional[float] = None
+        self.time: Optional[float] = None
+        self.output: Optional[str] = None
     # end __init__
 
     def __enter__(self) -> Any:
-        """Enters the object to run the task."""
+        """
+        Enters the object to run the task.
+
+        :return: The object.
+        """
 
         self.spin()
 
         return self
     # end __enter__
 
     def __exit__(
@@ -185,22 +193,67 @@
         if exception is not None:
             return False
         # end if
 
         return True
     # end __exit__
 
+    @property
+    def paused(self) -> bool:
+        """Returns the value of the property."""
+
+        return self._paused
+    # end paused
+
+    @property
+    def running(self) -> bool:
+        """Returns the value of the property."""
+
+        return self._running
+    # end running
+
+    def pause(self) -> None:
+        """Pauses the process."""
+
+        if self.paused:
+            warnings.warn(
+                f"Attempting to pause {self} "
+                f"when the process is paused."
+            )
+        # end if
+
+        self._paused = True
+    # end pause
+
+    def unpause(self) -> None:
+        """Unpauses the process."""
+
+        if not self.paused:
+            warnings.warn(
+                f"Attempting to unpause {self} "
+                f"when the process is running."
+            )
+        # end if
+
+        self._paused = False
+    # end unpause
+
     def stop(self) -> None:
+        """Stops the spinning process."""
 
-        self.running = False
+        self._running = False
 
         Spinner.instances.remove(self)
 
         Spinner.RUNNING = bool(Spinner.instances)
 
+        if Spinner.instances and Spinner.instances[-1].running:
+            Spinner.instances[-1].unpause()
+        # end if
+
         if self.delay:
             time.sleep(self.delay)
         # end if
 
         if self.clean or self.complete:
             sys.stdout.write(
                 ('\b' * len(self.output)) +
@@ -219,23 +272,29 @@
             sys.stdout.flush()
         # end if
     # ene stop
 
     def spin(self) -> None:
         """Runs the spinner."""
 
-        self.running = True
+        if Spinner.instances and Spinner.instances[-1].running:
+            Spinner.instances[-1].pause()
+        # end if
+
+        self._running = True
+
+        Spinner.RUNNING = True
 
         self.start = time.time()
         self.time = time.time()
 
         threading.Thread(target=self._run).start()
 
         Spinner.instances.append(self)
-    # end start
+    # end spin
 
     def create_message(
             self,
             cursor: Optional[str] = None,
             text: Optional[str] = None
     ) -> str:
         """
@@ -277,65 +336,80 @@
         if not cursor:
             return message + " "
         # end if
 
         return message + " " + cursor + " "
     # end create_message
 
-    def spinning_cursor(self) -> Generator[str, None, None]:
+    def _spinning_cursor(self) -> Generator[str, None, None]:
         """
         Returns the current spinner value.
 
         :return: The current state of the cursor.
         """
 
         while True:
             for cursor in self.elements:
                 self.time = time.time()
 
                 if self.silence:
-                    continue
+                    yield ""
                 # end if
 
                 self.output = self.create_message(
                     cursor=cursor, text=self.message
                 )
 
                 yield self.output
             # end for
         # end while
-    # end spinning_cursor
+    # end _spinning_cursor
 
-    def _run(self) -> None:
+    def step(self) -> None:
         """Runs the spinning wheel."""
 
         delay = self.delay
 
         if isinstance(delay, dt.timedelta):
             delay = delay.total_seconds()
         # end if
 
-        while (
-            self.running and
-            (
-                (self.stay is None) or
-                (callable(self.stay) and self.stay())
-            )
-        ):
-            Spinner.RUNNING = True
+        next_output = ""
 
-            next_output = next(self.spinner_generator)
+        if not self.paused:
+            next_output = next(self._spinner_generator)
 
             sys.stdout.write(next_output)
             sys.stdout.flush()
+        # end if
 
-            if delay:
-                time.sleep(delay)
-            # end if
+        if delay:
+            time.sleep(delay)
+        # end if
 
-            sys.stdout.write('\b' * len(next_output) * 2)
+        if not self.paused:
+            sys.stdout.write('\b' * len(next_output))
             sys.stdout.flush()
+        # end if
+    # end step
+
+    def _run(self) -> None:
+        """Runs the spinning wheel."""
+
+        sys.stdout.write(
+            ('\b' * 200)
+        )
+        sys.stdout.flush()
+
+        while (
+            self._running and
+            (
+                (self.stay is None) or
+                (callable(self.stay) and self.stay())
+            )
+        ):
+            self.step()
         # end while
-    # end spinner_task
+    # end _run
 # end Spinner
 
 spinner = Spinner
```

### Comparing `spinneroo-0.0.0/spinneroo.egg-info/PKG-INFO` & `spinneroo-1.0.0/spinneroo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 0.0.0
+Version: 1.0.0
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

