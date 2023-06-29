# Comparing `tmp/kiara_plugin.streamlit-0.4.3.tar.gz` & `tmp/kiara_plugin.streamlit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.streamlit-0.4.3.tar", last modified: Tue Jun 27 10:45:43 2023, max compression
+gzip compressed data, was "kiara_plugin.streamlit-0.4.4.tar", last modified: Thu Jun 29 08:57:58 2023, max compression
```

## Comparing `kiara_plugin.streamlit-0.4.3.tar` & `kiara_plugin.streamlit-0.4.4.tar`

### file list

```diff
@@ -1,151 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.127999 kiara_plugin.streamlit-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/apps/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/pipelines/components_doc_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/pipelines/operations_doc_onboarding.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.127999 kiara_plugin.streamlit-0.4.3/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/pipelines/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/examples/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/topic_modeling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/step_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workshop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/context/
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/container_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/scalars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/core_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/network_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/class_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/monkey_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:44:30.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.330222 kiara_plugin.streamlit-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/apps/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/jobs/download_journals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/apps/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/pipelines/example_file_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.330222 kiara_plugin.streamlit-0.4.4/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/pipelines/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/topic_modeling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/step_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/container_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/core_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/network_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.342223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/class_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/monkey_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:46.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.streamlit-0.4.3/.cruft.json` & `kiara_plugin.streamlit-0.4.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/.github/workflows/build-darwin.yaml` & `kiara_plugin.streamlit-0.4.4/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/.github/workflows/build-linux.yaml` & `kiara_plugin.streamlit-0.4.4/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/.github/workflows/build-windows.yaml` & `kiara_plugin.streamlit-0.4.4/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/.gitignore` & `kiara_plugin.streamlit-0.4.4/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -59,7 +59,8 @@
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
 ci/conda/kiara_plugin.streamlit/meta.yaml
+other_pipelines
```

### Comparing `kiara_plugin.streamlit-0.4.3/.pre-commit-config.yaml` & `kiara_plugin.streamlit-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/LICENSE` & `kiara_plugin.streamlit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/Makefile` & `kiara_plugin.streamlit-0.4.4/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/PKG-INFO` & `kiara_plugin.streamlit-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.streamlit
-Version: 0.4.3
+Version: 0.4.4
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
```

### Comparing `kiara_plugin.streamlit-0.4.3/README.md` & `kiara_plugin.streamlit-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/apps/components.py` & `kiara_plugin.streamlit-0.4.4/apps/operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # -*- coding: utf-8 -*-
 import os
 
 import streamlit as st
 
 import kiara_plugin.streamlit as kst
+from kiara.interfaces.python_api import JobDesc
 
 st.set_page_config(layout="wide")
-
 kst.init()
-st.kiara.api.set_active_context("components_doc", create=True)
 
-if "corpus_table" not in st.kiara.api.list_alias_names():
+st.kiara.api.set_active_context("_operation_doc", create=True)
+
+if "file_bundle" not in st.kiara.api.list_alias_names():
+    print("MISSING")
+
     with st.spinner("Downloading example data ..."):
