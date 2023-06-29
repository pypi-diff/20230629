# Comparing `tmp/kiara_plugin.develop-0.4.0.tar.gz` & `tmp/kiara_plugin.develop-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.develop-0.4.0.tar", last modified: Wed Jun 14 14:32:15 2023, max compression
+gzip compressed data, was "kiara_plugin.develop-0.4.1.tar", last modified: Thu Jun 29 08:58:28 2023, max compression
```

## Comparing `kiara_plugin.develop-0.4.0.tar` & `kiara_plugin.develop-0.4.1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/ci/conda/kiara_plugin.develop/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/ci/conda/kiara_plugin.develop/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/commitlint.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/docs/development/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/docs/development/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/development/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/development/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/packaging.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/docs/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.774965 kiara_plugin.develop-0.4.0/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/examples/pipelines/example_pipeline_develop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_models.fbs
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_models.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/example_job_{{ cookiecutter.project_slug }}.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.778965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/scripts/development/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/scripts/development/install_dev_env.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.770965 kiara_plugin.develop-0.4.0/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/
--rw-r--r--   0 runner    (1001) docker     (123)    19782 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7807 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/flatbuffers/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/meta.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/flatbuffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/javascript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.782965 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 14:32:15.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-14 14:32:15.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:32:15.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 14:32:15.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:31:49.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-14 14:32:15.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 14:32:15.000000 kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:32:15.786965 kiara_plugin.develop-0.4.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-14 14:31:38.000000 kiara_plugin.develop-0.4.0/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.216245 kiara_plugin.develop-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-29 08:58:28.216245 kiara_plugin.develop-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/commitlint.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/development/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/development/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/development/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/development/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/packaging.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/pipelines/example_pipeline_develop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_models.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_models.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/example_job_{{ cookiecutter.project_slug }}.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/scripts/development/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/development/install_dev_env.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-29 08:58:28.216245 kiara_plugin.develop-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)    19782 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7807 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/flatbuffers/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/meta.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/flatbuffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:57:37.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.develop-0.4.0/.cruft.json` & `kiara_plugin.develop-0.4.1/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'f30a92644095dd13556ab071b97d20008badaed3'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "878ca1dc79be3cd9dd7e4ee9edfa2e5d0789aad7",
+    "commit": "f30a92644095dd13556ab071b97d20008badaed3",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.develop-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/.github/workflows/build-darwin.yaml` & `kiara_plugin.develop-0.4.1/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/.github/workflows/build-linux.yaml` & `kiara_plugin.develop-0.4.1/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/.github/workflows/build-windows.yaml` & `kiara_plugin.develop-0.4.1/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/.gitignore` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
 pip-wheel-metadata/
 .python-version
-src/kiara_plugin/develop/version.txt
+src/kiara_plugin/{{ cookiecutter.project_slug }}/version.txt
 .direnv
 public
 site
 .dephell_report
 .direnv
 .mypy_cache
 .env
 docs/api-documentation.md
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
-ci/conda/kiara_plugin.develop/
+ci/conda/kiara_plugin.{{ cookiecutter.project_slug }}/meta.yaml
```

### Comparing `kiara_plugin.develop-0.4.0/.pre-commit-config.yaml` & `kiara_plugin.develop-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/LICENSE` & `kiara_plugin.develop-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/Makefile` & `kiara_plugin.develop-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/PKG-INFO` & `kiara_plugin.develop-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.develop
-Version: 0.4.0
+Version: 0.4.1
 Summary: Development utilities for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.develop
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.develop
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.develop
 Keywords: kiara
```

### Comparing `kiara_plugin.develop-0.4.0/README.md` & `kiara_plugin.develop-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/docs/development/core/index.md` & `kiara_plugin.develop-0.4.1/docs/development/core/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/docs/development/index.md` & `kiara_plugin.develop-0.4.1/docs/development/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/docs/index.md` & `kiara_plugin.develop-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/docs/packaging.md` & `kiara_plugin.develop-0.4.1/docs/packaging.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/docs/usage/index.md` & `kiara_plugin.develop-0.4.1/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.develop-0.4.1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.develop-0.4.1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/examples/pipelines/example_pipeline_develop.yaml` & `kiara_plugin.develop-0.4.1/examples/pipelines/example_pipeline_develop.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_models.ts` & `kiara_plugin.develop-0.4.1/kiara_models.ts`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore` & `kiara_plugin.develop-0.4.1/.gitignore`

 * *Files 24% similar despite different names*

