# Comparing `tmp/timeseriesflattener-1.2.1.tar.gz` & `tmp/timeseriesflattener-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-1.2.1.tar", last modified: Tue Jun 20 08:13:22 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.3.0.tar", last modified: Thu Jun 29 09:14:50 2023, max compression
```

## Comparing `timeseriesflattener-1.2.1.tar` & `timeseriesflattener-1.3.0.tar`

### file list

```diff
@@ -1,133 +1,139 @@
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.857203 timeseriesflattener-1.2.1/
--rw-r--r--   0 au484925 (903520038) staff       (20)      489 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.cookiecutter.json
--rw-r--r--   0 au484925 (903520038) staff       (20)      738 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.cruft.json
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.810689 timeseriesflattener-1.2.1/.github/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.804141 timeseriesflattener-1.2.1/.github/actions/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.810930 timeseriesflattener-1.2.1/.github/actions/test/
--rw-r--r--   0 au484925 (903520038) staff       (20)      892 2023-06-14 14:06:50.000000 timeseriesflattener-1.2.1/.github/actions/test/action.yml
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.811185 timeseriesflattener-1.2.1/.github/actions/test_tutorials/
--rw-r--r--   0 au484925 (903520038) staff       (20)      948 2023-06-15 08:56:38.000000 timeseriesflattener-1.2.1/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      529 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.github/dependabot.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      252 2023-03-01 09:46:41.000000 timeseriesflattener-1.2.1/.github/pull_request_template.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     1689 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.github/recommended_repo_setup.md
--rw-r--r--   0 au484925 (903520038) staff       (20)      465 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/.github/setup_ci.md
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.813253 timeseriesflattener-1.2.1/.github/workflows/
--rw-r--r--   0 au484925 (903520038) staff       (20)      720 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.github/workflows/check_for_rej.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2083 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.github/workflows/cruft.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      849 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      868 2023-06-07 11:02:56.000000 timeseriesflattener-1.2.1/.github/workflows/documentation.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      727 2023-03-23 07:54:31.000000 timeseriesflattener-1.2.1/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2446 2023-06-20 08:04:16.000000 timeseriesflattener-1.2.1/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2891 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     1132 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.github/workflows/stalebot.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     3056 2023-06-14 14:23:53.000000 timeseriesflattener-1.2.1/.github/workflows/static_type_checks.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2871 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.gitignore
--rw-r--r--   0 au484925 (903520038) staff       (20)      644 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 au484925 (903520038) staff       (20)     1286 2023-03-31 09:12:14.000000 timeseriesflattener-1.2.1/.zenodo.json
--rw-r--r--   0 au484925 (903520038) staff       (20)    55845 2023-06-20 08:13:15.000000 timeseriesflattener-1.2.1/CHANGELOG.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     5238 2023-03-01 10:46:04.000000 timeseriesflattener-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     4474 2023-03-01 11:40:47.000000 timeseriesflattener-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     1087 2022-12-06 14:15:36.000000 timeseriesflattener-1.2.1/LICENSE
--rw-r--r--   0 au484925 (903520038) staff       (20)      262 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/Makefile
--rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-20 08:13:22.856947 timeseriesflattener-1.2.1/PKG-INFO
--rw-r--r--   0 au484925 (903520038) staff       (20)     9122 2023-06-15 08:47:22.000000 timeseriesflattener-1.2.1/README.md
--rw-r--r--   0 au484925 (903520038) staff       (20)      658 2022-12-06 09:57:22.000000 timeseriesflattener-1.2.1/citation.cff
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.815419 timeseriesflattener-1.2.1/docs/
--rw-r--r--   0 au484925 (903520038) staff       (20)      633 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/docs/Makefile
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.817215 timeseriesflattener-1.2.1/docs/_static/
--rw-r--r--   0 au484925 (903520038) staff       (20)    15406 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.1/docs/_static/favicon.ico
--rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.1/docs/_static/icon.png
--rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.1/docs/_static/icon_dark.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   811066 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.1/docs/_static/terminology_figure.png
--rw-r--r--   0 au484925 (903520038) staff       (20)     4211 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.1/docs/conf.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2097 2023-04-19 11:55:26.000000 timeseriesflattener-1.2.1/docs/faq.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)      332 2023-06-14 14:10:35.000000 timeseriesflattener-1.2.1/docs/feature_specifications.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)     5280 2023-01-25 13:20:02.000000 timeseriesflattener-1.2.1/docs/index.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)      299 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.1/docs/installation.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)      312 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.1/docs/timeseriesflattener.rst
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.821236 timeseriesflattener-1.2.1/docs/tutorials/
--rw-r--r--   0 au484925 (903520038) staff       (20)   118804 2023-06-15 08:47:23.000000 timeseriesflattener-1.2.1/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 au484925 (903520038) staff       (20)    50220 2023-06-15 08:47:22.000000 timeseriesflattener-1.2.1/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 au484925 (903520038) staff       (20)    72388 2023-06-15 08:34:08.000000 timeseriesflattener-1.2.1/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.824164 timeseriesflattener-1.2.1/docs/tutorials/img/
--rw-r--r--   0 au484925 (903520038) staff       (20)    78953 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.1/docs/tutorials/img/term_a.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   109486 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.1/docs/tutorials/img/term_b.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   107613 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.1/docs/tutorials/img/term_c.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   250306 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.1/docs/tutorials/img/term_d.png
--rw-r--r--   0 au484925 (903520038) staff       (20)      370 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.1/docs/tutorials.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.1/icon.png
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.825406 timeseriesflattener-1.2.1/paper/
--rw-r--r--   0 au484925 (903520038) staff       (20)    14392 2023-03-31 09:12:14.000000 timeseriesflattener-1.2.1/paper/paper.bib
--rw-r--r--   0 au484925 (903520038) staff       (20)     9344 2023-03-31 09:12:14.000000 timeseriesflattener-1.2.1/paper/paper.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     4290 2023-06-20 08:13:15.000000 timeseriesflattener-1.2.1/pyproject.toml
--rw-r--r--   0 au484925 (903520038) staff       (20)       38 2023-06-20 08:13:22.857251 timeseriesflattener-1.2.1/setup.cfg
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.825702 timeseriesflattener-1.2.1/src/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1996 2023-06-14 14:28:54.000000 timeseriesflattener-1.2.1/src/conftest.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.828855 timeseriesflattener-1.2.1/src/timeseriesflattener/
--rw-r--r--   0 au484925 (903520038) staff       (20)      309 2023-06-14 08:57:30.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     4834 2023-06-15 08:30:34.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/aggregation_fns.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     5559 2023-06-14 12:58:48.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.830297 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-12-06 12:02:05.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     1977 2023-06-14 09:34:12.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     6308 2023-06-15 08:28:24.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.830924 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 au484925 (903520038) staff       (20)     7344 2023-06-15 08:34:18.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_specs/group_specs.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     8428 2023-06-15 08:34:18.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/feature_specs/single_specs.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    36395 2023-06-15 08:30:40.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2271 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2239 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/logger.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     7704 2023-06-14 11:44:29.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/misc_utils.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.831776 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/
--rw-r--r--   0 au484925 (903520038) staff       (20)     3008 2023-06-14 12:20:04.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.805312 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.805156 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.832365 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1477 2023-03-20 10:36:42.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 au484925 (903520038) staff       (20)   864795 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.834909 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1869 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    25543 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 au484925 (903520038) staff       (20)     1015 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.852681 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 au484925 (903520038) staff       (20)      784 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     1003 2023-03-20 10:36:42.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 au484925 (903520038) staff       (20)      980 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 au484925 (903520038) staff       (20)      816 2023-03-20 10:36:42.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 au484925 (903520038) staff       (20)   248865 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)   268962 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)   268904 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)  4316151 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)  4315816 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)    68900 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)    84570 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)     1392 2023-06-14 12:15:52.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     5179 2023-06-14 13:28:04.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.853556 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/__init__.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.853662 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_feature_cache/
--rw-r--r--   0 au484925 (903520038) staff       (20)     3425 2023-06-15 08:34:08.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.854356 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    16237 2023-06-15 08:34:01.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     1452 2023-06-14 10:33:38.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2305 2023-06-15 08:34:09.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.856205 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2023-02-07 08:39:43.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    18309 2023-06-15 08:34:09.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2688 2023-06-15 08:34:11.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2328 2023-06-14 10:33:38.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2319 2023-06-15 08:34:18.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     8190 2023-06-15 08:34:19.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2397 2023-06-14 11:20:11.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2342 2023-06-14 12:24:11.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/text_embedding_functions.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.856504 timeseriesflattener-1.2.1/src/timeseriesflattener/utils/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1065 2023-06-14 13:05:30.000000 timeseriesflattener-1.2.1/src/timeseriesflattener/utils/pydantic_basemodel.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:13:22.829541 timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/
--rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-20 08:13:22.000000 timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 au484925 (903520038) staff       (20)     4668 2023-06-20 08:13:22.000000 timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)        1 2023-06-20 08:13:22.000000 timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)      709 2023-06-20 08:13:22.000000 timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)       29 2023-06-20 08:13:22.000000 timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)     9396 2023-06-15 08:57:16.000000 timeseriesflattener-1.2.1/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.366249 timeseriesflattener-1.3.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.362249 timeseriesflattener-1.3.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.366249 timeseriesflattener-1.3.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.366249 timeseriesflattener-1.3.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.370249 timeseriesflattener-1.3.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      868 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    56049 2023-06-29 09:14:38.000000 timeseriesflattener-1.3.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11520 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.370249 timeseriesflattener-1.3.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.370249 timeseriesflattener-1.3.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.374249 timeseriesflattener-1.3.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   118804 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50220 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    72388 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.374249 timeseriesflattener-1.3.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.374249 timeseriesflattener-1.3.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-06-29 09:14:38.000000 timeseriesflattener-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     7039 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     8488 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    36395 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.362249 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.362249 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.382250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.386250 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.398251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18309 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.402251 timeseriesflattener-1.3.0/src/timeseriesflattener/utils/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:14:50.378250 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11520 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-29 09:14:50.000000 timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-06-29 09:14:37.000000 timeseriesflattener-1.3.0/tasks.py
```

### Comparing `timeseriesflattener-1.2.1/.cruft.json` & `timeseriesflattener-1.3.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/actions/test/action.yml` & `timeseriesflattener-1.3.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.3.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/dependabot.yml` & `timeseriesflattener-1.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/recommended_repo_setup.md` & `timeseriesflattener-1.3.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.3.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/cruft.yml` & `timeseriesflattener-1.3.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.3.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/documentation.yml` & `timeseriesflattener-1.3.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.3.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.3.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.3.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/stalebot.yml` & `timeseriesflattener-1.3.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.3.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.gitignore` & `timeseriesflattener-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.pre-commit-config.yaml` & `timeseriesflattener-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/.zenodo.json` & `timeseriesflattener-1.3.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/CHANGELOG.md` & `timeseriesflattener-1.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.0 (2023-06-29)
+
+### Feature
+
+* Add types to aggregation functions ([`560539f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/560539f2d1871043024539f863fc755cb101c28e))
+
 ## v1.2.1 (2023-06-20)
 
 
 
 ## v1.2.0 (2023-06-20)
```

### Comparing `timeseriesflattener-1.2.1/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/CONTRIBUTING.md` & `timeseriesflattener-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/LICENSE` & `timeseriesflattener-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/PKG-INFO` & `timeseriesflattener-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.2.1
+Version: 1.3.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.2.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.2.1/README.md` & `timeseriesflattener-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/Makefile` & `timeseriesflattener-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/_static/favicon.ico` & `timeseriesflattener-1.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/_static/icon.png` & `timeseriesflattener-1.3.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/_static/icon_dark.png` & `timeseriesflattener-1.3.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/_static/terminology_figure.png` & `timeseriesflattener-1.3.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/conf.py` & `timeseriesflattener-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/faq.rst` & `timeseriesflattener-1.3.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/index.rst` & `timeseriesflattener-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.3.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-1.3.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.3.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.3.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.3.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.3.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.3.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/icon.png` & `timeseriesflattener-1.3.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/paper/paper.bib` & `timeseriesflattener-1.3.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/paper/paper.md` & `timeseriesflattener-1.3.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/pyproject.toml` & `timeseriesflattener-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "1.2.1"
+version = "1.3.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8.0,<3.12.0"
 dependencies = [
     "scipy>=1.8.0",
     "scikit-learn>=1.1.2",
     "pydantic>=1.9.0",
-    "pandas>=1.4.0",
+    "pandas>=1.4.0, <2.0.0",
     "catalogue>=2.0.0",
     "numpy>=1.23.3",
     "pyarrow>=8.0.0",
     "protobuf<=4.23.3", # Other versions give errors with pytest, super weird!
     "frozendict>=2.3.4",
     "coloredlogs>14.0.0",
 ]
```

### Comparing `timeseriesflattener-1.2.1/src/conftest.py` & `timeseriesflattener-1.3.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/aggregation_fns.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/aggregation_fns.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,94 @@
 """Functions for resolving multiple values in a time-series into a single
 value."""
 
 
+from typing import Callable
+
 import catalogue
 from pandas import DataFrame, Series
+from pandas.core.groupby.generic import DataFrameGroupBy
 from scipy import stats
 
 aggregation_fns = catalogue.create("timeseriesflattener", "resolve_strategies")
+import pandas as pd
+
+AggregationFunType = Callable[[DataFrameGroupBy], pd.DataFrame]
 
 
-def latest(grouped_df: DataFrame) -> Series:
+def latest(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Get the latest value.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with only the latest value.
     """
-    return grouped_df.last()  # type: ignore
+    return grouped_df.last()
 
 
-def earliest(grouped_df: DataFrame) -> Series:
+def earliest(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Get the earliest value.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with only the earliest value in each group.
     """
-    return grouped_df.first()  # type: ignore
+    return grouped_df.first()
 
 
-def maximum(grouped_df: DataFrame) -> Series:
+def maximum(grouped_df: DataFrameGroupBy) -> DataFrame:
     return grouped_df.max()
 
 
-def minimum(grouped_df: DataFrame) -> Series:
+def minimum(grouped_df: DataFrameGroupBy) -> DataFrame:
     return grouped_df.min()
 
 
-def mean(grouped_df: DataFrame) -> Series:
+def mean(grouped_df: DataFrameGroupBy) -> DataFrame:
     return grouped_df.mean(numeric_only=True)
 
 
-def summed(grouped_df: DataFrame) -> Series:
+def summed(grouped_df: DataFrameGroupBy) -> DataFrame:
     return grouped_df.sum()
 
 
-def count(grouped_df: DataFrame) -> Series:
+def count(grouped_df: DataFrameGroupBy) -> DataFrame:
     return grouped_df.count()
 
 
-def variance(grouped_df: DataFrame) -> Series:
+def variance(grouped_df: DataFrameGroupBy) -> DataFrame:
     return grouped_df.var()
 
 
-def boolean(grouped_df: DataFrame) -> DataFrame:
+def boolean(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Returns a boolean value indicating whether or not event has occurred in
     look ahead/behind window.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with value column containing only 0 or 1s.
     """
-    grouped_df = (
+    df = (
         grouped_df["timestamp_val"]
         .apply(lambda x: (~x.isna()).sum())
         .reset_index(name="value")
     )
 
-    grouped_df.loc[grouped_df["value"] > 0, "value"] = 1
+    df.loc[df["value"] > 0, "value"] = 1
 
-    return grouped_df
+    return df
 
 
-def change_per_day(grouped_df: DataFrame) -> DataFrame:
+def change_per_day(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Returns the change in value per day.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with value column containing the change in value per day.
@@ -101,15 +107,15 @@
     return grouped_df.apply(
         lambda x: Series(
             {"value": stats.linregress(x.timestamp_val, x.value)[0]},
         ),
     )
 
 
-def concatenate(grouped_df: DataFrame) -> DataFrame:
+def concatenate(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Returns the concatenated values. This is useful for text data.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with value column containing the concatenated values.
@@ -118,15 +124,15 @@
     return grouped_df.apply(
         lambda x: Series(
             {"value": " ".join(x.value)},
         ),
     )
 
 
-def mean_number_of_characters(grouped_df: DataFrame) -> DataFrame:
+def mean_number_of_characters(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Returns the mean length of values. This is useful for text data.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with value column containing the concatenated values.
@@ -134,15 +140,15 @@
     return grouped_df.apply(
         lambda x: Series(
             {"value": x.value.str.len().mean()},
         ),
     )
 
 
-def type_token_ratio(grouped_df: DataFrame) -> DataFrame:
+def type_token_ratio(grouped_df: DataFrameGroupBy) -> DataFrame:
     """Returns the type-token ratio. This is useful for text data.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with value column containing the concatenated values.
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/feature_specs/group_specs.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/group_specs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 from dataclasses import dataclass
 from typing import Callable, Dict, List, Optional, Sequence, Union
 
 import pandas as pd
 from pydantic import Field
-from timeseriesflattener.aggregation_fns import concatenate
+from timeseriesflattener.aggregation_fns import AggregationFunType
 from timeseriesflattener.feature_specs.single_specs import (
     AnySpec,
     OutcomeSpec,
     PredictorSpec,
     TextPredictorSpec,
 )
 from timeseriesflattener.utils.pydantic_basemodel import BaseModel
@@ -33,15 +33,15 @@
 
     """
 
     # Shared attributes from GroupSpec
     prefix: str = "pred"
     lookbehind_days: List[float]
     named_dataframes: Sequence[NamedDataframe]
-    aggregation_fns: Sequence[Callable]
+    aggregation_fns: Sequence[AggregationFunType]
     fallback: Sequence[Union[int, float, str]]
 
     def create_combinations(self) -> List[PredictorSpec]:
         """Create all combinations from the group spec."""
         combination_dict = create_feature_combinations_from_dict(
             dictionary=self.__dict__,
         )
@@ -73,15 +73,15 @@
             during resolution, which is faster than non-incident outcomes.
 
     """
 
     # Shared attributes from GroupSpec
     prefix: str = "outc"
     named_dataframes: Sequence[NamedDataframe]
-    aggregation_fns: Sequence[Callable]
+    aggregation_fns: Sequence[AggregationFunType]
     fallback: Sequence[Union[int, float, str]]
 
     # Individual attributes
     lookahead_days: List[float]
     incident: Sequence[bool]
 
     def create_combinations(self) -> List[OutcomeSpec]:
@@ -105,15 +105,15 @@
 
 class TextPredictorGroupSpec(BaseModel):
     """A group of text predictor specifications. See PredictorGroupSpec and TextPredictorSpec for more details."""
 
     # Shared attributes from GroupSpec
     lookbehind_days: List[float]
     named_dataframes: Sequence[NamedDataframe]
-    aggregation_fns: Sequence[Callable]
+    aggregation_fns: Sequence[AggregationFunType]
     fallback: Sequence[Union[int, float, str]]
 
     embedding_fn_name: str
 
     prefix: str = "pred"
 
     # Individual attributes
@@ -123,21 +123,14 @@
         pandas series of strings and return a pandas dataframe of embeddings.
         Defaults to: None.""",
     )
     embedding_fn_kwargs: Optional[List[dict]] = Field(
         default=None,
         description="""Optional kwargs passed onto the embedding_fn.""",
     )
-    aggregation_fn: Sequence[Callable] = Field(
-        default=[concatenate],
-        description="""A function used for resolving multiple values within the
-        interval_days, i.e. how to combine texts within the lookbehind window.
-        Defaults to: concatenate. Other possible options are "latest" and
-        "earliest".""",
-    )
 
     def create_combinations(self) -> List[TextPredictorSpec]:
         """Create all combinations from the group spec."""
         combination_dict = create_feature_combinations_from_dict(
             dictionary=self.__dict__,
         )
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/feature_specs/single_specs.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/feature_specs/single_specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Callable, Optional, Union
 
 import pandas as pd
-from timeseriesflattener.aggregation_fns import concatenate
+from timeseriesflattener.aggregation_fns import AggregationFunType, concatenate
 from timeseriesflattener.utils.pydantic_basemodel import BaseModel
 
 
 @dataclass(frozen=True)
 class CoercedFloats:
     lookwindow: Union[float, int]
     fallback: Union[float, int]
@@ -42,15 +42,15 @@
         return f"{self.prefix}_{self.feature_base_name}"
 
 
 def get_temporal_col_name(
     prefix: str,
     feature_base_name: str,
     lookwindow: Union[float, int],
-    aggregation_fn: Callable,
+    aggregation_fn: AggregationFunType,
     fallback: Union[float, int],
 ) -> str:
     """Get the column name for the temporal feature."""
     coerced = coerce_floats(lookwindow=lookwindow, fallback=fallback)
     col_str = f"{prefix}_{feature_base_name}_within_{str(coerced.lookwindow)}_days_{aggregation_fn.__name__}_fallback_{coerced.fallback}"
     return col_str
 
@@ -75,15 +75,15 @@
         prefix: The prefix used for column name generation, e.g.
             <prefix>_<feature_name>_<metadata>. Defaults to "pred".
     """
 
     timeseries_df: pd.DataFrame
     feature_base_name: str
     lookahead_days: float
-    aggregation_fn: Callable
+    aggregation_fn: AggregationFunType
     fallback: Union[float, int]
     incident: bool
     prefix: str = "outc"
 
     def get_output_col_name(self) -> str:
         """Get the column name for the output column."""
         col_str = get_temporal_col_name(
@@ -123,15 +123,15 @@
             Requires that each entity only occurs once in the timeseries_df.
         prefix: The prefix used for column name generation, e.g.
             <prefix>_<feature_name>_<metadata>. Defaults to "pred".
     """
 
     timeseries_df: pd.DataFrame
     feature_base_name: str
-    aggregation_fn: Callable
+    aggregation_fn: AggregationFunType
     fallback: Union[float, int]
     lookbehind_days: float
     prefix: str = "pred"
 
     def get_output_col_name(self) -> str:
         """Generate the column name for the output column."""
         return get_temporal_col_name(
@@ -168,15 +168,15 @@
     feature_base_name: str
     fallback: Union[float, int]
     embedding_fn: Callable
     embedding_fn_kwargs: Optional[dict] = None
     lookbehind_days: float
     prefix: str = "pred"
 
-    aggregation_fn: Callable = concatenate
+    aggregation_fn: AggregationFunType = concatenate
 
     def get_output_col_name(self, additional_feature_name: Optional[str] = None) -> str:
         """Generate the column name for the output column.
         If interval days is a float, the decimal point is changed to an underscore.
 
         Args:
             additional_feature_name (Optional[str]): additional feature name to
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/misc_utils.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Generate synth data with outcome."""
 from pathlib import Path
 
 import numpy as np
-from psycop_ml_utils.synth_data_generator.synth_prediction_times_generator import (
+from timeseriesflattener.testing.synth_data_generator.synth_prediction_times_generator import (
     generate_synth_data,
 )
 
 if __name__ == "__main__":
     column_specifications = {
         "citizen_ids": {"column_type": "uniform_int", "min": 0, "max": 1_200_001},
         "timestamp": {"column_type": "datetime_uniform", "min": 0, "max": 5 * 365},
@@ -27,15 +27,15 @@
             "sd": 0.5,
             "min": 0,
             "fallback": np.nan,
         },
     }
 
     synth_df = generate_synth_data(
-        predictors=column_specifications,
+        predictors=column_specifications,  # type: ignore
         outcome_column_name="outc_dichotomous_t2d_within_30_days_max_fallback_0",
         n_samples=10_000,
         logistic_outcome_model="1*pred_hba1c_within_100_days_max_fallback_nan+1*pred_hdl_within_100_days_max_fallback_nan",
         prob_outcome=0.08,
     )
 
     synth_df.describe()
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Generate dataframe with prediction times."""
 
-from psycop_ml_utils.synth_data_generator.synth_col_generators import (
+from timeseriesflattener.misc_utils import PROJECT_ROOT
+from timeseriesflattener.testing.synth_data_generator.synth_col_generators import (
     generate_data_columns,
 )
-from timeseriesflattener.misc_utils import PROJECT_ROOT
 
 if __name__ == "__main__":
     # Get project root directory
 
     column_specs = {
         "entity_id": {
             "column_type": "uniform_int",
@@ -18,15 +18,15 @@
             "column_type": "datetime_uniform",
             "min": -5 * 365,
             "max": 0 * 365,
         },
     }
 
     df = generate_data_columns(
-        predictors=column_specs,
+        predictors=column_specs,  # type: ignore
         n_samples=10_000,
     )
 
     df.to_csv(
         PROJECT_ROOT / "tests" / "test_data" / "raw" / "synth_prediction_times.csv",
         index=False,
     )
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Generate raw binary dataframe."""
 
 from pathlib import Path
 
-from psycop_ml_utils.synth_data_generator.synth_col_generators import (
+from timeseriesflattener.testing.synth_data_generator.synth_col_generators import (
     generate_data_columns,
 )
 
 if __name__ == "__main__":
     # Get project root directory
     project_root = Path(__file__).resolve().parents[3]
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Generate raw float dataframe."""
 
-from psycop_ml_utils.synth_data_generator.synth_col_generators import (
+from timeseriesflattener.misc_utils import PROJECT_ROOT
+from timeseriesflattener.testing.synth_data_generator.synth_col_generators import (
     generate_data_columns,
 )
-from timeseriesflattener.misc_utils import PROJECT_ROOT
 
 if __name__ == "__main__":
     # Get project root directory
 
     column_specs = [
         {
             "entity_id": {
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Generate raw binary dataframe."""
 
 from pathlib import Path
 
-from psycop_ml_utils.synth_data_generator.synth_col_generators import (
+from timeseriesflattener.testing.synth_data_generator.synth_col_generators import (
     generate_data_columns,
 )
 
 if __name__ == "__main__":
     # Get project root directory
     project_root = Path(__file__).resolve().parents[3]
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener/utils/pydantic_basemodel.py` & `timeseriesflattener-1.3.0/src/timeseriesflattener/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.2.1
+Version: 1.3.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.2.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.3.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 src/timeseriesflattener/feature_cache/abstract_feature_cache.py
 src/timeseriesflattener/feature_cache/cache_to_disk.py
 src/timeseriesflattener/feature_specs/group_specs.py
 src/timeseriesflattener/feature_specs/single_specs.py
 src/timeseriesflattener/testing/load_synth_data.py
 src/timeseriesflattener/testing/text_embedding_functions.py
 src/timeseriesflattener/testing/utils_for_testing.py
+src/timeseriesflattener/testing/synth_data_generator/__init__.py
+src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+src/timeseriesflattener/testing/synth_data_generator/utils.py
 src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
 src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
 src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
 src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
 src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
 src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
 src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
```

### Comparing `timeseriesflattener-1.2.1/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-1.3.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 scipy>=1.8.0
 scikit-learn>=1.1.2
 pydantic>=1.9.0
-pandas>=1.4.0
+pandas<2.0.0,>=1.4.0
 catalogue>=2.0.0
 numpy>=1.23.3
 pyarrow>=8.0.0
 protobuf<=4.23.3
 frozendict>=2.3.4
 coloredlogs>14.0.0
```

### Comparing `timeseriesflattener-1.2.1/tasks.py` & `timeseriesflattener-1.3.0/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,19 +314,19 @@
 def test_tutorials(c: Context):
     c.run(
         "find docs/tutorials -name '*.ipynb' | grep -v 'nbconvert' | xargs jupyter nbconvert --to notebook --execute",
     )
 
 
 @task
-def pr(c: Context, auto_fix: bool = False):
+def pr(c: Context, auto_fix: bool = True):
     """Run all checks and update the PR."""
     add_and_commit(c)
     lint(c, auto_fix=auto_fix)
-    test(c, python_versions="3.8,3.11")
+    test(c, python_versions="3.9")
     test_tutorials(c)
     update_branch(c)
     update_pr(c)
 
 
 @task
 def docs(c: Context, view: bool = False, view_only: bool = False):
```

