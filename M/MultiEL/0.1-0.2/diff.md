# Comparing `tmp/MultiEL-0.1.tar.gz` & `tmp/MultiEL-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultiEL-0.1.tar", last modified: Thu Jun 29 09:42:36 2023, max compression
+gzip compressed data, was "MultiEL-0.2.tar", last modified: Thu Jun 29 09:59:52 2023, max compression
```

## Comparing `MultiEL-0.1.tar` & `MultiEL-0.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.781052 MultiEL-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 09:42:21.000000 MultiEL-0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/MultiEL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 09:42:36.000000 MultiEL-0.1/MultiEL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-29 09:42:36.000000 MultiEL-0.1/MultiEL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:42:36.000000 MultiEL-0.1/MultiEL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:42:36.000000 MultiEL-0.1/MultiEL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-29 09:42:36.000000 MultiEL-0.1/MultiEL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 09:42:36.000000 MultiEL-0.1/MultiEL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 09:42:36.781052 MultiEL-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-29 09:42:21.000000 MultiEL-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/checkpoint_callback/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/checkpoint_callback/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/datamodule/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/datamodule/joint_el_datamodule.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_aida.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_disambiguation_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_disambiguation_mel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_disambiguation_mel_new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_disambiguation_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_eval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel_new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel_new_aida.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel_new_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel_new_index_tackbp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/joint_el_mel_new_mewsli.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/task/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/joint_el_task.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/task/model/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/model/bert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/model/xlmr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/model/xlmr_large.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/task/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/optim/adamw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/task/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/transform/joint_el_bert_transform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/transform/joint_el_xlmr_raw_transform_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/transform/joint_el_xlmr_transform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/task/transform/joint_el_xlmr_transform_large.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.769052 MultiEL-0.1/bela/conf/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/trainer/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/trainer/gpu_1_host.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/conf/trainer/slurm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.777052 MultiEL-0.1/bela/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5069051 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/data/sp_model
--rw-r--r--   0 runner    (1001) docker     (123)  3331313 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/data/vocab
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.765052 MultiEL-0.1/bela/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.781052 MultiEL-0.1/bela/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/tests/data/el_catalogue.idx
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 09:42:21.000000 MultiEL-0.1/bela/tests/data/el_matcha_joint.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:42:36.781052 MultiEL-0.1/multiel/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-29 09:42:21.000000 MultiEL-0.1/multiel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-06-29 09:42:21.000000 MultiEL-0.1/multiel/bela_model.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:42:36.781052 MultiEL-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-29 09:42:21.000000 MultiEL-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.983152 MultiEL-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 09:59:34.000000 MultiEL-0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.963152 MultiEL-0.2/MultiEL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 09:59:52.000000 MultiEL-0.2/MultiEL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-29 09:59:52.000000 MultiEL-0.2/MultiEL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:59:52.000000 MultiEL-0.2/MultiEL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:59:52.000000 MultiEL-0.2/MultiEL.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-29 09:59:52.000000 MultiEL-0.2/MultiEL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 09:59:52.000000 MultiEL-0.2/MultiEL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 09:59:52.983152 MultiEL-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-29 09:59:34.000000 MultiEL-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.967152 MultiEL-0.2/bela/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/checkpoint_callback/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/checkpoint_callback/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/datamodule/joint_el_datamodule.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_aida.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_disambiguation_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_disambiguation_mel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_disambiguation_mel_new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_disambiguation_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_eval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel_new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel_new_aida.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel_new_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel_new_index_tackbp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/joint_el_mel_new_mewsli.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/joint_el_task.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/task/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/model/bert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/model/xlmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/model/xlmr_large.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/task/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/optim/adamw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.971152 MultiEL-0.2/bela/conf/task/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/transform/joint_el_bert_transform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/transform/joint_el_xlmr_raw_transform_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/transform/joint_el_xlmr_transform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/task/transform/joint_el_xlmr_transform_large.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.975152 MultiEL-0.2/bela/conf/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/trainer/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/trainer/gpu_1_host.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/conf/trainer/slurm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.979152 MultiEL-0.2/bela/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  5069051 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/data/sp_model
+-rw-r--r--   0 runner    (1001) docker     (123)  3331313 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/data/vocab
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.963152 MultiEL-0.2/bela/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.983152 MultiEL-0.2/bela/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/tests/data/el_catalogue.idx
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 09:59:34.000000 MultiEL-0.2/bela/tests/data/el_matcha_joint.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:59:52.983152 MultiEL-0.2/multiel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-29 09:59:34.000000 MultiEL-0.2/multiel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-06-29 09:59:34.000000 MultiEL-0.2/multiel/bela_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:59:52.983152 MultiEL-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-29 09:59:34.000000 MultiEL-0.2/setup.py
```

### Comparing `MultiEL-0.1/LICENSE` & `MultiEL-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/MultiEL.egg-info/PKG-INFO` & `MultiEL-0.2/MultiEL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiEL
-Version: 0.1
+Version: 0.2
 Summary: Multilingual Entity Linking model by BELA model
 Home-page: https://github.com/wannaphong/MultiEL
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/MultiEL
 Project-URL: Bug Reports, https://github.com/wannaphong/MultiEL/issues
