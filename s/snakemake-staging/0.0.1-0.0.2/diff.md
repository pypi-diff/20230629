# Comparing `tmp/snakemake_staging-0.0.1.tar.gz` & `tmp/snakemake_staging-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_staging-0.0.1.tar", max compression
+gzip compressed data, was "snakemake_staging-0.0.2.tar", max compression
```

## Comparing `snakemake_staging-0.0.1.tar` & `snakemake_staging-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-08 23:15:19.144878 snakemake_staging-0.0.1/LICENSE
--rw-r--r--   0        0        0     4255 2023-05-08 23:15:19.144878 snakemake_staging-0.0.1/README.md
--rw-r--r--   0        0        0     1015 2023-05-08 23:15:37.064664 snakemake_staging-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      925 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/__init__.py
--rw-r--r--   0        0        0      238 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/config.py
--rw-r--r--   0        0        0        0 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/git.py
--rw-r--r--   0        0        0      151 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/rules.py
--rw-r--r--   0        0        0     2148 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/stages.py
--rw-r--r--   0        0        0     1223 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/utils.py
--rw-r--r--   0        0        0       22 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/version.py
--rw-r--r--   0        0        0      106 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/workflow/Snakefile
--rw-r--r--   0        0        0       48 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/workflow/envs/git.yml
--rw-r--r--   0        0        0      409 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/workflow/rules/git.smk
--rw-r--r--   0        0        0     2256 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/workflow/rules/noop.smk
--rw-r--r--   0        0        0      357 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/workflow/rules/stages.smk
--rw-r--r--   0        0        0     1988 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/workflow/rules/zenodo.smk
--rw-r--r--   0        0        0     9148 2023-05-08 23:15:19.148878 snakemake_staging-0.0.1/src/snakemake_staging/zenodo.py
--rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 snakemake_staging-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4238 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/README.md
+-rw-r--r--   0        0        0      962 2023-06-29 11:52:05.243748 snakemake_staging-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      925 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/__init__.py
+-rw-r--r--   0        0        0      238 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/config.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/git.py
+-rw-r--r--   0        0        0      151 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/rules.py
+-rw-r--r--   0        0        0     2110 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/stages.py
+-rw-r--r--   0        0        0     6994 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/testing.py
+-rw-r--r--   0        0        0     1223 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/utils.py
+-rw-r--r--   0        0        0       22 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/version.py
+-rw-r--r--   0        0        0      106 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/workflow/Snakefile
+-rw-r--r--   0        0        0       48 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/workflow/envs/git.yml
+-rw-r--r--   0        0        0      409 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/workflow/rules/git.smk
+-rw-r--r--   0        0        0     2256 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/workflow/rules/noop.smk
+-rw-r--r--   0        0        0      786 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/workflow/rules/stages.smk
+-rw-r--r--   0        0        0     1988 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/workflow/rules/zenodo.smk
+-rw-r--r--   0        0        0     9148 2023-06-29 11:51:50.422949 snakemake_staging-0.0.2/src/snakemake_staging/zenodo.py
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 snakemake_staging-0.0.2/PKG-INFO
```

### Comparing `snakemake_staging-0.0.1/LICENSE` & `snakemake_staging-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_staging-0.0.1/README.md` & `snakemake_staging-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 ```python
 include: staging.snakefile()
 ```
 
 At this point, here's the full `Snakefile`:
 
 <details>
-<summary>Full Snakefile example</summary>
+<summary>Full Snakefile</summary>
 
 ```python
 import snakemake_staging as staging
 
 stage = staging.ZenodoStage(
     "zenodo-stage",
     config.get("restore", False)
@@ -116,16 +116,16 @@
 workflow in 3 ways:
 
 1. **Normal execution**: If you run something like
    `snakemake path/to/output1.txt` (where I have omitted the usual `--cores`
    and `--conda` arguments) will execute the workflow as normal, without
    staging out any files.
 
-2. **Stage upload**: If you instead have Snakemake target the
-   `zenodo-stage.zenodo.json` file (this filename can be changed by passing the
-   `info_file` argument to the `ZenodoStage` constructor), the `expensive` rule
-   will be executed, and the outputs will be uploaded to Zenodo, saving the
-   record information to `zenodo-stage.zenodo.json`.
+2. **Stage upload**: If you instead have Snakemake target the `staging__upload`
+   rule, the `expensive` rule will be executed, and the outputs will be uploaded
+   to Zenodo, saving the record information to `zenodo-stage.zenodo.json` (this
+   filename can be changed by passing the `info_file` argument to the
+   `ZenodoStage` constructor).
 
 3. **Stage restore**: Finally, after these outputs have been uploaded to Zenodo,
    you can call Snakemake `--config restore=True` to disable the `expensive`
    rule, and force the outputs to be restored from Zenodo.
```

