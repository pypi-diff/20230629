# Comparing `tmp/pipestat-0.3.1.tar.gz` & `tmp/pipestat-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestat-0.3.1.tar", last modified: Thu Aug 18 21:17:41 2022, max compression
+gzip compressed data, was "pipestat-0.4.0.tar", last modified: Thu Jun 29 19:25:12 2023, max compression
```

## Comparing `pipestat-0.3.1.tar` & `pipestat-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:41.703277 pipestat-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-08-18 21:17:34.000000 pipestat-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-18 21:17:34.000000 pipestat-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-08-18 21:17:41.703277 pipestat-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-08-18 21:17:34.000000 pipestat-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:41.703277 pipestat-0.3.1/pipestat/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7032 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/argparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6134 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    58196 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:41.703277 pipestat-0.3.1/pipestat/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/schemas/pipestat_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/schemas/status_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-18 21:17:34.000000 pipestat-0.3.1/pipestat/schemas/status_table_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:41.703277 pipestat-0.3.1/pipestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-08-18 21:17:41.000000 pipestat-0.3.1/pipestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-08-18 21:17:41.000000 pipestat-0.3.1/pipestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 21:17:41.000000 pipestat-0.3.1/pipestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-18 21:17:41.000000 pipestat-0.3.1/pipestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-18 21:17:41.000000 pipestat-0.3.1/pipestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-18 21:17:41.000000 pipestat-0.3.1/pipestat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:41.703277 pipestat-0.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-18 21:17:34.000000 pipestat-0.3.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-18 21:17:34.000000 pipestat-0.3.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-18 21:17:34.000000 pipestat-0.3.1/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-18 21:17:34.000000 pipestat-0.3.1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 21:17:41.703277 pipestat-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-08-18 21:17:34.000000 pipestat-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-29 19:25:01.000000 pipestat-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 19:25:01.000000 pipestat-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-29 19:25:12.569878 pipestat-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-29 19:25:01.000000 pipestat-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/backends/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/backends/dbbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/backends/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21733 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/schemas/pipestat_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/schemas/status_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/schemas/status_table_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 19:25:01.000000 pipestat-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:25:12.569878 pipestat-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-29 19:25:01.000000 pipestat-0.4.0/setup.py
```

### Comparing `pipestat-0.3.1/LICENSE` & `pipestat-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestat-0.3.1/PKG-INFO` & `pipestat-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.3.1
+Version: 0.4.0
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Run pytests](https://github.com/pepkit/pipestat/workflows/Run%20pytests/badge.svg)
+[![docs-badge](https://readthedocs.org/projects/pipestat/badge/?version=latest)](https://pipestat.databio.org/en/latest/)
+[![pypi-badge](https://img.shields.io/pypi/v/pipestat)](https://pypi.org/project/pipestat)
 [![codecov](https://codecov.io/gh/pepkit/pipestat/branch/master/graph/badge.svg?token=O07MXSQZ32)](https://codecov.io/gh/pepkit/pipestat)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+
 <img src="https://raw.githubusercontent.com/pepkit/pipestat/master/docs/img/pipestat_logo.svg?sanitize=true" alt="pipestat" height="70"/><br>
 
 Pipestat standardizes reporting of pipeline results. It provides 1) a standard specification for how pipeline outputs should be stored; and 2) an implementation to easily write results to that format from within Python or from the command line. A pipeline author defines all the outputs produced by a pipeline by writing a JSON-schema. The pipeline then uses pipestat to report pipeline outputs as the pipeline runs, either via the Python API or command line interface. The user configures results to be stored either in a [YAML-formatted file](https://yaml.org/spec/1.2/spec.html) or a [PostgreSQL database](https://www.postgresql.org/).
 
 See [Pipestat documentation](https://pipestat.databio.org) for complete details.
```

### Comparing `pipestat-0.3.1/README.md` & `pipestat-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 ![Run pytests](https://github.com/pepkit/pipestat/workflows/Run%20pytests/badge.svg)
+[![docs-badge](https://readthedocs.org/projects/pipestat/badge/?version=latest)](https://pipestat.databio.org/en/latest/)
+[![pypi-badge](https://img.shields.io/pypi/v/pipestat)](https://pypi.org/project/pipestat)
 [![codecov](https://codecov.io/gh/pepkit/pipestat/branch/master/graph/badge.svg?token=O07MXSQZ32)](https://codecov.io/gh/pepkit/pipestat)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+
 <img src="https://raw.githubusercontent.com/pepkit/pipestat/master/docs/img/pipestat_logo.svg?sanitize=true" alt="pipestat" height="70"/><br>
 
 Pipestat standardizes reporting of pipeline results. It provides 1) a standard specification for how pipeline outputs should be stored; and 2) an implementation to easily write results to that format from within Python or from the command line. A pipeline author defines all the outputs produced by a pipeline by writing a JSON-schema. The pipeline then uses pipestat to report pipeline outputs as the pipeline runs, either via the Python API or command line interface. The user configures results to be stored either in a [YAML-formatted file](https://yaml.org/spec/1.2/spec.html) or a [PostgreSQL database](https://www.postgresql.org/).
 
 See [Pipestat documentation](https://pipestat.databio.org) for complete details.
```

### Comparing `pipestat-0.3.1/pipestat/argparser.py` & `pipestat-0.4.0/pipestat/argparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,52 @@
-import argparse
+"""Construction of the CLI definition and parsing framework for the pipestat application"""
 
+import argparse
+import os
 from ubiquerg import VersionInHelpParser
-
 from ._version import __version__
+
 from .const import *
 
+REPORT_CMD = "report"
+INSPECT_CMD = "inspect"
+REMOVE_CMD = "remove"
+RETRIEVE_CMD = "retrieve"
+STATUS_CMD = "status"
+INIT_CMD = "init"
+SUBPARSER_MESSAGES = {
+    REPORT_CMD: "Report a result.",
+    INSPECT_CMD: "Inspect a database.",
+    REMOVE_CMD: "Remove a result.",
+    RETRIEVE_CMD: "Retrieve a result.",
+    STATUS_CMD: "Manage pipeline status.",
+    INIT_CMD: "Initialize generic config file",
+}
+
+STATUS_GET_CMD = "get"
+STATUS_SET_CMD = "set"
+STATUS_SUBPARSER_MESSAGES = {
+    STATUS_SET_CMD: "Set status.",
+    STATUS_GET_CMD: "Get status.",
+}
+
+__all__ = (
+    ["build_argparser", "SUBPARSER_MESSAGES", "STATUS_SUBPARSER_MESSAGES"]
+    + list(SUBPARSER_MESSAGES.keys())
+    + list(STATUS_SUBPARSER_MESSAGES.keys())
+)
+
 
 def _env_txt(arg_name):
     """
     Check if env var set and produce text
     """
     arg_val = os.environ.get(ENV_VARS[arg_name])
     txt = f"If not provided '{ENV_VARS[arg_name]}' env var will be used. "
-    return txt + (
-        "Currently not set" if arg_val is None else f"Currently set to: {arg_val}"
-    )
+    return txt + ("Currently not set" if arg_val is None else f"Currently set to: {arg_val}")
 
 
 def build_argparser(desc):
     """
     Builds argument parser.
     :param str desc: additional description to print in help
     :return argparse.ArgumentParser
@@ -27,51 +55,53 @@
     additional_description = desc
     parser = VersionInHelpParser(
         version=__version__, description=banner, epilog=additional_description
     )
 
     subparsers = parser.add_subparsers(dest="command")
 
-    def add_subparser(cmd, msg, subparsers):
+    def add_subparser(
+        cmd: str, msg: str, subparsers: argparse._SubParsersAction
+    ) -> argparse.ArgumentParser:
         return subparsers.add_parser(
             cmd,
             description=msg,
             help=msg,
             formatter_class=lambda prog: argparse.HelpFormatter(
                 prog, max_help_position=40, width=90
             ),
         )
 
     sps = {}
     # common arguments
-    for cmd in SUBPARSER_MSGS.keys():
-        sps[cmd] = add_subparser(cmd, SUBPARSER_MSGS[cmd], subparsers)
+    for cmd in SUBPARSER_MESSAGES.keys():
+        p = add_subparser(cmd, SUBPARSER_MESSAGES[cmd], subparsers)
         # status is nested and status subcommands require config path
-        if cmd == STATUS_CMD:
-            continue
-        sps[cmd].add_argument(
-            "-n",
-            "--namespace",
-            type=str,
-            metavar="N",
-            help=f"Name of the pipeline to report result for. {_env_txt('namespace')}",
-        )
+        if cmd != STATUS_CMD:
+            p.add_argument(
+                "-n",
+                "--project-name",
+                type=str,
+                metavar="N",
+                help=f"Name of the pipeline to report result for. {_env_txt('project_name')}",
+            )
+        sps[cmd] = p
 
     status_subparser = sps[STATUS_CMD]
     status_subparsers = status_subparser.add_subparsers(dest="subcommand")
 
     status_sps = {}
     for cmd, desc in STATUS_SUBPARSER_MESSAGES.items():
         status_sps[cmd] = add_subparser(cmd, desc, status_subparsers)
         status_sps[cmd].add_argument(
             "-n",
-            "--namespace",
+            "--project-name",
             type=str,
             metavar="N",
-            help=f"Name of the pipeline to report result for. {_env_txt('namespace')}",
+            help=f"Name of the pipeline to report result for. {_env_txt('project_name')}",
         )
         if cmd == STATUS_SET_CMD:
             status_sps[cmd].add_argument(
                 "status_identifier",
                 help="Status identifier to set.",
             )
         status_sps[cmd].add_argument(
@@ -111,23 +141,22 @@
             help=f"Path to the status schema. "
             f"Default will be used if not provided: {STATUS_SCHEMA}",
         )
         status_sps[cmd].add_argument(
             "--flag-dir",
             type=str,
             metavar="FD",
-            help=f"Path to the flag directory in case YAML file is "
-            f"the pipestat backend.",
+            help=f"Path to the flag directory in case YAML file is " f"the pipestat backend.",
         )
         status_sps[cmd].add_argument(
             "-r",
-            "--record-identifier",
+            "--sample-name",
             type=str,
             metavar="R",
-            help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
+            help=f"ID of the record to report the result for. {_env_txt('sample_name')}",
         )
 
     # remove, report and inspect
     for cmd in [REMOVE_CMD, REPORT_CMD, INSPECT_CMD, RETRIEVE_CMD]:
         sps[cmd].add_argument(
             "-f",
             "--results-file",
@@ -165,34 +194,33 @@
             help=f"Path to the status schema. "
             f"Default will be used if not provided: {STATUS_SCHEMA}",
         )
         sps[cmd].add_argument(
             "--flag-dir",
             type=str,
             metavar="FD",
-            help=f"Path to the flag directory in case YAML file is "
-            f"the pipestat backend.",
+            help=f"Path to the flag directory in case YAML file is " f"the pipestat backend.",
         )
 
     # remove and report
     for cmd in [REMOVE_CMD, REPORT_CMD, RETRIEVE_CMD]:
         sps[cmd].add_argument(
             "-i",
             "--result-identifier",
             required=True,
             type=str,
             metavar="I",
             help="ID of the result to report; needs to be defined in the schema",
         )
         sps[cmd].add_argument(
             "-r",
-            "--record-identifier",
+            "--sample-name",
             type=str,
             metavar="R",
-            help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
+            help=f"ID of the record to report the result for. {_env_txt('sample_name')}",
         )
 
     # report
     sps[REPORT_CMD].add_argument(
         "-v",
         "--value",
         required=True,
@@ -200,25 +228,31 @@
         help="Value of the result to report",
     )
 
     sps[REPORT_CMD].add_argument(
         "-o",
         "--overwrite",
         action="store_true",
-        help="Whether the result should override existing ones in "
-        "case of name clashes",
+        help="Whether the result should override existing ones in " "case of name clashes",
     )
 
     sps[REPORT_CMD].add_argument(
         "-t",
         "--skip-convert",
         action="store_true",
-        help="Whether skip result type conversion into the reqiuired "
+        help="Whether skip result type conversion into the required "
         "class in case it does not meet the schema requirements",
     )
 
+    sps[INIT_CMD].add_argument(
+        "-g",
+        "--generic-config",
+        action="store_true",
+        help="Creates a generic config file",
+    )
+
     # inspect
     sps[INSPECT_CMD].add_argument(
         "-d", "--data", action="store_true", help="Whether to display the data"
     )
 
     return parser
```

### Comparing `pipestat-0.3.1/pipestat/schemas/pipestat_config_schema.yaml` & `pipestat-0.4.0/pipestat/schemas/pipestat_config_schema.yaml`

 * *Files identical despite different names*

### Comparing `pipestat-0.3.1/pipestat.egg-info/PKG-INFO` & `pipestat-0.4.0/pipestat.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.3.1
+Version: 0.4.0
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Run pytests](https://github.com/pepkit/pipestat/workflows/Run%20pytests/badge.svg)
+[![docs-badge](https://readthedocs.org/projects/pipestat/badge/?version=latest)](https://pipestat.databio.org/en/latest/)
+[![pypi-badge](https://img.shields.io/pypi/v/pipestat)](https://pypi.org/project/pipestat)
 [![codecov](https://codecov.io/gh/pepkit/pipestat/branch/master/graph/badge.svg?token=O07MXSQZ32)](https://codecov.io/gh/pepkit/pipestat)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+
 <img src="https://raw.githubusercontent.com/pepkit/pipestat/master/docs/img/pipestat_logo.svg?sanitize=true" alt="pipestat" height="70"/><br>
 
 Pipestat standardizes reporting of pipeline results. It provides 1) a standard specification for how pipeline outputs should be stored; and 2) an implementation to easily write results to that format from within Python or from the command line. A pipeline author defines all the outputs produced by a pipeline by writing a JSON-schema. The pipeline then uses pipestat to report pipeline outputs as the pipeline runs, either via the Python API or command line interface. The user configures results to be stored either in a [YAML-formatted file](https://yaml.org/spec/1.2/spec.html) or a [PostgreSQL database](https://www.postgresql.org/).
 
 See [Pipestat documentation](https://pipestat.databio.org) for complete details.
```

### Comparing `pipestat-0.3.1/setup.py` & `pipestat-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 extra["install_requires"] = DEPENDENCIES
 
 
 # Additional files to include with package
 def get_static(name, condition=None):
     static = [
         os.path.join(name, f)
-        for f in os.listdir(
-            os.path.join(os.path.dirname(os.path.realpath(__file__)), name)
-        )
+        for f in os.listdir(os.path.join(os.path.dirname(os.path.realpath(__file__)), name))
     ]
     if condition is None:
         return static
     else:
         return [i for i in filter(lambda x: eval(condition), static)]
 
 
@@ -58,29 +56,27 @@
     version=version,
     description="A pipeline results reporter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="project, metadata, bioinformatics, sequencing, ngs, workflow",
     url="https://github.com/pepkit/" + PACKAGE,
     author="Michal Stolarczyk, Nathan Sheffield",
     license="BSD2",
     entry_points={
         "console_scripts": ["pipestat = pipestat.__main__:main"],
     },
     scripts=scripts,
     include_package_data=True,
     test_suite="tests",
     tests_require=(["mock", "pytest"]),
-    setup_requires=(
-        ["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []
-    ),
-    **extra
+    setup_requires=(["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []),
+    **extra,
 )
```

