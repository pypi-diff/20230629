# Comparing `tmp/nkululeko-0.49.1.tar.gz` & `tmp/nkululeko-0.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.49.1.tar", last modified: Wed Jun 21 19:55:50 2023, max compression
+gzip compressed data, was "nkululeko-0.50.0.tar", last modified: Thu Jun 29 12:06:41 2023, max compression
```

## Comparing `nkululeko-0.49.1.tar` & `nkululeko-0.50.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-21 19:55:50.056225 nkululeko-0.49.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6650 2023-06-21 16:22:54.000000 nkululeko-0.49.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.49.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18376 2023-06-21 19:55:50.056225 nkululeko-0.49.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.49.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-21 19:55:50.056225 nkululeko-0.49.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.49.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-06-19 14:49:48.000000 nkululeko-0.49.1/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2404 2023-06-21 11:09:59.000000 nkululeko-0.49.1/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.49.1/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.49.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-21 16:22:17.000000 nkululeko-0.49.1/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21705 2023-06-15 08:31:25.000000 nkululeko-0.49.1/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.49.1/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.49.1/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.49.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.49.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21183 2023-06-21 16:22:07.000000 nkululeko-0.49.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.49.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.49.1/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.49.1/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.49.1/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.49.1/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.49.1/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.49.1/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3756 2023-06-14 15:21:48.000000 nkululeko-0.49.1/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.49.1/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3012 2023-06-14 15:21:48.000000 nkululeko-0.49.1/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.49.1/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.49.1/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.49.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.49.1/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-21 11:41:47.000000 nkululeko-0.49.1/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.49.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.49.1/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.49.1/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.49.1/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.49.1/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.49.1/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.49.1/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.49.1/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.49.1/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.49.1/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.49.1/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.49.1/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.49.1/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.49.1/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.49.1/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.49.1/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.49.1/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.49.1/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.49.1/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.49.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.49.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2659 2023-06-21 11:28:55.000000 nkululeko-0.49.1/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-21 11:03:40.000000 nkululeko-0.49.1/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.49.1/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.49.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.49.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.49.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.49.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.49.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.49.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8831 2023-06-21 16:07:18.000000 nkululeko-0.49.1/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-21 19:55:50.056225 nkululeko-0.49.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18376 2023-06-21 19:55:50.000000 nkululeko-0.49.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-06-21 19:55:50.000000 nkululeko-0.49.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-21 19:55:50.000000 nkululeko-0.49.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-21 19:55:50.000000 nkululeko-0.49.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-21 19:55:50.000000 nkululeko-0.49.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.49.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-21 19:55:50.060225 nkululeko-0.49.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.49.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-29 12:06:41.921223 nkululeko-0.50.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6757 2023-06-29 11:58:53.000000 nkululeko-0.50.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.50.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18483 2023-06-29 12:06:41.921223 nkululeko-0.50.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.50.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-29 12:06:41.921223 nkululeko-0.50.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.50.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2404 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.50.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.50.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-29 11:57:42.000000 nkululeko-0.50.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21705 2023-06-23 11:40:37.000000 nkululeko-0.50.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.50.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.50.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.50.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.50.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21183 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.50.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.50.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.50.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.50.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.50.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.50.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.50.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.50.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.50.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.50.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.50.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.50.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.50.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.50.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.50.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.50.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.50.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.50.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10587 2023-06-29 11:42:43.000000 nkululeko-0.50.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.50.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.50.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.50.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.50.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.50.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.50.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.50.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.50.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.50.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.50.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.50.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.50.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.50.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-06-23 11:40:37.000000 nkululeko-0.50.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.50.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.50.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2659 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.50.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.50.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-06-23 11:40:37.000000 nkululeko-0.50.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.50.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.50.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.50.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.50.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9644 2023-06-29 11:29:44.000000 nkululeko-0.50.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-29 12:06:41.921223 nkululeko-0.50.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18483 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.50.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-29 12:06:41.921223 nkululeko-0.50.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.50.0/setup.py
```

### Comparing `nkululeko-0.49.1/CHANGELOG.md` & `nkululeko-0.50.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.50.0
+--------------
+* removed loso and added pre-selected logo (leave-one-group-out), aka folds
+
 Version 0.49.1
 --------------
 * bugfix: samples selection for augmentation didn't work
 
 Version 0.49.0
 --------------
 * added random-splicing
