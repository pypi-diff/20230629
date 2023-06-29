# Comparing `tmp/container-workflow-tool-1.5.3.tar.gz` & `tmp/container-workflow-tool-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container-workflow-tool-1.5.3.tar", last modified: Wed Jun  7 10:18:15 2023, max compression
+gzip compressed data, was "container-workflow-tool-1.5.4.tar", last modified: Thu Jun 29 12:07:31 2023, max compression
```

## Comparing `container-workflow-tool-1.5.3.tar` & `container-workflow-tool-1.5.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/cli_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f27.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f28.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f29.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f30.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f31.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f33.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f34.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/rawhide.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool/config/share/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/share/cwt_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/share/urls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/distgit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/git_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/koji.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23655 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:18:14.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/man/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/man/cwt.1
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_brew.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_distgit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_git_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.730057 container-workflow-tool-1.5.4/container_workflow_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/cli_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/container_workflow_tool/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f27.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f28.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f29.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f30.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f31.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f33.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/f34.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/rawhide.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/container_workflow_tool/config/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/share/cwt_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config/share/urls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/distgit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/koji.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23264 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/container_workflow_tool/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.730057 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:07:31.000000 container-workflow-tool-1.5.4/container_workflow_tool.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/man/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/man/cwt.1
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:31.734057 container-workflow-tool-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_brew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_distgit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-29 12:07:22.000000 container-workflow-tool-1.5.4/tests/test_utility.py
```

### Comparing `container-workflow-tool-1.5.3/LICENSE` & `container-workflow-tool-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/Makefile` & `container-workflow-tool-1.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/PKG-INFO` & `container-workflow-tool-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-workflow-tool
-Version: 1.5.3
+Version: 1.5.4
 Summary: A python3 tool to make rebuilding images easier by automating several steps of the process.
 Home-page: https://github.com/sclorg/container-workflow-tool
 Author: Petr Kubat
 Author-email: pkubat@redhat.com
 License: MIT
 Keywords: tool,containers,images,automate,workflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `container-workflow-tool-1.5.3/README.md` & `container-workflow-tool-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/cli.py` & `container-workflow-tool-1.5.4/container_workflow_tool/cli.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/cli_common.py` & `container-workflow-tool-1.5.4/container_workflow_tool/cli_common.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/default.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/default.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f27.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f27.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f28.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f28.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f29.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f29.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f30.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f30.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f31.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f31.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f32.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f32.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f33.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f33.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/f34.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/f34.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/rawhide.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/rawhide.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config/share/urls.yaml` & `container-workflow-tool-1.5.4/container_workflow_tool/config/share/urls.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/config.py` & `container-workflow-tool-1.5.4/container_workflow_tool/config.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/constants.py` & `container-workflow-tool-1.5.4/container_workflow_tool/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 action_map = {}
 action_map['git'] = {
-    'pullupstream': 'dist_git_changes',
+    'pullupstream': 'dist_git_merge_changes',
     'clonedownstream': 'pull_downstream',
     'cloneupstream': 'pull_upstream',
     'rebase': 'dist_git_rebase',
     'merge': 'merge_future_branches',
     'show': 'show_git_changes',
     'push': 'push_changes',
 }
```

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/distgit.py` & `container-workflow-tool-1.5.4/container_workflow_tool/distgit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import subprocess
 
 from git import Repo
 from git.exc import GitCommandError
 
-import container_workflow_tool.utility as u
+from container_workflow_tool import utility
 from container_workflow_tool.utility import RebuilderError
 from container_workflow_tool.dockerfile import DockerfileHandler
 from container_workflow_tool.sync import SyncHandler
 from container_workflow_tool.git_operations import GitOperations
 
 
 class DistgitAPI(GitOperations):
@@ -45,29 +45,30 @@
         ret = subprocess.run(script_path, shell=True, stderr=subprocess.PIPE,
                              stdout=subprocess.DEVNULL, cwd=component_path)
 
         if ret.returncode != 0:
             self.logger.info(template.format(name=component, status="Affected"))
             err = ret.stderr.decode('utf-8').strip()
             if err:
-                self.logger.error(u._2sp(err))
+                self.logger.error(utility._2sp(err))
         else:
             self.logger.info(template.format(name=component, status="OK"))
 
-    def dist_git_changes(self, images, rebase=False):
+    def dist_git_merge_changes(self, images, rebase=False):
         """Method to merge changes from upstream into downstream
 
         Pulls both downstream and upstream repositories into a temporary dir.
         Merge is done by copying tracked files from upstream into downstream.
 
         Args:
+            images (list): List of images to sync
             rebase (bool, optional): Specify if a rebase should be done instead
         """
         try:
-            for image in (images):
+            for image in images:
                 name = image["name"]
                 component = image["component"]
                 branch = image["git_branch"]
                 path = image["git_path"]
                 url = image["git_url"]
                 commands = image["commands"]
                 pull_upstr = image.get("pull_upstream", True)
@@ -88,26 +89,25 @@
                         else:
                             msg = "Not creating new commit in: "
                             self.logger.info(msg + component)
                 else:
                     ups_name = name.split('-')[0]
                     # Clone upstream repository
                     ups_path = os.path.join('upstreams/', ups_name)
-                    self._clone_upstream(url, ups_path, commands=commands)
+                    self.clone_upstream(url, ups_path, commands=commands)
                     # Save the upstream commit hash
                     ups_hash = Repo(ups_path).commit().hexsha
-                    self._pull_upstream(component, path, url, repo, ups_name, commands)
+                    self.pull_upstream(component, path, url, repo, ups_name, commands)
                     self.df_handler.update_dockerfile(
                         df_path, from_tag, downstream_from=downstream_from
                     )
                     repo.git.add("Dockerfile")
                     # It is possible for the git repository to have no changes
                     if repo.is_dirty():
-                        commit = self.get_commit_msg(rebase, image, ups_hash
-                        )
+                        commit = self.get_commit_msg(rebase, image, ups_hash)
                         if commit:
                             repo.git.commit("-m", commit)
                         else:
                             msg = "Not creating new commit in: "
                             self.logger.info(msg + component)
 
                 self._check_labels(df_path)
@@ -118,16 +118,16 @@
     def _clone_downstream(self, component, branch):
         """Clones downstream dist-git repo"""
         # Do not set up downstream repo if it already exists
         if os.path.isdir(component):
             self.logger.info("Using existing downstream repo: " + component)
             repo = Repo(component)
         else:
-            hostname_url = u._get_hostname_url(self.conf)
-            packager = u._get_packager(self.conf)
+            hostname_url = utility._get_hostname_url(self.conf)
+            packager = utility._get_packager(self.conf)
             # if packager is fedpkg then namespace is `container` else `containers`
             namespace = "container" if packager == "fedpkg" else "containers"
             component_path = f"{namespace}/{component}"
             # If hostname_url is specified use `git` otherwise `packager` command.
             if hostname_url:
                 cmd = "git"
                 ccomponent = f"{hostname_url}/{component_path}.git"
@@ -158,29 +158,29 @@
             try:
                 repo = Repo(component)
                 # If a commit message is provided do a commit first
                 if self.commit_msg and repo.is_dirty():
                     # commit_msg is set so it is always returned
                     commit = self.get_commit_msg(None, image)
                     repo.git.commit("-am", commit)
-                if self._get_unpushed_commits(repo):
+                if self.are_unpushed_commits_available(repo):
                     self.logger.info("Pushing: " + component)
 
                     repo.git.push()
                 else:
                     self.logger.info(f"There are no unpushed commits."
                                      f" Push skipped for {component}.")
             except GitCommandError as e:
                 failed.append(image)
                 self.logger.error(e)
 
         if failed:
             self.logger.error("Failed pushing images:")
             for image in failed:
-                self.logger.error(u._2sp(image["component"]))
+                self.logger.error(utility._2sp(image["component"]))
             self.logger.error("Please check the failures and push the changes manually.")
 
     # TODO: Multiple future branches?
     def merge_future_branches(self, images):
         """Merges current branch with future branches"""
         # Check for kerberos ticket
         failed = []
@@ -200,9 +200,9 @@
                 except GitCommandError as e:
                     failed.append(image)
                     self.logger.error(e)
                     continue
         if failed:
             self.logger.error("Failed merging images:")
             for image in failed:
-                self.logger.error(u._2sp(image["component"]))
+                self.logger.error(utility._2sp(image["component"]))
             self.logger.error("Please check the failures and push the changes manually.")
```

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/dockerfile.py` & `container-workflow-tool-1.5.4/container_workflow_tool/dockerfile.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/git_operations.py` & `container-workflow-tool-1.5.4/container_workflow_tool/git_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2020 SCL team at Red Hat
+# Copyright (c) 2023 SCL team at Red Hat
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -51,28 +51,28 @@
         Set the commit message to some other than the default one.
 
         Args:
             msg(str): Message to be written into the commit.
         """
         self.commit_msg = msg
 
-    def _do_git_reset(self, repo):
+    def do_git_reset(self, repo):
         file_list = ['--', '.gitignore'] + self.conf.ignore_files
         repo.git.reset(file_list)
         # One file at a time to make sure all files get reset even on error
         for f in file_list[1:]:
             repo.git.checkout('--', f, with_exceptions=False)
             self.logger.debug("Removing changes for: " + f)
             # Remove all ignored files that are also untracked
             untracked = repo.git.ls_files('-o').split('\n')
             if f in untracked:
                 repo.git.clean('-xfd', f)
                 self.logger.debug("Removing untracked ignored file: " + f)
 
-    def _clone_upstream(self, url, ups_path, commands=None):
+    def clone_upstream(self, url, ups_path, commands=None):
         """
         :params: url is URL to repofile from upstream. https://github.com/sclorg
         :param: ups_path is path where URL is cloned locally
         :params: commands has a format mentioned in config.yaml files
          Like for ./config/rawhide.yaml file and at the varnish container
          the structure is:
          varnish:
@@ -109,36 +109,41 @@
                 if ret.returncode != 0:
                     msg = "'{c}' failed".format(c=cmd.split(" "))
                     self.logger.error(ret.stderr)
                     raise RebuilderError(msg)
         os.chdir(oldcwd)
         return repo
 
-    def are_unpushed_commits_available(self, repo) -> bool:
+    def are_unpushed_commits_available(self, repo, branch_name="") -> bool:
         """
         Get unpushed commits
         :param repo: repo object to check for unpushed commits
+        :param branch_name: In case of gitlab, branch_name has to be defined.
+        :param branch_name: In case of gitlab, branch_name has to be defined.
+                            branch_name is e.g. rhel-8.7.0 and 'repo.active_branch.name' is 'rhel-8.7.0-<ubi_name>'
         :return: List of commits or empty array
         """
         branch = repo.active_branch.name
         # Get a list of commits that have not been pushed to remote
         select = "origin/" + branch + ".." + branch
-        if len(list(repo.iter_commits(select))) == 0:
-            return False
-        return True
+        if branch_name != "":
+            select = "origin/" + branch_name + ".." + branch
+        return bool(list(repo.iter_commits(select)))
 
-    def show_git_changes(self, tmp, components=None, diff=False):
+    def show_git_changes(self, tmp, components=None, diff=False, branch_name=""):
         """Shows changes made to tracked files in local downstream repositories
 
         Walks through all repositories and calls 'git-show' or 'git-diff' on each of them.
 
         Args:
             tmp (str): Path to the directory that is used to store git repositories
             components (list of str, optional): List of components to show changes for
             diff (boolean, optional): Controls whether the method calls git-show or git-diff
+            branch_name (str, optional): In case of gitlab, branch_name has to be defined.
+                            branch_name is e.g. rhel-8.7.0 and 'repo.active_branch.name' is 'rhel-8.7.0-<ubi_name>'
         """
         # Function to check if a path contains a git repository
         def is_git(x): return os.path.isdir(os.path.join(x, '.git'))
         files = None
         command = 'diff' if diff else 'show'
         # Create a list of repository paths
         if not components:
@@ -151,15 +156,15 @@
         if not files:
             self.logger.warn("No git repositories found in directory " + tmp)
         # Walk through the repositories and show changes made in the last commit
         for path in files:
             repo = Repo(path)
             # Only show changes if there are unpushed commits to show
             # or we only want the diff of unstaged changes
-            if self.are_unpushed_commits_available(repo) or diff:
+            if self.are_unpushed_commits_available(repo, branch_name=branch_name) or diff:
                 # Clears the screen
                 print(chr(27) + "[2J")
                 # Force pager for short git diffs
                 subprocess.run(
                     "git config core.pager 'less -+F' --replace-all",
                     cwd=path,
                     shell=True
@@ -225,15 +230,15 @@
         else:
             t = "Unknown rebase argument provided: {}"
             raise RebuilderError(t.format(str(rebase)))
         if ups_hash:
             commit += "\n created from upstream commit: " + ups_hash
         return commit
 
-    def _pull_upstream(self, component, path, url, repo, ups_name, commands):
+    def pull_upstream(self, component, path, url, repo, ups_name, commands):
         """Pulls an upstream repo and copies it into downstream"""
         ups_path = os.path.join('upstreams/', ups_name)
         cp_path = os.path.join(ups_path, path)
 
         # First check if there is a version upstream
         # If not we just skip the whole copy action
         if not os.path.exists(cp_path):
@@ -264,15 +269,15 @@
                 self.logger.warn("help.md file missing")
         # Add all the changes and remove those we do not want
         test_openshift_yaml_file = os.path.join(component, "test", "test-openshift.yaml")
         if os.path.exists(test_openshift_yaml_file):
             self.update_test_openshift_yaml(test_openshift_yaml_file, path, short_name=ups_name)
 
         repo.git.add("*")
-        self._do_git_reset(repo)
+        self.do_git_reset(repo)
         # TODO: Configurable?
         df_ext = self.df_ext
         df_path = os.path.join(component, "Dockerfile")
         if os.path.isfile(df_path + df_ext) and not os.path.islink(df_path + df_ext):
             try:
                 os.remove(df_path)
             except FileNotFoundError:
```

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/koji.py` & `container-workflow-tool-1.5.4/container_workflow_tool/koji.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/main.py` & `container-workflow-tool-1.5.4/container_workflow_tool/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import subprocess
 import os
 import shutil
 import re
 import tempfile
 import pprint
