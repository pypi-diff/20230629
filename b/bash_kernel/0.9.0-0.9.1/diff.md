# Comparing `tmp/bash_kernel-0.9.0.tar.gz` & `tmp/bash_kernel-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bash_kernel-0.9.0.tar", last modified: Sat Dec 17 19:21:30 2022, max compression
+gzip compressed data, was "bash_kernel-0.9.1.tar", last modified: Thu Jun 29 13:29:25 2023, max compression
```

## Comparing `bash_kernel-0.9.0.tar` & `bash_kernel-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       40 2022-05-30 12:31:46.755936 bash_kernel-0.9.0/.gitignore
--rw-r--r--   0        0        0      406 2022-12-17 19:18:46.284100 bash_kernel-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1526 2022-05-30 12:31:46.755936 bash_kernel-0.9.0/LICENSE
--rw-r--r--   0        0        0     2914 2022-12-17 19:11:30.528084 bash_kernel-0.9.0/README.rst
--rw-r--r--   0        0        0       65 2022-05-30 12:31:46.755936 bash_kernel-0.9.0/bash_kernel/__init__.py
--rw-r--r--   0        0        0      128 2022-05-30 12:31:46.755936 bash_kernel-0.9.0/bash_kernel/__main__.py
--rw-r--r--   0        0        0     7745 2022-12-17 19:08:58.839088 bash_kernel-0.9.0/bash_kernel/display.py
--rw-r--r--   0        0        0     1943 2022-12-17 19:08:58.839088 bash_kernel-0.9.0/bash_kernel/install.py
--rw-r--r--   0        0        0    10074 2022-12-17 19:09:14.799179 bash_kernel-0.9.0/bash_kernel/kernel.py
--rw-r--r--   0        0        0       78 2022-12-17 19:08:58.839088 bash_kernel-0.9.0/binder/postBuild
--rw-r--r--   0        0        0       12 2022-12-17 19:08:58.839088 bash_kernel-0.9.0/binder/requirements.txt
--rw-r--r--   0        0        0      539 2022-12-17 19:08:58.839088 bash_kernel-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 bash_kernel-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2022-05-30 12:31:46.755936 bash_kernel-0.9.1/.gitignore
+-rw-r--r--   0        0        0      406 2022-12-17 19:18:46.284100 bash_kernel-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1526 2022-05-30 12:31:46.755936 bash_kernel-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2930 2023-06-29 13:28:22.700963 bash_kernel-0.9.1/README.rst
+-rw-r--r--   0        0        0       65 2022-05-30 12:31:46.755936 bash_kernel-0.9.1/bash_kernel/__init__.py
+-rw-r--r--   0        0        0      128 2022-05-30 12:31:46.755936 bash_kernel-0.9.1/bash_kernel/__main__.py
+-rw-r--r--   0        0        0     7745 2022-12-17 19:08:58.839088 bash_kernel-0.9.1/bash_kernel/display.py
+-rw-r--r--   0        0        0     1943 2022-12-17 19:08:58.839088 bash_kernel-0.9.1/bash_kernel/install.py
+-rw-r--r--   0        0        0    11572 2023-06-29 13:29:10.593145 bash_kernel-0.9.1/bash_kernel/kernel.py
+-rw-r--r--   0        0        0       78 2022-12-17 19:08:58.839088 bash_kernel-0.9.1/binder/postBuild
+-rw-r--r--   0        0        0       12 2022-12-17 19:08:58.839088 bash_kernel-0.9.1/binder/requirements.txt
+-rw-r--r--   0        0        0      539 2022-12-17 19:08:58.839088 bash_kernel-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 bash_kernel-0.9.1/PKG-INFO
```

### Comparing `bash_kernel-0.9.0/LICENSE` & `bash_kernel-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bash_kernel-0.9.0/README.rst` & `bash_kernel-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-... image:: https://mybinder.org/badge_logo.svg
+.. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/takluyver/bash_kernel/master
 
 =========================
 A Jupyter kernel for bash
 =========================
 
 Installation
 ------------
 This requires IPython 3.
 
+.. code:: shell
+
     pip install bash_kernel
     python -m bash_kernel.install
 
 To use it, run one of:
 
 .. code:: shell