```

### Comparing `nkululeko-0.49.1/LICENSE` & `nkululeko-0.50.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/PKG-INFO` & `nkululeko-0.50.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.49.1
+Version: 0.50.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.50.0
+--------------
+* removed loso and added pre-selected logo (leave-one-group-out), aka folds
+
 Version 0.49.1
 --------------
 * bugfix: samples selection for augmentation didn't work
 
 Version 0.49.0
 --------------
 * added random-splicing
```

### Comparing `nkululeko-0.49.1/README.md` & `nkululeko-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/augment.py` & `nkululeko-0.50.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/augmenter.py` & `nkululeko-0.50.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/cacheddataset.py` & `nkululeko-0.50.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/dataset.py` & `nkululeko-0.50.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/dataset_csv.py` & `nkululeko-0.50.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/dataset_ravdess.py` & `nkululeko-0.50.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/demo.py` & `nkululeko-0.50.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/demo_predictor.py` & `nkululeko-0.50.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/experiment.py` & `nkululeko-0.50.0/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/explore.py` & `nkululeko-0.50.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_analyser.py` & `nkululeko-0.50.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_audmodel.py` & `nkululeko-0.50.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.50.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_clap.py` & `nkululeko-0.50.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_import.py` & `nkululeko-0.50.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_mld.py` & `nkululeko-0.50.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_opensmile.py` & `nkululeko-0.50.0/nkululeko/feats_opensmile.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,16 @@
                 self.df.index = self.df.index.droplevel(1)
             self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'False'
             except KeyError:
                 pass
         else:
-            self.util.debug('reusing extracted OS features.')
-            self.df = pd.read_pickle(storage)
-
+            self.util.debug(f'reusing extracted OS features: {storage}.')
+            self.df = self.util.get_store(storage, store_format)
 
     def extract_sample(self, signal, sr):
         smile = opensmile.Smile(
                 feature_set=self.feature_set,
                 feature_level=opensmile.FeatureLevel.Functionals,)
         feats = smile.process_signal(signal, sr)
         return feats.to_numpy()
```

### Comparing `nkululeko-0.49.1/nkululeko/feats_oxbow.py` & `nkululeko-0.50.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_praat.py` & `nkululeko-0.50.0/nkululeko/feats_praat.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
             self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'false'
             except KeyError:
                 pass
         else:
-            self.util.debug('reusing extracted Praat features.')
+            self.util.debug(f'reusing extracted Praat features: {storage}.')
             self.df = self.util.get_store(storage, store_format)
         self.util.debug(f'praat feature names: {self.df.columns}')
         self.df = self.df.astype(float)
 
 
 
     def extract_sample(self, signal, sr):
```

### Comparing `nkululeko-0.49.1/nkululeko/feats_trill.py` & `nkululeko-0.50.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feats_wav2vec2.py` & `nkululeko-0.50.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feature_extractor.py` & `nkululeko-0.50.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/featureset.py` & `nkululeko-0.50.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/feinberg_praat.py` & `nkululeko-0.50.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/filter_data.py` & `nkululeko-0.50.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/loss_ccc.py` & `nkululeko-0.50.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/loss_softf1loss.py` & `nkululeko-0.50.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model.py` & `nkululeko-0.50.0/nkululeko/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
         self.df_train, self.df_test, self.feats_train, self.feats_test = df_train, df_test, feats_train, feats_test
         self.util = Util()
         self.target = self.util.config_val('DATA', 'target', 'emotion')
         self.run = 0
         self.epoch = 0
-        self.loso = self.util.config_val('MODEL', 'loso', False)
         self.logo = self.util.config_val('MODEL', 'logo', False)
         self.xfoldx = self.util.config_val('MODEL', 'k_fold_cross', False)
                 
     def set_testdata(self, data_df, feats_df):
         self.df_test, self.feats_test = data_df, feats_df
 
     def reset_test(self,  df_test, feats_test):
