# Comparing `tmp/fspath-20230218.tar.gz` & `tmp/fspath-20230629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fspath-20230218.tar", last modified: Sat Feb 18 16:36:11 2023, max compression
+gzip compressed data, was "fspath-20230629.tar", last modified: Thu Jun 29 16:49:54 2023, max compression
```

## Comparing `fspath-20230218.tar` & `fspath-20230629.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-02-18 16:36:11.088311 fspath-20230218/
--rw-rw-r--   0 markus   (10001) markus   (10001)    34520 2023-02-18 16:34:18.000000 fspath-20230218/LICENSE
--rw-rw-r--   0 markus   (10001) markus   (10001)     1738 2023-02-18 16:36:11.092311 fspath-20230218/PKG-INFO
--rw-rw-r--   0 markus   (10001) markus   (10001)      957 2023-02-18 16:34:18.000000 fspath-20230218/README.rst
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-02-18 16:36:11.088311 fspath-20230218/fspath/
--rwxr-xr-x   0 markus   (10001) markus   (10001)     1012 2018-06-23 15:13:29.000000 fspath-20230218/fspath/__init__.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     1441 2023-02-18 16:34:23.000000 fspath-20230218/fspath/__pkginfo__.py
--rw-r--r--   0 markus   (10001) markus   (10001)     2510 2018-06-23 15:13:29.000000 fspath-20230218/fspath/_which.py
--rwxr-xr-x   0 markus   (10001) markus   (10001)     8543 2018-06-23 15:13:29.000000 fspath-20230218/fspath/cli.py
--rw-r--r--   0 markus   (10001) markus   (10001)      868 2018-06-23 15:13:29.000000 fspath-20230218/fspath/compat.py
--rw-r--r--   0 markus   (10001) markus   (10001)     4294 2018-06-23 15:13:29.000000 fspath-20230218/fspath/console.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    11656 2019-03-23 16:16:09.000000 fspath-20230218/fspath/debug.py
--rwxr-xr-x   0 markus   (10001) markus   (10001)    23609 2019-01-10 11:21:04.000000 fspath-20230218/fspath/fspath.py
--rw-r--r--   0 markus   (10001) markus   (10001)     1538 2018-06-23 15:13:29.000000 fspath-20230218/fspath/helper.py
--rw-r--r--   0 markus   (10001) markus   (10001)     3383 2018-06-23 15:13:29.000000 fspath-20230218/fspath/main.py
--rwxr-xr-x   0 markus   (10001) markus   (10001)      807 2018-06-23 15:13:29.000000 fspath-20230218/fspath/os_env.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     1429 2019-03-23 17:08:09.000000 fspath-20230218/fspath/progressbar.py
--rwxr-xr-x   0 markus   (10001) markus   (10001)    16559 2018-06-23 15:13:29.000000 fspath-20230218/fspath/sui.py
--rw-r--r--   0 markus   (10001) markus   (10001)     2666 2018-06-23 15:13:29.000000 fspath-20230218/fspath/win.py
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-02-18 16:36:11.088311 fspath-20230218/fspath.egg-info/
--rw-rw-r--   0 markus   (10001) markus   (10001)     1738 2023-02-18 16:36:11.000000 fspath-20230218/fspath.egg-info/PKG-INFO
--rw-rw-r--   0 markus   (10001) markus   (10001)      542 2023-02-18 16:36:11.000000 fspath-20230218/fspath.egg-info/SOURCES.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)        1 2023-02-18 16:36:11.000000 fspath-20230218/fspath.egg-info/dependency_links.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)       74 2023-02-18 16:36:11.000000 fspath-20230218/fspath.egg-info/entry_points.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)        4 2023-02-18 16:36:11.000000 fspath-20230218/fspath.egg-info/requires.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)        7 2023-02-18 16:36:11.000000 fspath-20230218/fspath.egg-info/top_level.txt
--rw-r--r--   0 markus   (10001) markus   (10001)       61 2023-02-18 16:36:11.092311 fspath-20230218/setup.cfg
--rwxr-xr-x   0 markus   (10001) markus   (10001)     1369 2018-06-23 15:13:29.000000 fspath-20230218/setup.py
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-02-18 16:36:11.088311 fspath-20230218/tests/
--rw-r--r--   0 markus   (10001) markus   (10001)      967 2018-06-23 15:13:29.000000 fspath-20230218/tests/test_FSPath.py
--rw-r--r--   0 markus   (10001) markus   (10001)      243 2018-06-23 15:13:29.000000 fspath-20230218/tests/test_OS_ENV.py
--rw-r--r--   0 markus   (10001) markus   (10001)     3109 2018-06-23 15:13:29.000000 fspath-20230218/tests/test_UI.py
--rw-r--r--   0 markus   (10001) markus   (10001)      418 2018-06-23 15:13:29.000000 fspath-20230218/tests/test_import_all.py
+drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-06-29 16:49:54.043486 fspath-20230629/
+-rw-rw-r--   0 markus   (10001) markus   (10001)    34520 2023-02-18 16:34:18.000000 fspath-20230629/LICENSE
+-rw-rw-r--   0 markus   (10001) markus   (10001)     1738 2023-06-29 16:49:54.043486 fspath-20230629/PKG-INFO
+-rw-rw-r--   0 markus   (10001) markus   (10001)      957 2023-02-18 16:34:18.000000 fspath-20230629/README.rst
+drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-06-29 16:49:54.039486 fspath-20230629/fspath/
+-rwxr-xr-x   0 markus   (10001) markus   (10001)     1011 2023-06-29 13:42:27.000000 fspath-20230629/fspath/__init__.py
+-rw-rw-r--   0 markus   (10001) markus   (10001)     1441 2023-06-29 16:43:09.000000 fspath-20230629/fspath/__pkginfo__.py
+-rw-r--r--   0 markus   (10001) markus   (10001)     2539 2023-06-29 14:47:16.000000 fspath-20230629/fspath/_which.py
+-rwxr-xr-x   0 markus   (10001) markus   (10001)     8716 2023-06-29 14:04:25.000000 fspath-20230629/fspath/cli.py
+-rw-r--r--   0 markus   (10001) markus   (10001)      867 2023-06-29 13:42:33.000000 fspath-20230629/fspath/compat.py
+-rw-r--r--   0 markus   (10001) markus   (10001)     4301 2023-06-29 13:54:58.000000 fspath-20230629/fspath/console.py
+-rwxrwxr-x   0 markus   (10001) markus   (10001)    11628 2023-06-29 13:59:49.000000 fspath-20230629/fspath/debug.py
+-rwxr-xr-x   0 markus   (10001) markus   (10001)    23677 2023-06-29 16:11:17.000000 fspath-20230629/fspath/fspath.py
+-rw-r--r--   0 markus   (10001) markus   (10001)     1538 2018-06-23 15:13:29.000000 fspath-20230629/fspath/helper.py
+-rw-r--r--   0 markus   (10001) markus   (10001)     3475 2023-06-29 13:54:12.000000 fspath-20230629/fspath/main.py
+-rwxr-xr-x   0 markus   (10001) markus   (10001)      807 2018-06-23 15:13:29.000000 fspath-20230629/fspath/os_env.py
+-rwxrwxr-x   0 markus   (10001) markus   (10001)     1474 2023-06-29 16:23:50.000000 fspath-20230629/fspath/progressbar.py
+-rwxr-xr-x   0 markus   (10001) markus   (10001)    16494 2023-06-29 14:02:50.000000 fspath-20230629/fspath/sui.py
+-rw-r--r--   0 markus   (10001) markus   (10001)     2716 2023-06-29 13:42:15.000000 fspath-20230629/fspath/win.py
+drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-06-29 16:49:54.039486 fspath-20230629/fspath.egg-info/
+-rw-rw-r--   0 markus   (10001) markus   (10001)     1738 2023-06-29 16:49:53.000000 fspath-20230629/fspath.egg-info/PKG-INFO
+-rw-rw-r--   0 markus   (10001) markus   (10001)      542 2023-06-29 16:49:54.000000 fspath-20230629/fspath.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus   (10001) markus   (10001)        1 2023-06-29 16:49:53.000000 fspath-20230629/fspath.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus   (10001) markus   (10001)       74 2023-06-29 16:49:53.000000 fspath-20230629/fspath.egg-info/entry_points.txt
+-rw-rw-r--   0 markus   (10001) markus   (10001)        4 2023-06-29 16:49:53.000000 fspath-20230629/fspath.egg-info/requires.txt
+-rw-rw-r--   0 markus   (10001) markus   (10001)        7 2023-06-29 16:49:53.000000 fspath-20230629/fspath.egg-info/top_level.txt
+-rw-r--r--   0 markus   (10001) markus   (10001)       61 2023-06-29 16:49:54.043486 fspath-20230629/setup.cfg
+-rwxrwxr-x   0 markus   (10001) markus   (10001)     1890 2023-06-29 16:23:50.000000 fspath-20230629/setup.py
+drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-06-29 16:49:54.043486 fspath-20230629/tests/
+-rw-rw-r--   0 markus   (10001) markus   (10001)      944 2023-06-29 16:23:50.000000 fspath-20230629/tests/test_FSPath.py
+-rw-r--r--   0 markus   (10001) markus   (10001)      243 2018-06-23 15:13:29.000000 fspath-20230629/tests/test_OS_ENV.py
+-rw-r--r--   0 markus   (10001) markus   (10001)     3109 2018-06-23 15:13:29.000000 fspath-20230629/tests/test_UI.py
+-rw-r--r--   0 markus   (10001) markus   (10001)      418 2018-06-23 15:13:29.000000 fspath-20230629/tests/test_import_all.py
```

### Comparing `fspath-20230218/LICENSE` & `fspath-20230629/LICENSE`

 * *Files identical despite different names*

### Comparing `fspath-20230218/PKG-INFO` & `fspath-20230629/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fspath
-Version: 20230218
+Version: 20230629
 Summary: semantic path names and more
 Home-page: https://github.com/return42/fspath
 Author: Markus Heiser
 Author-email: markus.heiser@darmarIT.de
 License: AGPLv3
 Keywords: path-names development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fspath-20230218/README.rst` & `fspath-20230629/README.rst`

 * *Files identical despite different names*

### Comparing `fspath-20230218/fspath/__init__.py` & `fspath-20230629/fspath/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,7 @@
 from .fspath import DevNull
 
 from .cli    import CLI
 from .os_env import OS_ENV
 from ._which import which
 
 from .progressbar import progressbar
