# Comparing `tmp/rope-1.8.0.tar.gz` & `tmp/rope-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rope-1.8.0.tar", last modified: Fri May  5 05:06:22 2023, max compression
+gzip compressed data, was "rope-1.9.0.tar", last modified: Thu Jun 29 12:27:10 2023, max compression
```

## Comparing `rope-1.8.0.tar` & `rope-1.9.0.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.501347 rope-1.8.0/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14368 2023-01-17 01:59:16.000000 rope-1.8.0/.all-contributorsrc
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      125 2022-07-29 12:45:37.000000 rope-1.8.0/.git-blame-ignore-revs
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.417344 rope-1.8.0/.github/
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.421344 rope-1.8.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      916 2022-07-29 12:45:37.000000 rope-1.8.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      595 2022-07-29 12:45:37.000000 rope-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      411 2023-01-17 01:59:16.000000 rope-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.421344 rope-1.8.0/.github/workflows/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      160 2022-07-29 12:45:37.000000 rope-1.8.0/.github/workflows/black.yml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      742 2023-05-05 04:53:06.000000 rope-1.8.0/.github/workflows/main.yml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      274 2023-01-17 01:59:16.000000 rope-1.8.0/.github/workflows/task-completed-checker-action.yml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1864 2022-07-29 12:46:52.000000 rope-1.8.0/.gitignore
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      120 2022-07-29 12:45:37.000000 rope-1.8.0/.readthedocs.yaml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9838 2023-05-05 04:58:59.000000 rope-1.8.0/CHANGELOG.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21134 2023-01-17 01:59:16.000000 rope-1.8.0/CONTRIBUTORS.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7652 2022-07-29 12:45:37.000000 rope-1.8.0/COPYING
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      150 2022-07-29 12:45:37.000000 rope-1.8.0/MANIFEST.in
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5673 2023-05-05 05:06:22.501347 rope-1.8.0/PKG-INFO
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4478 2023-05-05 04:53:06.000000 rope-1.8.0/README.rst
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.421344 rope-1.8.0/bin/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1607 2023-01-17 01:59:16.000000 rope-1.8.0/bin/tag-release.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.425345 rope-1.8.0/docs/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      634 2022-07-29 12:45:37.000000 rope-1.8.0/docs/Makefile
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2247 2022-09-19 07:11:34.000000 rope-1.8.0/docs/conf.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1719 2023-01-17 01:59:16.000000 rope-1.8.0/docs/configuration.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4518 2023-05-05 04:53:06.000000 rope-1.8.0/docs/contributing.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5165 2022-12-16 04:43:54.000000 rope-1.8.0/docs/default_config.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.425345 rope-1.8.0/docs/dev/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3906 2023-01-17 01:59:16.000000 rope-1.8.0/docs/dev/issues.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      526 2023-01-17 01:59:16.000000 rope-1.8.0/docs/index.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    28522 2023-01-17 01:59:16.000000 rope-1.8.0/docs/library.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      765 2022-07-29 12:45:37.000000 rope-1.8.0/docs/make.bat
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31016 2023-01-17 01:59:16.000000 rope-1.8.0/docs/overview.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      976 2023-05-05 05:01:06.000000 rope-1.8.0/docs/release-process.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1459 2022-09-19 07:41:21.000000 rope-1.8.0/docs/rope.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2256 2023-05-05 05:05:09.000000 rope-1.8.0/pyproject.toml
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.429345 rope-1.8.0/rope/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1431 2023-01-17 01:59:16.000000 rope-1.8.0/rope/__init__.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.441345 rope-1.8.0/rope/base/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      161 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3283 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/arguments.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2521 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/ast.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26263 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/builtins.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13675 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/change.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11774 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/codeanalyze.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13587 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/evaluate.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1370 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/exceptions.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8481 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/fscommands.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8342 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/history.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3841 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/libutils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1656 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/nameanalyze.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.445345 rope-1.8.0/rope/base/oi/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1682 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7397 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/doa.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3440 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/memorydb.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4547 2022-12-16 03:37:02.000000 rope-1.8.0/rope/base/oi/objectdb.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8624 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/objectinfo.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8532 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/runmod.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5862 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/soa.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7719 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/soi.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9829 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/oi/transform.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.449345 rope-1.8.0/rope/base/oi/type_hinting/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9057 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/evaluate.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2728 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/type_hinting/factory.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      715 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/interfaces.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.453345 rope-1.8.0/rope/base/oi/type_hinting/providers/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1856 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/composite.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6164 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/docstrings.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2116 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/inheritance.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1055 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/interfaces.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1419 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/numpydocstrings.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1525 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.453345 rope-1.8.0/rope/base/oi/type_hinting/resolvers/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      778 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/composite.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      405 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/interfaces.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      609 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/types.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5394 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/utils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10203 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/prefs.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15177 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/project.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12804 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/pycore.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6390 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/pynames.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2098 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/pynamesdef.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9271 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/pyobjects.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22557 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/pyobjectsdef.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11468 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/pyscopes.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10291 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/resourceobserver.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7812 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/resources.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5590 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/serializer.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1905 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/simplify.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1606 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/stdmods.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4907 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/taskhandle.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.457346 rope-1.8.0/rope/base/utils/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3949 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/utils/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1824 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/utils/datastructures.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1405 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/versioning.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22416 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/worder.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.457346 rope-1.8.0/rope/contrib/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      169 2022-07-29 12:45:37.000000 rope-1.8.0/rope/contrib/__init__.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.461346 rope-1.8.0/rope/contrib/autoimport/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      196 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2444 2022-07-29 12:45:37.000000 rope-1.8.0/rope/contrib/autoimport/defs.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3273 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/models.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5276 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/parse.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8394 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/pickle.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19728 2023-05-05 04:53:06.000000 rope-1.8.0/rope/contrib/autoimport/sqlite.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4826 2023-05-05 04:53:06.000000 rope-1.8.0/rope/contrib/autoimport/utils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1350 2022-07-29 12:45:37.000000 rope-1.8.0/rope/contrib/changestack.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26473 2022-12-15 11:40:37.000000 rope-1.8.0/rope/contrib/codeassist.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2935 2022-12-15 11:40:37.000000 rope-1.8.0/rope/contrib/finderrors.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4483 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/findit.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2194 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/fixmodnames.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6777 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/fixsyntax.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14845 2023-05-05 04:53:06.000000 rope-1.8.0/rope/contrib/generate.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.473346 rope-1.8.0/rope/refactor/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2126 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13432 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/change_signature.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8459 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/encapsulate_field.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    39187 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/extract.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8316 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/functionutils.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.477346 rope-1.8.0/rope/refactor/importutils/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13354 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/importutils/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14255 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/importutils/actions.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5790 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/importutils/importinfo.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21673 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/importutils/module_imports.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    25109 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/inline.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5913 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/introduce_factory.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3717 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/introduce_parameter.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2076 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/localtofield.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3829 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/method_object.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    34458 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/move.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2544 2022-12-15 11:40:37.000000 rope-1.8.0/rope/refactor/multiproject.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13040 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/occurrences.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31196 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/patchedast.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9348 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/rename.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11441 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/restructure.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12719 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/similarfinder.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3001 2022-12-15 11:40:37.000000 rope-1.8.0/rope/refactor/sourceutils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5152 2022-12-15 11:40:37.000000 rope-1.8.0/rope/refactor/suites.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1226 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/topackage.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6651 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/usefunction.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5740 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/wildcards.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.429345 rope-1.8.0/rope.egg-info/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5673 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/PKG-INFO
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5070 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/SOURCES.txt
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        1 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/dependency_links.txt
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      230 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/requires.txt
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        5 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/top_level.txt
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.489347 rope-1.8.0/ropetest/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    37493 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/advanced_oi_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    23217 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/builtinstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    35910 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/codeanalyzetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      787 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/conftest.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.493347 rope-1.8.0/ropetest/contrib/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/contrib/__init__.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.493347 rope-1.8.0/ropetest/contrib/autoimport/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      795 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/autoimport/autoimporttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      703 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/autoimport/conftest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2128 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/autoimport/modeltest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      647 2022-07-29 12:45:37.000000 rope-1.8.0/ropetest/contrib/autoimport/parsetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2237 2023-05-05 04:53:06.000000 rope-1.8.0/ropetest/contrib/autoimport/utilstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7286 2022-11-22 15:02:03.000000 rope-1.8.0/ropetest/contrib/autoimporttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      955 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/changestacktest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    56041 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/codeassisttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1629 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/finderrorstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5475 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/findittest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2066 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/fixmodnamestest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15157 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/generatetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2894 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/doatest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15912 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/historytest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6879 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/objectdbtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15681 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/objectinfertest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    48095 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/projecttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    52145 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/pycoretest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19385 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/pyscopestest.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.501347 rope-1.8.0/ropetest/refactor/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    38589 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    27113 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/change_signature_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)   101254 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/extracttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    69500 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/importutilstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    42803 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/inlinetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    41603 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/movetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3434 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/multiprojecttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    59540 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/patchedasttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    50303 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/renametest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9672 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/restructuretest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12065 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/similarfindertest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6766 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/suitestest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6400 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/usefunctiontest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5653 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/reprtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6404 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/runmodtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4801 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/serializer_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2203 2022-11-22 15:02:03.000000 rope-1.8.0/ropetest/simplifytest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3166 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/testutils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    16326 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/type_hinting_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1448 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/versioningtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      154 2023-05-05 05:06:22.501347 rope-1.8.0/setup.cfg
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)       38 2022-12-15 11:40:37.000000 rope-1.8.0/setup.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.163279 rope-1.9.0/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14368 2023-01-17 01:59:16.000000 rope-1.9.0/.all-contributorsrc
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      125 2022-07-29 12:45:37.000000 rope-1.9.0/.git-blame-ignore-revs
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.111282 rope-1.9.0/.github/
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.111282 rope-1.9.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      916 2022-07-29 12:45:37.000000 rope-1.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      595 2022-07-29 12:45:37.000000 rope-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      411 2023-01-17 01:59:16.000000 rope-1.9.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.111282 rope-1.9.0/.github/workflows/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      160 2022-07-29 12:45:37.000000 rope-1.9.0/.github/workflows/black.yml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      742 2023-05-05 04:53:06.000000 rope-1.9.0/.github/workflows/main.yml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      274 2023-01-17 01:59:16.000000 rope-1.9.0/.github/workflows/task-completed-checker-action.yml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1864 2022-07-29 12:46:52.000000 rope-1.9.0/.gitignore
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      120 2022-07-29 12:45:37.000000 rope-1.9.0/.readthedocs.yaml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9984 2023-06-29 12:22:53.000000 rope-1.9.0/CHANGELOG.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21134 2023-01-17 01:59:16.000000 rope-1.9.0/CONTRIBUTORS.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7652 2022-07-29 12:45:37.000000 rope-1.9.0/COPYING
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      150 2022-07-29 12:45:37.000000 rope-1.9.0/MANIFEST.in
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5697 2023-06-29 12:27:10.163279 rope-1.9.0/PKG-INFO
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4478 2023-05-05 04:53:06.000000 rope-1.9.0/README.rst
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.111282 rope-1.9.0/bin/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1607 2023-01-17 01:59:16.000000 rope-1.9.0/bin/tag-release.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.123281 rope-1.9.0/docs/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      634 2022-07-29 12:45:37.000000 rope-1.9.0/docs/Makefile
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2247 2022-09-19 07:11:34.000000 rope-1.9.0/docs/conf.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1719 2023-01-17 01:59:16.000000 rope-1.9.0/docs/configuration.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4518 2023-05-05 04:53:06.000000 rope-1.9.0/docs/contributing.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5165 2022-12-16 04:43:54.000000 rope-1.9.0/docs/default_config.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.123281 rope-1.9.0/docs/dev/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3906 2023-01-17 01:59:16.000000 rope-1.9.0/docs/dev/issues.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      526 2023-01-17 01:59:16.000000 rope-1.9.0/docs/index.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    28667 2023-06-29 12:14:37.000000 rope-1.9.0/docs/library.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      765 2022-07-29 12:45:37.000000 rope-1.9.0/docs/make.bat
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31016 2023-01-17 01:59:16.000000 rope-1.9.0/docs/overview.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      976 2023-05-05 05:01:06.000000 rope-1.9.0/docs/release-process.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1459 2022-09-19 07:41:21.000000 rope-1.9.0/docs/rope.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2290 2023-06-29 12:24:18.000000 rope-1.9.0/pyproject.toml
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.123281 rope-1.9.0/rope/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1431 2023-01-17 01:59:16.000000 rope-1.9.0/rope/__init__.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.131281 rope-1.9.0/rope/base/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      161 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3283 2022-12-15 11:40:37.000000 rope-1.9.0/rope/base/arguments.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2521 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/ast.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26263 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/builtins.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13675 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/change.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11774 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/codeanalyze.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13587 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/evaluate.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1370 2022-12-15 11:40:37.000000 rope-1.9.0/rope/base/exceptions.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8481 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/fscommands.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8342 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/history.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3841 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/libutils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1656 2022-12-15 11:40:37.000000 rope-1.9.0/rope/base/nameanalyze.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.131281 rope-1.9.0/rope/base/oi/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1682 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7397 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/doa.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3440 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/oi/memorydb.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4547 2022-12-16 03:37:02.000000 rope-1.9.0/rope/base/oi/objectdb.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8624 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/oi/objectinfo.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8532 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/runmod.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5862 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/oi/soa.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7719 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/soi.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9829 2022-12-15 11:40:37.000000 rope-1.9.0/rope/base/oi/transform.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.135280 rope-1.9.0/rope/base/oi/type_hinting/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9057 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/type_hinting/evaluate.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2728 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/oi/type_hinting/factory.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      715 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/interfaces.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.135280 rope-1.9.0/rope/base/oi/type_hinting/providers/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1856 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/composite.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6164 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/docstrings.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2116 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/inheritance.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1055 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/interfaces.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1419 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/numpydocstrings.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1525 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.135280 rope-1.9.0/rope/base/oi/type_hinting/resolvers/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/resolvers/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      778 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/resolvers/composite.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      405 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/oi/type_hinting/resolvers/interfaces.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      609 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/type_hinting/resolvers/types.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5394 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/oi/type_hinting/utils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10203 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/prefs.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15177 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/project.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12804 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/pycore.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6390 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/pynames.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2098 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/pynamesdef.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9271 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/pyobjects.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22557 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/pyobjectsdef.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11468 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/pyscopes.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10291 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/resourceobserver.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7812 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/resources.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5590 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/serializer.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1905 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/simplify.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1606 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/stdmods.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4907 2023-05-05 04:53:06.000000 rope-1.9.0/rope/base/taskhandle.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.139280 rope-1.9.0/rope/base/utils/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3949 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/utils/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1824 2022-12-15 11:40:37.000000 rope-1.9.0/rope/base/utils/datastructures.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1405 2023-01-17 01:59:16.000000 rope-1.9.0/rope/base/versioning.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22416 2022-07-29 12:45:37.000000 rope-1.9.0/rope/base/worder.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.139280 rope-1.9.0/rope/contrib/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      169 2022-07-29 12:45:37.000000 rope-1.9.0/rope/contrib/__init__.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.143280 rope-1.9.0/rope/contrib/autoimport/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      196 2023-01-17 01:59:16.000000 rope-1.9.0/rope/contrib/autoimport/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2444 2022-07-29 12:45:37.000000 rope-1.9.0/rope/contrib/autoimport/defs.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3524 2023-06-29 12:14:37.000000 rope-1.9.0/rope/contrib/autoimport/models.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5276 2023-01-17 01:59:16.000000 rope-1.9.0/rope/contrib/autoimport/parse.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8394 2023-01-17 01:59:16.000000 rope-1.9.0/rope/contrib/autoimport/pickle.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22217 2023-06-29 12:14:37.000000 rope-1.9.0/rope/contrib/autoimport/sqlite.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4826 2023-05-05 04:53:06.000000 rope-1.9.0/rope/contrib/autoimport/utils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1350 2022-07-29 12:45:37.000000 rope-1.9.0/rope/contrib/changestack.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26473 2022-12-15 11:40:37.000000 rope-1.9.0/rope/contrib/codeassist.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2935 2022-12-15 11:40:37.000000 rope-1.9.0/rope/contrib/finderrors.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4483 2023-01-17 01:59:16.000000 rope-1.9.0/rope/contrib/findit.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2194 2023-01-17 01:59:16.000000 rope-1.9.0/rope/contrib/fixmodnames.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6777 2023-01-17 01:59:16.000000 rope-1.9.0/rope/contrib/fixsyntax.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14845 2023-05-05 04:53:06.000000 rope-1.9.0/rope/contrib/generate.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.147280 rope-1.9.0/rope/refactor/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2126 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13432 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/change_signature.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8459 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/encapsulate_field.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    40319 2023-06-29 12:14:37.000000 rope-1.9.0/rope/refactor/extract.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8316 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/functionutils.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.151279 rope-1.9.0/rope/refactor/importutils/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13354 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/importutils/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14255 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/importutils/actions.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5790 2023-05-05 04:53:06.000000 rope-1.9.0/rope/refactor/importutils/importinfo.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21673 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/importutils/module_imports.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    25109 2023-05-05 04:53:06.000000 rope-1.9.0/rope/refactor/inline.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5913 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/introduce_factory.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3717 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/introduce_parameter.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2076 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/localtofield.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3829 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/method_object.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    34458 2023-05-05 04:53:06.000000 rope-1.9.0/rope/refactor/move.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2544 2022-12-15 11:40:37.000000 rope-1.9.0/rope/refactor/multiproject.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13040 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/occurrences.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31334 2023-06-29 12:14:37.000000 rope-1.9.0/rope/refactor/patchedast.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9348 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/rename.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11441 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/restructure.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12719 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/similarfinder.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3001 2022-12-15 11:40:37.000000 rope-1.9.0/rope/refactor/sourceutils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5152 2022-12-15 11:40:37.000000 rope-1.9.0/rope/refactor/suites.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1226 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/topackage.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6651 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/usefunction.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5740 2023-01-17 01:59:16.000000 rope-1.9.0/rope/refactor/wildcards.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.123281 rope-1.9.0/rope.egg-info/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5697 2023-06-29 12:27:10.000000 rope-1.9.0/rope.egg-info/PKG-INFO
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5070 2023-06-29 12:27:10.000000 rope-1.9.0/rope.egg-info/SOURCES.txt
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        1 2023-06-29 12:27:10.000000 rope-1.9.0/rope.egg-info/dependency_links.txt
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      254 2023-06-29 12:27:10.000000 rope-1.9.0/rope.egg-info/requires.txt
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        5 2023-06-29 12:27:10.000000 rope-1.9.0/rope.egg-info/top_level.txt
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.155279 rope-1.9.0/ropetest/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.9.0/ropetest/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    37493 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/advanced_oi_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    23217 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/builtinstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    35910 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/codeanalyzetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      787 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/conftest.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.159279 rope-1.9.0/ropetest/contrib/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.9.0/ropetest/contrib/__init__.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.159279 rope-1.9.0/ropetest/contrib/autoimport/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4358 2023-06-29 12:14:37.000000 rope-1.9.0/ropetest/contrib/autoimport/autoimporttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      703 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/autoimport/conftest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2128 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/autoimport/modeltest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      647 2022-07-29 12:45:37.000000 rope-1.9.0/ropetest/contrib/autoimport/parsetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2237 2023-05-05 04:53:06.000000 rope-1.9.0/ropetest/contrib/autoimport/utilstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7286 2022-11-22 15:02:03.000000 rope-1.9.0/ropetest/contrib/autoimporttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      955 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/changestacktest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    56041 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/codeassisttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1629 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/finderrorstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5475 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/findittest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2066 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/fixmodnamestest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15157 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/contrib/generatetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2894 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/doatest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15912 2022-12-15 11:40:37.000000 rope-1.9.0/ropetest/historytest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6879 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/objectdbtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15681 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/objectinfertest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    48095 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/projecttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    52145 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/pycoretest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19385 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/pyscopestest.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-06-29 12:27:10.163279 rope-1.9.0/ropetest/refactor/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    38589 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    27113 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/change_signature_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)   105634 2023-06-29 12:14:37.000000 rope-1.9.0/ropetest/refactor/extracttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    69500 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/importutilstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    42803 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/inlinetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    41603 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/movetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3434 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/multiprojecttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    59866 2023-06-29 12:14:37.000000 rope-1.9.0/ropetest/refactor/patchedasttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    50303 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/renametest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9672 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/restructuretest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12065 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/similarfindertest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6766 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/suitestest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6400 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/refactor/usefunctiontest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5653 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/reprtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6404 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/runmodtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4801 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/serializer_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2203 2022-11-22 15:02:03.000000 rope-1.9.0/ropetest/simplifytest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3166 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/testutils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    16326 2022-12-15 11:40:37.000000 rope-1.9.0/ropetest/type_hinting_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1448 2023-01-17 01:59:16.000000 rope-1.9.0/ropetest/versioningtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      154 2023-06-29 12:27:10.167278 rope-1.9.0/setup.cfg
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)       38 2022-12-15 11:40:37.000000 rope-1.9.0/setup.py
```

### Comparing `rope-1.8.0/.all-contributorsrc` & `rope-1.9.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/.github/ISSUE_TEMPLATE/bug-report.md` & `rope-1.9.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `rope-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/.github/workflows/main.yml` & `rope-1.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/.gitignore` & `rope-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/CHANGELOG.md` & `rope-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # **Upcoming release**
 
+# Release 1.9.0
+
+- #624, #693 Implement `nonlocal` keyword (@lieryan)
+- #697, #565 Automatically purge autoimport.db when there is schema change
+
 # Release 1.8.0
 
 - #650 Install pre-commit hooks on rope repository (@lieryan)
 - #655 Remove unused __init__() methods (@edreamleo, @lieryan)
 - #656 Reformat using black 23.1.0 (@edreamleo)
 - #674 Fix/supress all mypy complaints (@edreamleo)
 - #680 Remove a do-nothing statement in soi._handle_first_parameter (@edreamleo)
```