```

### Comparing `bash_kernel-0.9.0/bash_kernel/display.py` & `bash_kernel-0.9.1/bash_kernel/display.py`

 * *Files identical despite different names*

### Comparing `bash_kernel-0.9.0/bash_kernel/install.py` & `bash_kernel-0.9.1/bash_kernel/install.py`

 * *Files identical despite different names*

### Comparing `bash_kernel-0.9.0/bash_kernel/kernel.py` & `bash_kernel-0.9.1/bash_kernel/kernel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from ipykernel.kernelbase import Kernel
 from pexpect import replwrap, EOF
 import pexpect
 
 from subprocess import check_output
 import os.path
 import uuid
+import random
+import string
 
 import re
 import signal
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 version_pat = re.compile(r'version (\d+(\.\d+)+)')
 
 from .display import (extract_contents, build_cmds)
 
 class IREPLWrapper(replwrap.REPLWrapper):
     """A subclass of REPLWrapper that gives incremental output
@@ -21,41 +23,57 @@
 
     The parameters are the same as for REPLWrapper, except for one
     extra parameter:
 
     :param line_output_callback: a callback method to receive each batch
       of incremental output. It takes one string parameter.
     """
-    def __init__(self, cmd_or_spawn, orig_prompt, prompt_change,
+    def __init__(self, cmd_or_spawn, orig_prompt, prompt_change, unique_prompt,
                  extra_init_cmd=None, line_output_callback=None):
+        self.unique_prompt = unique_prompt
         self.line_output_callback = line_output_callback
+        # The extra regex at the start of PS1 below is designed to catch the
+        # `(envname) ` which conda/mamba add to the start of PS1 by default.
+        # Obviously anything else that looks like this, including user output,
+        # will be eaten.
+        # FIXME: work out if there is a way to update these by reading PS1
+        # after each command and checking that it has changed. The answer is
+        # probably no, as we never see individual commands but rather cells
+        # with possibly many commands, and would need to update this half-way
+        # through a cell.
+        self.ps1_re = r"(\(\w+\) )?" + re.escape(self.unique_prompt + ">")
+        self.ps2_re = re.escape(self.unique_prompt + "+")
         replwrap.REPLWrapper.__init__(self, cmd_or_spawn, orig_prompt,
-                                      prompt_change, extra_init_cmd=extra_init_cmd)
+                prompt_change, new_prompt=self.ps1_re,
+                continuation_prompt=self.ps2_re, extra_init_cmd=extra_init_cmd)
 
     def _expect_prompt(self, timeout=-1):
+        prompts = [self.ps1_re, self.ps2_re]
+
         if timeout == None:
             # "None" means we are executing code from a Jupyter cell by way of the run_command
-            # in the do_execute() code below, so do incremental output.
+            # in the do_execute() code below, so do incremental output, i.e.
+            # also look for end of line or carridge return
+            prompts.extend(['\r?\n', '\r'])
             while True:
-                pos = self.child.expect_exact([self.prompt, self.continuation_prompt, u'\r\n', u'\n', u'\r'],
-                                              timeout=None)
-                if pos == 2 or pos == 3:
+                pos = self.child.expect_list([re.compile(x) for x in prompts], timeout=None)
+                if pos == 2:
                     # End of line received.
                     self.line_output_callback(self.child.before + '\n')
-                elif pos == 4:
+                elif pos == 3:
                     # Carriage return ('\r') received.
                     self.line_output_callback(self.child.before + '\r')
                 else:
                     if len(self.child.before) != 0:
                         # Prompt received, but partial line precedes it.
                         self.line_output_callback(self.child.before)
                     break
         else:
-            # Otherwise, use existing non-incremental code
-            pos = replwrap.REPLWrapper._expect_prompt(self, timeout=timeout)
+            # Otherwise, wait (with timeout) until the next prompt
+            pos = self.child.expect_list([re.compile(x) for x in prompts], timeout=timeout)
 
         # Prompt received, so return normally
         return pos
 
 class BashKernel(Kernel):
     implementation = 'bash_kernel'
     implementation_version = __version__
