# Comparing `tmp/pyphetools-0.4.0.tar.gz` & `tmp/pyphetools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.4.0.tar", last modified: Thu Jun 29 12:57:10 2023, max compression
+gzip compressed data, was "pyphetools-0.4.1.tar", last modified: Thu Jun 29 14:19:20 2023, max compression
```

## Comparing `pyphetools-0.4.0.tar` & `pyphetools-0.4.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.457171 pyphetools-0.4.0/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.0/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.0/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-29 12:57:10.457171 pyphetools-0.4.0/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.0/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.385170 pyphetools-0.4.0/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.0/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.385170 pyphetools-0.4.0/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.0/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.385170 pyphetools-0.4.0/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.0/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.0/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.389170 pyphetools-0.4.0/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      882 2023-06-29 12:30:59.000000 pyphetools-0.4.0/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.0/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.4.0/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.0/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.0/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.0/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.0/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.0/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.0/pyphetools/creation/hgvs_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.0/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.0/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.4.0/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.0/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7501 2023-06-29 11:43:02.000000 pyphetools-0.4.0/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.4.0/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.4.0/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.0/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.4.0/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.0/pyphetools/creation/structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.0/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.0/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6088 2023-06-29 12:30:32.000000 pyphetools-0.4.0/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.0/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.389170 pyphetools-0.4.0/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.0/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.0/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.0/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.0/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.0/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.0/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.0/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.4.0/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.0/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.389170 pyphetools-0.4.0/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.4.0/pyphetools/validation/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.385170 pyphetools-0.4.0/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-29 12:57:10.000000 pyphetools-0.4.0/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2193 2023-06-29 12:57:10.000000 pyphetools-0.4.0/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-29 12:57:10.000000 pyphetools-0.4.0/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-06-29 12:57:10.000000 pyphetools-0.4.0/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-06-29 12:57:10.000000 pyphetools-0.4.0/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-06-29 12:56:21.000000 pyphetools-0.4.0/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-29 12:57:10.457171 pyphetools-0.4.0/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.393170 pyphetools-0.4.0/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.0/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.4.0/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.0/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.0/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.0/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.0/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.0/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.0/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.0/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.4.0/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.0/test/test_structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.0/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.0/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.385170 pyphetools-0.4.0/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 12:57:10.457171 pyphetools-0.4.0/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.0/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.275547 pyphetools-0.4.1/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.1/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.1/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-29 14:19:20.275547 pyphetools-0.4.1/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.1/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.1/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.1/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.1/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      882 2023-06-29 12:30:59.000000 pyphetools-0.4.1/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.1/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.1/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.1/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.1/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.1/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.1/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.1/pyphetools/creation/hgvs_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.1/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.1/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.4.1/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.1/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.1/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.4.1/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.1/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.4.1/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.1/pyphetools/creation/structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.1/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.1/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.1/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.1/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.1/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.1/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.1/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.1/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.1/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.4.1/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.1/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/validation/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2193 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-06-29 14:18:46.000000 pyphetools-0.4.1/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-29 14:19:20.275547 pyphetools-0.4.1/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.1/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.1/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.1/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.1/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.1/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.1/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.1/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.1/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.1/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.4.1/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.1/test/test_structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.1/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.1/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.275547 pyphetools-0.4.1/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.4.0/LICENSE` & `pyphetools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/PKG-INFO` & `pyphetools-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.0/README.md` & `pyphetools-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/docs/conf.py` & `pyphetools-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/analyze/downsampler.py` & `pyphetools-0.4.1/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/__init__.py` & `pyphetools-0.4.1/pyphetools/creation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/case_encoder.py` & `pyphetools-0.4.1/pyphetools/creation/case_encoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,38 @@
-import re
+from google.protobuf.json_format import MessageToJson
 import os
+import phenopackets
+import re
 from typing import List
 from collections import defaultdict
 from .hp_term import HpTerm
 from .hpo_cr import HpoConceptRecognizer
 from .simple_column_mapper import SimpleColumnMapper
 from .column_mapper import ColumnMapper
-from google.protobuf.json_format import MessageToJson
+
 from .individual import Individual
+from .variant import Variant
 
 ISO8601_REGEX = r"^P(\d+Y)?(\d+M)?(\d+D)?"
 
 
 class CaseEncoder:
     """encode a single case report with HPO terms in Phenopacket format
     """
 