### Comparing `snakemake_staging-0.0.1/pyproject.toml` & `snakemake_staging-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "snakemake-staging"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Dan Foreman-Mackey <foreman.mackey@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "snakemake_staging", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 snakemake = "*"  # TODO(dfm): Figure out a minimum version
 requests = "*"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-responses = "^0.23.1"
-flask = "^2.3.2"
+pytest = "*"
+flask = "*"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
@@ -30,15 +29,14 @@
 
 [tool.black]
 target-version = ["py38", "py39"]
 line-length = 88
 
 [tool.ruff]
 line-length = 89
-update-check = false
 target-version = "py38"
 select = ["F", "I", "E", "W", "YTT", "B", "Q", "PLE", "PLW"]
 ignore = []
 exclude = []
 
 [tool.ruff.isort]
 force-wrap-aliases = true
```

### Comparing `snakemake_staging-0.0.1/src/snakemake_staging/__init__.py` & `snakemake_staging-0.0.2/src/snakemake_staging/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_staging-0.0.1/src/snakemake_staging/stages.py` & `snakemake_staging-0.0.2/src/snakemake_staging/stages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from pathlib import Path
 from typing import List, Optional
 
-from snakemake.io import OutputFiles
-
 from snakemake_staging.config import _CONFIG
 from snakemake_staging.utils import PathLike, package_data, path_to_identifier
 
 STAGES: OrderedDict[str, "Stage"] = OrderedDict()
 
 
 class Stage(ABC):
```

### Comparing `snakemake_staging-0.0.1/src/snakemake_staging/utils.py` & `snakemake_staging-0.0.2/src/snakemake_staging/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake_staging-0.0.1/src/snakemake_staging/workflow/rules/noop.smk` & `snakemake_staging-0.0.2/src/snakemake_staging/workflow/rules/noop.smk`

 * *Files identical despite different names*

### Comparing `snakemake_staging-0.0.1/src/snakemake_staging/workflow/rules/zenodo.smk` & `snakemake_staging-0.0.2/src/snakemake_staging/workflow/rules/zenodo.smk`

 * *Files identical despite different names*

### Comparing `snakemake_staging-0.0.1/src/snakemake_staging/zenodo.py` & `snakemake_staging-0.0.2/src/snakemake_staging/zenodo.py`

 * *Files identical despite different names*

### Comparing `snakemake_staging-0.0.1/PKG-INFO` & `snakemake_staging-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-staging
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Dan Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -95,15 +95,15 @@
 ```python
 include: staging.snakefile()
 ```
 
 At this point, here's the full `Snakefile`:
 
 <details>
-<summary>Full Snakefile example</summary>
+<summary>Full Snakefile</summary>
 
 ```python
 import snakemake_staging as staging
 
 stage = staging.ZenodoStage(
     "zenodo-stage",
     config.get("restore", False)
@@ -131,17 +131,17 @@
 workflow in 3 ways:
 
 1. **Normal execution**: If you run something like
    `snakemake path/to/output1.txt` (where I have omitted the usual `--cores`
    and `--conda` arguments) will execute the workflow as normal, without
    staging out any files.
 
-2. **Stage upload**: If you instead have Snakemake target the
-   `zenodo-stage.zenodo.json` file (this filename can be changed by passing the
-   `info_file` argument to the `ZenodoStage` constructor), the `expensive` rule
-   will be executed, and the outputs will be uploaded to Zenodo, saving the
-   record information to `zenodo-stage.zenodo.json`.
+2. **Stage upload**: If you instead have Snakemake target the `staging__upload`
+   rule, the `expensive` rule will be executed, and the outputs will be uploaded
+   to Zenodo, saving the record information to `zenodo-stage.zenodo.json` (this
+   filename can be changed by passing the `info_file` argument to the
+   `ZenodoStage` constructor).
 
 3. **Stage restore**: Finally, after these outputs have been uploaded to Zenodo,
    you can call Snakemake `--config restore=True` to disable the `expensive`
    rule, and force the outputs to be restored from Zenodo.
```