@@ -75,14 +93,17 @@
 
     language_info = {'name': 'bash',
                      'codemirror_mode': 'shell',
                      'mimetype': 'text/x-sh',
                      'file_extension': '.sh'}
 
     def __init__(self, **kwargs):
+        # Make a random prompt, further reducing chances of accidental matches.
+        rand = ''.join(random.choices(string.ascii_uppercase, k=12))
+        self.unique_prompt = "PROMPT_" + rand
         Kernel.__init__(self, **kwargs)
         self._start_bash()
         self._known_display_ids = set()
 
     def _start_bash(self):
         # Signal handlers are inherited by forked processes, and we can't easily
         # reset it from the subprocess. Since kernelapp ignores SIGINT except in
@@ -93,20 +114,24 @@
             # Note: the next few lines mirror functionality in the
             # bash() function of pexpect/replwrap.py.  Look at the
             # source code there for comments and context for
             # understanding the code here.
             bashrc = os.path.join(os.path.dirname(pexpect.__file__), 'bashrc.sh')
             child = pexpect.spawn("bash", ['--rcfile', bashrc], echo=False,
                                   encoding='utf-8', codec_errors='replace')
-            ps1 = replwrap.PEXPECT_PROMPT[:5] + u'\[\]' + replwrap.PEXPECT_PROMPT[5:]
-            ps2 = replwrap.PEXPECT_CONTINUATION_PROMPT[:5] + u'\[\]' + replwrap.PEXPECT_CONTINUATION_PROMPT[5:]
+            # Following comment stolen from upstream's REPLWrap:
+            # If the user runs 'env', the value of PS1 will be in the output. To avoid
+            # replwrap seeing that as the next prompt, we'll embed the marker characters
+            # for invisible characters in the prompt; these show up when inspecting the
+            # environment variable, but not when bash displays the prompt.
+            ps1 = self.unique_prompt + u'\[\]' + ">"
+            ps2 = self.unique_prompt + u'\[\]' + "+"
             prompt_change = u"PS1='{0}' PS2='{1}' PROMPT_COMMAND=''".format(ps1, ps2)
-
             # Using IREPLWrapper to get incremental output
-            self.bashwrapper = IREPLWrapper(child, u'\$', prompt_change,
+            self.bashwrapper = IREPLWrapper(child, u'\$', prompt_change, self.unique_prompt,
                                             extra_init_cmd="export PAGER=cat",
                                             line_output_callback=self.process_output)
         finally:
             signal.signal(signal.SIGINT, sig)
 
         # Disable bracketed paste (see <https://github.com/takluyver/bash_kernel/issues/117>)
         self.bashwrapper.run_command("bind 'set enable-bracketed-paste off' >/dev/null 2>&1 || true")
@@ -178,16 +203,16 @@
             self._start_bash()
             self.process_output(output)
 
         if interrupted:
             return {'status': 'abort', 'execution_count': self.execution_count}
 
         try:
-            exitcode = int(self.bashwrapper.run_command('echo $?').rstrip())
-        except Exception:
+            exitcode = int(self.bashwrapper.run_command('echo $?').rstrip().split("\r\n")[0])
+        except Exception as exc:
             exitcode = 1
 
         if exitcode:
             error_content = {
                 'ename': '',
                 'evalue': str(exitcode),
                 'traceback': []
```

### Comparing `bash_kernel-0.9.0/pyproject.toml` & `bash_kernel-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bash_kernel-0.9.0/PKG-INFO` & `bash_kernel-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: bash_kernel
-Version: 0.9.0
+Version: 0.9.1
 Summary: A bash kernel for Jupyter
 Author-email: Thomas Kluyver <thomas@kluyver.me.uk>
 Description-Content-Type: text/x-rst
 Classifier: Framework :: Jupyter
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Requires-Dist: pexpect (>=4.0)
 Requires-Dist: ipykernel
 Project-URL: Source, https://github.com/takluyver/bash_kernel
 
-... image:: https://mybinder.org/badge_logo.svg
+.. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/takluyver/bash_kernel/master
 
 =========================
 A Jupyter kernel for bash
 =========================
 
 Installation
 ------------
 This requires IPython 3.
 
+.. code:: shell
+
     pip install bash_kernel
     python -m bash_kernel.install
 
 To use it, run one of:
 
 .. code:: shell
```

