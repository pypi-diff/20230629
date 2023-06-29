# Comparing `tmp/MultiEL-0.4.tar.gz` & `tmp/MultiEL-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultiEL-0.4.tar", last modified: Thu Jun 29 11:30:02 2023, max compression
+gzip compressed data, was "MultiEL-0.5.tar", last modified: Thu Jun 29 12:24:53 2023, max compression
```

## Comparing `MultiEL-0.4.tar` & `MultiEL-0.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.929386 MultiEL-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 11:29:49.000000 MultiEL-0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/MultiEL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 11:30:02.000000 MultiEL-0.4/MultiEL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-29 11:30:02.000000 MultiEL-0.4/MultiEL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:30:02.000000 MultiEL-0.4/MultiEL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:30:02.000000 MultiEL-0.4/MultiEL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 11:30:02.000000 MultiEL-0.4/MultiEL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 11:30:02.000000 MultiEL-0.4/MultiEL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 11:30:02.929386 MultiEL-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-29 11:29:49.000000 MultiEL-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/checkpoint_callback/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/checkpoint_callback/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/datamodule/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/datamodule/joint_el_datamodule.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_aida.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_disambiguation_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_disambiguation_mel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_disambiguation_mel_new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_disambiguation_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_eval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel_new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel_new_aida.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel_new_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel_new_index_tackbp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/joint_el_mel_new_mewsli.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/task/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/joint_el_task.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/task/model/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/model/bert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/model/xlmr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/model/xlmr_large.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/task/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/optim/adamw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.913384 MultiEL-0.4/bela/conf/task/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/transform/joint_el_bert_transform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/transform/joint_el_xlmr_raw_transform_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/transform/joint_el_xlmr_transform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/task/transform/joint_el_xlmr_transform_large.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.917385 MultiEL-0.4/bela/conf/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/trainer/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/trainer/gpu_1_host.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/conf/trainer/slurm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.921385 MultiEL-0.4/bela/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  5069051 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/data/sp_model
--rw-r--r--   0 runner    (1001) docker     (123)  3331313 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/data/vocab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.925385 MultiEL-0.4/bela/datamodule/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/datamodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/datamodule/joint_el_datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.925385 MultiEL-0.4/bela/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/evaluation/model_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.925385 MultiEL-0.4/bela/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/models/hf_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.925385 MultiEL-0.4/bela/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47023 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/task/joint_el_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.925385 MultiEL-0.4/bela/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.925385 MultiEL-0.4/bela/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/tests/data/el_catalogue.idx
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/tests/data/el_matcha_joint.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/tests/test_datamodules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/tests/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.929386 MultiEL-0.4/bela/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/transforms/hf_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    32166 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/transforms/joint_el_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/transforms/sentencepiece_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/transforms/spm_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.929386 MultiEL-0.4/bela/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/utils/analysis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/utils/prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-29 11:29:49.000000 MultiEL-0.4/bela/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:30:02.929386 MultiEL-0.4/multiel/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-29 11:29:49.000000 MultiEL-0.4/multiel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-06-29 11:29:49.000000 MultiEL-0.4/multiel/bela_model.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:30:02.929386 MultiEL-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-29 11:29:49.000000 MultiEL-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.390102 MultiEL-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 12:24:41.000000 MultiEL-0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.370102 MultiEL-0.5/MultiEL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-29 12:24:53.000000 MultiEL-0.5/MultiEL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-29 12:24:53.000000 MultiEL-0.5/MultiEL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:24:53.000000 MultiEL-0.5/MultiEL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:24:53.000000 MultiEL-0.5/MultiEL.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 12:24:53.000000 MultiEL-0.5/MultiEL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 12:24:53.000000 MultiEL-0.5/MultiEL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-29 12:24:53.390102 MultiEL-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 12:24:41.000000 MultiEL-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.370102 MultiEL-0.5/bela/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.374102 MultiEL-0.5/bela/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.374102 MultiEL-0.5/bela/conf/checkpoint_callback/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/checkpoint_callback/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.374102 MultiEL-0.5/bela/conf/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/datamodule/joint_el_datamodule.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_aida.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_disambiguation_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_disambiguation_mel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_disambiguation_mel_new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_disambiguation_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_eval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel_new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel_new_aida.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel_new_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel_new_index_tackbp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/joint_el_mel_new_mewsli.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.374102 MultiEL-0.5/bela/conf/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/joint_el_task.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.378102 MultiEL-0.5/bela/conf/task/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/model/bert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/model/xlmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/model/xlmr_large.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.378102 MultiEL-0.5/bela/conf/task/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/optim/adamw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.378102 MultiEL-0.5/bela/conf/task/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/transform/joint_el_bert_transform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/transform/joint_el_xlmr_raw_transform_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/transform/joint_el_xlmr_transform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/task/transform/joint_el_xlmr_transform_large.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.378102 MultiEL-0.5/bela/conf/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/trainer/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/trainer/gpu_1_host.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/conf/trainer/slurm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.382102 MultiEL-0.5/bela/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  5069051 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/data/sp_model
+-rw-r--r--   0 runner    (1001) docker     (123)  3331313 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/data/vocab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.386102 MultiEL-0.5/bela/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/datamodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/datamodule/joint_el_datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.386102 MultiEL-0.5/bela/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/evaluation/model_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.386102 MultiEL-0.5/bela/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/models/hf_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.386102 MultiEL-0.5/bela/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47023 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/task/joint_el_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.386102 MultiEL-0.5/bela/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.386102 MultiEL-0.5/bela/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/tests/data/el_catalogue.idx
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/tests/data/el_matcha_joint.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/tests/test_datamodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.390102 MultiEL-0.5/bela/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/transforms/hf_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32166 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/transforms/joint_el_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/transforms/sentencepiece_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/transforms/spm_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.390102 MultiEL-0.5/bela/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/utils/analysis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/utils/prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-29 12:24:41.000000 MultiEL-0.5/bela/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:24:53.390102 MultiEL-0.5/multiel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-29 12:24:41.000000 MultiEL-0.5/multiel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-06-29 12:24:41.000000 MultiEL-0.5/multiel/bela_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:24:53.390102 MultiEL-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-29 12:24:41.000000 MultiEL-0.5/setup.py
```

### Comparing `MultiEL-0.4/LICENSE` & `MultiEL-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/MultiEL.egg-info/PKG-INFO` & `MultiEL-0.5/MultiEL.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiEL
-Version: 0.4
+Version: 0.5
 Summary: Multilingual Entity Linking model by BELA model
 Home-page: https://github.com/wannaphong/MultiEL
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/MultiEL
 Project-URL: Bug Reports, https://github.com/wannaphong/MultiEL/issues
