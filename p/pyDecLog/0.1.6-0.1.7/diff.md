# Comparing `tmp/pyDecLog-0.1.6.tar.gz` & `tmp/pyDecLog-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDecLog-0.1.6.tar", last modified: Tue Jun 27 11:02:53 2023, max compression
+gzip compressed data, was "pyDecLog-0.1.7.tar", last modified: Thu Jun 29 09:14:38 2023, max compression
```

## Comparing `pyDecLog-0.1.6.tar` & `pyDecLog-0.1.7.tar`

### file list

```diff
@@ -1,60 +1,68 @@
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.901398 pyDecLog-0.1.6/
--rw-r--r--   0 gm_main    (501) staff       (20)      119 2023-06-26 19:28:02.000000 pyDecLog-0.1.6/.flake8
--rw-r--r--   0 gm_main    (501) staff       (20)        0 2023-06-27 06:17:56.000000 pyDecLog-0.1.6/.gitattributes
--rw-r--r--   0 gm_main    (501) staff       (20)     3191 2023-06-26 19:28:02.000000 pyDecLog-0.1.6/.gitignore
--rw-r--r--   0 gm_main    (501) staff       (20)      362 2023-06-26 20:31:42.000000 pyDecLog-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 gm_main    (501) staff       (20)     1077 2023-06-26 19:28:02.000000 pyDecLog-0.1.6/LICENSE
--rw-r--r--   0 gm_main    (501) staff       (20)     5723 2023-06-27 11:02:53.900854 pyDecLog-0.1.6/PKG-INFO
--rw-r--r--   0 gm_main    (501) staff       (20)     5355 2023-06-27 10:56:18.000000 pyDecLog-0.1.6/README.md
--rw-r--r--   0 gm_main    (501) staff       (20)        5 2023-06-27 11:01:53.000000 pyDecLog-0.1.6/VERSION
--rw-r--r--   0 gm_main    (501) staff       (20)       90 2023-06-27 10:58:21.000000 pyDecLog-0.1.6/__init__.py
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.874230 pyDecLog-0.1.6/examples/
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.882078 pyDecLog-0.1.6/examples/@arguments/
--rw-r--r--   0 gm_main    (501) staff       (20)    10002 2023-06-26 20:19:01.000000 pyDecLog-0.1.6/examples/@arguments/@arguments.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.882934 pyDecLog-0.1.6/examples/@description/
--rw-r--r--   0 gm_main    (501) staff       (20)     3403 2023-06-26 20:19:53.000000 pyDecLog-0.1.6/examples/@description/@description.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.883590 pyDecLog-0.1.6/examples/@memory/
--rw-r--r--   0 gm_main    (501) staff       (20)    13004 2023-06-26 20:20:17.000000 pyDecLog-0.1.6/examples/@memory/@memory.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.884322 pyDecLog-0.1.6/examples/@message/
--rw-r--r--   0 gm_main    (501) staff       (20)    11406 2023-06-26 20:21:08.000000 pyDecLog-0.1.6/examples/@message/@message.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.884983 pyDecLog-0.1.6/examples/@profile_locals/
--rw-r--r--   0 gm_main    (501) staff       (20)     5066 2023-06-26 20:21:38.000000 pyDecLog-0.1.6/examples/@profile_locals/@profile_locals.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.885691 pyDecLog-0.1.6/examples/@signature/
--rw-r--r--   0 gm_main    (501) staff       (20)     3712 2023-06-26 20:22:08.000000 pyDecLog-0.1.6/examples/@signature/@signature.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.886297 pyDecLog-0.1.6/examples/@timing/
--rw-r--r--   0 gm_main    (501) staff       (20)    11334 2023-06-26 20:22:40.000000 pyDecLog-0.1.6/examples/@timing/@timing.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.887072 pyDecLog-0.1.6/examples/@typing/
--rw-r--r--   0 gm_main    (501) staff       (20)     9210 2023-06-26 20:23:00.000000 pyDecLog-0.1.6/examples/@typing/@typing.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.887805 pyDecLog-0.1.6/examples/lprint/
--rw-r--r--   0 gm_main    (501) staff       (20)     8413 2023-06-27 08:21:32.000000 pyDecLog-0.1.6/examples/lprint/lprint.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.888654 pyDecLog-0.1.6/examples/multiple_decorators/
--rw-r--r--   0 gm_main    (501) staff       (20)     3992 2023-06-26 20:23:46.000000 pyDecLog-0.1.6/examples/multiple_decorators/multiple_decorators.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.889342 pyDecLog-0.1.6/examples/workflow/
--rw-r--r--   0 gm_main    (501) staff       (20)      943 2023-06-26 20:24:17.000000 pyDecLog-0.1.6/examples/workflow/workflow.py
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.891997 pyDecLog-0.1.6/pyDecLog.egg-info/
--rw-r--r--   0 gm_main    (501) staff       (20)     5723 2023-06-27 11:02:53.000000 pyDecLog-0.1.6/pyDecLog.egg-info/PKG-INFO
--rw-r--r--   0 gm_main    (501) staff       (20)     1054 2023-06-27 11:02:53.000000 pyDecLog-0.1.6/pyDecLog.egg-info/SOURCES.txt
--rw-r--r--   0 gm_main    (501) staff       (20)        1 2023-06-27 11:02:53.000000 pyDecLog-0.1.6/pyDecLog.egg-info/dependency_links.txt
--rw-r--r--   0 gm_main    (501) staff       (20)       29 2023-06-27 11:02:53.000000 pyDecLog-0.1.6/pyDecLog.egg-info/requires.txt
--rw-r--r--   0 gm_main    (501) staff       (20)        9 2023-06-27 11:02:53.000000 pyDecLog-0.1.6/pyDecLog.egg-info/top_level.txt
--rw-r--r--   0 gm_main    (501) staff       (20)    17956 2023-06-27 07:08:23.000000 pyDecLog-0.1.6/pyDecLog.py
--rw-r--r--   0 gm_main    (501) staff       (20)      174 2023-06-26 19:28:02.000000 pyDecLog-0.1.6/pyproject.toml
--rw-r--r--   0 gm_main    (501) staff       (20)       28 2023-06-27 10:07:58.000000 pyDecLog-0.1.6/requirements.txt
--rw-r--r--   0 gm_main    (501) staff       (20)       46 2023-06-27 10:18:53.000000 pyDecLog-0.1.6/requirements_dev.txt
--rw-r--r--   0 gm_main    (501) staff       (20)       38 2023-06-27 11:02:53.901565 pyDecLog-0.1.6/setup.cfg
--rw-r--r--   0 gm_main    (501) staff       (20)     1387 2023-06-27 11:01:34.000000 pyDecLog-0.1.6/setup.py
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 11:02:53.899679 pyDecLog-0.1.6/tests/
--rwxr-xr-x   0 gm_main    (501) staff       (20)       85 2023-06-26 19:28:02.000000 pyDecLog-0.1.6/tests/test_all.sh
--rw-r--r--   0 gm_main    (501) staff       (20)     4166 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_arguments.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3694 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_description.py
--rw-r--r--   0 gm_main    (501) staff       (20)     4119 2023-06-26 20:38:54.000000 pyDecLog-0.1.6/tests/test_get_log_and_level.py
--rw-r--r--   0 gm_main    (501) staff       (20)     1265 2023-06-26 20:34:06.000000 pyDecLog-0.1.6/tests/test_get_memory.py
--rw-r--r--   0 gm_main    (501) staff       (20)      785 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_get_time.py
--rw-r--r--   0 gm_main    (501) staff       (20)     2346 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_lprint.py
--rw-r--r--   0 gm_main    (501) staff       (20)     4189 2023-06-26 20:33:35.000000 pyDecLog-0.1.6/tests/test_memory.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3635 2023-06-26 20:33:32.000000 pyDecLog-0.1.6/tests/test_message.py
--rw-r--r--   0 gm_main    (501) staff       (20)      828 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_profile_locals.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3395 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_signature.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3816 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_timing.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3680 2023-06-26 20:36:47.000000 pyDecLog-0.1.6/tests/test_typing.py
--rwxr-xr-x   0 gm_main    (501) staff       (20)      431 2023-06-26 19:28:02.000000 pyDecLog-0.1.6/update_github.sh
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.527303 pyDecLog-0.1.7/
+-rw-r--r--   0 gm_main    (501) staff       (20)      119 2023-06-26 19:28:02.000000 pyDecLog-0.1.7/.flake8
+-rw-r--r--   0 gm_main    (501) staff       (20)        0 2023-06-27 06:17:56.000000 pyDecLog-0.1.7/.gitattributes
+-rw-r--r--   0 gm_main    (501) staff       (20)     3191 2023-06-26 19:28:02.000000 pyDecLog-0.1.7/.gitignore
+-rw-r--r--   0 gm_main    (501) staff       (20)      362 2023-06-26 20:31:42.000000 pyDecLog-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 gm_main    (501) staff       (20)       42 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/CHANGELOG.md
+-rw-r--r--   0 gm_main    (501) staff       (20)        0 2023-06-27 19:01:56.000000 pyDecLog-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 gm_main    (501) staff       (20)     1077 2023-06-26 19:28:02.000000 pyDecLog-0.1.7/LICENSE
+-rw-r--r--   0 gm_main    (501) staff       (20)       69 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/MANIFEST.in
+-rw-r--r--   0 gm_main    (501) staff       (20)     6367 2023-06-29 09:14:38.526681 pyDecLog-0.1.7/PKG-INFO
+-rw-r--r--   0 gm_main    (501) staff       (20)     5999 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/README.md
+-rw-r--r--   0 gm_main    (501) staff       (20)        6 2023-06-29 09:14:25.000000 pyDecLog-0.1.7/VERSION
+-rw-r--r--   0 gm_main    (501) staff       (20)       91 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/__init__.py
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.496785 pyDecLog-0.1.7/examples/
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.506205 pyDecLog-0.1.7/examples/@arguments/
+-rw-r--r--   0 gm_main    (501) staff       (20)    10002 2023-06-26 20:19:01.000000 pyDecLog-0.1.7/examples/@arguments/@arguments.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.506789 pyDecLog-0.1.7/examples/@description/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3403 2023-06-26 20:19:53.000000 pyDecLog-0.1.7/examples/@description/@description.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.507354 pyDecLog-0.1.7/examples/@machine/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3580 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/examples/@machine/@machine.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.507922 pyDecLog-0.1.7/examples/@memory/
+-rw-r--r--   0 gm_main    (501) staff       (20)    13004 2023-06-26 20:20:17.000000 pyDecLog-0.1.7/examples/@memory/@memory.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.508507 pyDecLog-0.1.7/examples/@message/
+-rw-r--r--   0 gm_main    (501) staff       (20)    11406 2023-06-26 20:21:08.000000 pyDecLog-0.1.7/examples/@message/@message.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.509111 pyDecLog-0.1.7/examples/@profile_locals/
+-rw-r--r--   0 gm_main    (501) staff       (20)     4932 2023-06-28 06:06:12.000000 pyDecLog-0.1.7/examples/@profile_locals/@profile_locals.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.509694 pyDecLog-0.1.7/examples/@signature/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3712 2023-06-26 20:22:08.000000 pyDecLog-0.1.7/examples/@signature/@signature.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.510804 pyDecLog-0.1.7/examples/@timing/
+-rw-r--r--   0 gm_main    (501) staff       (20)    11334 2023-06-26 20:22:40.000000 pyDecLog-0.1.7/examples/@timing/@timing.ipynb
+-rw-r--r--   0 gm_main    (501) staff       (20)       97 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/examples/@timing/README.md
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.511376 pyDecLog-0.1.7/examples/@typing/
+-rw-r--r--   0 gm_main    (501) staff       (20)     9210 2023-06-26 20:23:00.000000 pyDecLog-0.1.7/examples/@typing/@typing.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.511971 pyDecLog-0.1.7/examples/@user/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3091 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/examples/@user/@user.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.512662 pyDecLog-0.1.7/examples/lprint/
+-rw-r--r--   0 gm_main    (501) staff       (20)     6979 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/examples/lprint/lprint.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.513297 pyDecLog-0.1.7/examples/multiple_decorators/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3992 2023-06-26 20:23:46.000000 pyDecLog-0.1.7/examples/multiple_decorators/multiple_decorators.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.513896 pyDecLog-0.1.7/examples/workflow/
+-rw-r--r--   0 gm_main    (501) staff       (20)      943 2023-06-26 20:24:17.000000 pyDecLog-0.1.7/examples/workflow/workflow.py
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.517335 pyDecLog-0.1.7/pyDecLog.egg-info/
+-rw-r--r--   0 gm_main    (501) staff       (20)     6367 2023-06-29 09:14:38.000000 pyDecLog-0.1.7/pyDecLog.egg-info/PKG-INFO
+-rw-r--r--   0 gm_main    (501) staff       (20)     1182 2023-06-29 09:14:38.000000 pyDecLog-0.1.7/pyDecLog.egg-info/SOURCES.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)        1 2023-06-29 09:14:38.000000 pyDecLog-0.1.7/pyDecLog.egg-info/dependency_links.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)       29 2023-06-29 09:14:38.000000 pyDecLog-0.1.7/pyDecLog.egg-info/requires.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)        9 2023-06-29 09:14:38.000000 pyDecLog-0.1.7/pyDecLog.egg-info/top_level.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)    21243 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/pyDecLog.py
+-rw-r--r--   0 gm_main    (501) staff       (20)      174 2023-06-26 19:28:02.000000 pyDecLog-0.1.7/pyproject.toml
+-rw-r--r--   0 gm_main    (501) staff       (20)       29 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/requirements.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)       47 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/requirements_dev.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)       38 2023-06-29 09:14:38.527497 pyDecLog-0.1.7/setup.cfg
+-rw-r--r--   0 gm_main    (501) staff       (20)     1388 2023-06-29 09:10:53.000000 pyDecLog-0.1.7/setup.py
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-29 09:14:38.525839 pyDecLog-0.1.7/tests/
+-rwxr-xr-x   0 gm_main    (501) staff       (20)       85 2023-06-26 19:28:02.000000 pyDecLog-0.1.7/tests/test_all.sh
+-rw-r--r--   0 gm_main    (501) staff       (20)     4166 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_arguments.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3694 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_description.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     4119 2023-06-26 20:38:54.000000 pyDecLog-0.1.7/tests/test_get_log_and_level.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     1265 2023-06-26 20:34:06.000000 pyDecLog-0.1.7/tests/test_get_memory.py
+-rw-r--r--   0 gm_main    (501) staff       (20)      785 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_get_time.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     2346 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_lprint.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     4189 2023-06-26 20:33:35.000000 pyDecLog-0.1.7/tests/test_memory.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3635 2023-06-26 20:33:32.000000 pyDecLog-0.1.7/tests/test_message.py
+-rw-r--r--   0 gm_main    (501) staff       (20)      828 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_profile_locals.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3395 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_signature.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3816 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_timing.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3680 2023-06-26 20:36:47.000000 pyDecLog-0.1.7/tests/test_typing.py
+-rwxr-xr-x   0 gm_main    (501) staff       (20)      431 2023-06-26 19:28:02.000000 pyDecLog-0.1.7/update_github.sh
```

### Comparing `pyDecLog-0.1.6/.gitignore` & `pyDecLog-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/LICENSE` & `pyDecLog-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/PKG-INFO` & `pyDecLog-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecLog
-Version: 0.1.6
+Version: 0.1.7
 Summary: pyDecLog: a Python module for logging via decorators
 Home-page: https://github.com/kyaiooiayk/pyDecLog
 Author: kyaiooiayk
 Author-email: kayaiooiayk@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