### Comparing `rope-1.8.0/CONTRIBUTORS.md` & `rope-1.9.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/COPYING` & `rope-1.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/PKG-INFO` & `rope-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rope
-Version: 1.8.0
+Version: 1.9.0
 Summary: a python refactoring library...
 Author-email: Ali Gholami Rudi <aligrudi@users.sourceforge.net>
 Maintainer-email: Lie Ryan <lieryan.24@proton.me>
 License: LGPL-3.0-or-later
 Project-URL: Source, https://github.com/python-rope/rope
 Project-URL: Documentation, https://rope.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: dev
+Provides-Extra: release
 License-File: COPYING
 
 
 .. _GitHub python-rope / rope: https://github.com/python-rope/rope
 
 
 =========================================================================
```

### Comparing `rope-1.8.0/README.rst` & `rope-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/bin/tag-release.py` & `rope-1.9.0/bin/tag-release.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/Makefile` & `rope-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/conf.py` & `rope-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/configuration.rst` & `rope-1.9.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/contributing.rst` & `rope-1.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/default_config.py` & `rope-1.9.0/docs/default_config.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/dev/issues.rst` & `rope-1.9.0/docs/dev/issues.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/index.rst` & `rope-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/library.rst` & `rope-1.9.0/docs/library.rst`

 * *Files 0% similar despite different names*

```diff
@@ -840,17 +840,19 @@
 existing integrations should migrate to the sqlite3 storage as the pickle-based
 autoimport will be removed in the future.
 
 
 `rope.contrib.autoimport.sqlite`
 --------------------------------
 