@@ -39,18 +38,18 @@
         self.epoch = epoch
         dir = self.util.get_path('model_dir')
         name = f'{self.util.get_exp_name(only_train=True)}_{self.run}_{self.epoch:03d}.model'
         self.store_path = dir+name
 
 
     def _x_fold_cross(self):
-        # ignore train and test sets and do a "leave one speaker out"  evaluation
+        # ignore train and test sets and do a x-fold-cross  evaluation
         self.util.debug(f'ignoring splits and doing {self.xfoldx} fold cross validation')
-        feats = self.feats_train.append(self.feats_test)
-        annos = self.df_train.append(self.df_test)
+        feats = pd.concat([self.feats_train, self.feats_test])
+        annos = pd.concat([self.df_train, self.df_test])
         targets = annos[self.target]
         _skf = StratifiedKFold(n_splits=int(self.xfoldx))
         truths, preds, results = [], [], []
         g_index = 0
         # leave-one-speaker loop    
         for train_index, test_index in _skf.split(
             feats, 
@@ -77,80 +76,46 @@
             index=truth.index,
             name='prediction',
         )
         self.truths = truth
         self.preds = pred        
         results = np.asarray(results)
         self.util.debug(f'KFOLD: {self.xfoldx} folds: mean {results.mean():.3f}, std: {results.std():.3f}')
-
-    def _loso(self):
-        # ignore train and test sets and do a "leave one speaker out"  evaluation
-        self.util.debug('ignoring splits and doing LOSO')
-        feats = self.feats_train.append(self.feats_test)
-        annos = self.df_train.append(self.df_test)
-        targets = annos[self.target]
-        _logo = LeaveOneGroupOut()
-        truths, preds, results = [], [], []
-        speakers = annos['speaker']
-        g_index = 0
-        # leave-one-speaker loop    
-        for train_index, test_index in _logo.split(
-            feats, 
-            targets, 
-            groups=speakers,
-        ):
-            train_x = feats.iloc[train_index].to_numpy()
-            train_y = targets[train_index]
-            self.clf.fit(train_x, train_y)
-            
-            truth_x = feats.iloc[test_index].to_numpy()
-            truth_y = targets[test_index]
-            predict_y = self.clf.predict(truth_x)
-            report = Reporter(truth_y.astype(float), predict_y, self.run, self.epoch)
-            self.util.debug(f'result for speaker {g_index}: {report.get_result().get_test_result()} ')
-            truths.append(truth_y)
-            preds.append(predict_y)
-            g_index += 1
-            results.append(float(report.get_result().test))            
-        # combine speaker folds
-        truth = pd.concat(truths)
-        truth.name = 'truth'
-        pred = pd.Series(
-            np.concatenate(preds),
-            index=truth.index,
-            name='prediction',
-        )
-        self.truths = truth
-        self.preds = pred        
-        results = np.asarray(results)
-        self.util.debug(f'LOSO: {self.loso} folds: mean {results.mean():.3f}, std: {results.std():.3f}')
-
     def _do_logo(self):
         # ignore train and test sets and do a "leave one speaker group out"  evaluation
-        self.util.debug('ignoring splits and doing LOSGO')
-        feats = self.feats_train.append(self.feats_test)
-        annos = self.df_train.append(self.df_test)
+        self.util.debug(f'ignoring splits and doing LOGO with {self.logo} groups')
+        logo = int(self.logo)
+        feats = pd.concat([self.feats_train, self.feats_test])
+        annos = pd.concat([self.df_train, self.df_test])
         targets = annos[self.target]
-        _logo = LeaveOneGroupOut()
+        _logo = LeaveOneGroupOut()        
         truths, preds, results = [], [], []
         # get unique list of speakers
         speakers = annos['speaker'].unique()