-
```

### Comparing `fspath-20230218/fspath/__pkginfo__.py` & `fspath-20230629/fspath/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=invalid-name,redefined-builtin
 """
 python package meta informations
 """
 import platform
 
 package      = 'fspath'
-version      = '20230218'
+version      = '20230629'
 authors      = ['Markus Heiser', ]
 emails       = ['markus.heiser@darmarIT.de', ]
 copyright    = '2023 Markus Heiser'
 url          = 'https://github.com/return42/fspath'
 description  = 'semantic path names and more'
 license      = 'AGPLv3'
 keywords     = "path-names development"
```

### Comparing `fspath-20230218/fspath/_which.py` & `fspath-20230629/fspath/_which.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 u"""
 which - locate a command
 """
 # pylint: disable=invalid-name
 
 import sys
 import os
-import fspath
+import fspath  # pylint: disable=cyclic-import
 from .cli import CLI
 
 
 # ==============================================================================
 def which(cmd, findall=True):
 # ==============================================================================
     u"""Searches the fname in the ``PATH`` enviroment.
@@ -21,15 +21,15 @@
 
     If nothing is found, ``None`` is returned. If something matches, a list is
     returned. With option ``findall=False`` the first match is returned or
     ``None``, if nothing is found.
 
     """
     envpath = os.environ.get('PATH', None) or os.defpath