-        pipeline_file = os.path.join(
-            os.path.dirname(__file__), "pipelines", "components_doc_onboarding.yaml"
+        job_file = os.path.join(
+            os.path.dirname(__file__), "jobs", "download_journals.yaml"
         )
-        results = st.kiara.api.run_job(pipeline_file)
+        job_desc = JobDesc.create_from_file(path=job_file)
+
+        results = st.kiara.api.run_job(job_desc)
 
         for field_name, value in results.items():
             st.kiara.api.store_value(value, field_name)
 
-st.kiara.component_info()
+st.kiara.operation_documentation()
```

### Comparing `kiara_plugin.streamlit-0.4.3/apps/operations.py` & `kiara_plugin.streamlit-0.4.4/apps/components.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # -*- coding: utf-8 -*-
 import os
 
 import streamlit as st
 
 import kiara_plugin.streamlit as kst
+from kiara.interfaces.python_api import JobDesc
 
 st.set_page_config(layout="wide")
 
 kst.init()
-st.kiara.api.set_active_context("_operation_doc", create=True)
+st.kiara.api.set_active_context("components_doc", create=True)
+
+if "file_bundle" not in st.kiara.api.list_alias_names():
 
-if "corpus_files" not in st.kiara.api.list_alias_names():
     with st.spinner("Downloading example data ..."):
-        pipeline_file = os.path.join(
-            os.path.dirname(__file__), "pipelines", "operations_doc_onboarding.yaml"
+        job_file = os.path.join(
+            os.path.dirname(__file__), "jobs", "download_journals.yaml"
         )
-        results = st.kiara.api.run_job(pipeline_file)
+        job_desc = JobDesc.create_from_file(path=job_file)
+
+        results = st.kiara.api.run_job(job_desc)
 
         for field_name, value in results.items():
             st.kiara.api.store_value(value, field_name)
 
-st.kiara.operation_documentation()
+
+st.kiara.component_info()
```

### Comparing `kiara_plugin.streamlit-0.4.3/apps/pipelines/components_doc_onboarding.yaml` & `kiara_plugin.streamlit-0.4.4/apps/pipelines/example_file_onboarding.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 pipeline_name: operations_doc_onboarding
 doc: Onboard example datasets to be used in the operations doc app.
 steps:
-  - module_type: download.file_bundle
+  - module_type: import.file_bundle
     step_id: download_example_data
-  - module_type: file_bundle.pick.sub_folder
-    step_id: pick_corpus_data
-    input_links:
-      file_bundle: download_example_data.file_bundle
   - module_type: create.table.from.file_bundle
-    step_id: create_text_corpus
+    step_id: create_files_table
     input_links:
-      file_bundle: pick_corpus_data.file_bundle
+      file_bundle: download_example_data.file_bundle
   - module_type: file_bundle.pick.file
     step_id: pick_journal_nodes
     input_links:
       file_bundle: download_example_data.file_bundle
   - module_type: file_bundle.pick.file
     step_id: pick_journal_edges
     input_links:
@@ -26,25 +22,25 @@
   - module_type: create.table.from.file
     step_id: create_edges_table
     input_links:
       file: pick_journal_edges.file
 
 
 input_aliases:
-  download_example_data.url: "example_data_url"
-  pick_corpus_data.sub_path: "corpus_sub_folder"
+  download_example_data.source: "example_data_source"
+  download_example_data.sub_path: "sub_folder"
+  download_example_data.include_files: "include_files"
+  download_example_data.exclude_files: "exclude_files"
+  download_example_data.onboard_type: "onboard_type"
+  download_example_data.exclude_dirs: "exclude_dirs"
   pick_journal_edges.path: "journal_edges_path"
   pick_journal_nodes.path: "journal_nodes_path"
+  create_nodes_table.first_row_is_header: "nodes_first_row_is_header"
+  create_edges_table.first_row_is_header: "edges_first_row_is_header"
 
 output_aliases:
-  pick_corpus_data.file_bundle: "corpus_file_bundle"
-  create_text_corpus.table: "corpus_table"
+  download_example_data.file_bundle: "file_bundle"
+  create_files_table.table: "files_table"
   pick_journal_nodes.file: "nodes_file"
   pick_journal_edges.file: "edges_file"
   create_nodes_table.table: "nodes_table"
   create_edges_table.table: "edges_table"
-
-defaults:
-  example_data_url: "https://github.com/DHARPA-Project/kiara.examples/archive/refs/heads/main.zip"
-  corpus_sub_folder: "kiara.examples-main/examples/data/text_corpus/data"
-  journal_edges_path: "kiara.examples-main/examples/data/journals/JournalEdges1902.csv"
-  journal_nodes_path: "kiara.examples-main/examples/data/journals/JournalNodes1902.csv"
```

### Comparing `kiara_plugin.streamlit-0.4.3/docs/development.md` & `kiara_plugin.streamlit-0.4.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/docs/index.md` & `kiara_plugin.streamlit-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/pipeline.py` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/example.yaml` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/example.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/topic_modeling.yaml` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/topic_modeling.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/step_inputs.py` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/step_inputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_dynamic.py` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_dynamic.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_static.py` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_static.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/workflows.py` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/examples/streamlit/workshop.py` & `kiara_plugin.streamlit-0.4.4/examples/streamlit/workshop.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/mkdocs.yml` & `kiara_plugin.streamlit-0.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/pyproject.toml` & `kiara_plugin.streamlit-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
     "kiara_plugin.tabular>=0.4.28",
     "kiara_plugin.onboarding>=0.4.5",
-    "streamlit>=1.23.1.0",
+    "streamlit>=1.24.0",
     "streamlit-aggrid>=0.3.4",
     "importlib-resources",
     "pydot>=1.4.0",
     "pyvis>=0.3.0",
     "streamlit-tags>=1.2.8"
 ]
 dynamic = ["version"]
```

### Comparing `kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_info_pages.py` & `kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_module_doc.py` & `kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/setup.cfg` & `kiara_plugin.streamlit-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import streamlit as st
 from kiara.interfaces.python_api.models.info import InfoItemGroup, ItemInfo
 from kiara.models.documentation import (
     AuthorsMetadataModel,
     ContextMetadataModel,
     DocumentationMetadataModel,
 )
+from kiara.models.python_class import PythonClass
 from kiara_plugin.streamlit.defaults import AUTO_GEN_MARKER
 from streamlit.runtime.state import SessionStateProxy
 
 with warnings.catch_warnings():
     pass
 
 from typing import TYPE_CHECKING
@@ -202,14 +203,17 @@
 
     arguments: Dict[str, ArgInfo] = Field(
         description="The arguments for this component."
     )
     examples: List[Dict[str, Any]] = Field(
         description="The examples for this component.", default_factory=list
     )
+    python_class: PythonClass = Field(
+        description="The python class backing this component."
+    )
 
     @classmethod
     def base_instance_class(cls) -> Type[KiaraComponent]:
         return KiaraComponent
 
     @classmethod
     def create_from_instance(cls, kiara: "Kiara", instance: KiaraComponent, **kwargs):
@@ -238,14 +242,15 @@
         info = ComponentInfo(
             type_name=type_name,
             authors=authors_md,
             documentation=doc,
             context=context,
             arguments=args,
             examples=examples,
+            python_class=PythonClass.from_class(instance.__class__),
         )
         return info
 
 
 class ComponentsInfo(InfoItemGroup[ComponentInfo]):
     @classmethod
     def base_info_class(cls) -> Type[ComponentInfo]:
```

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/context/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/api.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/api.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/components.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 
     def render_info(  # type: ignore
         self, st: DeltaGenerator, key: str, item: ComponentInfo, options: InfoCompOptions  # type: ignore
     ):
         st.markdown(f"#### Component: `{item.type_name}`")
         st.markdown(item.documentation.full_doc)
 
+        st.markdown("##### Component code")
+
+        with st.expander(f"Class: `{item.python_class.python_class_name}`"):
+            st.write(item.python_class.dict())
+
         comp = self.get_component("fields_info")
         st.markdown("##### Arguments")
         arg_table: Dict[str, List[Any]] = {
             "field": [],
             "type": [],
             "required": [],
             "default": [],
```

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/assemblies.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/assemblies.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/container_types.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/container_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/scalars.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/scalars.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/operations/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/pipelines/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/assemblies.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/assemblies.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/core_types.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/core_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/network_data.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/network_data.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/tabular.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/tabular.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/components.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/models.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/modules/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/renderers/__init__.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/streamlit.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/class_loading.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/class_loading.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/components.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/monkey_patches.py` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/PKG-INFO` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.streamlit
-Version: 0.4.3
+Version: 0.4.4
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
```

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/SOURCES.txt` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
 .github/workflows/build-darwin.yaml
 .github/workflows/build-linux.yaml
 .github/workflows/build-windows.yaml
 apps/components.py
 apps/operations.py
-apps/pipelines/components_doc_onboarding.yaml
-apps/pipelines/operations_doc_onboarding.yaml
+apps/pipelines.py
+apps/jobs/download_journals.yaml
+apps/pipelines/example_file_onboarding.yaml
 ci/conda/conda-pkg-patch.yaml
 docs/SUMMARY.md
 docs/development.md
 docs/index.md
 docs/usage.md
 docs/stylesheets/extra.css
 examples/data/Readme.md
```

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/entry_points.txt` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/requires.txt` & `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 kiara_plugin.tabular>=0.4.28
 kiara_plugin.onboarding>=0.4.5
-streamlit>=1.23.1.0
+streamlit>=1.24.0
 streamlit-aggrid>=0.3.4
 importlib-resources
 pydot>=1.4.0
 pyvis>=0.3.0
 streamlit-tags>=1.2.8
 
 [all_plugins]
```

### Comparing `kiara_plugin.streamlit-0.4.3/tests/conftest.py` & `kiara_plugin.streamlit-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.3/tests/test_job_descs.py` & `kiara_plugin.streamlit-0.4.4/tests/test_job_descs.py`

 * *Files identical despite different names*