-        # create a random dictionary of groups
-        sdict = {}
-        for i, s in enumerate(speakers):
-            sdict[s] = random.sample(range(int(self.logo)), 1)[0]    
-        # add this to the annotations  
-        annos['speaker_groups'] = annos['speaker'].apply(lambda x: str(sdict[x]))
-        speaker_groups = annos['speaker_groups']
+        # check for folds columns
+        if not 'fold' in annos.columns:
+            self.util.debug(f'creating random folds for {logo} groups') 
+            # create a random dictionary of groups
+            sdict = {}
+            # randomize the speaker order
+            random.shuffle(speakers)
+            folds = list(range(logo))
+            for i, s in enumerate(speakers):
+                sdict[s] = folds[i % len(folds)]    
+            # add this to the annotations  
+            annos['fold'] = annos['speaker'].apply(lambda x: str(sdict[x]))
+        else:
+            fold_count = annos['fold'].nunique()
+            self.util.debug(f'using existing folds for {fold_count} groups')  
         g_index = 0
-        # leave-one-speaker loop    
+        # leave-one-group loop    
         for train_index, test_index in _logo.split(
             feats, 
             targets, 
-            groups=speaker_groups,
+            groups=annos['fold'],
         ):
             train_x = feats.iloc[train_index].to_numpy()
             train_y = targets[train_index]
             self.clf.fit(train_x, train_y)
             
             truth_x = feats.iloc[test_index].to_numpy()
             truth_y = targets[test_index]
@@ -180,18 +145,14 @@
         """Train the model"""
         # # first check if the model already has been trained
         # if os.path.isfile(self.store_path):
         #     self.load(self.run, self.epoch)
         #     self.util.debug(f'reusing model: {self.store_path}')
         #     return
 
-        # first check if leave on  speaker out is wanted
-        if self.loso:
-            self._loso()
-            return
         # then if leave one speaker group out validation is wanted
         if self.logo:
             self._do_logo()
             return
         # then if x fold cross validation is wanted
         if self.xfoldx:
             self._x_fold_cross()
@@ -248,15 +209,15 @@
         predictions =  self.clf.predict(self.feats_test.to_numpy())
         return predictions
 
     def predict(self):
         if self.feats_test.isna().to_numpy().any():
             self.util.debug(f'Model, test: replacing {self.feats_test.isna().sum().sum()} NANs with 0')
             self.feats_test = self.feats_test.fillna(0)
-        if self.loso or self.logo or self.xfoldx:
+        if self.logo or self.xfoldx:
             report = Reporter(self.truths.astype(float), self.preds, self.run, self.epoch)
             return report
         """Predict the whole eval feature set"""
         predictions = self.get_predictions()
         report = Reporter(self.df_test[self.target]\
             .to_numpy().astype(float), predictions, self.run, self.epoch)
         return report
```

### Comparing `nkululeko-0.49.1/nkululeko/model_cnn.py` & `nkululeko-0.50.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model_gmm.py` & `nkululeko-0.50.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model_knn.py` & `nkululeko-0.50.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model_knn_reg.py` & `nkululeko-0.50.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model_mlp.py` & `nkululeko-0.50.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model_mlp_regression.py` & `nkululeko-0.50.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/model_svm.py` & `nkululeko-0.50.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/modelrunner.py` & `nkululeko-0.50.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/nkululeko.py` & `nkululeko-0.50.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/plots.py` & `nkululeko-0.50.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/randomsplicer.py` & `nkululeko-0.50.0/nkululeko/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/randomsplicing.py` & `nkululeko-0.50.0/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/reporter.py` & `nkululeko-0.50.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/runmanager.py` & `nkululeko-0.50.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/scaler.py` & `nkululeko-0.50.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.50.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/test.py` & `nkululeko-0.50.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/test_predictor.py` & `nkululeko-0.50.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/nkululeko/util.py` & `nkululeko-0.50.0/nkululeko/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,14 +96,20 @@
     def make_segmented_index(self, df):
         if len(df)==0:
             return df
         if not isinstance(df.index, pd.MultiIndex):
             df.index = audformat.utils.to_segmented_index(df.index, allow_nat=False)
         return df
 