-import getpass
 import logging
 
 from git import Repo, GitError
 from typing import List, Any
 from pathlib import Path
 
 import container_workflow_tool.utility as u
@@ -49,14 +48,15 @@
         self.args = None
         self.tmp_workdir: str = None
         self.repo_url = None
         self.jira_header = None
 
         self.conf_name = config
         self.rebuild_reason = rebuild_reason
+        self.gitlab_usage = None
         self.do_image = None
         self.exclude_image = None
         self.do_set = None
         self.check_script = None
         self.image_set = None
         self.disable_klist = None
         self.output_file = None
@@ -115,18 +115,16 @@
             self.set_repo_url(args.repo_url)
         if getattr(args, 'commit_msg', None) is not None:
             self.set_commit_msg(args.commit_msg)
         if getattr(args, 'rebuild_reason', None) is not None and args.rebuild_reason:
             self.rebuild_reason = args.rebuild_reason
         if getattr(args, 'check_script', None) is not None and args.check_script:
             self.check_script = args.check_script
-        if getattr(args, 'disable_klist', None) is not None and args.disable_klist:
-            self.disable_klist = args.disable_klist
-        if getattr(args, 'latest_release', None) is not None and args.latest_release:
-            self.latest_release = args.latest_release
+        self.disable_klist = args.disable_klist
+        self.latest_release = args.latest_release
         if getattr(args, 'output_file', None) is not None and args.output_file:
             self.output_file = args.output_file
 
         # Image set to build
         if getattr(args, 'image_set', None) is not None and args.image_set:
             self.image_set = args.image_set
 
@@ -146,15 +144,15 @@
         return self._distgit
 
     @property
     def git_ops(self):
         if not self._git_ops:
             self._git_ops = GitOperations(self.base_image, self.conf,
                                           self.rebuild_reason,
-                                          self.logger.getChild("-git-ops"))
+                                          self.logger.getChild("git-ops"))
         return self._git_ops
 
     @property
     def brewapi(self):
         if not self._brewapi:
             self._brewapi = KojiAPI(self.conf, self.logger.getChild("koji"),
                                     self.latest_release)
