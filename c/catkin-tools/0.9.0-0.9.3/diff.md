# Comparing `tmp/catkin_tools-0.9.0.tar.gz` & `tmp/catkin_tools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catkin_tools-0.9.0.tar", last modified: Thu Jun  9 14:00:10 2022, max compression
+gzip compressed data, was "catkin_tools-0.9.3.tar", last modified: Thu Jun 29 09:31:41 2023, max compression
```

## Comparing `catkin_tools-0.9.0.tar` & `catkin_tools-0.9.3.tar`

### file list

```diff
@@ -1,102 +1,413 @@
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/
--rw-rw-r--   0 timon     (1000) timon     (1000)    11335 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/LICENSE
--rw-rw-r--   0 timon     (1000) timon     (1000)       31 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/MANIFEST.in
--rw-rw-r--   0 timon     (1000) timon     (1000)      634 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/PKG-INFO
--rw-rw-r--   0 timon     (1000) timon     (1000)      316 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/README.md
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.938557 catkin_tools-0.9.0/catkin_tools/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    16585 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/argument_parsing.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.938557 catkin_tools-0.9.0/catkin_tools/commands/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/commands/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10098 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/commands/catkin.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    21324 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/common.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     5025 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/config.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    37140 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/context.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/execution/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    31629 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/controllers.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2304 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/events.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    15199 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/executor.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10053 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/io.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    12798 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/job_server.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1820 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/jobs.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     6599 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/execution/stages.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/jobs/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    27722 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/catkin.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/jobs/cmake/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1918 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/cmake/python.cmake
--rw-rw-r--   0 timon     (1000) timon     (1000)      194 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/cmake/python_install_dir.cmake
--rw-rw-r--   0 timon     (1000) timon     (1000)    16275 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/cmake.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/jobs/commands/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/commands/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     9936 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/commands/cmake.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/commands/make.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     8774 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/jobs/utils.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    17045 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/metadata.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/notifications/
--rw-rw-r--   0 timon     (1000) timon     (1000)      649 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/notifications/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2302 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/notifications/impl.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.934557 catkin_tools-0.9.0/catkin_tools/notifications/resources/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/notifications/resources/linux/
--rw-rw-r--   0 timon     (1000) timon     (1000)    56725 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/notifications/resources/linux/catkin_icon.png
--rw-rw-r--   0 timon     (1000) timon     (1000)    31033 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/notifications/resources/linux/catkin_icon_red.png
--rw-rw-r--   0 timon     (1000) timon     (1000)     6716 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/resultspace.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/spaces/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/spaces/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      767 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/spaces/build.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      826 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/spaces/devel.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      755 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/spaces/install.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      748 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/spaces/log.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      762 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/spaces/source.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     5462 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/terminal_color.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1524 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/utils.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/verbs/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/__init__.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/
--rw-rw-r--   0 timon     (1000) timon     (1000)      960 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    30472 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/build.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    18499 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/cli.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/color.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/
--rw-rw-r--   0 timon     (1000) timon     (1000)      863 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7474 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/clean.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    17214 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_config/
--rw-rw-r--   0 timon     (1000) timon     (1000)      975 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_config/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10272 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_config/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_create/
--rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_create/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     6751 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_create/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.942557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_env/
--rw-rw-r--   0 timon     (1000) timon     (1000)      965 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_env/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     3921 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_env/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_init/
--rw-rw-r--   0 timon     (1000) timon     (1000)      868 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_init/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1956 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_init/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_list/
--rw-rw-r--   0 timon     (1000) timon     (1000)      885 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_list/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7864 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_list/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_locate/
--rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_locate/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7099 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_locate/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_profile/
--rw-rw-r--   0 timon     (1000) timon     (1000)      868 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_profile/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10205 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_profile/cli.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2975 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_shell_verbs.bash
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/
--rw-rw-r--   0 timon     (1000) timon     (1000)      901 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7892 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/cli.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     9462 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/test.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.938557 catkin_tools-0.9.0/catkin_tools.egg-info/
--rw-rw-r--   0 timon     (1000) timon     (1000)      634 2022-06-09 14:00:10.000000 catkin_tools-0.9.0/catkin_tools.egg-info/PKG-INFO
--rw-rw-r--   0 timon     (1000) timon     (1000)     2617 2022-06-09 14:00:10.000000 catkin_tools-0.9.0/catkin_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)        1 2022-06-09 14:00:10.000000 catkin_tools-0.9.0/catkin_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      986 2022-06-09 14:00:10.000000 catkin_tools-0.9.0/catkin_tools.egg-info/entry_points.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       56 2022-06-09 14:00:10.000000 catkin_tools-0.9.0/catkin_tools.egg-info/requires.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       13 2022-06-09 14:00:10.000000 catkin_tools-0.9.0/catkin_tools.egg-info/top_level.txt
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/completion/
--rw-rw-r--   0 timon     (1000) timon     (1000)    23450 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/completion/_catkin
--rw-rw-r--   0 timon     (1000) timon     (1000)     4989 2022-06-09 13:28:01.000000 catkin_tools-0.9.0/completion/catkin.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)       38 2022-06-09 14:00:10.946557 catkin_tools-0.9.0/setup.cfg
--rw-rw-r--   0 timon     (1000) timon     (1000)     5365 2022-06-09 13:34:56.000000 catkin_tools-0.9.0/setup.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/.github/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1782 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/.github/workflows/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1998 2023-02-23 16:54:15.000000 catkin_tools-0.9.3/.github/workflows/workflow.yml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      349 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/.gitignore
+-rw-rw-r--   0 timon     (1000) timon     (1000)    26060 2023-02-23 16:59:56.000000 catkin_tools-0.9.3/CHANGELOG.rst
+-rw-r--r--   0 timon     (1000) timon     (1000)    11335 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/LICENSE
+-rw-rw-r--   0 timon     (1000) timon     (1000)       31 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/MANIFEST.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)      615 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/PKG-INFO
+-rw-rw-r--   0 timon     (1000) timon     (1000)      316 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/README.md
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/catkin_tools/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    16585 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/argument_parsing.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/commands/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/catkin_tools/commands/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10098 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/commands/catkin.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    21324 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/common.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5025 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/config.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    37403 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/context.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/execution/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    31661 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/execution/controllers.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2304 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/events.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    15425 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/execution/executor.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10053 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/io.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    12798 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/job_server.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1820 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/jobs.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6599 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/stages.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/jobs/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    27764 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/jobs/catkin.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/jobs/cmake/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1918 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/cmake/python.cmake
+-rw-rw-r--   0 timon     (1000) timon     (1000)      194 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/cmake/python_install_dir.cmake
+-rw-rw-r--   0 timon     (1000) timon     (1000)    16276 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/jobs/cmake.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/jobs/commands/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/commands/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     9936 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/commands/cmake.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/commands/make.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8774 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/utils.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    17302 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/metadata.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/
+-rw-r--r--   0 timon     (1000) timon     (1000)      649 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/notifications/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2302 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/impl.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/
+-rw-r--r--   0 timon     (1000) timon     (1000)    56725 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon.png
+-rw-rw-r--   0 timon     (1000) timon     (1000)    31033 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_red.png
+-rw-rw-r--   0 timon     (1000) timon     (1000)    31532 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_yellow.png
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/
+-rw-r--r--   0 timon     (1000) timon     (1000)     1610 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Info.plist
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/
+-rwxr-xr-x   0 timon     (1000) timon     (1000)    20880 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/catkin build
+-rw-r--r--   0 timon     (1000) timon     (1000)        8 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/PkgInfo
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/
+-rw-r--r--   0 timon     (1000) timon     (1000)    67336 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 timon     (1000) timon     (1000)   107025 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/catkin_blue_logo_only.icns
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/
+-rw-r--r--   0 timon     (1000) timon     (1000)      436 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/Credits.rtf
+-rw-r--r--   0 timon     (1000) timon     (1000)       92 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/InfoPlist.strings
+-rw-r--r--   0 timon     (1000) timon     (1000)    26323 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/MainMenu.nib
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/
+-rw-r--r--   0 timon     (1000) timon     (1000)       74 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/.gitignore
+-rw-r--r--   0 timon     (1000) timon     (1000)    67336 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/AppIcon.icns
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8026 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/README.markdown
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/
+-rw-r--r--   0 timon     (1000) timon     (1000)      122 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.h
+-rw-r--r--   0 timon     (1000) timon     (1000)     3113 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.m
+-rw-r--r--   0 timon     (1000) timon     (1000)     1178 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Info.plist
+-rw-r--r--   0 timon     (1000) timon     (1000)      165 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Prefix.pch
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/
+-rw-r--r--   0 timon     (1000) timon     (1000)      436 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/Credits.rtf
+-rw-r--r--   0 timon     (1000) timon     (1000)       45 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/InfoPlist.strings
+-rw-r--r--   0 timon     (1000) timon     (1000)    45931 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/MainMenu.xib
+-rw-r--r--   0 timon     (1000) timon     (1000)      119 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/main.m
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/
+-rw-r--r--   0 timon     (1000) timon     (1000)    13799 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.pbxproj
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 timon     (1000) timon     (1000)      162 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 timon     (1000) timon     (1000)     1593 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/Terminal Notifier.xccheckout
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 timon     (1000) timon     (1000)     5102 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/Terminal Notifier.xcscheme
+-rw-r--r--   0 timon     (1000) timon     (1000)   107025 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/catkin_blue_logo_only.icns
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 timon     (1000) timon     (1000)     1174 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 timon     (1000) timon     (1000)     9426 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only128x128.png
+-rw-r--r--   0 timon     (1000) timon     (1000)     3212 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only16x16.png
+-rw-r--r--   0 timon     (1000) timon     (1000)    16330 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only256x256.png
+-rw-r--r--   0 timon     (1000) timon     (1000)     3961 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only32x32.png
+-rw-r--r--   0 timon     (1000) timon     (1000)    35515 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only512x512.png
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6716 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/resultspace.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/spaces/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      767 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/build.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      826 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/devel.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      755 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/install.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      748 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/log.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      762 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/source.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5462 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/terminal_color.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1524 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/utils.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/catkin_tools/verbs/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/
+-rw-r--r--   0 timon     (1000) timon     (1000)      960 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    30330 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/build.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    18708 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/cli.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/color.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/
+-rw-r--r--   0 timon     (1000) timon     (1000)      863 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7474 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/clean.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    17214 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/
+-rw-r--r--   0 timon     (1000) timon     (1000)      975 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10902 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6751 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      965 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3921 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/
+-rw-r--r--   0 timon     (1000) timon     (1000)      868 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1956 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      885 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7864 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/
+-rw-r--r--   0 timon     (1000) timon     (1000)      871 2022-04-19 21:21:18.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7099 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/
+-rw-r--r--   0 timon     (1000) timon     (1000)      868 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10205 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/cli.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2975 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_shell_verbs.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      901 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7892 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/cli.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     9462 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/test.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools.egg-info/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      615 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 timon     (1000) timon     (1000)    15182 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)        1 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      985 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       56 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/requires.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       13 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/top_level.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/completion/
+-rw-rw-r--   0 timon     (1000) timon     (1000)    23450 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/completion/_catkin
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5109 2023-02-23 16:54:15.000000 catkin_tools-0.9.3/completion/catkin.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/
+-rw-r--r--   0 timon     (1000) timon     (1000)        7 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/.gitignore
+-rw-r--r--   0 timon     (1000) timon     (1000)     6786 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/Makefile
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/_static/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/_static/.gitignore
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/_templates/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/_templates/.gitignore
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/advanced/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1001 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/catkin_shell_verbs.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)    41154 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_events.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)    86468 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_events.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)    45234 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_job_lifecycle.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)    78602 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_job_resources.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)     9187 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/job_executor.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1387 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/linked_develspace.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3892 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/verb_customization.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4580 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/build_types.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)    36590 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/catkin_build.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)   180757 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/catkin_tools_execution.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4795 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/cheat_sheet.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8838 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/conf.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/development/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2867 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/development/adding_build_types.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5950 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/development/extending_the_catkin_command.rst
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1120 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/README.md
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/
+-rwxrwxr-x   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/0_init.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      128 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/1_build_warning.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      124 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/2_build_err.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      269 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/all.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/docs/examples/failure_ws/src/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5270 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1926 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/sub/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      150 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/sub/CMakeLists.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5321 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1929 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5189 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       60 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1923 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5199 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      118 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/grep-errors.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1926 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/quickstart_ws/
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      914 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/0_quickstart.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      108 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/1_prebuild.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      254 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/1_prebuild.out
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      109 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/2_postbuild.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1278 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/2_postbuild.out
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      309 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/all.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      571 2023-06-29 09:20:07.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/0_checkout.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)       99 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/1_init.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      107 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/2_dry_run.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      236 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/3_build.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      118 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/4_build_v.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      125 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/5_build_i.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      110 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/6_build_partial.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      231 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/7_build_this.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      124 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/8_build_start_with.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/9_build_no_deps.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      601 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/all.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      395 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/slowrecord
+-rwxrwxr-x   0 timon     (1000) timon     (1000)     1812 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/slowrun
+-rw-rw-r--   0 timon     (1000) timon     (1000)    21600 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/executor_job_lifecycle.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)   118107 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/executor_job_lifecycle.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6066 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/history.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4405 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/index.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/installing.rst
+-rw-r--r--   0 timon     (1000) timon     (1000)     6713 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/make.bat
+-rw-rw-r--   0 timon     (1000) timon     (1000)    20283 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/mechanics.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)    19362 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/migration.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7960 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/quick_start.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      479 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/spelling_wordlist.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2722 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/troubleshooting.rst
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/docs/verbs/
+-rw-rw-r--   0 timon     (1000) timon     (1000)    14082 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_build.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4144 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_clean.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8995 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_config.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      403 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_create.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      500 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_env.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      998 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_init.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1338 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_list.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      398 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_locate.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6824 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_profile.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1931 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_test.rst
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/docs/verbs/cli/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6864 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_build.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2920 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_clean.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8287 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_config.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      631 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_create.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2669 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_create_pkg.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      822 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_env.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      469 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_init.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1965 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_list.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2323 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_locate.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      739 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_add.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      286 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_list.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      186 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_remove.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      309 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_rename.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      165 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_set.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3091 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_test.txt
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      665 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/dump_cli
+-rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/requirements.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       38 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/setup.cfg
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5365 2023-02-23 17:00:06.000000 catkin_tools-0.9.3/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      257 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/stdeb.cfg
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1250 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/README.md
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/tests/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.3/tests/system/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/tests/system/resources/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/build_type_condition/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       69 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/build_type_condition/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      425 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/build_type_condition/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_args/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      301 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_args/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      308 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_args/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      167 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      304 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_warning/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      161 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_warning/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      311 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_warning/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/depend_condition/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       69 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/depend_condition/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      404 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/depend_condition/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      134 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       37 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/fail.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      299 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      135 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      304 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       40 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/warn.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      636 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/CMakeLists.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/cmake/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       30 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/cmake/extras.cmake.develspace.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)       32 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/cmake/extras.cmake.installspace.in
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/include/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/include/make_products_0/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/include/make_products_0/fun.h
+-rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/lib.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      302 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      790 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/CMakeLists.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/cmake/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       36 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/cmake/extras.cmake.develspace.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)       38 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/cmake/extras.cmake.installspace.in
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/include/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/include/make_products_0/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/include/make_products_0/fun.h
+-rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/lib.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      308 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      129 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      270 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      218 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/setup.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)       33 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/lib.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      181 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      307 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      361 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/test_good.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      185 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      335 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      360 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/test_bad.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      225 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      318 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      360 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/test_bad.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      361 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/test_good.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      333 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      287 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/vanilla.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      207 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      250 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       70 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/vanilla.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1341 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      110 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/Config.cmake.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)      248 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       97 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/vanilla.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)       17 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/vanilla.h
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      273 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      281 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/test.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      269 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      277 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/test.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      173 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       49 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      334 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.3/tests/system/verbs/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_build/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3055 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_args.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    18014 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_build.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_bwlists.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      564 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_context.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1126 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_eclipse.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1152 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_modify_ws.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4604 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_pythonpath.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_unicode_in_env.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_whitespace_in_paths.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_clean/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_clean/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3820 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_clean/clean.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_config/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_config/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2836 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_config/test_config.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_init/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_init/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      838 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_init/test_init.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_profile/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_profile/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2610 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_profile/test_profile.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_test/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_test/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2935 2023-01-30 11:25:43.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_test/test_unit_tests.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5447 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/workspace_factory.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/test_code_format.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/unit/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 15:57:45.000000 catkin_tools-0.9.3/tests/unit/__init__.py
+-rw-r--r--   0 timon     (1000) timon     (1000)       13 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/tests/unit/ascii_text.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2437 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_common.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4649 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/unit/test_config.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      374 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_io.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4351 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_job_flag_regex.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1137 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_jobs.py
+-rw-r--r--   0 timon     (1000) timon     (1000)       17 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/tests/unit/unicode_text.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5260 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/tests/utils.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1234 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/workspace_assertions.py
```

### Comparing `catkin_tools-0.9.0/LICENSE` & `catkin_tools-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/PKG-INFO` & `catkin_tools-0.9.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: catkin_tools
-Version: 0.9.0
+Version: 0.9.3
 Summary: Command line tools for working with catkin.
 Home-page: https://catkin-tools.readthedocs.org/
 Author: William Woodall
 Author-email: william@osrfoundation.org
 Maintainer: William Woodall
 Maintainer-email: william@osrfoundation.org
 License: Apache 2.0
 Keywords: catkin
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 License-File: LICENSE
 
 Provides command line tools for working with catkin.
