# Comparing `tmp/python-lsp-server-1.7.3.tar.gz` & `tmp/python-lsp-server-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-server-1.7.3.tar", last modified: Mon May 15 11:38:25 2023, max compression
+gzip compressed data, was "python-lsp-server-1.7.4.tar", last modified: Thu Jun 29 17:12:25 2023, max compression
```

## Comparing `python-lsp-server-1.7.3.tar` & `python-lsp-server-1.7.4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.877593 python-lsp-server-1.7.3/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/.coveragerc
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/.gitattributes
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.849594 python-lsp-server-1.7.3/.github/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.853594 python-lsp-server-1.7.3/.github/workflows/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1228 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/.github/workflows/release.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1386 2022-12-26 21:07:40.000000 python-lsp-server-1.7.3/.github/workflows/static.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1433 2022-12-26 21:07:40.000000 python-lsp-server-1.7.3/.github/workflows/test-linux.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1434 2022-12-26 21:07:40.000000 python-lsp-server-1.7.3/.github/workflows/test-mac.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1129 2022-12-26 21:07:40.000000 python-lsp-server-1.7.3/.github/workflows/test-win.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1319 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/.gitignore
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2717 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/.policy.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      445 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/.pylintrc
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    38440 2023-05-15 11:35:17.000000 python-lsp-server-1.7.3/CHANGELOG.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8858 2022-12-29 15:51:51.000000 python-lsp-server-1.7.3/CONFIGURATION.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1147 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      128 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/MANIFEST.in
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8718 2023-05-15 11:38:25.877593 python-lsp-server-1.7.3/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8094 2023-05-15 11:24:53.000000 python-lsp-server-1.7.3/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      762 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/RELEASE.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.853594 python-lsp-server-1.7.3/docs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1052 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/docs/autoimport.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.857594 python-lsp-server-1.7.3/pylsp/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      760 2022-12-26 17:45:43.000000 python-lsp-server-1.7.3/pylsp/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3874 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/__main__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9545 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/_utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       22 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/pylsp/_version.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.857594 python-lsp-server-1.7.3/pylsp/config/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/config/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6355 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/config/config.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2248 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/config/flake8_conf.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1268 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/config/pycodestyle_conf.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    13742 2022-12-29 15:51:51.000000 python-lsp-server-1.7.3/pylsp/config/schema.json
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2729 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/config/source.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2308 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/hookspecs.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1421 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/lsp.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.865594 python-lsp-server-1.7.3/pylsp/plugins/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/plugins/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4415 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/_resolvers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2756 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/_rope_task_handle.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/plugins/autopep8_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1345 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/plugins/definition.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7478 2022-12-18 03:24:12.000000 python-lsp-server-1.7.3/pylsp/plugins/flake8_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7050 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/plugins/folding.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      995 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/plugins/highlight.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1643 2022-12-29 19:03:44.000000 python-lsp-server-1.7.3/pylsp/plugins/hover.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10150 2023-03-18 18:10:05.000000 python-lsp-server-1.7.3/pylsp/plugins/jedi_completion.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1876 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/plugins/jedi_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/mccabe_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1395 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/plugins/preload_imports.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3945 2022-12-26 21:07:40.000000 python-lsp-server-1.7.3/pylsp/plugins/pycodestyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4291 2023-03-18 18:10:05.000000 python-lsp-server-1.7.3/pylsp/plugins/pydocstyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2752 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/pyflakes_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    12120 2023-05-15 11:24:53.000000 python-lsp-server-1.7.3/pylsp/plugins/pylint_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      961 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/plugins/references.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8306 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/rope_autoimport.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5979 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/rope_completion.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1899 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/plugins/rope_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2503 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/plugins/signature.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8168 2022-12-29 15:51:51.000000 python-lsp-server-1.7.3/pylsp/plugins/symbols.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6943 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/plugins/yapf_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    23223 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/python_lsp.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/pylsp/text_edit.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3725 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/pylsp/uris.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    15297 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/pylsp/workspace.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3109 2023-05-15 11:24:53.000000 python-lsp-server-1.7.3/pyproject.toml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.865594 python-lsp-server-1.7.3/python_lsp_server.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8718 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/python_lsp_server.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2504 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/python_lsp_server.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/python_lsp_server.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      900 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/python_lsp_server.egg-info/entry_points.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      748 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/python_lsp_server.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2023-05-15 11:38:25.000000 python-lsp-server-1.7.3/python_lsp_server.egg-info/top_level.txt
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.865594 python-lsp-server-1.7.3/scripts/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.865594 python-lsp-server-1.7.3/scripts/circle/
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)      464 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/scripts/circle/pypi.sh
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2562 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/scripts/jsonschema2md.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      155 2023-05-15 11:38:25.877593 python-lsp-server-1.7.3/setup.cfg
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)      298 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.869593 python-lsp-server-1.7.3/test/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      275 2022-12-26 17:14:29.000000 python-lsp-server-1.7.3/test/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      292 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/conftest.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4794 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/test/fixtures.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-15 11:38:25.877593 python-lsp-server-1.7.3/test/plugins/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2019-06-21 09:28:02.000000 python-lsp-server-1.7.3/test/plugins/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8201 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_autoimport.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2067 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_autopep8_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    19813 2023-03-18 18:10:05.000000 python-lsp-server-1.7.3/test/plugins/test_completion.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3147 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/test/plugins/test_definitions.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7705 2022-12-18 03:24:12.000000 python-lsp-server-1.7.3/test/plugins/test_flake8_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4922 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/plugins/test_folding.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1566 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/plugins/test_highlight.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3072 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_hover.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2573 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/plugins/test_jedi_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1253 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_mccabe_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4730 2022-12-26 21:07:40.000000 python-lsp-server-1.7.3/test/plugins/test_pycodestyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1769 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_pydocstyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1877 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_pyflakes_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4934 2022-12-29 15:51:51.000000 python-lsp-server-1.7.3/test/plugins/test_pylint_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2453 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/test/plugins/test_references.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1388 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/plugins/test_rope_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2656 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_signature.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3249 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/plugins/test_symbols.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3375 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/test/plugins/test_yapf_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3032 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/test_document.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4260 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/test_language_server.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8363 2022-12-11 17:32:03.000000 python-lsp-server-1.7.3/test/test_text_edit.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/test_uris.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2022-10-31 15:56:57.000000 python-lsp-server-1.7.3/test/test_utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14473 2023-04-03 01:06:12.000000 python-lsp-server-1.7.3/test/test_workspace.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.935712 python-lsp-server-1.7.4/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/.coveragerc
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/.gitattributes
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.899705 python-lsp-server-1.7.4/.github/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.903705 python-lsp-server-1.7.4/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1228 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/.github/workflows/release.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1386 2022-12-26 21:07:40.000000 python-lsp-server-1.7.4/.github/workflows/static.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1433 2022-12-26 21:07:40.000000 python-lsp-server-1.7.4/.github/workflows/test-linux.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1434 2022-12-26 21:07:40.000000 python-lsp-server-1.7.4/.github/workflows/test-mac.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1129 2022-12-26 21:07:40.000000 python-lsp-server-1.7.4/.github/workflows/test-win.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1319 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2717 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/.policy.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      445 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/.pylintrc
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    39212 2023-06-29 17:09:22.000000 python-lsp-server-1.7.4/CHANGELOG.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8858 2022-12-29 15:51:51.000000 python-lsp-server-1.7.4/CONFIGURATION.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1147 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      128 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/MANIFEST.in
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8718 2023-06-29 17:12:25.935712 python-lsp-server-1.7.4/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8094 2023-05-15 11:24:53.000000 python-lsp-server-1.7.4/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      762 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/RELEASE.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.903705 python-lsp-server-1.7.4/docs/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1052 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/docs/autoimport.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.907706 python-lsp-server-1.7.4/pylsp/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      760 2022-12-26 17:45:43.000000 python-lsp-server-1.7.4/pylsp/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3874 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/__main__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9545 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/_utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       22 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/pylsp/_version.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.911707 python-lsp-server-1.7.4/pylsp/config/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/config/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6355 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/config/config.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2248 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/config/flake8_conf.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1268 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/config/pycodestyle_conf.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13742 2022-12-29 15:51:51.000000 python-lsp-server-1.7.4/pylsp/config/schema.json
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2729 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/config/source.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2308 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/hookspecs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1421 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/lsp.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.923709 python-lsp-server-1.7.4/pylsp/plugins/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/plugins/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4415 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/plugins/_resolvers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2810 2023-06-29 16:58:38.000000 python-lsp-server-1.7.4/pylsp/plugins/_rope_task_handle.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/plugins/autopep8_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1345 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/plugins/definition.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7478 2022-12-18 03:24:12.000000 python-lsp-server-1.7.4/pylsp/plugins/flake8_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7050 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/plugins/folding.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      995 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/plugins/highlight.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1643 2022-12-29 19:03:44.000000 python-lsp-server-1.7.4/pylsp/plugins/hover.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10150 2023-03-18 18:10:05.000000 python-lsp-server-1.7.4/pylsp/plugins/jedi_completion.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1876 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/plugins/jedi_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/plugins/mccabe_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1395 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/plugins/preload_imports.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3945 2022-12-26 21:07:40.000000 python-lsp-server-1.7.4/pylsp/plugins/pycodestyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4291 2023-03-18 18:10:05.000000 python-lsp-server-1.7.4/pylsp/plugins/pydocstyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2752 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/plugins/pyflakes_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12058 2023-06-29 16:58:38.000000 python-lsp-server-1.7.4/pylsp/plugins/pylint_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      961 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/plugins/references.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8306 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/plugins/rope_autoimport.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5979 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/plugins/rope_completion.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1899 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/plugins/rope_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2503 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/plugins/signature.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8168 2022-12-29 15:51:51.000000 python-lsp-server-1.7.4/pylsp/plugins/symbols.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6943 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/plugins/yapf_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    23223 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/pylsp/python_lsp.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/pylsp/text_edit.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3725 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/pylsp/uris.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    16407 2023-06-29 16:58:38.000000 python-lsp-server-1.7.4/pylsp/workspace.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3109 2023-05-15 11:24:53.000000 python-lsp-server-1.7.4/pyproject.toml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.923709 python-lsp-server-1.7.4/python_lsp_server.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8718 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/python_lsp_server.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2504 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/python_lsp_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/python_lsp_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      900 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/python_lsp_server.egg-info/entry_points.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      748 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/python_lsp_server.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2023-06-29 17:12:25.000000 python-lsp-server-1.7.4/python_lsp_server.egg-info/top_level.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.923709 python-lsp-server-1.7.4/scripts/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.923709 python-lsp-server-1.7.4/scripts/circle/
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      464 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/scripts/circle/pypi.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2562 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/scripts/jsonschema2md.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      155 2023-06-29 17:12:25.935712 python-lsp-server-1.7.4/setup.cfg
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      298 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.927710 python-lsp-server-1.7.4/test/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      275 2022-12-26 17:14:29.000000 python-lsp-server-1.7.4/test/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      292 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/conftest.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4794 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/test/fixtures.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-29 17:12:25.935712 python-lsp-server-1.7.4/test/plugins/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2019-06-21 09:28:02.000000 python-lsp-server-1.7.4/test/plugins/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8201 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_autoimport.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2067 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_autopep8_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    19813 2023-03-18 18:10:05.000000 python-lsp-server-1.7.4/test/plugins/test_completion.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3147 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/test/plugins/test_definitions.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7705 2022-12-18 03:24:12.000000 python-lsp-server-1.7.4/test/plugins/test_flake8_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4922 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/plugins/test_folding.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1566 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/plugins/test_highlight.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3072 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_hover.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2573 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/plugins/test_jedi_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1253 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_mccabe_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4730 2022-12-26 21:07:40.000000 python-lsp-server-1.7.4/test/plugins/test_pycodestyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1769 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_pydocstyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1877 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_pyflakes_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4934 2022-12-29 15:51:51.000000 python-lsp-server-1.7.4/test/plugins/test_pylint_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2453 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/test/plugins/test_references.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1388 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/plugins/test_rope_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2656 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_signature.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3249 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/plugins/test_symbols.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3375 2023-04-03 01:06:12.000000 python-lsp-server-1.7.4/test/plugins/test_yapf_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3032 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/test_document.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4260 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/test_language_server.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8363 2022-12-11 17:32:03.000000 python-lsp-server-1.7.4/test/test_text_edit.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/test_uris.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2022-10-31 15:56:57.000000 python-lsp-server-1.7.4/test/test_utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    14767 2023-06-29 16:58:38.000000 python-lsp-server-1.7.4/test/test_workspace.py
```

### Comparing `python-lsp-server-1.7.3/.github/workflows/release.yml` & `python-lsp-server-1.7.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/.github/workflows/static.yml` & `python-lsp-server-1.7.4/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/.github/workflows/test-linux.yml` & `python-lsp-server-1.7.4/.github/workflows/test-linux.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/.github/workflows/test-mac.yml` & `python-lsp-server-1.7.4/.github/workflows/test-mac.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/.github/workflows/test-win.yml` & `python-lsp-server-1.7.4/.github/workflows/test-win.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/.gitignore` & `python-lsp-server-1.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/.policy.yml` & `python-lsp-server-1.7.4/.policy.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/CHANGELOG.md` & `python-lsp-server-1.7.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # History of changes
 