@@ -13,14 +13,17 @@
 
 # pyDecLog
 
 ![PyPI Version](https://img.shields.io/pypi/v/pyDecLog.svg)
 ![Python Version](https://img.shields.io/pypi/pyversions/pyDecLog.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyDecLog)
 ![License](https://img.shields.io/pypi/l/pyDecLog)
+![Stars](https://img.shields.io/github/stars/kyaiooiayk/pyDecLog)
+![Issues](https://img.shields.io/github/issues/kyaiooiayk/pyDecLog)
+![Forks](https://img.shields.io/github/forks/kyaiooiayk/pyDecLog)
 
 pyDecLog: a simple and easy to use Python module for logging via decorators.
 ***
 
 ## 🚀Quick start
 - Say we have the following workflow
 ```python
@@ -59,15 +62,15 @@
     # Set console level to the same level of the message so it is shown in the console
     lprint(console_log_level="info").info("Workflow ends!")
 
 
 if __name__ == "__main__":
     workflow()
 ```
-- Upin execution the following is printed on console:
+- Upon execution the following is printed on console:
 ```shell
 Workflow starts!
 Workflow ends!
 ```
 - Upon execution a `LOG.log` file is written:
 ```shell
 2023/06/24 | 18:20:50 | ERROR Workflow starts!
@@ -86,93 +89,103 @@
 ## 🚀Useful for
 - Keep track of Python pipelines.
 - Log info about a function during development both on python script or jupyter notebook.
 ***
 
 ## ⚙️Installation
 - Create your own virtual environment and run `pip install -r requirements.txt`
-- Via pip: `pip install pyDecLog`   
+- Via pip: `pip install pyDecLog`
 ***
 
 ## 🔗Dependencies
 - PyDevLog requires Python 3.5 or higher, and the following packages:
   - `pympler`
   - `numpy`
 ***
 
 ## 🧑‍🤝‍🧑Contributions
 - All contributions (bug, suggestion, new feature) are welcome.
 ***
 
 ## 🎨Available decorators
-- `@comment`: log all the print statements inside a decorated function
-- `@timing`: log the function elapsed time
-- `@signature`: log function's signature
 - `@arguments`: log function's args and kwargs
-- `@message`: log the function's print statements
-- `@typing`: log function's args, kwargs and output type
-- `@memory`: log function's args, kwargs and output their memory usage
+- `@comment`: log all function's inner print statements
 - `@description`: log function's output from the `__doc__` dunder method
-- `@profile_local`: log function's local persistent variables.
+- `@machine`: log machine OS system and hardware
+- `@memory`: log function's args, kwargs and output memory usage
+- `@message`: log function's print statements
+- `@profile_locals`: log function's local persistent variables
+- `@signature`: log function's signature
+- `@timing`: log function's elapsed time
+- `@typing`: log function's args, kwargs and output type
+- `@user`: log user info
 ***
 
 ## 🪄Features
 - Mix and match the decorators you want.
 - Can control logging levels as a whole or individually. Choose from the following:
   - `CRITICAL`
   - `ERROR`
   - `WARNING`
   - `INFO`
   - `DEBUG`
 - Can control where logging messages are piped: to log file or both log file and console. When controlling the message at the console level the following hierarchy is enforced:
-  ```
-    CRITICAL : 50
-    ERROR    : 40
-    WARNING  : 30
-    INFO     : 20
-    DEBUG    : 10
-    NOTSET   : 0
-  ```
+```
+CRITICAL : 50
+ERROR    : 40
+WARNING  : 30
+INFO     : 20
+DEBUG    : 10
+NOTSET   : 0
+```
 - Can add comments directly to log file even outside a function.
 ***
 
 ## ⚠️Known issues
-- `@profile_locals` does not write to the log file. Its output needs to be piped separately to the log. See the following example:
+- `@profile_locals` does not write to the log file. Its output needs to be piped separately to the LOG.log file. See the following example:
 ```python
 from pyDecLog import profile_locals as profile
 from pyDecLog import lprint
+from pympler.asizeof import asizeof
 
 @profile
-def func():
-    local1 = 1
-    local2 = 2
+def func(x):
+    local_1 = 1
+    local_2 = 2
     return 1
 
 func()
 
 for key, value in func.locals.items():
     msg = f"Variable: {key} | value: {value} | type: {type(value)} | size: {asizeof(value)}"
 
     lprint(console_log_level="debug").debug(msg)
 ```
+- The following `LOG.log` is the written:
+```shell
+2023/06/28 | 07:04:52 | DEBUG Variable: x | value: 1 | type: <class 'int'> | size: 32
+2023/06/28 | 07:04:52 | DEBUG Variable: local_1 | value: 1 | type: <class 'int'> | size: 32
+2023/06/28 | 07:04:52 | DEBUG Variable: local_2 | value: 2 | type: <class 'int'> | size: 32
+```
 ***
 
 ## 📚Tutorials
 - See the `examples` folder.
 ***
 
 ## 📚References
 - [Decorators with parameters?](https://stackoverflow.com/questions/5929107/decorators-with-parameters)
 - [How to expose persistent local variables? Part#1](https://code.activestate.com/recipes/577283-decorator-to-expose-local-variables-of-a-function-/)
 - [How to expose persistent local variables? Part#2](https://stackoverflow.com/questions/9186395/python-is-there-a-way-to-get-a-local-function-variable-from-within-a-decorator)
 - [How to time your code](https://stackoverflow.com/questions/17579357/time-time-vs-timeit-timeit)
 ***
 
 ## 📝Changelog
-- `0.1.4`  first release (26/06/23).
+- `0.1.6` - First release (26/06/23).
+- `0.1.7` - Added `@machine` and  `@user` (29/06/23).
 ***
 
 ## 📝To-do
 - There is no planned development.
 ***
 
 ## 🪪License
```

### Comparing `pyDecLog-0.1.6/README.md` & `pyDecLog-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # pyDecLog
 
 ![PyPI Version](https://img.shields.io/pypi/v/pyDecLog.svg)
 ![Python Version](https://img.shields.io/pypi/pyversions/pyDecLog.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyDecLog)
 ![License](https://img.shields.io/pypi/l/pyDecLog)
+![Stars](https://img.shields.io/github/stars/kyaiooiayk/pyDecLog)
+![Issues](https://img.shields.io/github/issues/kyaiooiayk/pyDecLog)
+![Forks](https://img.shields.io/github/forks/kyaiooiayk/pyDecLog)
 
 pyDecLog: a simple and easy to use Python module for logging via decorators.
 ***
 
 ## 🚀Quick start
 - Say we have the following workflow
 ```python
@@ -46,15 +49,15 @@
     # Set console level to the same level of the message so it is shown in the console
     lprint(console_log_level="info").info("Workflow ends!")
 
 
 if __name__ == "__main__":
     workflow()
 ```
-- Upin execution the following is printed on console:
+- Upon execution the following is printed on console:
 ```shell
 Workflow starts!
 Workflow ends!
 ```
 - Upon execution a `LOG.log` file is written:
 ```shell
 2023/06/24 | 18:20:50 | ERROR Workflow starts!
@@ -73,93 +76,103 @@
 ## 🚀Useful for
 - Keep track of Python pipelines.
 - Log info about a function during development both on python script or jupyter notebook.
 ***
 
 ## ⚙️Installation
 - Create your own virtual environment and run `pip install -r requirements.txt`
-- Via pip: `pip install pyDecLog`   
+- Via pip: `pip install pyDecLog`
 ***
 
 ## 🔗Dependencies
 - PyDevLog requires Python 3.5 or higher, and the following packages:
   - `pympler`
   - `numpy`
 ***
 
 ## 🧑‍🤝‍🧑Contributions
 - All contributions (bug, suggestion, new feature) are welcome.
 ***
 
 ## 🎨Available decorators
-- `@comment`: log all the print statements inside a decorated function
-- `@timing`: log the function elapsed time
-- `@signature`: log function's signature
 - `@arguments`: log function's args and kwargs
-- `@message`: log the function's print statements
-- `@typing`: log function's args, kwargs and output type
-- `@memory`: log function's args, kwargs and output their memory usage
+- `@comment`: log all function's inner print statements
 - `@description`: log function's output from the `__doc__` dunder method
-- `@profile_local`: log function's local persistent variables.
+- `@machine`: log machine OS system and hardware
+- `@memory`: log function's args, kwargs and output memory usage
+- `@message`: log function's print statements
+- `@profile_locals`: log function's local persistent variables
+- `@signature`: log function's signature
+- `@timing`: log function's elapsed time
+- `@typing`: log function's args, kwargs and output type
+- `@user`: log user info
 ***
 
 ## 🪄Features
 - Mix and match the decorators you want.
 - Can control logging levels as a whole or individually. Choose from the following:
   - `CRITICAL`
   - `ERROR`
   - `WARNING`
   - `INFO`
   - `DEBUG`
 - Can control where logging messages are piped: to log file or both log file and console. When controlling the message at the console level the following hierarchy is enforced:
-  ```
-    CRITICAL : 50
-    ERROR    : 40
-    WARNING  : 30
-    INFO     : 20
-    DEBUG    : 10
-    NOTSET   : 0
-  ```
+```
+CRITICAL : 50
+ERROR    : 40
+WARNING  : 30
+INFO     : 20
+DEBUG    : 10
+NOTSET   : 0
+```
 - Can add comments directly to log file even outside a function.
 ***
 
 ## ⚠️Known issues
-- `@profile_locals` does not write to the log file. Its output needs to be piped separately to the log. See the following example:
+- `@profile_locals` does not write to the log file. Its output needs to be piped separately to the LOG.log file. See the following example:
 ```python
 from pyDecLog import profile_locals as profile
 from pyDecLog import lprint
+from pympler.asizeof import asizeof
 
 @profile
-def func():
-    local1 = 1
-    local2 = 2
+def func(x):
+    local_1 = 1
+    local_2 = 2
     return 1
 
 func()
 
 for key, value in func.locals.items():
     msg = f"Variable: {key} | value: {value} | type: {type(value)} | size: {asizeof(value)}"
 
     lprint(console_log_level="debug").debug(msg)
 ```
+- The following `LOG.log` is the written:
+```shell
+2023/06/28 | 07:04:52 | DEBUG Variable: x | value: 1 | type: <class 'int'> | size: 32
+2023/06/28 | 07:04:52 | DEBUG Variable: local_1 | value: 1 | type: <class 'int'> | size: 32
+2023/06/28 | 07:04:52 | DEBUG Variable: local_2 | value: 2 | type: <class 'int'> | size: 32
+```
 ***
 
 ## 📚Tutorials
 - See the `examples` folder.
 ***
 
 ## 📚References
 - [Decorators with parameters?](https://stackoverflow.com/questions/5929107/decorators-with-parameters)
 - [How to expose persistent local variables? Part#1](https://code.activestate.com/recipes/577283-decorator-to-expose-local-variables-of-a-function-/)
 - [How to expose persistent local variables? Part#2](https://stackoverflow.com/questions/9186395/python-is-there-a-way-to-get-a-local-function-variable-from-within-a-decorator)
 - [How to time your code](https://stackoverflow.com/questions/17579357/time-time-vs-timeit-timeit)
 ***
 
 ## 📝Changelog
-- `0.1.4`  first release (26/06/23).
+- `0.1.6` - First release (26/06/23).
+- `0.1.7` - Added `@machine` and  `@user` (29/06/23).
 ***
 
 ## 📝To-do
 - There is no planned development.
 ***
 
 ## 🪪License
```

### Comparing `pyDecLog-0.1.6/examples/@arguments/@arguments.ipynb` & `pyDecLog-0.1.7/examples/@arguments/@arguments.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/@description/@description.ipynb` & `pyDecLog-0.1.7/examples/@description/@description.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/@memory/@memory.ipynb` & `pyDecLog-0.1.7/examples/@memory/@memory.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/@message/@message.ipynb` & `pyDecLog-0.1.7/examples/@message/@message.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/@profile_locals/@profile_locals.ipynb` & `pyDecLog-0.1.7/examples/multiple_decorators/multiple_decorators.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9264274691358024%*

 * *Differences: {"'cells'": "{0: {'id': 'de24a110', 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2023-06-26T20:23:43.113411Z', 'start_time': '2023-06-26T20:23:43.027001Z'}}, "*

 * *            "'source': {insert: [(0, 'from pyDecLog import arguments as arg\\n'), (1, 'from "*

 * *            "pyDecLog import signature as sign\\n'), (2, 'from pyDecLog import message as "*

 * *            "mes\\n'), (3, 'from pyDecLog import timing as tim\\n'), (5, 'from pyDecLog import "*

 * *            "description as doc\\n'), (6, 'from pyDecLog  […]*

```diff
@@ -1,184 +1,119 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "dc4d14df",
+            "id": "de24a110",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.062358Z",
-                    "start_time": "2023-06-26T20:21:35.974138Z"
+                    "end_time": "2023-06-26T20:23:43.113411Z",
+                    "start_time": "2023-06-26T20:23:43.027001Z"
                 }
             },
             "outputs": [],
             "source": [
-                "from pyDecLog import profile_locals as profile\n",
+                "from pyDecLog import arguments as arg\n",
+                "from pyDecLog import signature as sign\n",
+                "from pyDecLog import message as mes\n",
+                "from pyDecLog import timing as tim\n",
                 "from pyDecLog import lprint\n",
-                "from pympler.asizeof import asizeof"
+                "from pyDecLog import description as doc\n",
+                "from pyDecLog import memory as mem\n",
+                "import time"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "6decb965",
+            "id": "d1aaae69",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.187102Z",
-                    "start_time": "2023-06-26T20:21:36.063824Z"
+                    "end_time": "2023-06-26T20:23:43.118176Z",
+                    "start_time": "2023-06-26T20:23:43.115033Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "rm: LOG.log: No such file or directory\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "rm LOG.log"
+                "@doc\n",
+                "@sign\n",
+                "@arg\n",
+                "@tim\n",
+                "@mes\n",
+                "def sum_(first, second=2):\n",
+                "    \"\"\"Sum two numbers.\"\"\"\n",
+                "\n",
+                "    print(\"Some message on console\")\n",
+                "    result = first + second\n",
+                "    time.sleep(2)\n",
+                "    print(\"Result is: \" + str(result))\n",
+                "    return result"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "04d6842e",
+            "id": "2ec36230",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.193566Z",
-                    "start_time": "2023-06-26T20:21:36.190799Z"
+                    "end_time": "2023-06-26T20:23:45.130641Z",
+                    "start_time": "2023-06-26T20:23:43.120967Z"
                 }
             },
             "outputs": [],
             "source": [
-                "@profile\n",
-                "def func(x):    \n",
-                "    local1 = 1\n",
-                "    local2 = 2\n",
-                "    return x"
+                "%timeit\n",
+                "dummy = sum_(1,1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "7e4782d1",
+            "id": "f5c35439",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.197855Z",
-                    "start_time": "2023-06-26T20:21:36.195529Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "output = func(1)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "id": "16f4c167",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.210141Z",
-                    "start_time": "2023-06-26T20:21:36.199790Z"
-                }
-            },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "{'x': 1, 'local1': 1, 'local2': 2}"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "func.locals"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "id": "94b954b8",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.219724Z",
-                    "start_time": "2023-06-26T20:21:36.212057Z"
-                }
-            },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Variable: x | value: 1 | type: <class 'int'> | size: 32\n",
-                        "Variable: local1 | value: 1 | type: <class 'int'> | size: 32\n",
-                        "Variable: local2 | value: 2 | type: <class 'int'> | size: 32\n"
-                    ]
-                }
-            ],
-            "source": [
-                "for key, value in func.locals.items():\n",
-                "    msg = f\"Variable: {key} | value: {value} | type: {type(value)} | size: {asizeof(value)}\"\n",
-                "\n",
-                "    lprint(console_log_level=\"debug\").debug(msg)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "id": "c1a74b32",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-06-26T20:21:36.346514Z",
-                    "start_time": "2023-06-26T20:21:36.221865Z"
+                    "end_time": "2023-06-26T20:23:45.262547Z",
+                    "start_time": "2023-06-26T20:23:45.133318Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023/06/26 | 21:21:36 | DEBUG Variable: x | value: 1 | type: <class 'int'> | size: 32\r\n",
-                        "2023/06/26 | 21:21:36 | DEBUG Variable: local1 | value: 1 | type: <class 'int'> | size: 32\r\n",
-                        "2023/06/26 | 21:21:36 | DEBUG Variable: local2 | value: 2 | type: <class 'int'> | size: 32\r\n"
+                        "2023/06/26 | 21:23:43 | DEBUG Method's description: Sum two numbers.\r\n",
+                        "2023/06/26 | 21:23:43 | DEBUG Method's name: sum_\r\n",
+                        "2023/06/26 | 21:23:43 | DEBUG Method's signature: (first, second=2)\r\n",
+                        "2023/06/26 | 21:23:43 | DEBUG Method's name: sum_\r\n",
+                        "2023/06/26 | 21:23:43 | DEBUG Method's args: (1, 1)\r\n",
+                        "2023/06/26 | 21:23:43 | DEBUG Method's kwargs: {}\r\n",
+                        "2023/06/26 | 21:23:45 | INFO Some message on console\r\n",
+                        "2023/06/26 | 21:23:45 | INFO Result is: 2\r\n",
+                        "2023/06/26 | 21:23:45 | DEBUG sum_ was executed in: 2.005 sec\r\n"
                     ]
                 }
             ],
             "source": [
                 "cat LOG.log"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a70d1584",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f8aeba37",
+            "id": "16088581",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "trainingAI",
             "language": "python",
-            "name": "python3"
+            "name": "trainingai"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `pyDecLog-0.1.6/examples/@signature/@signature.ipynb` & `pyDecLog-0.1.7/examples/@signature/@signature.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/@timing/@timing.ipynb` & `pyDecLog-0.1.7/examples/@timing/@timing.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/@typing/@typing.ipynb` & `pyDecLog-0.1.7/examples/@typing/@typing.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/examples/lprint/lprint.ipynb` & `pyDecLog-0.1.7/examples/lprint/lprint.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802389705882353%*

 * *Differences: {"'cells'": "{0: {'execution_count': None, 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2023-06-29T09:06:19.334464Z', 'start_time': '2023-06-29T09:06:19.209779Z'}}}, 1: "*

 * *            "{'execution_count': None}, 2: {'execution_count': None}, 3: {'execution_count': "*

 * *            "None}, 4: {'execution_count': None}, 5: {'execution_count': None}, 6: "*

 * *            "{'execution_count': None, 'outputs': []}, 7: {'execution_count': None, 'outputs': "*

 * *            "[]}, 8: {'execution_count': None}, 9: { […]*

```diff
@@ -1,183 +1,155 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "id": "9cb27718",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-27T08:20:07.739784Z",
-                    "start_time": "2023-06-27T08:20:07.648708Z"
+                    "end_time": "2023-06-29T09:06:19.334464Z",
+                    "start_time": "2023-06-29T09:06:19.209779Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from pyDecLog import lprint"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "id": "45c5909a",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:07.863992Z",
                     "start_time": "2023-06-27T08:20:07.741557Z"
                 }
             },
             "outputs": [],
             "source": [
                 "rm LOG.log"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "id": "8384c3a8",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:07.872199Z",
                     "start_time": "2023-06-27T08:20:07.868291Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").info(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "id": "4769e6bc",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:07.877535Z",
                     "start_time": "2023-06-27T08:20:07.874011Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").debug(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "id": "dc49abfd",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:07.882597Z",
                     "start_time": "2023-06-27T08:20:07.879448Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").warning(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "id": "574e4456",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:07.887116Z",
                     "start_time": "2023-06-27T08:20:07.884154Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").error(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "id": "8fb665d2",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:07.892617Z",
                     "start_time": "2023-06-27T08:20:07.888842Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "simple CRITICAL message\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").critical(\"simple CRITICAL message\") "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "id": "406e0cf9",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.018051Z",
                     "start_time": "2023-06-27T08:20:07.894519Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "2023/06/27 | 09:20:07 | INFO simple message\r\n",
-                        "2023/06/27 | 09:20:07 | DEBUG simple message\r\n",
-                        "2023/06/27 | 09:20:07 | WARNING simple message\r\n",
-                        "2023/06/27 | 09:20:07 | ERROR simple message\r\n",
-                        "2023/06/27 | 09:20:07 | CRITICAL simple CRITICAL message\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "cat LOG.log"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": null,
             "id": "8f069c4c",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.151067Z",
                     "start_time": "2023-06-27T08:20:08.023489Z"
                 }
             },
             "outputs": [],
             "source": [
                 "rm LOG.log"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "id": "56a6761b",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.161165Z",
                     "start_time": "2023-06-27T08:20:08.153609Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Results 5 is: 3\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "lprint = lprint(console_log_level=\"critical\")\n",
                 "def sum_(first=0, second=0):\n",
                 "    \"\"\"Sum two numbers.\n",
                 "    \"\"\"\n",
                 "\n",
                 "    result = first + second    \n",
@@ -189,35 +161,23 @@
                 "    \n",
                 "    return result\n",
                 "dummy = sum_(1,2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": null,
             "id": "b85bfd41",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.292458Z",
                     "start_time": "2023-06-27T08:20:08.163599Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "2023/06/27 | 09:20:08 | INFO Results 1 is: 3\r\n",
-                        "2023/06/27 | 09:20:08 | DEBUG Results 2 is: 3\r\n",
-                        "2023/06/27 | 09:20:08 | WARNING Results 3 is: 3\r\n",
-                        "2023/06/27 | 09:20:08 | ERROR Results 4 is: 3\r\n",
-                        "2023/06/27 | 09:20:08 | CRITICAL Results 5 is: 3\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "cat LOG.log"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "45223a88",
@@ -234,86 +194,62 @@
             "source": [
                 "- Logging an exception in python with an error can be done in the `logging.exception()` method.\n",
                 "- This function logs a message with level `ERROR` on this logger. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": null,
             "id": "bb2c6349",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.425251Z",
                     "start_time": "2023-06-27T08:20:08.295718Z"
                 }
             },
             "outputs": [],
             "source": [
                 "rm LOG.log"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": null,
             "id": "4c06ea42",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.433921Z",
                     "start_time": "2023-06-27T08:20:08.428526Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Error occurred while printing pyDecLog\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from pyDecLog import lprint\n",
                 "\n",
                 "try:\n",
                 "    printf(\"GeeksforGeeks\")\n",
                 "except Exception as Argument:\n",
                 "    # Equivalent to logging.exception(\"Error occurred while printing pyDecLog\")    \n",
                 "    lprint(console_log_level=\"error\").error(\"Error occurred while printing pyDecLog\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": null,
             "id": "01442a6c",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-06-27T08:20:08.562108Z",
                     "start_time": "2023-06-27T08:20:08.435722Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "2023/06/27 | 09:20:08 | ERROR Error occurred while printing pyDecLog\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "cat LOG.log"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "7ecbab2c",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "trainingAI",
             "language": "python",
             "name": "trainingai"
```

### Comparing `pyDecLog-0.1.6/examples/workflow/workflow.py` & `pyDecLog-0.1.7/examples/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/pyDecLog.egg-info/PKG-INFO` & `pyDecLog-0.1.7/pyDecLog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecLog
-Version: 0.1.6
+Version: 0.1.7
 Summary: pyDecLog: a Python module for logging via decorators
 Home-page: https://github.com/kyaiooiayk/pyDecLog
 Author: kyaiooiayk
 Author-email: kayaiooiayk@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
@@ -13,14 +13,17 @@
 
 # pyDecLog
 
 ![PyPI Version](https://img.shields.io/pypi/v/pyDecLog.svg)
 ![Python Version](https://img.shields.io/pypi/pyversions/pyDecLog.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyDecLog)
 ![License](https://img.shields.io/pypi/l/pyDecLog)
+![Stars](https://img.shields.io/github/stars/kyaiooiayk/pyDecLog)
+![Issues](https://img.shields.io/github/issues/kyaiooiayk/pyDecLog)
+![Forks](https://img.shields.io/github/forks/kyaiooiayk/pyDecLog)
 
 pyDecLog: a simple and easy to use Python module for logging via decorators.
 ***
 
 ## 🚀Quick start
 - Say we have the following workflow
 ```python
@@ -59,15 +62,15 @@
     # Set console level to the same level of the message so it is shown in the console
     lprint(console_log_level="info").info("Workflow ends!")
 
 
 if __name__ == "__main__":
     workflow()
 ```
-- Upin execution the following is printed on console:
+- Upon execution the following is printed on console:
 ```shell
 Workflow starts!
 Workflow ends!
 ```
 - Upon execution a `LOG.log` file is written:
 ```shell
 2023/06/24 | 18:20:50 | ERROR Workflow starts!
@@ -86,93 +89,103 @@
 ## 🚀Useful for
 - Keep track of Python pipelines.
 - Log info about a function during development both on python script or jupyter notebook.
 ***
 
 ## ⚙️Installation
 - Create your own virtual environment and run `pip install -r requirements.txt`
-- Via pip: `pip install pyDecLog`   
+- Via pip: `pip install pyDecLog`
 ***
 
 ## 🔗Dependencies
 - PyDevLog requires Python 3.5 or higher, and the following packages:
   - `pympler`
   - `numpy`
 ***
 
 ## 🧑‍🤝‍🧑Contributions
 - All contributions (bug, suggestion, new feature) are welcome.
 ***
 
 ## 🎨Available decorators
-- `@comment`: log all the print statements inside a decorated function
-- `@timing`: log the function elapsed time
-- `@signature`: log function's signature
 - `@arguments`: log function's args and kwargs
-- `@message`: log the function's print statements
-- `@typing`: log function's args, kwargs and output type
-- `@memory`: log function's args, kwargs and output their memory usage
+- `@comment`: log all function's inner print statements
 - `@description`: log function's output from the `__doc__` dunder method
-- `@profile_local`: log function's local persistent variables.
+- `@machine`: log machine OS system and hardware
+- `@memory`: log function's args, kwargs and output memory usage
+- `@message`: log function's print statements
+- `@profile_locals`: log function's local persistent variables
+- `@signature`: log function's signature
+- `@timing`: log function's elapsed time
+- `@typing`: log function's args, kwargs and output type
+- `@user`: log user info
 ***
 
 ## 🪄Features
 - Mix and match the decorators you want.
 - Can control logging levels as a whole or individually. Choose from the following:
   - `CRITICAL`
   - `ERROR`
   - `WARNING`
   - `INFO`
   - `DEBUG`
 - Can control where logging messages are piped: to log file or both log file and console. When controlling the message at the console level the following hierarchy is enforced:
-  ```
-    CRITICAL : 50
-    ERROR    : 40
-    WARNING  : 30
-    INFO     : 20
-    DEBUG    : 10
-    NOTSET   : 0
-  ```
+```
+CRITICAL : 50
+ERROR    : 40
+WARNING  : 30
+INFO     : 20
+DEBUG    : 10
+NOTSET   : 0
+```
 - Can add comments directly to log file even outside a function.
 ***
 
 ## ⚠️Known issues
-- `@profile_locals` does not write to the log file. Its output needs to be piped separately to the log. See the following example:
+- `@profile_locals` does not write to the log file. Its output needs to be piped separately to the LOG.log file. See the following example:
 ```python
 from pyDecLog import profile_locals as profile
 from pyDecLog import lprint
+from pympler.asizeof import asizeof
 
 @profile
-def func():
-    local1 = 1
-    local2 = 2
+def func(x):
+    local_1 = 1
+    local_2 = 2
     return 1
 
 func()
 
 for key, value in func.locals.items():
     msg = f"Variable: {key} | value: {value} | type: {type(value)} | size: {asizeof(value)}"
 
     lprint(console_log_level="debug").debug(msg)
 ```
+- The following `LOG.log` is the written:
+```shell
+2023/06/28 | 07:04:52 | DEBUG Variable: x | value: 1 | type: <class 'int'> | size: 32
+2023/06/28 | 07:04:52 | DEBUG Variable: local_1 | value: 1 | type: <class 'int'> | size: 32
+2023/06/28 | 07:04:52 | DEBUG Variable: local_2 | value: 2 | type: <class 'int'> | size: 32
+```
 ***
 
 ## 📚Tutorials
 - See the `examples` folder.
 ***
 
 ## 📚References
 - [Decorators with parameters?](https://stackoverflow.com/questions/5929107/decorators-with-parameters)
 - [How to expose persistent local variables? Part#1](https://code.activestate.com/recipes/577283-decorator-to-expose-local-variables-of-a-function-/)
 - [How to expose persistent local variables? Part#2](https://stackoverflow.com/questions/9186395/python-is-there-a-way-to-get-a-local-function-variable-from-within-a-decorator)
 - [How to time your code](https://stackoverflow.com/questions/17579357/time-time-vs-timeit-timeit)
 ***
 
 ## 📝Changelog
-- `0.1.4`  first release (26/06/23).
+- `0.1.6` - First release (26/06/23).
+- `0.1.7` - Added `@machine` and  `@user` (29/06/23).
 ***
 
 ## 📝To-do
 - There is no planned development.
 ***
 
 ## 🪪License
```

### Comparing `pyDecLog-0.1.6/pyDecLog.egg-info/SOURCES.txt` & `pyDecLog-0.1.7/pyDecLog.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 .flake8
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
+CHANGELOG.md
+CONTRIBUTING.md
 LICENSE
+MANIFEST.in
 README.md
 VERSION
 __init__.py
 pyDecLog.py
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 setup.py
 update_github.sh
 examples/@arguments/@arguments.ipynb
 examples/@description/@description.ipynb
+examples/@machine/@machine.ipynb
 examples/@memory/@memory.ipynb
 examples/@message/@message.ipynb
 examples/@profile_locals/@profile_locals.ipynb
 examples/@signature/@signature.ipynb
 examples/@timing/@timing.ipynb
+examples/@timing/README.md
 examples/@typing/@typing.ipynb
+examples/@user/@user.ipynb
 examples/lprint/lprint.ipynb
 examples/multiple_decorators/multiple_decorators.ipynb
 examples/workflow/workflow.py
 pyDecLog.egg-info/PKG-INFO
 pyDecLog.egg-info/SOURCES.txt
 pyDecLog.egg-info/dependency_links.txt
 pyDecLog.egg-info/requires.txt
```

### Comparing `pyDecLog-0.1.6/pyDecLog.py` & `pyDecLog-0.1.7/pyDecLog.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from contextlib import redirect_stdout
 from io import StringIO
 import numpy as np
 import inspect
 from sys import getsizeof
 import sys
 from pympler.asizeof import asizeof
-
+import psutil
+import platform
 
 LOG_FILE_NAME = "LOG"
 LOG_FILE_PATH = "./"
 CONSOLE_LOG_LEVEL = "critical"
 
 
 def lprint(
@@ -41,14 +42,15 @@
     logger_obj = get_logger(
         log_file_name=log_file_name,
         console_log_level=console_log_level,
         log_file_path=log_file_path,
     )
     return logger_obj
 
+
 def _get_time(t_start: float, t_end: float, unit: str):
     """Get elapsed time given the unit.
 
     Parameters
     ----------
     t_start : float
         kernel time at start of process.
@@ -579,14 +581,124 @@
         return res
 
     @property
     def locals(self):
         return self._locals
 
 
+def machine(
+    func_: None = None,
+    level: str = "debug",
+    console_log_level: str = CONSOLE_LOG_LEVEL,
+    log_file_name: str = LOG_FILE_NAME,
+    log_file_path: str = LOG_FILE_PATH,
+):
+    """Profile local machine hardware.
+
+    Parameters
+    ----------
+    func_ : None, optional
+        Wrapped function, by default None
+    level : str, optional
+        Log level: "debug", "info", "critical" or "error", by default "debug"
+    console_log_level : str, optional
+        Console log level. Same options as log level, by default CONSOLE_LOG_LEVEL.
+    log_file_name : str, optional
+        Name of the log file, by default LOG_FILE_NAME.
+    log_file_path : str, optional
+        Path of the log file, by default LOG_FILE_PATH.
+
+    Raises
+    ------
+    RunTimeWarning
+        Raise if called with positional arguments.
+    """
+
+    def _decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            log_level = _get_log_level(
+                level, console_log_level, log_file_name, log_file_path
+            )
+
+            log_level(f"Platform: {platform.platform()}")
+            log_level(f"System: {platform.system()}")
+            log_level(f"Release: {platform.release()}")
+            log_level(f"Version: {platform.version()}")
+            log_level(f"No LOGICAL CPUs? {psutil.cpu_count(logical=True)}")
+            log_level(f"No PHYSICAL CPUs? {psutil.cpu_count(logical=False)}")
+            log_level(f"RAM {psutil.virtual_memory().total/1.e9} [Gb]")
+
+            # Call the decorated function
+            output = func(*args, **kwargs)
+
+            return output
+
+        return wrapper
+
+    if callable(func_):
+        return _decorator(func_)
+    elif func_ is None:
+        return _decorator
+    else:
+        raise RuntimeWarning("Positional arguments are not supported!")
+
+
+def user(
+    func_: None = None,
+    level: str = "debug",
+    console_log_level: str = CONSOLE_LOG_LEVEL,
+    log_file_name: str = LOG_FILE_NAME,
+    log_file_path: str = LOG_FILE_PATH,
+):
+    """Profile local machine hardware.
+
+    Parameters
+    ----------
+    func_ : None, optional
+        Wrapped function, by default None
+    level : str, optional
+        Log level: "debug", "info", "critical" or "error", by default "debug"
+    console_log_level : str, optional
+        Console log level. Same options as log level, by default CONSOLE_LOG_LEVEL.
+    log_file_name : str, optional
+        Name of the log file, by default LOG_FILE_NAME.
+    log_file_path : str, optional
+        Path of the log file, by default LOG_FILE_PATH.
+
+    Raises
+    ------
+    RunTimeWarning
+        Raise if called with positional arguments.
+    """
+
+    def _decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            log_level = _get_log_level(
+                level, console_log_level, log_file_name, log_file_path
+            )
+
+            log_level(f"User: {os.getlogin()}")
+
+            # Call the decorated function
+            output = func(*args, **kwargs)
+
+            return output
+
+        return wrapper
+
+    if callable(func_):
+        return _decorator(func_)
+    elif func_ is None:
+        return _decorator
+    else:
+        raise RuntimeWarning("Positional arguments are not supported!")
+
+
 def get_logger(
     log_file_name: str = LOG_FILE_NAME,
     log_file_path: str = LOG_FILE_PATH,
     console_log_level: str = CONSOLE_LOG_LEVEL,
 ):
     """Creates a Log File and returns Logger object.
```

### Comparing `pyDecLog-0.1.6/setup.py` & `pyDecLog-0.1.7/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     url=URL,
     python_requires=PYTHON_REQUIRES,
     install_requires=INSTALL_REQUIRES,
     extra_requires=EXTRAS_REQUIRES,
     packages=find_packages(),
     py_modules=["pyDecLog"],
     classifiers=CLASSIFIERS,
-)
+)
```

### Comparing `pyDecLog-0.1.6/tests/test_arguments.py` & `pyDecLog-0.1.7/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_description.py` & `pyDecLog-0.1.7/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_get_log_and_level.py` & `pyDecLog-0.1.7/tests/test_get_log_and_level.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_get_memory.py` & `pyDecLog-0.1.7/tests/test_get_memory.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_get_time.py` & `pyDecLog-0.1.7/tests/test_get_time.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_lprint.py` & `pyDecLog-0.1.7/tests/test_lprint.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_memory.py` & `pyDecLog-0.1.7/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_message.py` & `pyDecLog-0.1.7/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_profile_locals.py` & `pyDecLog-0.1.7/tests/test_profile_locals.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_signature.py` & `pyDecLog-0.1.7/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_timing.py` & `pyDecLog-0.1.7/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.6/tests/test_typing.py` & `pyDecLog-0.1.7/tests/test_typing.py`

 * *Files identical despite different names*