-    def __init__(self, hpo_cr: HpoConceptRecognizer, pmid: str, age_at_last_exam=None) -> None:
+    def __init__(self, 
+                 hpo_cr: HpoConceptRecognizer, 
+                 pmid: str, 
+                 individual_id:str, 
+                 metadata:phenopackets.MetaData, 
+                 age_at_last_exam=None, 
+                 sex:str=None, 
+                 age:str=None, 
+                 disease_id:str=None, 
+                 disease_label:str=None) -> None:
         if not isinstance(hpo_cr, HpoConceptRecognizer):
             raise ValueError(
                 "concept_recognizer argument must be HpoConceptRecognizer but was {type(concept_recognizer)}")
         self._hpo_concept_recognizer = hpo_cr
         if not pmid.startswith("PMID:"):
             raise ValueError(f"Malformed pmid argument ({pmid}). Must start with PMID:")
         self._pmid = pmid
@@ -30,14 +42,22 @@
                 self._age_at_last_examination = age_at_last_exam
             else:
                 raise ValueError(f"Could not parse {age_at_last_exam} as ISO8601 period")
         else:
             self._age_at_last_examination = None
         self._seen_hpo_terms = set() # Use to prevent duplicate HP annotations
         self._annotations = defaultdict(list)
+        self._individual_id = individual_id
+        if not isinstance(metadata, phenopackets.MetaData):
+            raise ValueError(f"metadata argument must be phenopackets.MetaData but was {type(metadata)}")
+        self._sex = sex
+        self._age = age
+        self._disease_id = disease_id
+        self._disease_label = disease_label
+        self._interpretations = []
 
     def add_vignette(self, vignette, custom_d=None, custom_age=None, false_positive=[], excluded_terms=set()) -> List[
         HpTerm]:
         """
         false_positive: words or phrases that should not be parsed to HP terms
         """
         if custom_d is None:
@@ -89,14 +109,25 @@
             elif self._age_at_last_examination is not None:
                 self._annotations[self._age_at_last_examination].append(hpo_term)
             else:
                 self._annotations["N/A"].append(hpo_term)
             return HpTerm.term_list_to_dataframe([hpo_term])
         else:
             return ValueError("Must call function with non-None value for either id or label argument")
+        
+        
+    def add_variant_or_interpretation(self, variant):
+        if isinstance(variant, Variant):
+            self._interpretations.append(variant.to_ga4gh_variant_interpretation())
+        elif isinstance(variant, phenopackets.VariantInterpretation):
+            self._interpretations.append(variant)
+        else:
+            raise ValueError(f"variant argument must be pyphetools Variant or GA4GH \
+                phenopackets.VariantInterpretation but was {type(variant)}")
+            
 
     def initialize_simple_column_maps(self, column_name_to_hpo_label_map, observed, excluded, non_measured=None):
         if observed is None or excluded is None:
             raise ValueError("Symbols for observed (e.g., +, Y, yes) and excluded (e.g., -, N, no) required")
         if not isinstance(column_name_to_hpo_label_map, dict):
             raise ValueError("column_name_to_hpo_label_map must be a dict with column to HPO label mappings")
         simple_mapper_d = defaultdict(ColumnMapper)
@@ -106,32 +137,37 @@
                                      non_measured=non_measured)
             simple_mapper_d[column_name] = mpr
         return simple_mapper_d
 
     def get_hpo_term_dict(self):
         return self._annotations
 
-    def get_phenopacket(self, individual_id, metadata, sex=None, age=None, disease_id=None, disease_label=None,
-                        variants=None):
-        if not isinstance(variants, list):
-            variants = [variants]
-        individual = Individual(individual_id=individual_id, sex=sex, age=age, hpo_terms=self._annotations,
-                                variant_list=variants, disease_id=disease_id, disease_label=disease_label)
+    def get_phenopacket(self):
+        if not isinstance(interpretations, list):
+            interpretations = [interpretations]
+        individual = Individual(individual_id=self._individual_id, 
+                                sex=self._sex, 
+                                age=self._age, 
+                                hpo_terms=self._annotations,
+                                interpretation_list=self._interpretations, 
+                                disease_id=self._disease_id, 
+                                disease_label=self._disease_label)
         phenopacket_id = self._pmid.replace(":", "_") + "_" + individual.id.replace(" ", "_").replace(":", "_")