-By default, the sqlite3-based only stores autoimport cache in an in-memory
+Currently, the sqlite3-based only stores autoimport cache in an in-memory
 sqlite3 database, you can make it write the import cache to persistent storage
-by passing memory=False to AutoImport constructor.
+by passing memory=False to AutoImport constructor. This default will change in
+the future, if you want to always store the autoimport cache in-memory, then
+you need to explicitly pass memory=True.
 
 It must be closed when done with the ``AutoImport.close()`` method.
 
 AutoImport can search for a name from both modules and statements you can import from them.
 
 .. code-block:: python
```

### Comparing `rope-1.8.0/docs/make.bat` & `rope-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/overview.rst` & `rope-1.9.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/release-process.rst` & `rope-1.9.0/docs/release-process.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/docs/rope.rst` & `rope-1.9.0/docs/rope.rst`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/pyproject.toml` & `rope-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Topic :: Software Development',
 ]
-version = '1.8.0'
+version = '1.9.0'
 dependencies = ['pytoolconfig[global] >= 1.2.2']
 
 [[project.authors]]
 name = 'Ali Gholami Rudi'
 email = 'aligrudi@users.sourceforge.net'
 
 [[project.maintainers]]
@@ -46,16 +46,19 @@
     "sphinx-rtd-theme>=1.0.0",
 ]
 dev = [
     'pytest>=7.0.1',
     'pytest-timeout>=2.1.0',
     'build>=0.7.0',
     'pre-commit>=2.20.0',
-    'pip-tools>=6.12.1',
+]
+release = [
     'toml>=0.10.2',
+    'twine>=4.0.2',
+    'pip-tools>=6.12.1',
 ]
 [tool.setuptools]
 packages = [
     'rope',
     'rope.base',
     'rope.base.oi',
     'rope.base.oi.type_hinting',
```