@@ -445,24 +443,24 @@
         Args:
             repo_url: url of .repo file used for the build
         """
         self.repo_url = repo_url
 
     def list_images(self):
         """Prints list of images that we work with"""
-        for i in self._get_images():
-            self.logger.info(i["component"])
+        for image in self._get_images():
+            self.logger.info(image["component"])
 
     def print_upstream(self):
         """Prints the upstream name and url for images used in config"""
-        for i in self._get_images():
+        for image in self._get_images():
             ups_name = re.search(r".*\/([a-zA-Z0-9-]+).git",
-                                 i["git_url"]).group(1)
-            msg = f"{i.get('component')} {i.get('name')} {ups_name} " \
-                  f"{i.get('git_url')} {i.get('git_path')} {i.get('git_branch')}"
+                                 image["git_url"]).group(1)
+            msg = f"{image.get('component')} {image.get('name')} {ups_name} " \
+                  f"{image.get('git_url')} {image.get('git_path')} {image.get('git_branch')}"
             self.logger.info(msg)
 
     def show_config_contents(self):
         """Prints the symbols and values of configuration used"""
         for key in self.conf:
             value = getattr(self.conf, key)
             # Do not print clutter the output with unnecessary content
@@ -498,110 +496,102 @@
     def pull_downstream(self):
         """
         Pulls downstream dist-git repositories and does not make any further changes to them
 
         Additionally runs a script against each repository if check_script is set,
         checking its exit value.
         """
-        self._check_kerb_ticket()
-        tmp = self._get_tmp_workdir()
-        self._change_workdir(tmp)
-        images = self._get_images()
-        for i in images:
-            self.distgit._clone_downstream(i["component"], i["git_branch"])
+        tmp, images = self.preparation()
+        for image in images:
+            self.distgit._clone_downstream(image["component"], image["git_branch"])
         # If check script is set, run the script provided for each config entry
         if self.check_script:
-            for i in images:
-                self.distgit.check_script(i["component"], self.check_script,
-                                          i["git_branch"])
+            for image in images:
+                self.distgit.check_script(image["component"], self.check_script,
+                                          image["git_branch"])
 
     def pull_upstream(self):
         """
         Pulls upstream git repositories and does not make any further changes to them
 
         Additionally runs a script against each repository if check_script is set,
         checking its exit value.
         """
-        tmp = self._get_tmp_workdir()
-        self._change_workdir(tmp)
-        images = self._get_images()
-        for i in images:
+        tmp, images = self.preparation()
+        for image in images:
             # Use unversioned name as a path for the repository
-            ups_name = i["name"].split('-')[0]
-            self.distgit._clone_upstream(i["git_url"],
-                                         ups_name,
-                                         commands=i["commands"])
+            ups_name = image["name"].split('-')[0]
+            self.git_ops.clone_upstream(image["git_url"], ups_name, commands=image["commands"])
         # If check script is set, run the script provided for each config entry
         if self.check_script:
-            for i in images:
-                ups_name = i["name"].split('-')[0]
-                self.distgit.check_script(i["component"], self.check_script,
-                                          os.path.join(ups_name, i["git_path"]))
+            for image in images:
+                ups_name = image["name"].split('-')[0]
+                self.distgit.check_script(image["component"], self.check_script,
+                                          os.path.join(ups_name, image["git_path"]))
 
-    def push_changes(self):
-        """Pushes changes for all components into downstream dist-git repository"""
+    def preparation(self):
         # Check for kerberos ticket
         self._check_kerb_ticket()
         tmp = self._get_tmp_workdir(setup_dir=False)
         if not tmp:
             msg = "Temporary directory structure does not exist. Pull upstream/rebase first."
             raise RebuilderError(msg)
         self._change_workdir(tmp)
         images = self._get_images()
+        return tmp, images
+
+    def push_changes(self):
+        """Pushes changes for all components into downstream dist-git repository"""
 
+        tmp, images = self.preparation()
         self.distgit.push_changes(tmp, images)
 
     def dist_git_rebase(self):
         """
         Do a rebase against a new base/s2i image.
         Does not pull in upstream changes of layered images.
         """
-        self.dist_git_changes(rebase=True)
-
-    def dist_git_changes(self, rebase: bool = False):
-        """Method to merge changes from upstream into downstream
+        self.dist_git_merge_changes(rebase=True)
 
