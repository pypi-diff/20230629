# Comparing `tmp/kiara_plugin.service-0.4.1.tar.gz` & `tmp/kiara_plugin.service-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.service-0.4.1.tar", last modified: Fri Jun 16 07:21:04 2023, max compression
+gzip compressed data, was "kiara_plugin.service-0.4.2.tar", last modified: Thu Jun 29 08:36:25 2023, max compression
```

## Comparing `kiara_plugin.service-0.4.1.tar` & `kiara_plugin.service-0.4.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/ci/conda/kiara_plugin.service/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/ci/conda/kiara_plugin.service/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/pipelines/example_pipeline_service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/input.css
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/operation_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/operations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/value_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/value_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:20:37.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.691097 kiara_plugin.service-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.695097 kiara_plugin.service-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.691097 kiara_plugin.service-0.4.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/ci/conda/kiara_plugin.service/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/ci/conda/kiara_plugin.service/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.691097 kiara_plugin.service-0.4.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/examples/pipelines/example_pipeline_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.691097 kiara_plugin.service-0.4.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.699097 kiara_plugin.service-0.4.2/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.691097 kiara_plugin.service-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.691097 kiara_plugin.service-0.4.2/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/cli/service/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.707097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/operations/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/operations/operation_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/operations/operations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/value_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/value_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.703097 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-29 08:36:25.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-29 08:36:25.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:36:25.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-29 08:36:25.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:35:50.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-29 08:36:25.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:36:25.000000 kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:36:25.711097 kiara_plugin.service-0.4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-29 08:35:35.000000 kiara_plugin.service-0.4.2/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.service-0.4.1/.cruft.json` & `kiara_plugin.service-0.4.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.service-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.service-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.github/workflows/build-darwin.yaml` & `kiara_plugin.service-0.4.2/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.github/workflows/build-linux.yaml` & `kiara_plugin.service-0.4.2/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.github/workflows/build-windows.yaml` & `kiara_plugin.service-0.4.2/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.gitignore` & `kiara_plugin.service-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/.pre-commit-config.yaml` & `kiara_plugin.service-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/LICENSE` & `kiara_plugin.service-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/Makefile` & `kiara_plugin.service-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/PKG-INFO` & `kiara_plugin.service-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.service
-Version: 0.4.1
+Version: 0.4.2
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.1/README.md` & `kiara_plugin.service-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/ci/conda/kiara_plugin.service/meta.yaml.template` & `kiara_plugin.service-0.4.2/ci/conda/kiara_plugin.service/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/docs/development.md` & `kiara_plugin.service-0.4.2/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/docs/index.md` & `kiara_plugin.service-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.service-0.4.2/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.service-0.4.2/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/examples/pipelines/example_pipeline_service.yaml` & `kiara_plugin.service-0.4.2/examples/pipelines/example_pipeline_service.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/mkdocs.yml` & `kiara_plugin.service-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/pyproject.toml` & `kiara_plugin.service-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.41",
-    "kiara_plugin.core_types>=0.4.18",
+    "kiara>=0.4.44",
+    "kiara_plugin.core_types>=0.4.20",
     "starlite==1.39.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
```

### Comparing `kiara_plugin.service-0.4.1/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.service-0.4.2/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/scripts/documentation/gen_info_pages.py` & `kiara_plugin.service-0.4.2/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/scripts/documentation/gen_module_doc.py` & `kiara_plugin.service-0.4.2/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/setup.cfg` & `kiara_plugin.service-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/setup.py` & `kiara_plugin.service-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/__init__.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/defaults.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/commands.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/interfaces/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/models.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/modules/__init__.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/__init__.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/__init__.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/jobs.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/modules.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/modules.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/operations.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/operations.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/pipeline.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,14 @@
 
         print(f"PIPELINE: {pipeline}")
         pipeline_config = get_pipeline_config(pipeline=pipeline)
         info = PipelineStructureInfo.create_from_instance(
             kiara=kiara_api.context, instance=pipeline_config.structure
         )
         return info
+
+    @get(path="/list", api_func=get_pipeline_config)
+    async def list_pipelines(self, kiara_api: KiaraAPI) -> List[str]:
+
+        pipelines = kiara_api.list_operations(operation_types="pipeline")
+        print(pipelines)
+        return list(pipelines.keys())
```

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/render.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/render.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/values.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/values.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/workflows.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/service.py` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/openapi/service.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/favicon.ico` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/main.css` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/main.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/simple.css` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/static/simple.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/job_finished.html` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/jobs/job_finished.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/macros.html` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/macros.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html` & `kiara_plugin.service-0.4.2/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/PKG-INFO` & `kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.service
-Version: 0.4.1
+Version: 0.4.2
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/SOURCES.txt` & `kiara_plugin.service-0.4.2/src/kiara_plugin.service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/tests/conftest.py` & `kiara_plugin.service-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.1/tests/test_job_descs.py` & `kiara_plugin.service-0.4.2/tests/test_job_descs.py`

 * *Files identical despite different names*