### Comparing `rope-1.8.0/rope/__init__.py` & `rope-1.9.0/rope/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/arguments.py` & `rope-1.9.0/rope/base/arguments.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/ast.py` & `rope-1.9.0/rope/base/ast.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/builtins.py` & `rope-1.9.0/rope/base/builtins.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/change.py` & `rope-1.9.0/rope/base/change.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/codeanalyze.py` & `rope-1.9.0/rope/base/codeanalyze.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/evaluate.py` & `rope-1.9.0/rope/base/evaluate.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/exceptions.py` & `rope-1.9.0/rope/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/fscommands.py` & `rope-1.9.0/rope/base/fscommands.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/history.py` & `rope-1.9.0/rope/base/history.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/libutils.py` & `rope-1.9.0/rope/base/libutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/nameanalyze.py` & `rope-1.9.0/rope/base/nameanalyze.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/__init__.py` & `rope-1.9.0/rope/base/oi/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/doa.py` & `rope-1.9.0/rope/base/oi/doa.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/memorydb.py` & `rope-1.9.0/rope/base/oi/memorydb.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/objectdb.py` & `rope-1.9.0/rope/base/oi/objectdb.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/objectinfo.py` & `rope-1.9.0/rope/base/oi/objectinfo.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/runmod.py` & `rope-1.9.0/rope/base/oi/runmod.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/soa.py` & `rope-1.9.0/rope/base/oi/soa.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/soi.py` & `rope-1.9.0/rope/base/oi/soi.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/transform.py` & `rope-1.9.0/rope/base/oi/transform.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/evaluate.py` & `rope-1.9.0/rope/base/oi/type_hinting/evaluate.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/factory.py` & `rope-1.9.0/rope/base/oi/type_hinting/factory.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/interfaces.py` & `rope-1.9.0/rope/base/oi/type_hinting/interfaces.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/providers/composite.py` & `rope-1.9.0/rope/base/oi/type_hinting/providers/composite.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/providers/docstrings.py` & `rope-1.9.0/rope/base/oi/type_hinting/providers/docstrings.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/providers/inheritance.py` & `rope-1.9.0/rope/base/oi/type_hinting/providers/inheritance.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/providers/interfaces.py` & `rope-1.9.0/rope/base/oi/type_hinting/providers/interfaces.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/providers/numpydocstrings.py` & `rope-1.9.0/rope/base/oi/type_hinting/providers/numpydocstrings.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py` & `rope-1.9.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/resolvers/composite.py` & `rope-1.9.0/rope/base/oi/type_hinting/resolvers/composite.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/resolvers/types.py` & `rope-1.9.0/rope/base/oi/type_hinting/resolvers/types.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/oi/type_hinting/utils.py` & `rope-1.9.0/rope/base/oi/type_hinting/utils.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/prefs.py` & `rope-1.9.0/rope/base/prefs.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/project.py` & `rope-1.9.0/rope/base/project.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/pycore.py` & `rope-1.9.0/rope/base/pycore.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/pynames.py` & `rope-1.9.0/rope/base/pynames.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/pynamesdef.py` & `rope-1.9.0/rope/base/pynamesdef.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/pyobjects.py` & `rope-1.9.0/rope/base/pyobjects.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/pyobjectsdef.py` & `rope-1.9.0/rope/base/pyobjectsdef.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/pyscopes.py` & `rope-1.9.0/rope/base/pyscopes.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/resourceobserver.py` & `rope-1.9.0/rope/base/resourceobserver.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/resources.py` & `rope-1.9.0/rope/base/resources.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/serializer.py` & `rope-1.9.0/rope/base/serializer.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/simplify.py` & `rope-1.9.0/rope/base/simplify.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/stdmods.py` & `rope-1.9.0/rope/base/stdmods.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/taskhandle.py` & `rope-1.9.0/rope/base/taskhandle.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/utils/__init__.py` & `rope-1.9.0/rope/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/utils/datastructures.py` & `rope-1.9.0/rope/base/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/versioning.py` & `rope-1.9.0/rope/base/versioning.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/base/worder.py` & `rope-1.9.0/rope/base/worder.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/autoimport/defs.py` & `rope-1.9.0/rope/contrib/autoimport/defs.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/autoimport/models.py` & `rope-1.9.0/rope/contrib/autoimport/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         columns = ", ".join(self.columns)
         placeholders = ", ".join(["?"] * len(self.columns))
         return FinalQuery(
             f"INSERT INTO {self.query}({columns}) VALUES ({placeholders})"
         )
 
     def drop_table(self) -> FinalQuery:
-        return FinalQuery(f"DROP TABLE {self.query}")
+        return FinalQuery(f"DROP TABLE IF EXISTS {self.query}")
 
     def delete_from(self) -> FinalQuery:
         return FinalQuery(f"DELETE FROM {self.query}")
 
 
 class Model(ABC):
     @property
@@ -69,14 +69,26 @@
         ]
         metadata_table_definition = ", ".join(metadata_table)
         connection.execute(
             f"CREATE TABLE IF NOT EXISTS {cls.table_name}({metadata_table_definition})"
         )
 
 
+class Metadata(Model):
+    table_name = "metadata"
+
+    schema = {
+        "version_hash": "TEXT",
+        "hash_data": "TEXT",
+        "created_at": "TEXT",
+    }
+    columns = list(schema.keys())
+    objects = Query(table_name, columns)
+
+
 class Name(Model):
     table_name = "names"
     schema = {
         "name": "TEXT",
         "module": "TEXT",
         "package": "TEXT",
         "source": "INTEGER",
```

### Comparing `rope-1.8.0/rope/contrib/autoimport/parse.py` & `rope-1.9.0/rope/contrib/autoimport/parse.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/autoimport/pickle.py` & `rope-1.9.0/rope/contrib/autoimport/pickle.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/autoimport/sqlite.py` & `rope-1.9.0/rope/contrib/autoimport/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """AutoImport module for rope."""
 
 import contextlib
+import json
 import re
 import sqlite3
 import sys
+import warnings
 from collections import OrderedDict
 from concurrent.futures import Future, ProcessPoolExecutor, as_completed
+from datetime import datetime
 from itertools import chain
 from pathlib import Path
 from typing import Generator, Iterable, Iterator, List, Optional, Set, Tuple
 
-from rope.base import exceptions, libutils, resourceobserver, taskhandle
+from rope.base import exceptions, libutils, resourceobserver, taskhandle, versioning
 from rope.base.project import Project
 from rope.base.resources import Resource
 from rope.contrib.autoimport import models
 from rope.contrib.autoimport.defs import (
     ModuleFile,
     Name,
     NameType,
@@ -59,64 +62,114 @@
 
         def filter_package(package: Package) -> bool:
             return package.name not in existing and not package.name.startswith("_")
 
     return filter(filter_package, packages)
 
 
+_deprecated_default: bool = object()  # type: ignore
+
+
 class AutoImport:
     """A class for finding the module that provides a name.
 
     This class maintains a cache of global names in python modules.
     Note that this cache is not accurate and might be out of date.
 
     """
 
     connection: sqlite3.Connection
     underlined: bool
     project: Project
     project_package: Package
 
-    def __init__(self, project: Project, observe=True, underlined=False, memory=True):
+    def __init__(
+        self,
+        project: Project,
+        observe: bool = True,
+        underlined: bool = False,
+        memory: bool = _deprecated_default,
+    ):
         """Construct an AutoImport object.
 
         Parameters
         ___________
         project : rope.base.project.Project
             the project to use for project imports
         observe : bool
             if true, listen for project changes and update the cache.
         underlined : bool
             If `underlined` is `True`, underlined names are cached, too.
-        memory : bool
-            if true, don't persist to disk
+        memory:
+            If true, don't persist to disk
+
+            DEPRECATION NOTICE: The default value will change to use an on-disk
+            database by default in the future. If you want to use an in-memory
+            database, you need to pass `memory=True` explicitly:
+
+                autoimport = AutoImport(..., memory=True)
         """
         self.project = project
         project_package = get_package_tuple(Path(project.root.real_path), project)
         assert project_package is not None
         assert project_package.path is not None
         self.project_package = project_package
         self.underlined = underlined
-        db_path: str
-        if memory or project.ropefolder is None:
-            db_path = ":memory:"
-        else:
-            db_path = str(Path(project.ropefolder.real_path) / "autoimport.db")
-        self.connection = sqlite3.connect(db_path)
+        if memory is _deprecated_default:
+            memory = True
+            warnings.warn(
+                "The default value for `AutoImport(memory)` argument will "
+                "change to use an on-disk database by default in the future. "
+                "If you want to use an in-memory database, you need to pass "
+                "`AutoImport(memory=True)` explicitly.",
+                DeprecationWarning,
+            )
+        self.connection = self.create_database_connection(
+            project=project,
+            memory=memory,
+        )
         self._setup_db()
         if observe:
             observer = resourceobserver.ResourceObserver(
                 changed=self._changed, moved=self._moved, removed=self._removed
             )
             project.add_observer(observer)
 
+    @classmethod
+    def create_database_connection(
+        cls,
+        *,
+        project: Optional[Project] = None,
+        memory: bool = False,
+    ) -> sqlite3.Connection:
+        """
+        Create an sqlite3 connection
+
+        project : rope.base.project.Project
+            the project to use for project imports
+        memory : bool
+            if true, don't persist to disk
+        """
+        if not memory and project is None:
+            raise Exception("if memory=False, project must be provided")
+        db_path: str
+        if memory or project is None or project.ropefolder is None:
+            db_path = ":memory:"
+        else:
+            db_path = str(Path(project.ropefolder.real_path) / "autoimport.db")
+        return sqlite3.connect(db_path)
+
     def _setup_db(self):
-        models.Name.create_table(self.connection)
-        models.Package.create_table(self.connection)
-        self.connection.commit()
+        models.Metadata.create_table(self.connection)
+        version_hash = list(
+            self._execute(models.Metadata.objects.select("version_hash"))
+        )
+        current_version_hash = versioning.calculate_version_hash(self.project)
+        if not version_hash or version_hash[0][0] != current_version_hash:
+            self.clear_cache()
 
     def import_assist(self, starting: str):
         """
         Find modules that have a global name that starts with `starting`.
 
         For a more complete list, use the search or search_full methods.
 
@@ -375,18 +428,34 @@
     def clear_cache(self):
         """Clear all entries in global-name cache.
 
         It might be a good idea to use this function before
         regenerating global names.
 
         """
-        self._execute(models.Name.objects.drop_table())
-        self._execute(models.Package.objects.drop_table())
-        self._setup_db()
-        self.connection.commit()
+        with self.connection:
+            self._execute(models.Name.objects.drop_table())
+            self._execute(models.Package.objects.drop_table())
+            self._execute(models.Metadata.objects.drop_table())
+            models.Name.create_table(self.connection)
+            models.Package.create_table(self.connection)
+            models.Metadata.create_table(self.connection)
+            data = (
+                versioning.calculate_version_hash(self.project),
+                json.dumps(versioning.get_version_hash_data(self.project)),
+                datetime.utcnow().isoformat(),
+            )
+            assert models.Metadata.columns == [
+                "version_hash",
+                "hash_data",
+                "created_at",
+            ]
+            self._execute(models.Metadata.objects.insert_into(), data)
+
+            self.connection.commit()
 
     def find_insertion_line(self, code):
         """Guess at what line the new import should be inserted."""
         match = re.search(r"^(def|class)\s+", code)
         if match is not None:
             code = code[: match.start()]
         try:
```

### Comparing `rope-1.8.0/rope/contrib/autoimport/utils.py` & `rope-1.9.0/rope/contrib/autoimport/utils.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/changestack.py` & `rope-1.9.0/rope/contrib/changestack.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/codeassist.py` & `rope-1.9.0/rope/contrib/codeassist.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/finderrors.py` & `rope-1.9.0/rope/contrib/finderrors.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/findit.py` & `rope-1.9.0/rope/contrib/findit.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/fixmodnames.py` & `rope-1.9.0/rope/contrib/fixmodnames.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/fixsyntax.py` & `rope-1.9.0/rope/contrib/fixsyntax.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/contrib/generate.py` & `rope-1.9.0/rope/contrib/generate.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/__init__.py` & `rope-1.9.0/rope/refactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/change_signature.py` & `rope-1.9.0/rope/refactor/change_signature.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/encapsulate_field.py` & `rope-1.9.0/rope/refactor/encapsulate_field.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/extract.py` & `rope-1.9.0/rope/refactor/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from typing import Dict
 from contextlib import contextmanager
 from itertools import chain
+from typing import Dict
 
 from rope.base import ast, codeanalyze
 from rope.base.change import ChangeContents, ChangeSet
 from rope.base.exceptions import RefactoringError
 from rope.base.utils.datastructures import OrderedSet
 from rope.refactor import patchedast, similarfinder, sourceutils, suites, usefunction
 
@@ -725,43 +725,66 @@
         if self.info.one_line:
             return self._get_single_expression_function_body()
         return self._get_multiline_function_body(returns)
 
     def _get_multiline_function_body(self, returns):
         unindented_body = sourceutils.fix_indentation(self.info.extracted, 0)
         unindented_body = self._insert_globals(unindented_body)
+        unindented_body = self._insert_nonlocals(unindented_body)
         if returns:
             unindented_body += "\nreturn %s" % self._get_comma_form(returns)
         return unindented_body
 
     def _get_single_expression_function_body(self):
         extracted = _get_single_expression_body(self.info.extracted, info=self.info)
         body = "return " + extracted
-        return self._insert_globals(body)
+        body = self._insert_globals(body)
+        body = self._insert_nonlocals(body)
+        return body
 
     def _insert_globals(self, unindented_body):
         globals_in_body = self._get_globals_in_body(unindented_body)
         globals_ = self.info_collector.globals_ & (
             self.info_collector.written | self.info_collector.maybe_written
         )
         globals_ = globals_ - globals_in_body
 
         if globals_:
             unindented_body = "global {}\n{}".format(
                 ", ".join(globals_), unindented_body
             )
         return unindented_body
 
+    def _insert_nonlocals(self, unindented_body):
+        nonlocals_in_body = self._get_nonlocals_in_body(unindented_body)
+        nonlocals_ = self.info_collector.nonlocals_ & (
+            self.info_collector.written | self.info_collector.maybe_written
+        )
+        nonlocals_ = nonlocals_ - nonlocals_in_body
+
+        if nonlocals_:
+            unindented_body = "nonlocal {}\n{}".format(
+                ", ".join(nonlocals_), unindented_body
+            )
+        return unindented_body
+
     @staticmethod
     def _get_globals_in_body(unindented_body):
         node = _parse_text(unindented_body)
         visitor = _GlobalFinder()
         visitor.visit(node)
         return visitor.globals_
 
+    @staticmethod
+    def _get_nonlocals_in_body(unindented_body):
+        node = _parse_text(unindented_body)
+        visitor = _NonlocalFinder()
+        visitor.visit(node)
+        return visitor.nonlocals_
+
 
 class _ExtractVariableParts:
     def __init__(self, info):
         self.info = info
 
     def get_definition(self):
         extracted = _get_single_expression_body(self.info.extracted, info=self.info)
@@ -787,14 +810,15 @@
         self.written = OrderedSet()
         self.read = OrderedSet()
         self.postread = OrderedSet()
         self.postwritten = OrderedSet()
         self.host_function = True
         self.conditional = False
         self.globals_ = OrderedSet()
+        self.nonlocals_ = OrderedSet()
         self.surrounded_by_loop = 0
         self.loop_depth = 0
 
     def _read_variable(self, name, lineno):
         if self.start <= lineno <= self.end:
             if name not in self.written:
                 if not self.conditional or name not in self.maybe_written:
@@ -830,14 +854,17 @@
                 visitor.visit(child)
             for name in visitor.read - visitor.written:
                 self._read_variable(name, node.lineno)
 
     def _Global(self, node):
         self.globals_.add(*node.names)
 
+    def _Nonlocal(self, node):
+        self.nonlocals_.add(*node.names)
+
     def _AsyncFunctionDef(self, node):
         self._FunctionDef(node)
 
     def _Name(self, node):
         if isinstance(node.ctx, (ast.Store, ast.AugStore)):
             self._written_variable(node.id, node.lineno)
         if not isinstance(node.ctx, ast.Store):
@@ -1070,14 +1097,22 @@
     def __init__(self):
         self.globals_ = OrderedSet()
 
     def _Global(self, node):
         self.globals_.add(*node.names)
 
 
+class _NonlocalFinder(ast.RopeNodeVisitor):
+    def __init__(self):
+        self.nonlocals_ = OrderedSet()
+
+    def _Nonlocal(self, node):
+        self.nonlocals_.add(*node.names)
+
+
 def _get_function_kind(scope):
     return scope.pyobject.get_kind()
 
 
 def _parse_text(body):
     body = sourceutils.fix_indentation(body, 0)
     try:
```

### Comparing `rope-1.8.0/rope/refactor/functionutils.py` & `rope-1.9.0/rope/refactor/functionutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/importutils/__init__.py` & `rope-1.9.0/rope/refactor/importutils/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/importutils/actions.py` & `rope-1.9.0/rope/refactor/importutils/actions.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/importutils/importinfo.py` & `rope-1.9.0/rope/refactor/importutils/importinfo.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/importutils/module_imports.py` & `rope-1.9.0/rope/refactor/importutils/module_imports.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/inline.py` & `rope-1.9.0/rope/refactor/inline.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/introduce_factory.py` & `rope-1.9.0/rope/refactor/introduce_factory.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/introduce_parameter.py` & `rope-1.9.0/rope/refactor/introduce_parameter.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/localtofield.py` & `rope-1.9.0/rope/refactor/localtofield.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/method_object.py` & `rope-1.9.0/rope/refactor/method_object.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/move.py` & `rope-1.9.0/rope/refactor/move.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/multiproject.py` & `rope-1.9.0/rope/refactor/multiproject.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/occurrences.py` & `rope-1.9.0/rope/refactor/occurrences.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/patchedast.py` & `rope-1.9.0/rope/refactor/patchedast.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,14 +553,18 @@
             children.extend(["if", if_])
         self._handle(node, children)
 
     def _Global(self, node):
         children = ["global", *self._child_nodes(node.names, ",")]
         self._handle(node, children)
 
+    def _Nonlocal(self, node):
+        children = ["nonlocal", *self._child_nodes(node.names, ",")]
+        self._handle(node, children)
+
     def _If(self, node):
         children = ["elif"] if self._is_elif(node) else ["if"]
         children.extend([node.test, ":"])
         children.extend(node.body)
         if node.orelse:
             if len(node.orelse) == 1 and self._is_elif(node.orelse[0]):
                 pass
```

### Comparing `rope-1.8.0/rope/refactor/rename.py` & `rope-1.9.0/rope/refactor/rename.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/restructure.py` & `rope-1.9.0/rope/refactor/restructure.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/similarfinder.py` & `rope-1.9.0/rope/refactor/similarfinder.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/sourceutils.py` & `rope-1.9.0/rope/refactor/sourceutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/suites.py` & `rope-1.9.0/rope/refactor/suites.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/topackage.py` & `rope-1.9.0/rope/refactor/topackage.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/usefunction.py` & `rope-1.9.0/rope/refactor/usefunction.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope/refactor/wildcards.py` & `rope-1.9.0/rope/refactor/wildcards.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/rope.egg-info/PKG-INFO` & `rope-1.9.0/rope.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rope
-Version: 1.8.0
+Version: 1.9.0
 Summary: a python refactoring library...
 Author-email: Ali Gholami Rudi <aligrudi@users.sourceforge.net>
 Maintainer-email: Lie Ryan <lieryan.24@proton.me>
 License: LGPL-3.0-or-later
 Project-URL: Source, https://github.com/python-rope/rope
 Project-URL: Documentation, https://rope.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: dev
+Provides-Extra: release
 License-File: COPYING
 
 
 .. _GitHub python-rope / rope: https://github.com/python-rope/rope
 
 
 =========================================================================
```

### Comparing `rope-1.8.0/rope.egg-info/SOURCES.txt` & `rope-1.9.0/rope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/advanced_oi_test.py` & `rope-1.9.0/ropetest/advanced_oi_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/builtinstest.py` & `rope-1.9.0/ropetest/builtinstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/codeanalyzetest.py` & `rope-1.9.0/ropetest/codeanalyzetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/conftest.py` & `rope-1.9.0/ropetest/conftest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/autoimport/conftest.py` & `rope-1.9.0/ropetest/contrib/autoimport/conftest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/autoimport/modeltest.py` & `rope-1.9.0/ropetest/contrib/autoimport/modeltest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/autoimport/parsetest.py` & `rope-1.9.0/ropetest/contrib/autoimport/parsetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/autoimport/utilstest.py` & `rope-1.9.0/ropetest/contrib/autoimport/utilstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/autoimporttest.py` & `rope-1.9.0/ropetest/contrib/autoimporttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/changestacktest.py` & `rope-1.9.0/ropetest/contrib/changestacktest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/codeassisttest.py` & `rope-1.9.0/ropetest/contrib/codeassisttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/finderrorstest.py` & `rope-1.9.0/ropetest/contrib/finderrorstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/findittest.py` & `rope-1.9.0/ropetest/contrib/findittest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/fixmodnamestest.py` & `rope-1.9.0/ropetest/contrib/fixmodnamestest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/contrib/generatetest.py` & `rope-1.9.0/ropetest/contrib/generatetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/doatest.py` & `rope-1.9.0/ropetest/doatest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/historytest.py` & `rope-1.9.0/ropetest/historytest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/objectdbtest.py` & `rope-1.9.0/ropetest/objectdbtest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/objectinfertest.py` & `rope-1.9.0/ropetest/objectinfertest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/projecttest.py` & `rope-1.9.0/ropetest/projecttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/pycoretest.py` & `rope-1.9.0/ropetest/pycoretest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/pyscopestest.py` & `rope-1.9.0/ropetest/pyscopestest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/__init__.py` & `rope-1.9.0/ropetest/refactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/change_signature_test.py` & `rope-1.9.0/ropetest/refactor/change_signature_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/extracttest.py` & `rope-1.9.0/ropetest/refactor/extracttest.py`

 * *Files 1% similar despite different names*

```diff
@@ -3101,14 +3101,183 @@
                 return (g := 4)
 
             f()
             print(g)
         """)
         self.assertEqual(expected, refactored)
 
+    def test_extraction_with_nonlocal_variable(self):
+        code = dedent("""\
+            def outer():
+                a = 0
+                def inner():
+                    nonlocal a
+                    a = 3
+        """)
+        extract_target = "a = 3"
+        start, end = code.index(extract_target), code.index(extract_target) + len(
+            extract_target
+        )
+        refactored = self.do_extract_method(code, start, end, "extracted")
+        expected = dedent("""\
+            def outer():
+                a = 0
+                def inner():
+                    nonlocal a
+                    extracted()
+
+                def extracted():
+                    nonlocal a
+                    a = 3
+        """)
+        self.assertEqual(expected, refactored)
+
+    def test_extraction_method_with_nonlocal_variable_and_nonlocal_declaration(self):
+        code = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    g = 2
+
+                inner()
+                print(g)
+        """)
+        start, end = 52, 78
+        refactored = self.do_extract_method(code, start, end, "_g")
+        expected = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    _g()
+
+                def _g():
+                    nonlocal g
+
+                    g = 2
+
+                inner()
+                print(g)
+        """)
+        self.assertEqual(expected, refactored)
+
+    def test_extraction_one_line_with_nonlocal_variable_read_only(self):
+        code = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    a = g
+
+                inner()
+                print(g)
+        """)
+        extract_target = "= g"
+        start, end = code.index(extract_target) + 2, code.index(extract_target) + 3
+        refactored = self.do_extract_method(code, start, end, "_g")
+        expected = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    a = _g()
+
+                def _g():
+                    return g
+
+                inner()
+                print(g)
+        """)
+        self.assertEqual(expected, refactored)
+
+    @testutils.only_for_versions_higher("3.8")
+    def test_extraction_one_line_with_nonlocal_variable(self):
+        code = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    while g := 4:
+                        pass
+
+                inner()
+                print(g)
+        """)
+        extract_target = "g := 4"
+        start, end = code.index(extract_target), code.index(extract_target) + len(
+            extract_target
+        )
+        refactored = self.do_extract_method(code, start, end, "_g")
+        expected = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    while _g():
+                        pass
+
+                def _g():
+                    nonlocal g
+                    return (g := 4)
+
+                inner()
+                print(g)
+        """)
+        self.assertEqual(expected, refactored)
+
+    @testutils.only_for_versions_higher("3.8")
+    def test_extraction_one_line_with_nonlocal_variable_has_postread(self):
+        code = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    while g := 4:
+                        print(g)
+
+                inner()
+                print(g)
+        """)
+        extract_target = "g := 4"
+        start, end = code.index(extract_target), code.index(extract_target) + len(
+            extract_target
+        )
+        refactored = self.do_extract_method(code, start, end, "_g")
+        expected = dedent("""\
+            def outer():
+                g = None
+
+                def inner():
+                    nonlocal g
+
+                    while g := _g():
+                        print(g)
+
+                def _g():
+                    nonlocal g
+                    return (g := 4)
+
+                inner()
+                print(g)
+        """)
+        self.assertEqual(expected, refactored)
+
     def test_extract_method_with_nested_double_with_as(self):
         code = dedent("""\
             with open("test") as file1:
                 with open("test") as file2:
                     print(file1, file2)
         """)
         start, end = self._convert_line_range_to_offset(code, 3, 4)
```

### Comparing `rope-1.8.0/ropetest/refactor/importutilstest.py` & `rope-1.9.0/ropetest/refactor/importutilstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/inlinetest.py` & `rope-1.9.0/ropetest/refactor/inlinetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/movetest.py` & `rope-1.9.0/ropetest/refactor/movetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/multiprojecttest.py` & `rope-1.9.0/ropetest/refactor/multiprojecttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/patchedasttest.py` & `rope-1.9.0/ropetest/refactor/patchedasttest.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,14 +733,21 @@
     def test_global_node(self):
         source = "global a, b\n"
         ast_frag = patchedast.get_patched_ast(source, True)
         checker = _ResultChecker(self, ast_frag)
         checker.check_region("Global", 0, len(source) - 1)
         checker.check_children("Global", ["global", " ", "a", "", ",", " ", "b"])
 
+    def test_nonlocal_node(self):
+        source = "nonlocal a, b\n"
+        ast_frag = patchedast.get_patched_ast(source, True)
+        checker = _ResultChecker(self, ast_frag)
+        checker.check_region("Nonlocal", 0, len(source) - 1)
+        checker.check_children("Nonlocal", ["nonlocal", " ", "a", "", ",", " ", "b"])
+
     def test_if_node(self):
         source = "if True:\n    pass\nelse:\n    pass\n"
         ast_frag = patchedast.get_patched_ast(source, True)
         checker = _ResultChecker(self, ast_frag)
         checker.check_region("If", 0, len(source) - 1)
         checker.check_children(
             "If",
```

### Comparing `rope-1.8.0/ropetest/refactor/renametest.py` & `rope-1.9.0/ropetest/refactor/renametest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/restructuretest.py` & `rope-1.9.0/ropetest/refactor/restructuretest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/similarfindertest.py` & `rope-1.9.0/ropetest/refactor/similarfindertest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/suitestest.py` & `rope-1.9.0/ropetest/refactor/suitestest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/refactor/usefunctiontest.py` & `rope-1.9.0/ropetest/refactor/usefunctiontest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/reprtest.py` & `rope-1.9.0/ropetest/reprtest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/runmodtest.py` & `rope-1.9.0/ropetest/runmodtest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/serializer_test.py` & `rope-1.9.0/ropetest/serializer_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/simplifytest.py` & `rope-1.9.0/ropetest/simplifytest.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/testutils.py` & `rope-1.9.0/ropetest/testutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/type_hinting_test.py` & `rope-1.9.0/ropetest/type_hinting_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.8.0/ropetest/versioningtest.py` & `rope-1.9.0/ropetest/versioningtest.py`

 * *Files identical despite different names*