```

### Comparing `MultiEL-0.1/MultiEL.egg-info/SOURCES.txt` & `MultiEL-0.2/MultiEL.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,13 +35,14 @@
 bela/conf/task/transform/joint_el_bert_transform.yaml
 bela/conf/task/transform/joint_el_xlmr_raw_transform_large.yaml
 bela/conf/task/transform/joint_el_xlmr_transform.yaml
 bela/conf/task/transform/joint_el_xlmr_transform_large.yaml
 bela/conf/trainer/cpu.yaml
 bela/conf/trainer/gpu_1_host.yaml
 bela/conf/trainer/slurm.yaml
+bela/data/__init__.py
 bela/data/sp_model
 bela/data/vocab
 bela/tests/data/el_catalogue.idx
 bela/tests/data/el_matcha_joint.jsonl
 multiel/__init__.py
 multiel/bela_model.py
```

### Comparing `MultiEL-0.1/PKG-INFO` & `MultiEL-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiEL
-Version: 0.1
+Version: 0.2
 Summary: Multilingual Entity Linking model by BELA model
 Home-page: https://github.com/wannaphong/MultiEL
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/MultiEL
 Project-URL: Bug Reports, https://github.com/wannaphong/MultiEL/issues
```

### Comparing `MultiEL-0.1/README.md` & `MultiEL-0.2/README.md`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/config.py` & `MultiEL-0.2/bela/conf/config.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el.yaml` & `MultiEL-0.2/bela/conf/joint_el.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_aida.yaml` & `MultiEL-0.2/bela/conf/joint_el_aida.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_disambiguation_large.yaml` & `MultiEL-0.2/bela/conf/joint_el_disambiguation_large.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_disambiguation_mel.yaml` & `MultiEL-0.2/bela/conf/joint_el_disambiguation_mel.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_disambiguation_mel_new.yaml` & `MultiEL-0.2/bela/conf/joint_el_disambiguation_mel_new.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_disambiguation_only.yaml` & `MultiEL-0.2/bela/conf/joint_el_disambiguation_only.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_eval.yaml` & `MultiEL-0.2/bela/conf/joint_el_eval.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel_new.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel_new.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel_new_aida.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel_new_aida.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel_new_index.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel_new_index.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel_new_index_debug_mention_detection.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel_new_index_tackbp.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel_new_index_tackbp.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/joint_el_mel_new_mewsli.yaml` & `MultiEL-0.2/bela/conf/joint_el_mel_new_mewsli.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/conf/trainer/slurm.yaml` & `MultiEL-0.2/bela/conf/trainer/slurm.yaml`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/data/sp_model` & `MultiEL-0.2/bela/data/sp_model`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/data/vocab` & `MultiEL-0.2/bela/data/vocab`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/bela/main.py` & `MultiEL-0.2/bela/main.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/multiel/__init__.py` & `MultiEL-0.2/multiel/__init__.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/multiel/bela_model.py` & `MultiEL-0.2/multiel/bela_model.py`

 * *Files identical despite different names*

### Comparing `MultiEL-0.1/setup.py` & `MultiEL-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 with open("requirements.txt","r",encoding="utf-8-sig") as f:
     requirements = [i.strip() for i in f.readlines()]
 
 setup(
     name="MultiEL",
-    version="0.1",
+    version="0.2",
     description="Multilingual Entity Linking model by BELA model",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/MultiEL",
     packages=["multiel", "bela"],
```