-        Pulls both downstream and upstream repositories into a temporary directory.
-        Merge is done by copying tracked files from upstream into downstream.
-
-        Args:
-            rebase (bool, optional): Specifies whether a rebase should be done instead.
-        """
-        # Check for kerberos ticket
-        self._check_kerb_ticket()
-        tmp = self._get_tmp_workdir()
-        self._change_workdir(tmp)
-        images = self._get_images()
-        self.distgit.dist_git_changes(images, rebase)
+    def git_changes_report(self, tmp):
         self.logger.info("\nGit location: " + tmp)
         if self.args:
             tmp_str = ' --tmp ' + self.tmp_workdir if self.tmp_workdir else '"'
             self.logger.info("You can view changes made by running:")
             self.logger.info(f"cwt --base {self.base_image} {tmp_str} git show")
         if self.args:
             self.logger.info(
                 "To push and build run:"
                 "cwt git push && cwt build"
                 "[base/core/s2i] --repo-url link-to-repo-file")
 
+    def dist_git_merge_changes(self, rebase: bool = False):
+        """Method to merge changes from upstream into downstream
+
+        Pulls both downstream and upstream repositories into a temporary directory.
+        Merge is done by copying tracked files from upstream into downstream.
+
+        Args:
+            rebase (bool, optional): Specifies whether a rebase should be done instead.
+        """
+        tmp, images = self.preparation()
+        self.distgit.dist_git_merge_changes(images, rebase)
+        self.git_changes_report(tmp=tmp)
+
     def merge_future_branches(self):
         """Merges current branch with future branches"""
         # Check for kerberos ticket
-        self._check_kerb_ticket()
-        tmp = self._get_tmp_workdir()
-        self._change_workdir(tmp)
-        images = self._get_images()
+        tmp, images = self.preparation()
         self.distgit.merge_future_branches(images)
 
     def show_git_changes(self, components: List = None):
         """Shows changes made to tracked files in local downstream repositories
 
         Args:
             components (list of str, optional): List of components to show changes for
         Walks through all downstream repositories and calls 'git-show' on each of them.
         """
+        tmp, _ = self.preparation()
         if not components:
             images = self._get_images()
-            components = [i["component"] for i in images]
-        tmp = self._get_tmp_workdir()
-        self._change_workdir(tmp)
+            components = [image["component"] for image in images]
         self.distgit.show_git_changes(tmp, components)
```

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/sync.py` & `container-workflow-tool-1.5.4/container_workflow_tool/sync.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool/utility.py` & `container-workflow-tool-1.5.4/container_workflow_tool/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import argparse
 import os
 import logging
-
+from pathlib import Path
 import textwrap
+import contextlib
 
 
 class RebuilderError(Exception):
     pass
 
 
 class ArgParser(argparse.ArgumentParser):
@@ -69,14 +70,28 @@
     if len(conf) > 2:
         raise RebuilderError("You can only use one image_set argument with the --config option.")
     config_path = conf[0]
     image_set = conf[1] if len(conf) > 1 else 'current'
     return config_path, image_set
 
 
+@contextlib.contextmanager
+def cwd(path):
+    """
+    Changes CWD to the temporary directory.
+    Yields the temporary directory.
+    """
+    prev_cwd = Path.cwd()
+    os.chdir(path)
+    try:
+        yield
+    finally:
+        os.chdir(prev_cwd)
+
+
 def setup_logger(logger_id, level=logging.INFO):
     logger = logging.getLogger(logger_id)
     logger.setLevel(level)
     format_str = "%(name)s - %(levelname)s: %(message)s"
     # Debug handler
     debug = logging.StreamHandler(sys.stdout)
     formatter = logging.Formatter(format_str)
```

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool.egg-info/PKG-INFO` & `container-workflow-tool-1.5.4/container_workflow_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-workflow-tool
-Version: 1.5.3
+Version: 1.5.4
 Summary: A python3 tool to make rebuilding images easier by automating several steps of the process.
 Home-page: https://github.com/sclorg/container-workflow-tool
 Author: Petr Kubat
 Author-email: pkubat@redhat.com
 License: MIT
 Keywords: tool,containers,images,automate,workflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `container-workflow-tool-1.5.3/container_workflow_tool.egg-info/SOURCES.txt` & `container-workflow-tool-1.5.4/container_workflow_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/man/cwt.1` & `container-workflow-tool-1.5.4/man/cwt.1`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/setup.py` & `container-workflow-tool-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         if system_path is None:
             system_path = []
     return os.path.join(*(['/'] + system_path))
 
 
 setup(
     name='container-workflow-tool',
-    version="1.5.3",
+    version="1.5.4",
     description='A python3 tool to make rebuilding images easier by automating several steps of the process.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='tool,containers,images,automate, workflow',
     author='Petr Kubat',
     author_email='pkubat@redhat.com',
     url='https://github.com/sclorg/container-workflow-tool',
```

### Comparing `container-workflow-tool-1.5.3/tests/test_brew.py` & `container-workflow-tool-1.5.4/tests/test_brew.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/tests/test_cli.py` & `container-workflow-tool-1.5.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/tests/test_distgit.py` & `container-workflow-tool-1.5.4/tests/test_distgit.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,52 +58,52 @@
         tmp = self.ir._get_tmp_workdir()
         cpath = os.path.join(tmp, 's2i')
         assert os.path.isdir(cpath)
         dpath = os.path.join(cpath, 'base', 'Dockerfile')
         assert os.path.isfile(dpath)
 
     @pytest.mark.distgit
-    def test_distgit_changes(self):
+    def test_distgit_merge_changes(self):
         self.ir.conf["from_tag"] = "test"
         tmp = Path(self.ir._get_tmp_workdir())
-        self.ir.dist_git_changes()
+        self.ir.dist_git_merge_changes()
         dpath = tmp / self.component / 'Dockerfile'
         assert os.path.isfile(dpath)
         assert not (tmp / self.component / "test" / "test-openshift.yaml").exists()
         tag_found = False
         with open(dpath) as f:
             if ":test" in f.read():
                 tag_found = True
         assert tag_found
         shutil.rmtree(tmp / self.component)
 
     @pytest.mark.distgit
-    def test_distgit_changes_openshift_yaml(self):
+    def test_distgit_merge_changes_openshift_yaml(self):
         # TODO
         # As soon as s2i-base-container will contain file 'test/test-openshift.yaml'
         # Then change it to once
         flexmock(GitOperations).should_receive("update_test_openshift_yaml").never()
         self.ir.conf["from_tag"] = "test"
         tmp = Path(self.ir._get_tmp_workdir())
         self.ir.distgit._clone_downstream(self.component, "main")
-        self.ir.dist_git_changes()
+        self.ir.dist_git_merge_changes()
         dpath = tmp / self.component / 'Dockerfile'
         assert os.path.isfile(dpath)
         tag_found = False
         with open(dpath) as f:
             if ":test" in f.read():
                 tag_found = True
         assert tag_found
         shutil.rmtree(tmp / self.component)
 
     @pytest.mark.distgit
     def test_tag_dockerfile(self):
         tmp = Path(self.ir._get_tmp_workdir())
         self.ir.conf["from_tag"] = "test"
-        self.ir.dist_git_changes()
+        self.ir.dist_git_merge_changes()
         cpath = tmp / self.component
         dpath = cpath / 'Dockerfile'
         found_tag = False
         with open(dpath) as f:
             if ":test" in f.read():
                 found_tag = True
         assert found_tag
```

### Comparing `container-workflow-tool-1.5.3/tests/test_dockerfile.py` & `container-workflow-tool-1.5.4/tests/test_dockerfile.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/tests/test_git_operations.py` & `container-workflow-tool-1.5.4/tests/test_git_operations.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/tests/test_print.py` & `container-workflow-tool-1.5.4/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/tests/test_rebuilder.py` & `container-workflow-tool-1.5.4/tests/test_rebuilder.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.3/tests/test_utility.py` & `container-workflow-tool-1.5.4/tests/test_utility.py`

 * *Files identical despite different names*