-
```

### Comparing `catkin_tools-0.9.0/catkin_tools/argument_parsing.py` & `catkin_tools-0.9.3/catkin_tools/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/commands/catkin.py` & `catkin_tools-0.9.3/catkin_tools/commands/catkin.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/common.py` & `catkin_tools-0.9.3/catkin_tools/common.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/config.py` & `catkin_tools-0.9.3/catkin_tools/config.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/context.py` & `catkin_tools-0.9.3/catkin_tools/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,16 @@
                 return None
             else:
                 workspace = workspace_hint
         opts_vars['workspace'] = workspace
 
         # Get the active profile
         profile = profile or opts_vars.get('profile', None) or metadata.get_active_profile(workspace)
+        if not metadata.active_profile_set(workspace):
+            metadata.set_active_profile(workspace, profile)
         opts_vars['profile'] = profile
 
         # Initialize empty metadata/args
         config_metadata = {}
         context_args = {}
 
         # Get the metadata stored in the workspace if it was found
@@ -445,39 +447,41 @@
         if self.install:
             sticky_env = get_resultspace_environment(self.install_space_abs, quiet=True)
         else:
             sticky_env = get_resultspace_environment(self.devel_space_abs, quiet=True)
 
         self.cached_cmake_prefix_path = ''
         if 'CMAKE_PREFIX_PATH' in sticky_env:
-            split_result_cmake_prefix_path = sticky_env.get('CMAKE_PREFIX_PATH', '').split(':')
+            split_result_cmake_prefix_path = \
+                sticky_env.get('CMAKE_PREFIX_PATH', '').replace('::', ':').strip(':').split(':')
             if len(split_result_cmake_prefix_path) > 1:
                 self.cached_cmake_prefix_path = ':'.join(split_result_cmake_prefix_path[1:])
 
         # Either load an explicit environment or get it from the current environment
         self.env_cmake_prefix_path = ''
         if self.extend_path:
             extended_env = get_resultspace_environment(self.extend_path, quiet=False)
-            self.env_cmake_prefix_path = extended_env.get('CMAKE_PREFIX_PATH', '')
+            self.env_cmake_prefix_path = extended_env.get('CMAKE_PREFIX_PATH', '').replace('::', ':').strip(':')
             if not self.env_cmake_prefix_path:
                 print(clr("@!@{rf}Error:@| Could not load environment from workspace: '{}', "
                           "target environment (env.sh) does not provide 'CMAKE_PREFIX_PATH'").format(self.extend_path))
                 print(extended_env)
                 sys.exit(1)
         else:
             # Get the current CMAKE_PREFIX_PATH
             if 'CMAKE_PREFIX_PATH' in os.environ:
-                split_result_cmake_prefix_path = os.environ['CMAKE_PREFIX_PATH'].split(':')
+                split_result_cmake_prefix_path = \
+                    os.environ['CMAKE_PREFIX_PATH'].replace('::', ':').strip(':').split(':')
                 if len(split_result_cmake_prefix_path) > 1 and (
                         (not self.install and split_result_cmake_prefix_path[0] == self.devel_space_abs) or
                         (self.install and split_result_cmake_prefix_path[0] == self.install_space_abs)):
 
                     self.env_cmake_prefix_path = ':'.join(split_result_cmake_prefix_path[1:])
                 else:
-                    self.env_cmake_prefix_path = os.environ.get('CMAKE_PREFIX_PATH', '').rstrip(':')
+                    self.env_cmake_prefix_path = os.environ.get('CMAKE_PREFIX_PATH', '').replace('::', ':').strip(':')
 
         # Add warning for empty extend path
         if (self.devel_layout == 'linked' and
             (self.extend_path is None and
              not self.cached_cmake_prefix_path and
              not self.env_cmake_prefix_path)):
             self.warnings += [clr(
```

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/controllers.py` & `catkin_tools-0.9.3/catkin_tools/execution/controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,20 +312,20 @@
                     warneds[jid] = templates['warned']
                 else:
                     successfuls[jid] = templates['successful']
             else:
                 abandoneds[jid] = templates['abandoned']
 
         # Combine successfuls and ignoreds, sort by key
-        if len(successfuls) + len(ignoreds) > 0:
+        if len(successfuls) + len(warneds) + len(ignoreds) > 0:
             wide_log("")
             wide_log(clr("[{}] Successful {}:").format(self.label, self.jobs_label))
             wide_log("")
             print_items_in_columns(
-                sorted(itertools.chain(successfuls.items(), ignoreds.items())),
+                sorted(itertools.chain(successfuls.items(), warneds.items(), ignoreds.items())),
                 number_of_columns)
         else:
             wide_log("")
             wide_log(clr("[{}] No {} succeeded.").format(self.label, self.jobs_label))
             wide_log("")
 
         # Print out buildlisted jobs
@@ -338,28 +338,28 @@
         # Print out skiplisted jobs
         if len(skiplisted) > 0:
             wide_log("")
             wide_log(clr("[{}] Skiplisted {}:").format(self.label, self.jobs_label))
             wide_log("")
             print_items_in_columns(sorted(skiplisted.items()), number_of_columns)
 
-        # Print out jobs that failed
-        if len(faileds) > 0:
-            wide_log("")
-            wide_log(clr("[{}] Failed {}:").format(self.label, self.jobs_label))
-            wide_log("")
-            print_items_in_columns(sorted(faileds.items()), number_of_columns)
-
         # Print out jobs that were abandoned
         if len(abandoneds) > 0:
             wide_log("")
             wide_log(clr("[{}] Abandoned {}:").format(self.label, self.jobs_label))
             wide_log("")
             print_items_in_columns(sorted(abandoneds.items()), number_of_columns)
 
+        # Print out jobs that failed
+        if len(faileds) > 0:
+            wide_log("")
+            wide_log(clr("[{}] Failed {}:").format(self.label, self.jobs_label))
+            wide_log("")
+            print_items_in_columns(sorted(faileds.items()), number_of_columns)
+
         wide_log("")
 
     def print_compact_summary(self, completed_jobs, warned_jobs, failed_jobs):
         """Print a compact build summary."""
 
         notification_title = ""
         notification_msg = []
```

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/events.py` & `catkin_tools-0.9.3/catkin_tools/execution/events.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/executor.py` & `catkin_tools-0.9.3/catkin_tools/execution/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 # limitations under the License.
 
 import asyncio
 import traceback
 from concurrent.futures import FIRST_COMPLETED
 from concurrent.futures import ThreadPoolExecutor
 from itertools import tee
+from sys import version_info
 
 from osrf_pycommon.process_utils import async_execute_process
 from osrf_pycommon.process_utils import get_loop
 
 from catkin_tools.common import FakeLock
 from catkin_tools.execution import job_server
 
 from .events import ExecutionEvent
 from .io import IOBufferLogger
 from .stages import CommandStage
 from .stages import FunctionStage
 
+PY37 = version_info[:2] >= (3, 7)
+
 
 def split(values, cond):
     """Split an iterable based on a condition."""
     head, tail = tee((cond(v), v) for v in values)
     return [v for c, v in head if c], [v for c, v in tail if not c]
 
 
@@ -256,15 +259,18 @@
             # Notify that the job is being started
             event_queue.put(ExecutionEvent(
                 'STARTED_JOB',
                 job_id=job.jid))
 
             # Start the job coroutine
             active_jobs.append(job)
-            active_job_fs.add(async_job(verb, job, threadpool, locks, event_queue, log_path))
+            if PY37:
+                active_job_fs.add(asyncio.create_task(async_job(verb, job, threadpool, locks, event_queue, log_path)))
+            else:
+                active_job_fs.add(async_job(verb, job, threadpool, locks, event_queue, log_path))
 
         # Report running jobs
         event_queue.put(ExecutionEvent(
             'JOB_STATUS',
             pending=[j.jid for j in pending_jobs],
             queued=[j.jid for j in queued_jobs],
             active=[j.jid for j in active_jobs],
```

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/io.py` & `catkin_tools-0.9.3/catkin_tools/execution/io.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/job_server.py` & `catkin_tools-0.9.3/catkin_tools/execution/job_server.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/jobs.py` & `catkin_tools-0.9.3/catkin_tools/execution/jobs.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/execution/stages.py` & `catkin_tools-0.9.3/catkin_tools/execution/stages.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/jobs/catkin.py` & `catkin_tools-0.9.3/catkin_tools/jobs/catkin.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,17 +710,19 @@
 ]
 DEVEL_LINK_SKIPLIST = DEVEL_LINK_PREBUILD_SKIPLIST + [
     os.path.join('etc', 'catkin', 'profile.d', '05.catkin_make.bash'),
     os.path.join('etc', 'catkin', 'profile.d', '05.catkin_make_isolated.bash'),
     os.path.join('etc', 'catkin', 'profile.d', '05.catkin-test-results.sh'),
     'env.sh',
     'setup.bash',
+    'setup.fish',
     'setup.zsh',
     'setup.sh',
     'local_setup.bash',
+    'local_setup.fish',
     'local_setup.zsh',
     'local_setup.sh',
     '_setup_util.py',
 ]
 DEVEL_LINK_SKIP_DIRECTORIES = [
     '__pycache__',
 ]
```

### Comparing `catkin_tools-0.9.0/catkin_tools/jobs/cmake/python.cmake` & `catkin_tools-0.9.3/catkin_tools/jobs/cmake/python.cmake`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/jobs/cmake.py` & `catkin_tools-0.9.3/catkin_tools/jobs/cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             out, err = subprocess.Popen(
                 ['dpkg-architecture', '-qDEB_HOST_MULTIARCH'],
                 stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()
         except (OSError, FileNotFoundError):
             return ''
     # be sure to return empty string or a valid multiarch tuple
     decoded = out.decode().strip()
-    assert(not decoded or decoded.count('-') == 2)
+    assert (not decoded or decoded.count('-') == 2)
     return decoded
 
 
 def generate_env_file(logger, event_queue, context, install_target):
     env_file_path = os.path.join(install_target, 'env.sh')
     if os.path.exists(env_file_path):
         return 0
```

### Comparing `catkin_tools-0.9.0/catkin_tools/jobs/commands/cmake.py` & `catkin_tools-0.9.3/catkin_tools/jobs/commands/cmake.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/jobs/commands/make.py` & `catkin_tools-0.9.3/catkin_tools/jobs/commands/make.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/jobs/utils.py` & `catkin_tools-0.9.3/catkin_tools/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/metadata.py` & `catkin_tools-0.9.3/catkin_tools/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,15 @@
         if reset:
             print("Deleting existing metadata from catkin_tools metadata directory: %s" % metadata_root_path)
             shutil.rmtree(metadata_root_path)
             os.mkdir(metadata_root_path)
     else:
         # Create a new .catkin_tools directory
         os.mkdir(metadata_root_path)
+        os.mkdir(os.path.join(metadata_root_path, 'profiles'))
 
     # Write the README file describing the directory
     with open(os.path.join(metadata_root_path, 'README'), 'w') as metadata_readme:
         metadata_readme.write(METADATA_README_TEXT)
 
     # Migrate the metadata, if necessary
     migrate_metadata(workspace_path)
@@ -353,14 +354,20 @@
     profiles_data = get_profiles_data(workspace_path)
     if 'active' in profiles_data:
         return profiles_data['active']
 
     return DEFAULT_PROFILE_NAME
 
 
+def active_profile_set(workspace_path):
+    """Check if the active profile is set in profiles.yml"""
+    profiles_data = get_profiles_data(workspace_path)
+    return 'active' in profiles_data
+
+
 def get_profiles_data(workspace_path):
     """Get the contents of the profiles file.
 
     This file contains information such as the currently active profile.
 
     :param workspace_path: The exact path to the root of a catkin_tools workspace
     :type workspace_path: str
```

### Comparing `catkin_tools-0.9.0/catkin_tools/notifications/__init__.py` & `catkin_tools-0.9.3/catkin_tools/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/notifications/impl.py` & `catkin_tools-0.9.3/catkin_tools/notifications/impl.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/notifications/resources/linux/catkin_icon.png` & `catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/notifications/resources/linux/catkin_icon_red.png` & `catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_red.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/resultspace.py` & `catkin_tools-0.9.3/catkin_tools/resultspace.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/spaces/build.py` & `catkin_tools-0.9.3/catkin_tools/spaces/build.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/spaces/devel.py` & `catkin_tools-0.9.3/catkin_tools/spaces/devel.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/spaces/install.py` & `catkin_tools-0.9.3/catkin_tools/spaces/install.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/spaces/log.py` & `catkin_tools-0.9.3/catkin_tools/spaces/log.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/spaces/source.py` & `catkin_tools-0.9.3/catkin_tools/spaces/source.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/terminal_color.py` & `catkin_tools-0.9.3/catkin_tools/terminal_color.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/utils.py` & `catkin_tools-0.9.3/catkin_tools/utils.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/build.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,44 +349,43 @@
     # Assert start_with package is in the workspace
     verify_start_with_option(
         start_with,
         packages,
         all_packages,
         packages_to_be_built + packages_to_be_built_deps)
 
-    # Populate .catkin file if we're not installing
+    # Populate .catkin file containing source space paths
     # NOTE: This is done to avoid the Catkin CMake code from doing it,
     # which isn't parallel-safe. Catkin CMake only modifies this file if
     # it's package source path isn't found.
-    if not context.install:
-        dot_catkin_file_path = os.path.join(context.devel_space_abs, '.catkin')
-        # If the file exists, get the current paths
-        if os.path.exists(dot_catkin_file_path):
-            dot_catkin_paths = open(dot_catkin_file_path, 'r').read().split(';')
-        else:
-            dot_catkin_paths = []
-
-        # Update the list with the new packages (in topological order)
-        packages_to_be_built_paths = [
-            os.path.join(context.source_space_abs, path)
-            for path, pkg in packages_to_be_built
-        ]
-
-        new_dot_catkin_paths = [
-            os.path.join(context.source_space_abs, path)
-            for path in [os.path.join(context.source_space_abs, path) for path, pkg in all_packages]
-            if path in dot_catkin_paths or path in packages_to_be_built_paths
-        ]
-
-        # Write the new file if it's different, otherwise, leave it alone
-        if dot_catkin_paths == new_dot_catkin_paths:
-            wide_log("[build] Package table is up to date.")
-        else:
-            wide_log("[build] Updating package table.")
-            open(dot_catkin_file_path, 'w').write(';'.join(new_dot_catkin_paths))
+    dot_catkin_file_path = os.path.join(context.devel_space_abs, '.catkin')
+    # If the file exists, get the current paths
+    if os.path.exists(dot_catkin_file_path):
+        dot_catkin_paths = open(dot_catkin_file_path, 'r').read().split(';')
+    else:
+        dot_catkin_paths = []
+
+    # Update the list with the new packages (in topological order)
+    packages_to_be_built_paths = [
+        os.path.join(context.source_space_abs, path)
+        for path, pkg in packages_to_be_built
+    ]
+
+    new_dot_catkin_paths = [
+        os.path.join(context.source_space_abs, path)
+        for path in [os.path.join(context.source_space_abs, path) for path, pkg in all_packages]
+        if path in dot_catkin_paths or path in packages_to_be_built_paths
+    ]
+
+    # Write the new file if it's different, otherwise, leave it alone
+    if dot_catkin_paths == new_dot_catkin_paths:
+        wide_log("[build] Package table is up to date.")
+    else:
+        wide_log("[build] Updating package table.")
+        open(dot_catkin_file_path, 'w').write(';'.join(new_dot_catkin_paths))
 
     # Remove packages before start_with
     if start_with is not None:
         for path, pkg in list(packages_to_be_built):
             if pkg.name != start_with:
                 wide_log(clr("@!@{pf}Skipping@|  @{gf}---@| @{cf}{}@|").format(pkg.name))
                 packages_to_be_built.pop(0)
@@ -496,17 +495,16 @@
         # Get actual build deps
         deps = [
             p.name for _, p
             in get_cached_recursive_build_depends_in_workspace(pkg, packages_to_be_built)
             if p.name not in prebuild_jobs
         ]
         # All jobs depend on the prebuild jobs if they're defined
-        if not no_deps:
-            for j in prebuild_jobs.values():
-                deps.append(j.jid)
+        for j in prebuild_jobs.values():
+            deps.append(j.jid)
 
         # Determine the job parameters
         build_job_kwargs = dict(
             context=context,
             package=pkg,
             package_path=pkg_path,
             dependencies=deps,
```

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from catkin_tools.common import is_tty
 from catkin_tools.common import log
 from catkin_tools.context import Context
 from catkin_tools.jobs.utils import CommandMissing
 from catkin_tools.jobs.utils import loadenv
 from catkin_tools.metadata import find_enclosing_workspace
 from catkin_tools.metadata import get_metadata
+from catkin_tools.metadata import init_metadata_root
 from catkin_tools.metadata import update_metadata
 from catkin_tools.resultspace import load_resultspace_environment
 from catkin_tools.terminal_color import set_color
 
 from .build import build_isolated_workspace
 from .build import determine_packages_to_be_built
 from .build import verify_start_with_option
@@ -248,22 +249,23 @@
                 sys.exit(clr("[build] @!@{rf}Error:@| In order to use --this, "
                              "the current directory must be part of a catkin package."))
 
     if opts.no_deps and not opts.packages and not opts.unbuilt:
         sys.exit(clr("[build] @!@{rf}Error:@| With --no-deps, you must specify packages to build."))
 
     # Load the context
-    if opts.build_this or opts.start_with_this:
-        ctx = Context.load(opts.workspace, opts.profile, opts, append=True, strict=True)
-    else:
-        ctx = Context.load(opts.workspace, opts.profile, opts, append=True)
+    ctx = Context.load(opts.workspace, opts.profile, opts, append=True, strict=True)
 
     # Handle no workspace
-    if ctx is None:
+    if ctx is None and (opts.build_this or opts.start_with_this):
         sys.exit(clr("[build] @!@{rf}Error:@| The current folder is not part of a catkin workspace."))
+    elif ctx is None:
+        init_metadata_root(opts.workspace or os.getcwd())
+        ctx = Context.load(opts.workspace, opts.profile, opts, append=True)
+        log(clr('@!@{cf}Initialized new catkin workspace in `{}`@|').format(ctx.workspace))
 
     # Initialize the build configuration
     make_args, makeflags, cli_flags, jobserver = configure_make_args(
         ctx.make_args, ctx.jobs_args, ctx.use_internal_make_jobserver)
 
     # Set the jobserver memory limit
     if jobserver and opts.mem_limit:
```

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_build/color.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/color.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/clean.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/clean.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_clean/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_config/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_config/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import argparse
 import os
 import sys
 
 from catkin_tools.argument_parsing import add_cmake_and_make_and_catkin_make_args
 from catkin_tools.argument_parsing import add_context_args
 from catkin_tools.context import Context
+from catkin_tools.metadata import init_metadata_root
 from catkin_tools.terminal_color import ColorMapper
 from catkin_tools.terminal_color import fmt
 
 color_mapper = ColorMapper()
 clr = color_mapper.clr
 
 
@@ -175,29 +176,43 @@
         # Try to find a metadata directory to get context defaults
         # Otherwise use the specified directory
         context = Context.load(
             opts.workspace,
             opts.profile,
             opts,
             append=opts.append_args,
-            remove=opts.remove_args)
+            remove=opts.remove_args,
+            strict=True)
 
         do_init = opts.init or not no_action
         summary_notes = []
 
-        if not context.initialized() and do_init:
-            summary_notes.append(clr('@!@{cf}Initialized new catkin workspace in `{}`@|').format(context.workspace))
+        if not context and not do_init:
+            # Don't initialize a new workspace
+            print(clr('@!@{rf}WARNING:@| Workspace is not yet initialized. '
+                      'Use catkin init or run catkin config with --init.'))
+
+        else:
+            # Either initialize it or it already exists
+            if not context:
+                init_metadata_root(opts.workspace or os.getcwd())
+                context = Context.load(
+                    opts.workspace,
+                    opts.profile,
+                    opts,
+                    append=opts.append_args,
+                    remove=opts.remove_args)
+                summary_notes.append(clr('@!@{cf}Initialized new catkin workspace in `{}`@|').format(context.workspace))
 
-        if context.initialized() or do_init:
             Context.save(context)
 
-        if opts.mkdirs and not context.source_space_exists():
-            os.makedirs(context.source_space_abs)
+            if opts.mkdirs and not context.source_space_exists():
+                os.makedirs(context.source_space_abs)
 
-        print(context.summary(notes=summary_notes))
+            print(context.summary(notes=summary_notes))
 
     except IOError as exc:
         # Usually happens if workspace is already underneath another catkin_tools workspace
         print(clr("@!@{rf}Error:@| Could not configure catkin workspace: {}").format(exc), file=sys.stderr)
         return 1
 
     return 0
```

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_create/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_create/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_env/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_env/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_init/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_init/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_list/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_list/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_locate/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_locate/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_profile/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_profile/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_shell_verbs.bash` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_shell_verbs.bash`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/__init__.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/cli.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools/verbs/catkin_test/test.py` & `catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/test.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/catkin_tools.egg-info/PKG-INFO` & `catkin_tools-0.9.3/catkin_tools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: catkin-tools
-Version: 0.9.0
+Version: 0.9.3
 Summary: Command line tools for working with catkin.
 Home-page: https://catkin-tools.readthedocs.org/
 Author: William Woodall
 Author-email: william@osrfoundation.org
 Maintainer: William Woodall
 Maintainer-email: william@osrfoundation.org
 License: Apache 2.0
 Keywords: catkin
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 License-File: LICENSE
 
 Provides command line tools for working with catkin.
-
```

### Comparing `catkin_tools-0.9.0/catkin_tools.egg-info/entry_points.txt` & `catkin_tools-0.9.3/catkin_tools.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 devel = catkin_tools.spaces.devel:description
 install = catkin_tools.spaces.install:description
 log = catkin_tools.spaces.log:description
 source = catkin_tools.spaces.source:description
 
 [console_scripts]
 catkin = catkin_tools.commands.catkin:main
-
```

### Comparing `catkin_tools-0.9.0/completion/_catkin` & `catkin_tools-0.9.3/completion/_catkin`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.0/completion/catkin.bash` & `catkin_tools-0.9.3/completion/catkin.bash`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,20 @@
       if [[ ${prev} == --extend || ${prev} == --*-space ]] ; then
         # add directory completion
         compopt -o nospace 2>/dev/null
         COMPREPLY+=($(compgen -d -S "/" -- ${cur}))
       fi
       ;;
     clean)
-      local catkin_clean_opts=$(catkin clean --help 2>&1 | sed -ne $OPTS_FILTER | sort -u)
-      COMPREPLY=($(compgen -W "${catkin_clean_opts}" -- ${cur}))
+      if [[ ${cur} == -* ]]; then
+        local catkin_clean_opts=$(catkin clean --help 2>&1 | sed -ne $OPTS_FILTER | sort -u)
+        COMPREPLY=($(compgen -W "${catkin_clean_opts}" -- ${cur}))
+      else
+        COMPREPLY=($(compgen -W "$(_catkin_pkgs)" -- ${cur}))
+      fi
       ;;
     create)
       if [[ "${words[@]}" == *" pkg"* ]] ; then
         local catkin_create_pkg_opts=$(catkin create pkg --help 2>&1 | sed -ne $OPTS_FILTER | sort -u)
         COMPREPLY=($(compgen -W "${catkin_create_pkg_opts}" -- ${cur}))
       else
         COMPREPLY=($(compgen -W "pkg" -- ${cur}))
```

### Comparing `catkin_tools-0.9.0/setup.py` & `catkin_tools-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 mode = ((os.stat(file)[ST_MODE]) | 0o444) & 0o7777
                 log.info("changing permissions of %s to %o" % (file, mode))
                 os.chmod(file, mode)
 
 
 setup(
     name='catkin_tools',
-    version='0.9.0',
+    version='0.9.3',
     python_requires='>=3.5',
     packages=find_packages(exclude=['tests*', 'docs']),
     package_data={
         'catkin_tools': [
             'jobs/cmake/python.cmake',
             'jobs/cmake/python_install_dir.cmake',
             'verbs/catkin_shell_verbs.bash',
```