+## Version 1.7.4 (2023/06/29)
+
+### Issues Closed
+
+* [Issue 393](https://github.com/python-lsp/python-lsp-server/issues/393) - Environment path doesn't expand user directory
+
+In this release 1 issue was closed.
+
+### Pull Requests Merged
+
+* [PR 394](https://github.com/python-lsp/python-lsp-server/pull/394) - Resolve homedir references in Jedi environment path, by [@odiroot](https://github.com/odiroot)
+* [PR 381](https://github.com/python-lsp/python-lsp-server/pull/381) - Report progress even when initialization fails, by [@syphar](https://github.com/syphar)
+* [PR 380](https://github.com/python-lsp/python-lsp-server/pull/380) - Fix pylint hang on file with many errors, by [@hetmankp](https://github.com/hetmankp)
+
+In this release 3 pull requests were closed.
+
+----
+
 ## Version 1.7.3 (2023/05/15)
 
 ### Issues Closed
 
 * [Issue 369](https://github.com/python-lsp/python-lsp-server/issues/369) - Failed to load hook pylsp_lint: [Errno 2] No such file or directory: '' ([PR 371](https://github.com/python-lsp/python-lsp-server/pull/371) by [@Ultimator14](https://github.com/Ultimator14))
 
 In this release 1 issue was closed.
```

### Comparing `python-lsp-server-1.7.3/CONFIGURATION.md` & `python-lsp-server-1.7.4/CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/LICENSE` & `python-lsp-server-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/PKG-INFO` & `python-lsp-server-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-server
-Version: 1.7.3
+Version: 1.7.4
 Summary: Python Language Server for the Language Server Protocol
 Author: Python Language Server Contributors
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-server
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `python-lsp-server-1.7.3/README.md` & `python-lsp-server-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/RELEASE.md` & `python-lsp-server-1.7.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/docs/autoimport.md` & `python-lsp-server-1.7.4/docs/autoimport.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/__init__.py` & `python-lsp-server-1.7.4/pylsp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/__main__.py` & `python-lsp-server-1.7.4/pylsp/__main__.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/_utils.py` & `python-lsp-server-1.7.4/pylsp/_utils.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/config/config.py` & `python-lsp-server-1.7.4/pylsp/config/config.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/config/flake8_conf.py` & `python-lsp-server-1.7.4/pylsp/config/flake8_conf.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/config/pycodestyle_conf.py` & `python-lsp-server-1.7.4/pylsp/config/pycodestyle_conf.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/config/schema.json` & `python-lsp-server-1.7.4/pylsp/config/schema.json`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/config/source.py` & `python-lsp-server-1.7.4/pylsp/config/source.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/hookspecs.py` & `python-lsp-server-1.7.4/pylsp/hookspecs.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/lsp.py` & `python-lsp-server-1.7.4/pylsp/lsp.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/_resolvers.py` & `python-lsp-server-1.7.4/pylsp/plugins/_resolvers.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/_rope_task_handle.py` & `python-lsp-server-1.7.4/pylsp/plugins/_rope_task_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,17 @@
 
     def __init__(self, workspace: Workspace):
         self.workspace = workspace
         self.job_sets = []
         self.observers = []
 
     def create_jobset(self, name="JobSet", count: Optional[int] = None):
-        report_iter = self.workspace.report_progress(name, None, None)
+        report_iter = self.workspace.report_progress(
+            name, None, None, skip_token_initialization=True
+        )
         result = PylspJobSet(count, report_iter)
         self.job_sets.append(result)
         self._inform_observers()
         return result
 
     def stop(self) -> None:
         pass
```

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/autopep8_format.py` & `python-lsp-server-1.7.4/pylsp/plugins/autopep8_format.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/definition.py` & `python-lsp-server-1.7.4/pylsp/plugins/definition.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/flake8_lint.py` & `python-lsp-server-1.7.4/pylsp/plugins/flake8_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/folding.py` & `python-lsp-server-1.7.4/pylsp/plugins/folding.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/highlight.py` & `python-lsp-server-1.7.4/pylsp/plugins/highlight.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/hover.py` & `python-lsp-server-1.7.4/pylsp/plugins/hover.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/jedi_completion.py` & `python-lsp-server-1.7.4/pylsp/plugins/jedi_completion.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/jedi_rename.py` & `python-lsp-server-1.7.4/pylsp/plugins/jedi_rename.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/mccabe_lint.py` & `python-lsp-server-1.7.4/pylsp/plugins/mccabe_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/preload_imports.py` & `python-lsp-server-1.7.4/pylsp/plugins/preload_imports.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/pycodestyle_lint.py` & `python-lsp-server-1.7.4/pylsp/plugins/pycodestyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/pydocstyle_lint.py` & `python-lsp-server-1.7.4/pylsp/plugins/pydocstyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/pyflakes_lint.py` & `python-lsp-server-1.7.4/pylsp/plugins/pyflakes_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/pylint_lint.py` & `python-lsp-server-1.7.4/pylsp/plugins/pylint_lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,15 @@
 
         cwd = document._workspace.root_path
         if not cwd:
             cwd = os.path.dirname(__file__)
 
         with Popen(cmd, stdout=PIPE, stderr=PIPE,
                    cwd=cwd, universal_newlines=True) as process:
-            process.wait()
-            json_out = process.stdout.read()
-            err = process.stderr.read()
+            json_out, err = process.communicate()
 
         if err != '':
             log.error("Error calling pylint: '%s'", err)
 
         # pylint prints nothing rather than [] when there are no diagnostics.
         # json.loads will not parse an empty string, so just return.
         if not json_out.strip():
```

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/references.py` & `python-lsp-server-1.7.4/pylsp/plugins/references.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/rope_autoimport.py` & `python-lsp-server-1.7.4/pylsp/plugins/rope_autoimport.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/rope_completion.py` & `python-lsp-server-1.7.4/pylsp/plugins/rope_completion.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/rope_rename.py` & `python-lsp-server-1.7.4/pylsp/plugins/rope_rename.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/signature.py` & `python-lsp-server-1.7.4/pylsp/plugins/signature.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/symbols.py` & `python-lsp-server-1.7.4/pylsp/plugins/symbols.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/plugins/yapf_format.py` & `python-lsp-server-1.7.4/pylsp/plugins/yapf_format.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/python_lsp.py` & `python-lsp-server-1.7.4/pylsp/python_lsp.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/text_edit.py` & `python-lsp-server-1.7.4/pylsp/text_edit.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/uris.py` & `python-lsp-server-1.7.4/pylsp/uris.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/pylsp/workspace.py` & `python-lsp-server-1.7.4/pylsp/workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -131,62 +131,79 @@
 
     @contextmanager
     def report_progress(
         self,
         title: str,
         message: Optional[str] = None,
         percentage: Optional[int] = None,
+        skip_token_initialization: bool = False,
     ) -> Generator[Callable[[str, Optional[int]], None], None, None]:
+        """
+        Report progress to the editor / client.
+
+        ``skip_token_initialization` is necessary due to some current
+        limitations of our LSP implementation. When `report_progress`
+        is used from a synchronous LSP handler, the token initialization
+        will time out because we can't receive the response.
+
+        Many editors will still correctly show the progress messages though, which
+        is why we are giving progress users the option to skip the initialization
+        of the progress token.
+        """
         if self._config:
             client_supports_progress_reporting = (
                 self._config.capabilities.get("window", {}).get("workDoneProgress", False)
             )
         else:
             client_supports_progress_reporting = False
 
         if client_supports_progress_reporting:
-            try:
-                token = self._progress_begin(title, message, percentage)
-            except Exception:  # pylint: disable=broad-exception-caught
-                log.warning(
-                    "There was an error while trying to initialize progress reporting."
-                    "Likely progress reporting was used in a synchronous LSP handler, "
-                    "which is not supported by progress reporting yet.",
-                    exc_info=True
-                )
+            token = self._progress_begin(title, message, percentage, skip_token_initialization)
 
-            else:
-                def progress_message(message: str, percentage: Optional[int] = None) -> None:
-                    self._progress_report(token, message, percentage)
-
-                try:
-                    yield progress_message
-                finally:
-                    self._progress_end(token)
+            def progress_message(message: str, percentage: Optional[int] = None) -> None:
+                self._progress_report(token, message, percentage)
 
-                return
+            try:
+                yield progress_message
+            finally:
+                self._progress_end(token)
+
+            return
 
         # FALLBACK:
-        # If the client doesn't support progress reporting, or if we failed to
-        # initialize it, we have a dummy method for the caller to use.
+        # If the client doesn't support progress reporting, we have a dummy method
+        # for the caller to use.
         def dummy_progress_message(message: str, percentage: Optional[int] = None) -> None:
             # pylint: disable=unused-argument
             pass
 
         yield dummy_progress_message
 
     def _progress_begin(
         self,
         title: str,
         message: Optional[str] = None,
         percentage: Optional[int] = None,
+        skip_token_initialization: bool = False,
     ) -> str:
         token = str(uuid.uuid4())
 
-        self._endpoint.request(self.M_INITIALIZE_PROGRESS, {'token': token}).result(timeout=1.0)
+        if not skip_token_initialization:
+            try:
+                self._endpoint.request(self.M_INITIALIZE_PROGRESS, {'token': token}).result(timeout=1.0)
+            except Exception:  # pylint: disable=broad-exception-caught
+                log.warning(
+                    "There was an error while trying to initialize progress reporting."
+                    "Likely progress reporting was used in a synchronous LSP handler, "
+                    "which is not supported by progress reporting yet. "
+                    "To prevent waiting for the timeout you can set "
+                    "`skip_token_initialization=True`. "
+                    "Not every editor will show progress then, but many will.",
+                    exc_info=True
+                )
 
         value = {
             "kind": "begin",
             "title": title,
         }
         if message is not None:
             value["message"] = message
@@ -385,14 +402,19 @@
         env_vars = None
 
         if self._config:
             jedi_settings = self._config.plugin_settings('jedi', document_path=self.path)
             jedi.settings.auto_import_modules = jedi_settings.get('auto_import_modules',
                                                                   DEFAULT_AUTO_IMPORT_MODULES)
             environment_path = jedi_settings.get('environment')
+            # Jedi itself cannot deal with homedir-relative paths.
+            # On systems, where it is expected, expand the home directory.
+            if environment_path and os.name != 'nt':
+                environment_path = os.path.expanduser(environment_path)
+
             extra_paths = jedi_settings.get('extra_paths') or []
             env_vars = jedi_settings.get('env_vars')
 
         # Drop PYTHONPATH from env_vars before creating the environment because that makes
         # Jedi throw an error.
         if env_vars is None:
             env_vars = os.environ.copy()
```

### Comparing `python-lsp-server-1.7.3/pyproject.toml` & `python-lsp-server-1.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/python_lsp_server.egg-info/PKG-INFO` & `python-lsp-server-1.7.4/python_lsp_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-server
-Version: 1.7.3
+Version: 1.7.4
 Summary: Python Language Server for the Language Server Protocol
 Author: Python Language Server Contributors
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-server
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `python-lsp-server-1.7.3/python_lsp_server.egg-info/SOURCES.txt` & `python-lsp-server-1.7.4/python_lsp_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/python_lsp_server.egg-info/entry_points.txt` & `python-lsp-server-1.7.4/python_lsp_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/python_lsp_server.egg-info/requires.txt` & `python-lsp-server-1.7.4/python_lsp_server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/scripts/jsonschema2md.py` & `python-lsp-server-1.7.4/scripts/jsonschema2md.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/fixtures.py` & `python-lsp-server-1.7.4/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_autoimport.py` & `python-lsp-server-1.7.4/test/plugins/test_autoimport.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_autopep8_format.py` & `python-lsp-server-1.7.4/test/plugins/test_autopep8_format.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_completion.py` & `python-lsp-server-1.7.4/test/plugins/test_completion.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_definitions.py` & `python-lsp-server-1.7.4/test/plugins/test_definitions.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_flake8_lint.py` & `python-lsp-server-1.7.4/test/plugins/test_flake8_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_folding.py` & `python-lsp-server-1.7.4/test/plugins/test_folding.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_highlight.py` & `python-lsp-server-1.7.4/test/plugins/test_highlight.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_hover.py` & `python-lsp-server-1.7.4/test/plugins/test_hover.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_jedi_rename.py` & `python-lsp-server-1.7.4/test/plugins/test_jedi_rename.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_mccabe_lint.py` & `python-lsp-server-1.7.4/test/plugins/test_mccabe_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_pycodestyle_lint.py` & `python-lsp-server-1.7.4/test/plugins/test_pycodestyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_pydocstyle_lint.py` & `python-lsp-server-1.7.4/test/plugins/test_pydocstyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_pyflakes_lint.py` & `python-lsp-server-1.7.4/test/plugins/test_pyflakes_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_pylint_lint.py` & `python-lsp-server-1.7.4/test/plugins/test_pylint_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_references.py` & `python-lsp-server-1.7.4/test/plugins/test_references.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_rope_rename.py` & `python-lsp-server-1.7.4/test/plugins/test_rope_rename.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_signature.py` & `python-lsp-server-1.7.4/test/plugins/test_signature.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_symbols.py` & `python-lsp-server-1.7.4/test/plugins/test_symbols.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/plugins/test_yapf_format.py` & `python-lsp-server-1.7.4/test/plugins/test_yapf_format.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/test_document.py` & `python-lsp-server-1.7.4/test/test_document.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/test_language_server.py` & `python-lsp-server-1.7.4/test/test_language_server.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/test_text_edit.py` & `python-lsp-server-1.7.4/test/test_text_edit.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/test_uris.py` & `python-lsp-server-1.7.4/test/test_uris.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/test_utils.py` & `python-lsp-server-1.7.4/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.3/test/test_workspace.py` & `python-lsp-server-1.7.4/test/test_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,27 +323,32 @@
     assert [call[0][0]["params"]["value"] for call in progress_calls] == [
         {"kind": "begin", "title": "some_title"},
         {"kind": "end"},
     ]
 
 
 @pytest.mark.parametrize("exc", [Exception("something"), TimeoutError()])
-def test_progress_initialization_fails(workspace, consumer, endpoint, exc):
+def test_progress_initialization_fails_but_is_skipped(workspace, consumer, endpoint, exc):
     def failing_token_initialization(self, *_args, **_kwargs):
         raise exc
     endpoint._dispatcher.m_window__work_done_progress__create = failing_token_initialization
 
     workspace._config.capabilities['window'] = {"workDoneProgress": True}
 
-    with workspace.report_progress("some_title"):
+    with workspace.report_progress("some_title", skip_token_initialization=True):
         pass
 
     # we only see the failing token initialization call, no other calls
-    init_call, = consumer.call_args_list
-    assert init_call[0][0]['method'] == 'window/workDoneProgress/create'
+    progress_calls = consumer.call_args_list
+    assert all(call[0][0]["method"] == "$/progress" for call in progress_calls)
+    assert len({call[0][0]["params"]["token"] for call in progress_calls}) == 1
+    assert [call[0][0]["params"]["value"] for call in progress_calls] == [
+        {"kind": "begin", "title": "some_title"},
+        {"kind": "end"},
+    ]
 
 
 def test_progress_with_percent(workspace, consumer):
     workspace._config.capabilities['window'] = {"workDoneProgress": True}
 
     with workspace.report_progress(
         "some_title", "initial message", percentage=1
```

