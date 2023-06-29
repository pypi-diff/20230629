# Comparing `tmp/kiara_plugin.onboarding-0.4.5.tar.gz` & `tmp/kiara_plugin.onboarding-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.onboarding-0.4.5.tar", last modified: Tue Jun 27 10:09:28 2023, max compression
+gzip compressed data, was "kiara_plugin.onboarding-0.4.6.tar", last modified: Thu Jun 29 08:31:55 2023, max compression
```

## Comparing `kiara_plugin.onboarding-0.4.5.tar` & `kiara_plugin.onboarding-0.4.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml.rej
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/ci/conda/kiara_plugin.onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/ci/conda/kiara_plugin.onboarding/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/pipelines/example_pipeline_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/models/
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:08:54.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml.rej
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/ci/conda/kiara_plugin.onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/ci/conda/kiara_plugin.onboarding/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/examples/pipelines/example_pipeline_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.458628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.462628 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:31:21.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:31:55.000000 kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:55.466628 kiara_plugin.onboarding-0.4.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-06-29 08:31:07.000000 kiara_plugin.onboarding-0.4.6/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.onboarding-0.4.5/.cruft.json` & `kiara_plugin.onboarding-0.4.6/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.onboarding-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.github/workflows/build-darwin.yaml` & `kiara_plugin.onboarding-0.4.6/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml` & `kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml.rej` & `kiara_plugin.onboarding-0.4.6/.github/workflows/build-linux.yaml.rej`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.github/workflows/build-windows.yaml` & `kiara_plugin.onboarding-0.4.6/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.gitignore` & `kiara_plugin.onboarding-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/.pre-commit-config.yaml` & `kiara_plugin.onboarding-0.4.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/LICENSE` & `kiara_plugin.onboarding-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/Makefile` & `kiara_plugin.onboarding-0.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/PKG-INFO` & `kiara_plugin.onboarding-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.onboarding
-Version: 0.4.5
+Version: 0.4.6
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.5/README.md` & `kiara_plugin.onboarding-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/ci/conda/kiara_plugin.onboarding/meta.yaml.template` & `kiara_plugin.onboarding-0.4.6/ci/conda/kiara_plugin.onboarding/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/docs/development.md` & `kiara_plugin.onboarding-0.4.6/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/docs/index.md` & `kiara_plugin.onboarding-0.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.onboarding-0.4.6/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/examples/pipelines/example_pipeline_onboarding.yaml` & `kiara_plugin.onboarding-0.4.6/examples/pipelines/example_pipeline_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/mkdocs.yml` & `kiara_plugin.onboarding-0.4.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/pyproject.toml` & `kiara_plugin.onboarding-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_info_pages.py` & `kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_module_doc.py` & `kiara_plugin.onboarding-0.4.6/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/setup.cfg` & `kiara_plugin.onboarding-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/setup.py` & `kiara_plugin.onboarding-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/__init__.py` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/models/__init__.py` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,18 @@
         else:
             sub_path = tokens[3]
 
         url = f"https://github.com/{tokens[0]}/{tokens[1]}/archive/refs/heads/{tokens[2]}.zip"
 
         archive_zip: KiaraFile
         archive_zip = download_file(  # type: ignore
-            url=url, attach_metadata=attach_metadata, return_md5_hash=False
+            url=url,
+            attach_metadata=attach_metadata,
+            file_name=f"{tokens[1]}-{tokens[2]}.zip",
+            return_md5_hash=False,
         )
 
         base_sub_path = f"{tokens[1]}-{tokens[2]}"
 
         if sub_path:
             if import_config.sub_path:
                 new_sub_path = "/".join([base_sub_path, sub_path, import_config.sub_path])  # type: ignore
```

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file.py` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/zenodo.py` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin/onboarding/modules/zenodo.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/PKG-INFO` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.onboarding
-Version: 0.4.5
+Version: 0.4.6
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/SOURCES.txt` & `kiara_plugin.onboarding-0.4.6/src/kiara_plugin.onboarding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/tests/conftest.py` & `kiara_plugin.onboarding-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.5/tests/test_job_descs.py` & `kiara_plugin.onboarding-0.4.6/tests/test_job_descs.py`

 * *Files identical despite different names*