-        return individual.to_ga4gh_phenopacket(metadata=metadata, phenopacket_id=phenopacket_id)
+        return individual.to_ga4gh_phenopacket(metadata=self._metadata, phenopacket_id=phenopacket_id)
 
-    def output_phenopacket(self, outdir, phenopacket):
+    def output_phenopacket(self, outdir):
         """write a phenopacket to an output directory
 
         Args:
             outdir (str): name of directory to write phenopackets
             phenopacket (Phenopacket): GA4GH Phenopacket object
         """
         if not os.path.exists(outdir):
             os.makedirs(outdir)
+        phenopacket = self.get_phenopacket()
         phenopacket_id = phenopacket.id
         json_string = MessageToJson(phenopacket)
         fname = phenopacket_id.replace(" ", "_") + ".json"
         outpth = os.path.join(outdir, fname)
         with open(outpth, "wt") as fh:
             fh.write(json_string)
             print(f"Wrote phenopacket to {outpth}")
```

### Comparing `pyphetools-0.4.0/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.4.1/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/hgvs_variant.py` & `pyphetools-0.4.1/pyphetools/creation/hgvs_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/hp_term.py` & `pyphetools-0.4.1/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/hpo_cr.py` & `pyphetools-0.4.1/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.4.1/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/hpo_parser.py` & `pyphetools-0.4.1/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/individual.py` & `pyphetools-0.4.1/pyphetools/creation/individual.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         return self._age
     
     @property
     def hpo_terms(self):
         return self._hpo_terms
     
     @property
-    def variant_list(self):
-        return self._variant_list
+    def interpretation_list(self):
+        return self._interpretation_list
     
     def add_variant(self, v, acmg=None):
         if not isinstance(v, Variant):
             raise ValueError(f"variant argument must be pyphetools Variant type but was {type(v)}")
         self._interpretation_list.append(v.to_ga4gh_variant_interpretation(acmg=acmg))
     
     def to_ga4gh_phenopacket(self, metadata, phenopacket_id=None):
```

### Comparing `pyphetools-0.4.0/pyphetools/creation/metadata.py` & `pyphetools-0.4.1/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/structural_variant.py` & `pyphetools-0.4.1/pyphetools/creation/structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.4.1/pyphetools/creation/variant_column_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         if transcript is None or len(transcript) < 3:
             raise ValueError(f"Invalid transcript: \"{transcript}\"")
         self._transcript = transcript
         self._validator = VariantValidator(genome_build=assembly, transcript=transcript)
         self._column_name = column_name
         self._genotype_column = genotype_column
         self._delimiter = delimiter
-        self._variant_symbol_d = {}
         self._non_hgvs_variant_map = non_hgvs_variant_map
 
     def map_cell(self, cell_contents, genotype_contents=None, delimiter=None) -> List[Variant]:
         if delimiter is None:
             delimiter = self._delimiter
         if delimiter is not None:
             items = [x.strip() for x in cell_contents.split(delimiter)]
@@ -50,19 +49,14 @@
             items = [cell_contents]
         variant_interpretation_list = []
         for item in items:
             if item in self._non_hgvs_variant_map:
                 variant: Variant = self._non_hgvs_variant_map.get(item)
                 interpretation = variant.to_ga4gh_variant_interpretation()
                 variant_interpretation_list.append(interpretation)
-            elif item in self._variant_symbol_d:
-                variant_list = self._variant_symbol_d.get(item)
-                for v in variant_list:
-                    v.set_genotype(self._default_genotype)
-                    variant_interpretation_list.append(v.to_ga4gh_variant_interpretation())
             else:
                 try:
                     variant = self._validator.encode_hgvs(item)
                     if genotype_contents is not None:
                         if 'hom' in genotype_contents.lower():
                             variant.set_homozygous()
                         elif 'het' in genotype_contents.lower():
@@ -117,17 +111,14 @@
 
     def get_column_name(self):
         return self._column_name
 
     def get_genotype_colname(self):
         return self._genotype_column
 
-    def set_variant_symbol_dictionary(self, variant_sym_d):
-        self._variant_symbol_d = variant_sym_d
-
     def _print_summary(self):
         """Dump some of the attributes of the object, for debugging
         """
         print("VariantColumnMapper")
         print(f"transcript: {self._transcript}")
         print(f"column_name: {self._column_name}")
         print(f"genotype_column: {self._genotype_column}")
