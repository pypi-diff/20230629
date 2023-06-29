# Comparing `tmp/pyphetools-0.3.5.tar.gz` & `tmp/pyphetools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.3.5.tar", last modified: Wed Jun 28 23:15:29 2023, max compression
+gzip compressed data, was "pyphetools-0.3.6.tar", last modified: Wed Jun 28 23:32:40 2023, max compression
```

## Comparing `pyphetools-0.3.5.tar` & `pyphetools-0.3.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.960682 pyphetools-0.3.5/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.3.5/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.3.5/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-28 23:15:29.960682 pyphetools-0.3.5/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.3.5/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.244672 pyphetools-0.3.5/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.3.5/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.288673 pyphetools-0.3.5/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.3.5/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.384674 pyphetools-0.3.5/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.3.5/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.3.5/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.748679 pyphetools-0.3.5/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      910 2023-06-28 19:42:05.000000 pyphetools-0.3.5/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.3.5/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.3.5/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    10807 2023-06-28 21:41:29.000000 pyphetools-0.3.5/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.3.5/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.3.5/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.3.5/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.3.5/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.3.5/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.3.5/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.3.5/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.3.5/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7496 2023-06-28 19:27:47.000000 pyphetools-0.3.5/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.3.5/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.3.5/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.3.5/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.3.5/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7002 2023-06-28 21:38:20.000000 pyphetools-0.3.5/pyphetools/creation/structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1025 2023-06-28 19:41:47.000000 pyphetools-0.3.5/pyphetools/creation/sv_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.3.5/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      270 2023-06-28 18:30:12.000000 pyphetools-0.3.5/pyphetools/creation/var_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5498 2023-06-28 23:14:47.000000 pyphetools-0.3.5/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6169 2023-06-28 23:14:41.000000 pyphetools-0.3.5/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3227 2023-06-27 16:40:26.000000 pyphetools-0.3.5/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.900681 pyphetools-0.3.5/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.3.5/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.3.5/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.3.5/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.3.5/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.3.5/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.3.5/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.3.5/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.3.5/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.3.5/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.900681 pyphetools-0.3.5/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.3.5/pyphetools/validation/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.332673 pyphetools-0.3.5/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-28 23:15:29.000000 pyphetools-0.3.5/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2224 2023-06-28 23:15:29.000000 pyphetools-0.3.5/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-28 23:15:29.000000 pyphetools-0.3.5/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-06-28 23:15:29.000000 pyphetools-0.3.5/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-06-28 23:15:29.000000 pyphetools-0.3.5/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-06-28 19:29:08.000000 pyphetools-0.3.5/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-28 23:15:29.960682 pyphetools-0.3.5/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.920681 pyphetools-0.3.5/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.3.5/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.3.5/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.3.5/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.3.5/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.3.5/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.3.5/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.3.5/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.3.5/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.3.5/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.3.5/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.3.5/test/test_structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.3.5/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1439 2023-05-11 14:18:42.000000 pyphetools-0.3.5/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.244672 pyphetools-0.3.5/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:15:29.960682 pyphetools-0.3.5/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.3.5/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.345127 pyphetools-0.3.6/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.3.6/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.3.6/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-28 23:32:40.345127 pyphetools-0.3.6/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.3.6/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.341127 pyphetools-0.3.6/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.3.6/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.341127 pyphetools-0.3.6/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.3.6/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.341127 pyphetools-0.3.6/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.3.6/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.3.6/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.341127 pyphetools-0.3.6/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      910 2023-06-28 19:42:05.000000 pyphetools-0.3.6/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.3.6/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.3.6/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10807 2023-06-28 21:41:29.000000 pyphetools-0.3.6/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.3.6/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.3.6/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.3.6/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.3.6/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.3.6/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.3.6/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.3.6/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.3.6/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7496 2023-06-28 19:27:47.000000 pyphetools-0.3.6/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.3.6/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.3.6/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.3.6/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.3.6/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7002 2023-06-28 21:38:20.000000 pyphetools-0.3.6/pyphetools/creation/structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1025 2023-06-28 19:41:47.000000 pyphetools-0.3.6/pyphetools/creation/sv_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.3.6/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      270 2023-06-28 18:30:12.000000 pyphetools-0.3.6/pyphetools/creation/var_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5498 2023-06-28 23:14:47.000000 pyphetools-0.3.6/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6169 2023-06-28 23:14:41.000000 pyphetools-0.3.6/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3227 2023-06-27 16:40:26.000000 pyphetools-0.3.6/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.345127 pyphetools-0.3.6/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.3.6/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.3.6/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.3.6/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.3.6/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.3.6/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.3.6/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.3.6/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.3.6/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.3.6/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.345127 pyphetools-0.3.6/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.3.6/pyphetools/validation/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.341127 pyphetools-0.3.6/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-28 23:32:40.000000 pyphetools-0.3.6/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2224 2023-06-28 23:32:40.000000 pyphetools-0.3.6/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-28 23:32:40.000000 pyphetools-0.3.6/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-06-28 23:32:40.000000 pyphetools-0.3.6/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-06-28 23:32:40.000000 pyphetools-0.3.6/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-06-28 23:32:07.000000 pyphetools-0.3.6/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-28 23:32:40.345127 pyphetools-0.3.6/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.345127 pyphetools-0.3.6/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.3.6/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.3.6/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.3.6/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.3.6/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.3.6/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.3.6/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.3.6/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.3.6/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.3.6/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.3.6/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.3.6/test/test_structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.3.6/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1439 2023-05-11 14:18:42.000000 pyphetools-0.3.6/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.341127 pyphetools-0.3.6/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-28 23:32:40.345127 pyphetools-0.3.6/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.3.6/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.3.5/LICENSE` & `pyphetools-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/PKG-INFO` & `pyphetools-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.3.5
+Version: 0.3.6
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.3.5/README.md` & `pyphetools-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/docs/conf.py` & `pyphetools-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/analyze/downsampler.py` & `pyphetools-0.3.6/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/__init__.py` & `pyphetools-0.3.6/pyphetools/creation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/case_encoder.py` & `pyphetools-0.3.6/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.3.6/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/hp_term.py` & `pyphetools-0.3.6/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/hpo_cr.py` & `pyphetools-0.3.6/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.3.6/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/hpo_parser.py` & `pyphetools-0.3.6/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/individual.py` & `pyphetools-0.3.6/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/metadata.py` & `pyphetools-0.3.6/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/structural_variant.py` & `pyphetools-0.3.6/pyphetools/creation/structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/sv_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/sv_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/variant.py` & `pyphetools-0.3.6/pyphetools/creation/variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.3.6/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/creation/variant_validator.py` & `pyphetools-0.3.6/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.3.6/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/focus_count_table.py` & `pyphetools-0.3.6/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/hpo_category.py` & `pyphetools-0.3.6/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.3.6/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/phenopacket_table.py` & `pyphetools-0.3.6/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/simple_patient.py` & `pyphetools-0.3.6/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/simple_variant.py` & `pyphetools-0.3.6/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools/output/term_count.py` & `pyphetools-0.3.6/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.3.6/pyphetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.3.5
+Version: 0.3.6
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.3.5/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.3.6/pyphetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/pyproject.toml` & `pyphetools-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.3.5"
+version = "0.3.6"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.3.5/test/test_age_column_mapper.py` & `pyphetools-0.3.6/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_case_encoder.py` & `pyphetools-0.3.6/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_column_mapper.py` & `pyphetools-0.3.6/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_constant_column_mapper.py` & `pyphetools-0.3.6/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_custom_column_mapper.py` & `pyphetools-0.3.6/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_hp_term.py` & `pyphetools-0.3.6/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_hpo_category.py` & `pyphetools-0.3.6/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_hpo_cr.py` & `pyphetools-0.3.6/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_hpo_parser.py` & `pyphetools-0.3.6/test/test_hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_option_column_mapper.py` & `pyphetools-0.3.6/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_structural_variant.py` & `pyphetools-0.3.6/test/test_structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_threshold_column_mapper.py` & `pyphetools-0.3.6/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/test/test_variant.py` & `pyphetools-0.3.6/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2html.py` & `pyphetools-0.3.6/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2html4.py` & `pyphetools-0.3.6/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2html5.py` & `pyphetools-0.3.6/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2latex.py` & `pyphetools-0.3.6/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2man.py` & `pyphetools-0.3.6/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2odt.py` & `pyphetools-0.3.6/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.3.6/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2pseudoxml.py` & `pyphetools-0.3.6/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2s5.py` & `pyphetools-0.3.6/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2xetex.py` & `pyphetools-0.3.6/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rst2xml.py` & `pyphetools-0.3.6/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.5/venv/bin/rstpep2html.py` & `pyphetools-0.3.6/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