+    def _get_value_descript(self, section, name):
+        if self.config_val(section, name, False):
+            val = self.config_val(section, name, False)
+            return f'_{name}-{str(val)}'
+        return ''
+
     def get_exp_name(self, only_train = False, only_data = False):
         if only_train:
             # try to get only the train tables
             trains_val = self.config_val('DATA', 'trains', False)
             if trains_val:
                 ds = '_'.join(ast.literal_eval(glob_conf.config['DATA']['trains']))
             else:
@@ -116,36 +122,46 @@
             mt = f'_{glob_conf.config["MODEL"]["type"]}'
         ft = '_'.join(ast.literal_eval(glob_conf.config['FEATS']['type']))
         ft += '_'
         set = self.config_val('FEATS', 'set', False)
         set_string = ''
         if set:
             set_string += set
-        lr_string = ''
-        if self.config_val('MODEL', 'learning_rate', False) and not only_data:
-            lr = self.config_val('MODEL', 'learning_rate', False)
-            lr_string = f'_lr-{str(lr)}'
-        loss_string = ''
-        if self.config_val('MODEL', 'loss', False) and not only_data:
-            loss = self.config_val('MODEL', 'loss', False)
-            loss_string = f'_loss-{loss}'
-        drop_string = ''
-        if self.config_val('MODEL', 'drop', False) and not only_data:
-            drop = self.config_val('MODEL', 'drop', False)
-            drop_string = f'_drop-{str(drop)}'
+        # lr_string = ''
+        # if self.config_val('MODEL', 'learning_rate', False) and not only_data:
+        #     lr = self.config_val('MODEL', 'learning_rate', False)
+        #     lr_string = f'_lr-{str(lr)}'
+        # logo_string = ''
+        # if self.config_val('MODEL', 'logo', False):
+        #     logo = self.config_val('MODEL', 'logo', False)
+        #     logo_string = f'_logo-{str(logo)}'
+        # loss_string = ''
+        # if self.config_val('MODEL', 'loss', False) and not only_data:
+        #     loss = self.config_val('MODEL', 'loss', False)
+        #     loss_string = f'_loss-{loss}'
+        # drop_string = ''
+        # if self.config_val('MODEL', 'drop', False) and not only_data:
+        #     drop = self.config_val('MODEL', 'drop', False)
+        #     drop_string = f'_drop-{str(drop)}'
         layer_string = ''
         layer_s = self.config_val('MODEL', 'layers', False)
         if layer_s and not only_data:
             layers = ast.literal_eval(layer_s)
             sorted_layers = sorted(layers.items(), key=lambda x: x[1])
             for l in sorted_layers:
                 layer_string += f'{str(l[1])}-'
         return_string = f'{ds}{mt}_{ft}{set_string}'\
-            f'{layer_string[:-1]}{lr_string}{drop_string}{loss_string}'.replace('__','')
-        return return_string
+            f'{layer_string[:-1]}'
+        options = [['MODEL', 'drop'], ['MODEL', 'loss'], ['MODEL', 'logo'], 
+                   ['MODEL', 'learning_rate'],  ['MODEL', 'k_fold_cross']]
+        for option in options:
+            return_string += self._get_value_descript(option[0], option[1])
+        # return_string = f'{ds}{mt}_{ft}{set_string}'\
+        #     f'{layer_string[:-1]}{lr_string}{drop_string}{loss_string}{logo_string}'.replace('__','')
+        return return_string.replace('__','')
 
     def get_plot_name(self):
         try:
             plot_name = glob_conf.config['PLOT']['name']
         except KeyError:
             plot_name = self.get_exp_name()
         return plot_name
```

### Comparing `nkululeko-0.49.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.50.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.49.1
+Version: 0.50.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.50.0
+--------------
+* removed loso and added pre-selected logo (leave-one-group-out), aka folds
+
 Version 0.49.1
 --------------
 * bugfix: samples selection for augmentation didn't work
 
 Version 0.49.0
 --------------
 * added random-splicing
```

### Comparing `nkululeko-0.49.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.50.0/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.49.1/setup.cfg` & `nkululeko-0.50.0/setup.cfg`

 * *Files identical despite different names*