-    hits = list()
+    hits = []
     cmd  = fspath.FSPath(cmd)
 
     if sys.platform == 'win32':
         exe = [x.lower() for x in os.environ.get("PATHEXT", [""]).split(";")]
         for folder in envpath.split(os.pathsep):
             for ext in exe:
                 fullname = fspath.FSPath(folder) / cmd + ext
```

### Comparing `fspath-20230218/fspath/cli.py` & `fspath-20230629/fspath/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             , action  = 'store_true'
             , help    = 'run in quiet mode' )
 
     def addCMDParser(self, func, cmdName=None):
         """Add subcommand parser"""
 
         if self.cliSubParsers is None:
+            # pylint: disable=broad-exception-raised
             raise Exception("this command-line has no sub-commands!")
 
         subCmd = self.cliSubParsers.add_parser(
             cmdName or func.__name__
             , epilog          = func.__doc__
             , formatter_class = HelpFormatter
             , help            = ((func.__doc__ or "").strip().split("\n") + [ "sorry, no help available" ])[0]
@@ -159,22 +160,22 @@
             else:
                 _retVal = self.cmdFunc(cmd_args)
             try:
                 if _retVal is None:
                     _exitCode = 0
                 else:
                     _exitCode = int(_retVal)
-            except Exception as exc: # pylint: disable=W0703
+            except Exception as exc: # pylint: disable=unused-variable, broad-exception-caught
                 pass
 
-        except CLIApplError as exc: # pylint: disable=W0703
+        except CLIApplError as exc: # pylint: disable=unused-variable
             _exitCode  = exc.exitCode
             self.ERR.write(u"ERROR (%s): %s\n" % (exc.exitCode, exc.message))
 
-        except Exception as exc: # pylint: disable=W0703
+        except Exception as exc: # pylint: disable=unused-variable, broad-exception-caught
             if cmd_args.debug:
                 raise
             _exitCode  = 42
             _exception = str(exc)
             sys.stderr.write(u"FATAL ERROR: %s\n" % _exception)
         sys.exit(_exitCode)
 
@@ -208,15 +209,15 @@
         ..
         """
 
         # only complete when called from _py_argcomplete()
         if '_ARGCOMPLETE' not in os.environ:
             return
         try:
-            import argcomplete  # pylint: disable=import-error
+            import argcomplete  # pylint: disable=import-error, import-outside-toplevel
         except ImportError:
             self.ERR.write("TAB-completion, python-argcomplete not installed.")
             sys.exit(1)
         argcomplete.autocomplete(self.parser)
 
 
 def CONSOLE(arround=5, frame=None):
@@ -233,15 +234,15 @@
     lineNo = frame.f_lineno
 
     ns = dict(**frame.f_globals)
     ns.update(**frame.f_locals)
 
     histfile = os.path.join(os.path.expanduser("~"), ".kernel-doc-history")
     try:
-        import readline, rlcompleter  # pylint: disable=W0612
+        import readline, rlcompleter  # pylint: disable=import-outside-toplevel
         readline.set_completer(rlcompleter.Completer(namespace=ns).complete)
         readline.parse_and_bind("tab: complete")
         readline.set_history_length(1000)
         if os.path.exists(histfile):
             readline.read_history_file(histfile)
     except ImportError:
         readline = None
@@ -270,8 +271,7 @@
     fName  = frame.f_code.co_filename
     lineNo = frame.f_lineno
     sys.stderr.write("%s:%s: [WARNING] usage of CONSOLE / debug not activated!\n" % (fName, lineNo))
 
 __builtins__["CONSOLE"] = DUMMY_CONSOLE
 if DEBUG:
     __builtins__["CONSOLE"] = CONSOLE
-
```

### Comparing `fspath-20230218/fspath/compat.py` & `fspath-20230629/fspath/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
                 return line.strip()
 
         def prefixed_lines():
             # type: () -> Generator
             for line in text.splitlines(True):
                 yield (prefix + line if predicate(line) else line)
         return ''.join(prefixed_lines())
-
```

### Comparing `fspath-20230218/fspath/console.py` & `fspath-20230629/fspath/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- mode: python; coding: utf-8 -*-
-# pylint: disable=invalid-name, bad-continuation
+# pylint: disable=invalid-name
 """
 Some *console* stuff
 """
 
 import os
 import sys
 
@@ -61,15 +61,15 @@
 def consoleDimensionsLinux():
     u"""Returns count of (row, columns) from current console"""
     rows, columns = os.popen('stty size', 'r').read().split()
     return rows, columns
 
 def consoleDimensionsWIN():
     u"""Returns count of (row, columns) from current console"""
-    # pylint: disable=too-many-locals
+    # pylint: disable=too-many-locals, import-outside-toplevel
     from ctypes import windll, create_string_buffer
 
     # stdin handle is -10
     # stdout handle is -11
     # stderr handle is -12
 
     h = windll.kernel32.GetStdHandle(-12)
```

### Comparing `fspath-20230218/fspath/debug.py` & `fspath-20230629/fspath/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; mode: python -*-
-# pylint: disable=invalid-name, logging-not-lazy
+# pylint: disable=invalid-name, logging-not-lazy, arguments-renamed
 
 """
 Small collection for debugging and introspection purpose.
 """
 
 # ==============================================================================
 #  imports ...
@@ -215,15 +215,15 @@
         console.interact(port, banner=banner)
 
 
 # ==============================================================================
 class Pdb(pdb.Pdb):  # pylint: disable=R0904
 # ==============================================================================
 
-    # pylint: disable=no-self-use, missing-docstring
+    # pylint: disable=missing-docstring
     u"""Abstraction Layer for PDB"""
     def do_src(self, arg):
         if not arg:
             arg = 3
         six.print_(descrFrame(self.curframe, int(arg)))
 
     def help_src(self):
@@ -241,16 +241,15 @@
 
 
 # ==============================================================================
 class RemotePdb(Pdb): # pylint: disable=R0904
 # ==============================================================================
     u"""Simple remote PDB"""
 
-    # pylint: disable=no-self-use, missing-docstring
-    # pylint: disable=super-init-not-called
+    # pylint: disable=missing-docstring, super-init-not-called
     def __init__(self, port, addr="127.0.0.1"):
         """Initialize the socket and initialize pdb."""
 
         self.old_stdout = sys.stdout
         self.old_stderr = sys.stderr
         self.old_stdin  = sys.stdin
```

### Comparing `fspath-20230218/fspath/fspath.py` & `fspath-20230629/fspath/fspath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8; mode: python -*-
 u"""
 semantic path names and much more
 """
 
-# pylint: disable=invalid-name, bad-continuation
+# pylint: disable=invalid-name
 
 # ==============================================================================
 # imports
 # ==============================================================================
 
 import sys
 import io
@@ -258,19 +258,18 @@
     def POSIXPATH(self):
         u"""The path name in *POSIX* notation.
 
         Helpfull if you are on MS-Windows and need the POSIX name.
         """
         if os.sep == "/":
             return six.text_type(self)
-        else:
-            p = six.text_type(self)
-            if p[1] == ":":
-                p = "/" + p.replace(":", "", 1)
-            return p.replace(os.sep, "/")
+        p = six.text_type(self)
+        if p[1] == ":":
+            p = "/" + p.replace(":", "", 1)
+        return p.replace(os.sep, "/")
 
     @property
     def NTPATH(self):
         u"""The path name in the Windows (NT) notation.
         """
         retVal = None
         if os.sep == "\\":
@@ -516,15 +515,15 @@
         if system == 'Windows':
             os.startfile(self) # pylint: disable=no-member
             return
         cmd = 'xdg-open'
         if system in ('FreeBSD', 'Darwin'):
             cmd = 'open'
 
-        from ._which import which
+        from ._which import which  # pylint: disable=import-outside-toplevel, cyclic-import
         cmd = which(cmd, findall=False)
         if cmd:
             os.system(cmd + " " + self)
 
     def readFile(self, encoding='utf-8', errors='strict'):
         u"""read entire file"""
         with self.openTextFile(encoding=encoding, errors=errors) as f:
@@ -692,15 +691,15 @@
        from fspath import callEXE
        out, err, rc = callEXE("arp", "-a")
 
        print("stdout: %s" % out)
        print("stderr: %s" % err)
        print("exit code = %d" % rc)
     """
-    from ._which import which
+    from ._which import which  # pylint: disable=import-outside-toplevel, cyclic-import
     exe = which(cmd, findall=False)
     if exe is None:
         raise IOError('command "%s" not availble!' % cmd)
     proc = exe.Popen(*args, **kwargs)
     stdout, stderr = proc.communicate()
     retVal = proc.returncode
     return (stdout, stderr, retVal)
```

### Comparing `fspath-20230218/fspath/helper.py` & `fspath-20230629/fspath/helper.py`

 * *Files identical despite different names*

### Comparing `fspath-20230218/fspath/main.py` & `fspath-20230629/fspath/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     u"""list file names matching regular expression
 
     To find e.g. all '.py' files in current folder use::
 
         fspath find ".*\\.py$"  .
     """
     for match in cli.folder.reMatchFind(
+            # pylint: disable=superfluous-parens
             cli.regexpr, use_dirs=(not cli.nodirs), use_files=(not cli.nofiles)):
         cli.OUT.write(match + "\n")
 
 def _cli_extract(cli):
     u"""extract TAR or ZIP file"""
     verbose = False
     try:
@@ -51,15 +52,15 @@
 # ==============================================================================
 
     u"""
     Tools from the fspath library
     """
     cli = CLI(description=main.__doc__)
 
-    from .win import _cli_py2exe
+    from .win import _cli_py2exe  # pylint: disable=import-outside-toplevel
     py2exe = cli.addCMDParser(_cli_py2exe, cmdName='py2exe')
     py2exe.add_argument(
         "script"
         , type = FSPath
         , help = "pathname of the script to wrap")
     py2exe.add_argument(
         "--shebang"
```

### Comparing `fspath-20230218/fspath/os_env.py` & `fspath-20230629/fspath/os_env.py`

 * *Files identical despite different names*

### Comparing `fspath-20230218/fspath/progressbar.py` & `fspath-20230629/fspath/progressbar.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,18 +32,19 @@
     Show progress-bar
 
     * step: step number
     * maxSteps: max. steps
     * barSize: char length of the progress-bar
     """
 
-    percent = float(100)/maxSteps*step
+    percent = 0
+    if step and maxSteps:
+        percent = float(100)/maxSteps*step
 
     prompt = "\r" + prompt
     if barSize is None:
         barSize = consoleDimension()[1]
         barSize = barSize - 3 - len(prompt) - len(" %3d%%"  % (100,))
 
     p_bar = fillchar * int(round(percent / 100 * barSize))
     pipe.write((prompt +  "[%s] %3.0f%%") % (p_bar.ljust(barSize, restchar), percent))
     pipe.flush()
-
```

### Comparing `fspath-20230218/fspath/sui.py` & `fspath-20230629/fspath/sui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- mode: python; coding: utf-8 -*-
 """
 Simple user interface via terminal (win & \*nix)
 
 This module is in a very early stage, don't use it!
 """
-# pylint: disable=invalid-name, bad-continuation, wrong-import-position
+# pylint: disable=invalid-name, wrong-import-position
 
 # ==============================================================================
 # imports
 # ==============================================================================
 
 import os
 import sys
@@ -48,16 +48,17 @@
 
     def __init__(self, cli=None):
         if cli is not None:
             self.cli    = cli
             self.ui_out = cli.OUT
 
     if CONSOLE_TYPE == 'tty':
-        import tty     # pylint: disable=E0401
-        import termios # pylint: disable=E0401
+        # pylint: disable=import-outside-toplevel
+        import tty
+        import termios
         @classmethod
         def getchr(cls):
             "Get a single unicode character on Linux & Unix."
             f = cls.ui_in.fileno()
             m = termios.tcgetattr(f)
             try:
                 tty.setraw(f)
@@ -82,15 +83,15 @@
             if ord(c3) != 0x33:
                 return c1 + c2 + c3
             c4 = cls.getchr()
             return c1 + c2 + c3 + c4
 
 
     elif CONSOLE_TYPE == 'cmd':
-        import msvcrt   # pylint: disable=E0401
+        import msvcrt   # pylint: disable=import-outside-toplevel
         @classmethod
         def getchr(cls):
             "Get a single unicode character on Windows."
             ch = msvcrt.getwch()
             if ch == KEY.CTRL_C:
                 raise KeyboardInterrupt
             return ch
@@ -276,15 +277,15 @@
         prompt = _PathMinibuffer(msg, cls)
         prompt(default)
 
         while 1: # pylint: disable=too-many-nested-blocks
             ch = cls.readkey()
             if ch == stop_char:
                 break
-            elif ch == KEY.BACKSPACE:
+            if ch == KEY.BACKSPACE:
                 if in_fspath:
                     in_fspath = in_fspath[:-1]
                     prompt(in_fspath)
 
             elif ch == KEY.TAB:
                 compl = [re.sub(r"^" + re.escape(in_fspath), '', p, count=1)
                          for p in glob(in_fspath + '.*') + glob(in_fspath + '*')]
@@ -415,24 +416,24 @@
     col_start,       col_end      = "",   " "
     sep_start,       sep_end      = "",   " "
     sep_line = "="
 
     def __init__(self, *cols):
         self.coldef = cols
 
-    def get_value(self, attr, row, default='?'):  # pylint: disable=no-self-use
+    def get_value(self, attr, row, default='?'):
         u"""get value from col (attr) and row"""
         val = default
         if hasattr(row, "__getitem__"):
             val = row.get(attr, default)
         else:
             val = getattr(row, attr, None)
         return val
 
-    def escape(self, value): # pylint: disable=no-self-use
+    def escape(self, value):
         u"""escape value"""
         return value
 
     def __call__(self, rows):
         out = u""
         out += self.table_start
```

### Comparing `fspath-20230218/fspath/win.py` & `fspath-20230629/fspath/win.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Windows stuff
 """
 # pylint: disable=invalid-name
 
 import os
 import io
 import six
-from .fspath import FSPath
 
 # ==============================================================================
 def wrapScriptExe(script, shebang = u"#!python.exe"):
 # ==============================================================================
     u"""Wraps a single script into a MS-Win ``.exe``.
 
     Only the ``script`` file contents is wraped into the ``.exe``, not the whole
@@ -26,14 +25,16 @@
        * This is in an experimental state!
        * This makes use of undocumented pip APIs (ATM pip has no offical API)
        * Use it with care!
        * Shebang is always ``#!python.exe``
 
     """
 
+    # pylint: disable=import-outside-toplevel
+    from .fspath import FSPath
     from pip._vendor.distlib.scripts import ScriptMaker
     from pip._vendor.distlib.compat import ZipFile
 
     origin   = FSPath(script)
     exec_out = origin.suffix('.exe')
     shebang  = six.b(shebang + u"\r\n")
     linesep  = os.linesep.encode('utf-8')
```

### Comparing `fspath-20230218/fspath.egg-info/PKG-INFO` & `fspath-20230629/fspath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fspath
-Version: 20230218
+Version: 20230629
 Summary: semantic path names and more
 Home-page: https://github.com/return42/fspath
 Author: Markus Heiser
 Author-email: markus.heiser@darmarIT.de
 License: AGPLv3
 Keywords: path-names development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fspath-20230218/fspath.egg-info/SOURCES.txt` & `fspath-20230629/fspath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fspath-20230218/tests/test_FSPath.py` & `fspath-20230629/tests/test_FSPath.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     url = 'https://github.com/return42/fspath/archive/master.zip'
     arch = TMP / 'fspath.zip'
 
     if arch.EXISTS:
         arch.delete()
     assert not arch.EXISTS
 
-    arch.download(url,
-                  chunksize=1024, ticker=True)
+    arch.download(url, chunksize=1024, ticker=True)
     assert arch.EXISTS
     assert arch.SIZE > MIN_FILESIZE
 
 def test_ZIP():
     arch = TMP / 'fspath.zip'
     arch_folder = TMP / 'fspath-master'
     if arch_folder.EXISTS:
@@ -34,8 +33,7 @@
 
 def test_makedirs():
     foo = TMP / 'foo'
     if foo.EXISTS:
         foo.delete()
     assert foo.makedirs()
     assert not foo.makedirs()
-
```

### Comparing `fspath-20230218/tests/test_UI.py` & `fspath-20230629/tests/test_UI.py`

 * *Files identical despite different names*