```

### Comparing `pyphetools-0.4.0/pyphetools/creation/variant_validator.py` & `pyphetools-0.4.1/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.4.1/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/focus_count_table.py` & `pyphetools-0.4.1/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/hpo_category.py` & `pyphetools-0.4.1/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.4.1/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/phenopacket_table.py` & `pyphetools-0.4.1/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/simple_patient.py` & `pyphetools-0.4.1/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/simple_variant.py` & `pyphetools-0.4.1/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools/output/term_count.py` & `pyphetools-0.4.1/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.4.1/pyphetools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.0/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.4.1/pyphetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/pyproject.toml` & `pyphetools-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.4.0"
+version = "0.4.1"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.4.0/test/test_age_column_mapper.py` & `pyphetools-0.4.1/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_case_encoder.py` & `pyphetools-0.4.1/test/test_case_encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import unittest
 import os
 import pandas as pd
 from pyphetools.creation import HpoParser, CaseEncoder
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 # The API requires us to pass a column name but the column name will not be used in the tests
 TEST_COLUMN = "test"
+from pyphetools.creation import MetaData
 
 class TestCaseParse(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         hpparser = HpoParser(hpo_json_file=HP_JSON_FILENAME)
         cls._hpo_cr = hpparser.get_hpo_concept_recognizer()
-        cls._parser = CaseEncoder(hpo_cr=cls._hpo_cr, pmid="PMID:1")
+        metadata = MetaData(created_by="ORCID:0000-0002-0736-9199")
+        metadata.default_versions_with_hpo(version="2022-05-05")
+        cls._parser = CaseEncoder(hpo_cr=cls._hpo_cr, individual_id="arbitrary", pmid="PMID:1", metadata=metadata.to_ga4gh())
 
     def test_chief_complaint(self):
         """
         Expect to get
         HP:0000365 	Hearing impairment 	True 	True
         HP:0001742 	Nasal congestion 	True 	True
         HP:0025267 	Snoring
@@ -50,15 +53,17 @@
     def test_excluded2(self):
         """
         The goal if this test is to enzure that 'Seizure' is annotated as 'excluded'
         """
         vignette = "The patient is not on seizure medication at this time."
         excluded = set()
         excluded.add("Seizure")
-        encoder = CaseEncoder(hpo_cr=self._hpo_cr, pmid="PMID:1")
+        metadata = MetaData(created_by="ORCID:0000-0002-0736-9199")
+        metadata.default_versions_with_hpo(version="2022-05-05")
+        encoder = CaseEncoder(hpo_cr=self._hpo_cr, individual_id="id", metadata=metadata.to_ga4gh(), pmid="PMID:1")
         df = encoder.add_vignette(vignette=vignette, excluded_terms=excluded)
         self.assertEqual(1, len(df))
         
         self.assertEqual("HP:0001250", df.iloc[0]['id'])
         self.assertEqual("Seizure",df.iloc[0]['label'])
         self.assertFalse(df.iloc[0]['observed'])
         self.assertTrue(df.iloc[0]['measured'])
```

### Comparing `pyphetools-0.4.0/test/test_column_mapper.py` & `pyphetools-0.4.1/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_constant_column_mapper.py` & `pyphetools-0.4.1/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_custom_column_mapper.py` & `pyphetools-0.4.1/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_hp_term.py` & `pyphetools-0.4.1/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_hpo_category.py` & `pyphetools-0.4.1/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_hpo_cr.py` & `pyphetools-0.4.1/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_hpo_parser.py` & `pyphetools-0.4.1/test/test_hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_option_column_mapper.py` & `pyphetools-0.4.1/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_structural_variant.py` & `pyphetools-0.4.1/test/test_structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_threshold_column_mapper.py` & `pyphetools-0.4.1/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/test/test_variant.py` & `pyphetools-0.4.1/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2html.py` & `pyphetools-0.4.1/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2html4.py` & `pyphetools-0.4.1/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2html5.py` & `pyphetools-0.4.1/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2latex.py` & `pyphetools-0.4.1/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2man.py` & `pyphetools-0.4.1/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2odt.py` & `pyphetools-0.4.1/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.4.1/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2pseudoxml.py` & `pyphetools-0.4.1/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2s5.py` & `pyphetools-0.4.1/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2xetex.py` & `pyphetools-0.4.1/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rst2xml.py` & `pyphetools-0.4.1/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.0/venv/bin/rstpep2html.py` & `pyphetools-0.4.1/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

