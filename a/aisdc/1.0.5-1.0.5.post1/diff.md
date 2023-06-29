# Comparing `tmp/aisdc-1.0.5.tar.gz` & `tmp/aisdc-1.0.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisdc-1.0.5.tar", last modified: Mon Jun  5 20:43:21 2023, max compression
+gzip compressed data, was "aisdc-1.0.5.post1.tar", last modified: Thu Jun 29 10:47:39 2023, max compression
```

## Comparing `aisdc-1.0.5.tar` & `aisdc-1.0.5.post1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.089487 aisdc-1.0.5/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.5/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-06-05 20:43:21.089487 aisdc-1.0.5/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-17 12:52:16.000000 aisdc-1.0.5/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/attacks/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/attacks/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      977 2023-06-05 19:25:56.000000 aisdc-1.0.5/aisdc/attacks/attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/attacks/attribute_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2166 2023-05-17 12:52:16.000000 aisdc-1.0.5/aisdc/attacks/dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3616 2023-05-17 12:52:16.000000 aisdc-1.0.5/aisdc/attacks/failfast.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26233 2023-06-05 19:25:56.000000 aisdc-1.0.5/aisdc/attacks/likelihood_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12913 2023-05-19 21:41:45.000000 aisdc-1.0.5/aisdc/attacks/report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    30917 2023-06-05 19:25:56.000000 aisdc-1.0.5/aisdc/attacks/worst_case_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10176 2023-05-19 21:41:45.000000 aisdc-1.0.5/aisdc/generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-17 12:52:16.000000 aisdc-1.0.5/aisdc/metrics.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/preprocessing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/preprocessing/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/preprocessing/loaders.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/safemodel/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc/safemodel/classifiers/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/dp_svc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7620 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/new_model_template.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7221 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-05-02 15:16:25.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safekeras.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6347 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-05-11 14:01:54.000000 aisdc-1.0.5/aisdc/safemodel/classifiers/safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/reporting.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.5/aisdc/safemodel/rules.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    30820 2023-05-23 09:33:16.000000 aisdc-1.0.5/aisdc/safemodel/safemodel.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.085487 aisdc-1.0.5/aisdc.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1484 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      181 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-06-05 20:43:21.000000 aisdc-1.0.5/aisdc.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-06-05 20:43:21.089487 aisdc-1.0.5/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1879 2023-06-05 20:27:42.000000 aisdc-1.0.5/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-05 20:43:21.089487 aisdc-1.0.5/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-05-02 15:16:25.000000 aisdc-1.0.5/tests/test_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_attacks_dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_attacks_via_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_attribute_inference_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_data_interface.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5595 2023-05-17 12:52:16.000000 aisdc-1.0.5/tests/test_failfast.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6782 2023-05-19 21:41:45.000000 aisdc-1.0.5/tests/test_generate_report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8107 2023-06-05 19:25:56.000000 aisdc-1.0.5/tests/test_lira_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_loaders.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.5/tests/test_metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safekeras2.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16955 2023-05-23 09:33:17.000000 aisdc-1.0.5/tests/test_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11863 2023-05-17 12:52:16.000000 aisdc-1.0.5/tests/test_saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.5/tests/test_safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13595 2023-05-25 09:59:37.000000 aisdc-1.0.5/tests/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.5.post1/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5005 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-17 12:52:16.000000 aisdc-1.0.5.post1/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      977 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/aisdc/attacks/attribute_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2166 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3616 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26233 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/likelihood_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12913 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    30917 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/attacks/worst_case_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10176 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-17 12:52:16.000000 aisdc-1.0.5.post1/aisdc/metrics.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/preprocessing/loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/dp_svc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7620 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/new_model_template.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7221 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-06-21 12:33:24.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safekeras.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6347 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-05-11 14:01:54.000000 aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/reporting.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/aisdc/safemodel/rules.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    30820 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/aisdc/safemodel/safemodel.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/aisdc.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5005 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1484 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      186 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-06-29 10:47:39.000000 aisdc-1.0.5.post1/aisdc.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1890 2023-06-29 10:47:14.000000 aisdc-1.0.5.post1/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-29 10:47:39.487583 aisdc-1.0.5.post1/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attacks_dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attacks_via_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_attribute_inference_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_data_interface.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5595 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_failfast.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6782 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8107 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_lira_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_loaders.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.5.post1/tests/test_metrics.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-06-29 10:39:36.000000 aisdc-1.0.5.post1/tests/test_safekeras2.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16955 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11863 2023-05-17 12:52:16.000000 aisdc-1.0.5.post1/tests/test_saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.5.post1/tests/test_safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13595 2023-06-29 10:39:50.000000 aisdc-1.0.5.post1/tests/test_worst_case_attack.py
```

### Comparing `aisdc-1.0.5/LICENSE` & `aisdc-1.0.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/PKG-INFO` & `aisdc-1.0.5.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.5
+Version: 1.0.5.post1
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.5/README.md` & `aisdc-1.0.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/attack.py` & `aisdc-1.0.5.post1/aisdc/attacks/attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/attribute_attack.py` & `aisdc-1.0.5.post1/aisdc/attacks/attribute_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/dataset.py` & `aisdc-1.0.5.post1/aisdc/attacks/dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/failfast.py` & `aisdc-1.0.5.post1/aisdc/attacks/failfast.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/likelihood_attack.py` & `aisdc-1.0.5.post1/aisdc/attacks/likelihood_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/report.py` & `aisdc-1.0.5.post1/aisdc/attacks/report.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/attacks/worst_case_attack.py` & `aisdc-1.0.5.post1/aisdc/attacks/worst_case_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/generate_report.py` & `aisdc-1.0.5.post1/aisdc/generate_report.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/metrics.py` & `aisdc-1.0.5.post1/aisdc/metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/preprocessing/loaders.py` & `aisdc-1.0.5.post1/aisdc/preprocessing/loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/dp_svc.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/dp_svc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/new_model_template.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/new_model_template.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/safekeras.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safekeras.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/saferandomforestclassifier.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/saferandomforestclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/safesvc.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/classifiers/safetf.py` & `aisdc-1.0.5.post1/aisdc/safemodel/classifiers/safetf.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/reporting.py` & `aisdc-1.0.5.post1/aisdc/safemodel/reporting.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/rules.json` & `aisdc-1.0.5.post1/aisdc/safemodel/rules.json`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc/safemodel/safemodel.py` & `aisdc-1.0.5.post1/aisdc/safemodel/safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/aisdc.egg-info/PKG-INFO` & `aisdc-1.0.5.post1/aisdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.5
+Version: 1.0.5.post1
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aisdc-1.0.5/aisdc.egg-info/SOURCES.txt` & `aisdc-1.0.5.post1/aisdc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/setup.py` & `aisdc-1.0.5.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="aisdc",
-    version="1.0.5",
+    version="1.0.5.post1",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="Tools for the statistical disclosure control of machine learning models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/AI-SDC",
     packages=find_packages(exclude=["tests"]),
     package_data={"aisdc.safemodel": ["rules.json"]},
     python_requires=">=3.8,<3.11",
     install_requires=[
         "dictdiffer~=0.9.0",
         "fpdf~=1.7.2",
-        "joblib~=1.1.0",
+        "joblib~=1.1.1",
         "multiprocess~=0.70.12.2",
-        "numpy~=1.21",
-        "pandas~=1.5.0",
-        "scikit_learn~=1.1.2",
-        "scipy~=1.7",
-        "tensorflow~=2.10.0",
-        "tensorflow_privacy~=0.8.7",
+        "numpy~=1.22.0",
+        "pandas~=1.5.3",
+        "scikit_learn~=1.1.3",
+        "scipy~=1.9.0",
+        "tensorflow~=2.12.0",
+        "tensorflow_privacy==0.8.10",
         "uuid~=1.30",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

### Comparing `aisdc-1.0.5/tests/test_attacks.py` & `aisdc-1.0.5.post1/tests/test_attacks.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_attacks_dataset.py` & `aisdc-1.0.5.post1/tests/test_attacks_dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_attacks_via_safemodel.py` & `aisdc-1.0.5.post1/tests/test_attacks_via_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_attribute_inference_attack.py` & `aisdc-1.0.5.post1/tests/test_attribute_inference_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_data_interface.py` & `aisdc-1.0.5.post1/tests/test_data_interface.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_failfast.py` & `aisdc-1.0.5.post1/tests/test_failfast.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_generate_report.py` & `aisdc-1.0.5.post1/tests/test_generate_report.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_lira_attack.py` & `aisdc-1.0.5.post1/tests/test_lira_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_loaders.py` & `aisdc-1.0.5.post1/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_metrics.py` & `aisdc-1.0.5.post1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_safedecisiontreeclassifier.py` & `aisdc-1.0.5.post1/tests/test_safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_safekeras2.py` & `aisdc-1.0.5.post1/tests/test_safekeras2.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_safemodel.py` & `aisdc-1.0.5.post1/tests/test_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_saferandomforestclassifier.py` & `aisdc-1.0.5.post1/tests/test_saferandomforestclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_safesvc.py` & `aisdc-1.0.5.post1/tests/test_safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.5/tests/test_worst_case_attack.py` & `aisdc-1.0.5.post1/tests/test_worst_case_attack.py`

 * *Files identical despite different names*