```diff
@@ -43,23 +43,24 @@
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
 pip-wheel-metadata/
 .python-version
-src/kiara_plugin/{{ cookiecutter.project_slug }}/version.txt
+src/kiara_plugin/develop/version.txt
 .direnv
 public
 site
 .dephell_report
 .direnv
 .mypy_cache
 .env
 docs/api-documentation.md
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
-ci/conda/kiara_plugin.{{ cookiecutter.project_slug }}/meta.yaml
+ci/conda/kiara_plugin.develop/
+dev.py
```

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/README.md` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py` & `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/mkdocs.yml` & `kiara_plugin.develop-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/output.txt` & `kiara_plugin.develop-0.4.1/output.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/pyproject.toml` & `kiara_plugin.develop-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara_plugin.core_types>=0.4.17",
+    "kiara>=0.4.44",
+    "kiara_plugin.core_types>=0.4.20",
+    "kiara_plugin.tabular>=0.4.28",
+    "kiara_plugin.onboarding>=0.4.5",
     "diskcache>=5.4.0",
     "httpx>=0.23.0",
     "pydantic-to-typescript>=1.0.9"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

### Comparing `kiara_plugin.develop-0.4.0/scripts/development/install_dev_env.sh` & `kiara_plugin.develop-0.4.1/scripts/development/install_dev_env.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.develop-0.4.1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/scripts/documentation/gen_info_pages.py` & `kiara_plugin.develop-0.4.1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/scripts/documentation/gen_module_doc.py` & `kiara_plugin.develop-0.4.1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/setup.cfg` & `kiara_plugin.develop-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/setup.py` & `kiara_plugin.develop-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/__init__.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/__init__.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/models.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/conda/states.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/states.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/defaults.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/conda.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/conda.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/debug.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/debug.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/interfaces/cli/dev.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/dev.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/models.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/meta.yaml.j2` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/meta.yaml.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/__init__.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/flatbuffers.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/flatbuffers.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/schema/javascript.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/javascript.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin/develop/utils.py` & `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/utils.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/PKG-INFO` & `kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.develop
-Version: 0.4.0
+Version: 0.4.1
 Summary: Development utilities for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.develop
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.develop
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.develop
 Keywords: kiara
```

### Comparing `kiara_plugin.develop-0.4.0/src/kiara_plugin.develop.egg-info/SOURCES.txt` & `kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
 .github/workflows/build-darwin.yaml
 .github/workflows/build-linux.yaml
 .github/workflows/build-windows.yaml
 ci/conda/conda-pkg-patch.yaml
-ci/conda/kiara_plugin.develop/meta.yaml.template
 docs/SUMMARY.md
 docs/index.md
 docs/packaging.md
 docs/development/index.md
 docs/development/core/index.md
 docs/stylesheets/extra.css
 docs/usage/index.md
@@ -115,14 +114,15 @@
 src/kiara_plugin/develop/conda/states.py
 src/kiara_plugin/develop/interfaces/__init__.py
 src/kiara_plugin/develop/interfaces/cli/__init__.py
 src/kiara_plugin/develop/interfaces/cli/conda.py
 src/kiara_plugin/develop/interfaces/cli/debug.py
 src/kiara_plugin/develop/interfaces/cli/dev.py
 src/kiara_plugin/develop/modules/__init__.py
+src/kiara_plugin/develop/modules/pipelines/__init__.py
 src/kiara_plugin/develop/pipelines/.gitkeep
 src/kiara_plugin/develop/pipelines/__init__.py
 src/kiara_plugin/develop/resources/.gitkeep
 src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
 src/kiara_plugin/develop/resources/templates/meta.yaml.j2
 src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
 src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
```

### Comparing `kiara_plugin.develop-0.4.0/tests/conftest.py` & `kiara_plugin.develop-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.0/tests/test_job_descs.py` & `kiara_plugin.develop-0.4.1/tests/test_job_descs.py`

 * *Files identical despite different names*

