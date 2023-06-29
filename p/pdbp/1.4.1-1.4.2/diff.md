# Comparing `tmp/pdbp-1.4.1.tar.gz` & `tmp/pdbp-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.4.1.tar", last modified: Thu Jun 22 15:50:46 2023, max compression
+gzip compressed data, was "pdbp-1.4.2.tar", last modified: Thu Jun 29 21:48:04 2023, max compression
```

## Comparing `pdbp-1.4.1.tar` & `pdbp-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:50:46.460670 pdbp-1.4.1/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.1/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.1/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.1/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.1/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-22 15:50:46.460728 pdbp-1.4.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4805 2023-06-22 15:48:47.000000 pdbp-1.4.1/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.1/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-06-22 15:50:46.460919 pdbp-1.4.1/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5379 2023-06-22 15:48:47.000000 pdbp-1.4.1/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:50:46.460029 pdbp-1.4.1/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.1/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:50:46.460562 pdbp-1.4.1/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      109 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    53998 2023-06-22 15:48:47.000000 pdbp-1.4.1/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:48:04.510915 pdbp-1.4.2/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.2/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.2/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.2/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.2/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.2/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-29 21:48:04.510974 pdbp-1.4.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4805 2023-06-22 15:48:47.000000 pdbp-1.4.2/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.2/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-06-29 21:48:04.511145 pdbp-1.4.2/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5379 2023-06-29 21:47:09.000000 pdbp-1.4.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:48:04.510263 pdbp-1.4.2/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.2/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:48:04.510811 pdbp-1.4.2/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      109 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    57865 2023-06-29 21:47:09.000000 pdbp-1.4.2/src/pdbp.py
```

### Comparing `pdbp-1.4.1/.gitignore` & `pdbp-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.1/CODE_OF_CONDUCT.md` & `pdbp-1.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.1/CONTRIBUTING.md` & `pdbp-1.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.1/LICENSE` & `pdbp-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.1/PKG-INFO` & `pdbp-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.1
+Version: 1.4.2
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
```

### Comparing `pdbp-1.4.1/README.md` & `pdbp-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.1/setup.py` & `pdbp-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.4.1",
+    version="1.4.2",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
```

### Comparing `pdbp-1.4.1/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.4.2/src/pdbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.1
+Version: 1.4.2
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
```

### Comparing `pdbp-1.4.1/src/pdbp.py` & `pdbp-1.4.2/src/pdbp.py`

 * *Files 6% similar despite different names*

```diff
@@ -976,15 +976,80 @@
                 if s:
                     last_return_color = self.config.last_return_color
                     if (
                         last_return_color == self.config.pm_return_value_color
                         and not self.config.exception_caught
                     ):
                         print(s, file=self.stdout)
-                    needs_extra_line = True
+                        needs_extra_line = True
+            elif "exc" in frame.f_locals and "msg" in frame.f_locals:
+                s = str(frame.f_locals["msg"]).strip()
+                e = str(frame.f_locals["exc"]).strip()
+                e = e.split("<class '")[-1].split("'>")[0] + ":"
+                if s and self.has_traceback:
+                    if self.config.highlight:
+                        the_return_color = self.__get_return_color(s)
+                        s = Color.set(the_return_color, s)
+                        e = Color.set(the_return_color, e)
+                    last_return_color = self.config.last_return_color
+                    lastline = None
+                    try:
+                        lastline = inspect.getsourcelines(self.curframe)[0][-1]
+                        lastline = str(lastline)
+                    except Exception:
+                        lastline = ""
+                    if (
+                        last_return_color == self.config.pm_return_value_color
+                        and not self.config.exception_caught
+                        and "raise " in lastline
+                        and "(msg" in lastline.replace(" ", "")
+                    ):
+                        print(e, file=self.stdout)
+                        print(" " + s, file=self.stdout)
+                        needs_extra_line = True
+            elif "msg" in frame.f_locals or "message" in frame.f_locals:
+                s = None
+                s2 = None
+                if "msg" in frame.f_locals:
+                    s = str(frame.f_locals["msg"]).strip()
+                if "message" in frame.f_locals:
+                    s2 = str(frame.f_locals["message"]).strip()
+                if (s or s2) and self.has_traceback:
+                    if self.config.highlight:
+                        if s:
+                            the_return_color = self.__get_return_color(s)
+                            s = Color.set(the_return_color, s)
+                        if s2:
+                            the_return_color_2 = self.__get_return_color(s2)
+                            s2 = Color.set(the_return_color_2, s2)
+                    last_return_color = self.config.last_return_color
+                    lastline = None
+                    try:
+                        lastline = inspect.getsourcelines(self.curframe)[0][-1]
+                        lastline = str(lastline)
+                    except Exception:
+                        lastline = ""
+                    if (
+                        last_return_color == self.config.pm_return_value_color
+                        and not self.config.exception_caught
+                        and "raise " in lastline
+                        and s
+                        and "(msg" in lastline.replace(" ", "")
+                    ):
+                        print(s, file=self.stdout)
+                        needs_extra_line = True
+                    elif (
+                        last_return_color == self.config.pm_return_value_color
+                        and not self.config.exception_caught
+                        and "raise " in lastline
+                        and s2
+                        and "(message" in lastline.replace(" ", "")
+                    ):
+                        print(s2, file=self.stdout)
+                        needs_extra_line = True
             if "__return__" in frame.f_locals:
                 rv = frame.f_locals["__return__"]
                 try:
                     s = repr(rv)
                 except KeyboardInterrupt:
                     raise
                 except Exception:
@@ -1009,20 +1074,31 @@
     def _format_exc_for_sticky(self, exc):
         if len(exc) != 2:
             return "pdbp: got unexpected __exception__: %r" % (exc,)
         exc_type, exc_value = exc
         s = ""
         try:
             try:
-                s = exc_type.__name__
+                try:
+                    module = str(exc_type.__module__)
+                    module = module.split("<class '")[-1].split("'>")[0]
+                    if module != "builtins":
+                        s = module + "." + exc_type.__name__.strip()
+                    else:
+                        s = exc_type.__name__.strip()
+                except Exception:
+                    s = exc_type.__name__.strip()
             except AttributeError:
-                s = str(exc_type)
+                s = str(exc_type).strip()
             if exc_value is not None:
                 s += ": "
-                s += str(exc_value)
+                s2 = str(exc_value)
+                if s2.startswith("Message:") and s2.count("Message:") == 1:
+                    s2 = "\n " + s2.split("Message:")[-1].strip()
+                s += s2
         except KeyboardInterrupt:
             raise
         except Exception as exc:
             try:
                 s += "(unprintable exception: %r)" % (exc,)
             except Exception:
                 s += "(unprintable exception)"
```

