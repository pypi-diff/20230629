# Comparing `tmp/up_pyperplan-0.3.0.4.dev1.tar.gz` & `tmp/up_pyperplan-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_pyperplan-0.3.0.4.dev1.tar", last modified: Tue Mar 28 09:37:46 2023, max compression
+gzip compressed data, was "up_pyperplan-1.0.0.tar", last modified: Thu Jun 29 13:46:02 2023, max compression
```

## Comparing `up_pyperplan-0.3.0.4.dev1.tar` & `up_pyperplan-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:37:46.493435 up_pyperplan-0.3.0.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 09:37:43.000000 up_pyperplan-0.3.0.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-28 09:37:46.493435 up_pyperplan-0.3.0.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-28 09:37:43.000000 up_pyperplan-0.3.0.4.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 09:37:46.493435 up_pyperplan-0.3.0.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-28 09:37:43.000000 up_pyperplan-0.3.0.4.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:37:46.493435 up_pyperplan-0.3.0.4.dev1/up_pyperplan/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-28 09:37:43.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-03-28 09:37:43.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-03-28 09:37:43.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan/grounder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:37:46.493435 up_pyperplan-0.3.0.4.dev1/up_pyperplan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-28 09:37:46.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-28 09:37:46.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:37:46.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 09:37:46.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 09:37:46.000000 up_pyperplan-0.3.0.4.dev1/up_pyperplan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:46:02.936810 up_pyperplan-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 13:45:59.000000 up_pyperplan-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-29 13:46:02.936810 up_pyperplan-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-29 13:45:59.000000 up_pyperplan-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:46:02.936810 up_pyperplan-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-29 13:45:59.000000 up_pyperplan-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:46:02.936810 up_pyperplan-1.0.0/up_pyperplan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 13:45:59.000000 up_pyperplan-1.0.0/up_pyperplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-29 13:45:59.000000 up_pyperplan-1.0.0/up_pyperplan/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-29 13:45:59.000000 up_pyperplan-1.0.0/up_pyperplan/grounder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:46:02.936810 up_pyperplan-1.0.0/up_pyperplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-29 13:46:02.000000 up_pyperplan-1.0.0/up_pyperplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 13:46:02.000000 up_pyperplan-1.0.0/up_pyperplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:46:02.000000 up_pyperplan-1.0.0/up_pyperplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 13:46:02.000000 up_pyperplan-1.0.0/up_pyperplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:46:02.000000 up_pyperplan-1.0.0/up_pyperplan.egg-info/top_level.txt
```

### Comparing `up_pyperplan-0.3.0.4.dev1/LICENSE` & `up_pyperplan-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `up_pyperplan-0.3.0.4.dev1/README.md` & `up_pyperplan-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `up_pyperplan-0.3.0.4.dev1/setup.py` & `up_pyperplan-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `up_pyperplan-0.3.0.4.dev1/up_pyperplan/__init__.py` & `up_pyperplan-1.0.0/up_pyperplan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import subprocess
 import re
 
 
-VERSION = (0, 3, 0)
+VERSION = (1, 0, 0)
 __version__ = ".".join(str(x) for x in VERSION)
 
 try:
     git_version = subprocess.check_output(["git", "describe", "--tags",
                                            "--dirty=-wip"],
                                           stderr=subprocess.STDOUT)
     output = git_version.strip().decode('ascii')
```

### Comparing `up_pyperplan-0.3.0.4.dev1/up_pyperplan/engine.py` & `up_pyperplan-1.0.0/up_pyperplan/engine.py`

 * *Files identical despite different names*

### Comparing `up_pyperplan-0.3.0.4.dev1/up_pyperplan/grounder.py` & `up_pyperplan-1.0.0/up_pyperplan/grounder.py`

 * *Files identical despite different names*