@@ -40,7 +40,44 @@
 ```python
 from multiel import BELA
 
 bela_run = BELA(device="cuda")
 
 print(bela_run.process_batch(["นายกประยุทธ์ประกาศจัดการเลือกตั้ง"]))
 ```
+
+output:
+```python
+[{'offsets': [0], 'lengths': [12], 'entities': ['Q2108126'], 'md_scores': [0.22365164756774902], 'el_scores': [0.6967974901199341]}]
+```
+
+#### API
+
+```python
+from multiel import BELA
+
+BELA(
+ md_threshold:float=0.2,
+ el_threshold:float=0.4, 
+ checkpoint_name: str="wiki", 
+ device: str="cuda:0",
+ config_name:str="joint_el_mel_new",
+ repo:str="wannaphong/BELA"
+)
+```
+
+- md_threshold: md threshold
+- el_threshold: Entity Linking threshold
+- checkpoint_name: checkpoint name (wiki, aida, mewsli, and e2e) or your file name with extension
+- device: device
+- config_name: config name (in the BELA project)
+- repo: Huggingface Hub repo (Default [wannaphong/BELA](https://huggingface.co/wannaphong/BELA))
+
+**Predict**
+
+```python
+BELA.process_batch([str, str])
+```
+
+## License
+
+MIT license and the model is MIT license. ([BELA is MIT licensed](https://github.com/facebookresearch/BELA/blob/main/LICENSE))
```

### Comparing `MultiEL-0.4/MultiEL.egg-info/SOURCES.txt` & `MultiEL-0.5/MultiEL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/PKG-INFO` & `MultiEL-0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiEL
-Version: 0.4
+Version: 0.5
 Summary: Multilingual Entity Linking model by BELA model
 Home-page: https://github.com/wannaphong/MultiEL
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/MultiEL
 Project-URL: Bug Reports, https://github.com/wannaphong/MultiEL/issues
@@ -40,7 +40,44 @@
 ```python
 from multiel import BELA
 
 bela_run = BELA(device="cuda")
 
 print(bela_run.process_batch(["นายกประยุทธ์ประกาศจัดการเลือกตั้ง"]))
 ```
+
+output:
+```python
+[{'offsets': [0], 'lengths': [12], 'entities': ['Q2108126'], 'md_scores': [0.22365164756774902], 'el_scores': [0.6967974901199341]}]
+```
+
+#### API
+
+```python
+from multiel import BELA
+
+BELA(
+ md_threshold:float=0.2,
+ el_threshold:float=0.4, 
+ checkpoint_name: str="wiki", 
+ device: str="cuda:0",
+ config_name:str="joint_el_mel_new",
+ repo:str="wannaphong/BELA"
+)
+```
+
+- md_threshold: md threshold
+- el_threshold: Entity Linking threshold
+- checkpoint_name: checkpoint name (wiki, aida, mewsli, and e2e) or your file name with extension
+- device: device
+- config_name: config name (in the BELA project)
+- repo: Huggingface Hub repo (Default [wannaphong/BELA](https://huggingface.co/wannaphong/BELA))
+
+**Predict**
+
+```python
+BELA.process_batch([str, str])
+```
+
+## License
+
+MIT license and the model is MIT license. ([BELA is MIT licensed](https://github.com/facebookresearch/BELA/blob/main/LICENSE))
```

### Comparing `MultiEL-0.4/bela/conf/config.py` & `MultiEL-0.5/bela/conf/config.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el.yaml` & `MultiEL-0.5/bela/conf/joint_el.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_aida.yaml` & `MultiEL-0.5/bela/conf/joint_el_aida.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_disambiguation_large.yaml` & `MultiEL-0.5/bela/conf/joint_el_disambiguation_large.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_disambiguation_mel.yaml` & `MultiEL-0.5/bela/conf/joint_el_disambiguation_mel.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_disambiguation_mel_new.yaml` & `MultiEL-0.5/bela/conf/joint_el_disambiguation_mel_new.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_disambiguation_only.yaml` & `MultiEL-0.5/bela/conf/joint_el_disambiguation_only.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_eval.yaml` & `MultiEL-0.5/bela/conf/joint_el_eval.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel_new.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel_new.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel_new_aida.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel_new_aida.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel_new_index.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel_new_index.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel_new_index_tackbp.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel_new_index_tackbp.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/joint_el_mel_new_mewsli.yaml` & `MultiEL-0.5/bela/conf/joint_el_mel_new_mewsli.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/conf/trainer/slurm.yaml` & `MultiEL-0.5/bela/conf/trainer/slurm.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/data/sp_model` & `MultiEL-0.5/bela/data/sp_model`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/data/vocab` & `MultiEL-0.5/bela/data/vocab`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/datamodule/joint_el_datamodule.py` & `MultiEL-0.5/bela/datamodule/joint_el_datamodule.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/evaluation/model_eval.py` & `MultiEL-0.5/bela/evaluation/model_eval.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/models/hf_encoder.py` & `MultiEL-0.5/bela/models/hf_encoder.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/task/joint_el_task.py` & `MultiEL-0.5/bela/task/joint_el_task.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/tests/test_datamodules.py` & `MultiEL-0.5/bela/tests/test_datamodules.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/tests/test_models.py` & `MultiEL-0.5/bela/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/tests/test_transforms.py` & `MultiEL-0.5/bela/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/transforms/hf_transform.py` & `MultiEL-0.5/bela/transforms/hf_transform.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/transforms/joint_el_transform.py` & `MultiEL-0.5/bela/transforms/joint_el_transform.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/transforms/sentencepiece_pb2.py` & `MultiEL-0.5/bela/transforms/sentencepiece_pb2.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/transforms/spm_transform.py` & `MultiEL-0.5/bela/transforms/spm_transform.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/utils/analysis_utils.py` & `MultiEL-0.5/bela/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/bela/utils/prediction_utils.py` & `MultiEL-0.5/bela/utils/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/multiel/__init__.py` & `MultiEL-0.5/multiel/__init__.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/multiel/bela_model.py` & `MultiEL-0.5/multiel/bela_model.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.4/setup.py` & `MultiEL-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 with open("requirements.txt","r",encoding="utf-8-sig") as f:
     requirements = [i.strip() for i in f.readlines()]
 
 setup(
     name="MultiEL",
-    version="0.4",
+    version="0.5",
     description="Multilingual Entity Linking model by BELA model",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/MultiEL",
     packages=["multiel", "bela"],
```

