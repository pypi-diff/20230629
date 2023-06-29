# Comparing `tmp/zshot-0.0.7.tar.gz` & `tmp/zshot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zshot-0.0.7.tar", last modified: Wed Jan  4 15:23:21 2023, max compression
+gzip compressed data, was "zshot-0.0.8.tar", last modified: Thu Jun 29 16:50:42 2023, max compression
```

## Comparing `zshot-0.0.7.tar` & `zshot-0.0.8.tar`

### file list

```diff
@@ -1,126 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.376684 zshot-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-04 15:23:11.000000 zshot-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-01-04 15:23:21.376684 zshot-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-01-04 15:23:11.000000 zshot-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-04 15:23:21.376684 zshot-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-04 15:23:11.000000 zshot-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.364684 zshot-0.0.7/zshot/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.364684 zshot-0.0.7/zshot/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/evaluation/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/evaluation/dataset/med_mentions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/med_mentions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/med_mentions/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/med_mentions/med_mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/med_mentions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/evaluation/dataset/ontonotes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/ontonotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/ontonotes/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/dataset/ontonotes/onto_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/metrics/rel_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/evaluation/metrics/seqeval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/metrics/seqeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/metrics/seqeval/seqeval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/run_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/evaluation/zshot_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/linker/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_blink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/linker/linker_regen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_regen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_regen/linker_regen.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_regen/trie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_regen/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_smxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/linker/linker_tars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/mentions_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/mentions_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_flair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_smxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_tars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.368684 zshot-0.0.7/zshot/mentions_extractor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/utils/ExtractorType.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/mentions_extractor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/pipeline_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/relation_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/relation_extractor_zsrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/relations_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/relation_extractor/zsrc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/zsrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/zsrc/data_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/zsrc/decide_entity_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/relation_extractor/zsrc/zero_shot_rel_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/evaluation/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/evaluation/test_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/tests/linker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/linker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/linker/test_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/linker/test_regen_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/linker/test_smxm_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/linker/test_tars_linker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/tests/mentions_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/mentions_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/mentions_extractor/test_flair_mentions_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/mentions_extractor/test_mention_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/mentions_extractor/test_smxm_mentions_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/mentions_extractor/test_spacy_mentions_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/mentions_extractor/test_tars_mentions_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/tests/relations_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/relations_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/relations_extractor/test_relations_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/test_zshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/utils/test_displacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/tests/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.372684 zshot-0.0.7/zshot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/alignment_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.376684 zshot-0.0.7/zshot/utils/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/data_models/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/data_models/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/data_models/relation_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/data_models/span.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.376684 zshot-0.0.7/zshot/utils/displacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/displacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/displacy/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/displacy/displacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/displacy/relations_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/displacy/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.376684 zshot-0.0.7/zshot/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.376684 zshot-0.0.7/zshot/utils/models/smxm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/smxm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/smxm/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/smxm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/smxm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.376684 zshot-0.0.7/zshot/utils/models/tars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/tars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/utils/models/tars/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-01-04 15:23:11.000000 zshot-0.0.7/zshot/zshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 15:23:21.364684 zshot-0.0.7/zshot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-01-04 15:23:21.000000 zshot-0.0.7/zshot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-01-04 15:23:21.000000 zshot-0.0.7/zshot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 15:23:21.000000 zshot-0.0.7/zshot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 15:23:21.000000 zshot-0.0.7/zshot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-04 15:23:21.000000 zshot-0.0.7/zshot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-04 15:23:21.000000 zshot-0.0.7/zshot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.303703 zshot-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-29 16:50:30.000000 zshot-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-06-29 16:50:42.303703 zshot-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-29 16:50:30.000000 zshot-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 16:50:42.303703 zshot-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-29 16:50:30.000000 zshot-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.275703 zshot-0.0.8/zshot/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.279703 zshot-0.0.8/zshot/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.283703 zshot-0.0.8/zshot/evaluation/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.283703 zshot-0.0.8/zshot/evaluation/dataset/med_mentions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/med_mentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/med_mentions/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/med_mentions/med_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/med_mentions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.287703 zshot-0.0.8/zshot/evaluation/dataset/ontonotes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/ontonotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/ontonotes/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/dataset/ontonotes/onto_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.287703 zshot-0.0.8/zshot/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/metrics/rel_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.287703 zshot-0.0.8/zshot/evaluation/metrics/seqeval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/metrics/seqeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/metrics/seqeval/seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/run_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/evaluation/zshot_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.291703 zshot-0.0.8/zshot/linker/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_blink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.291703 zshot-0.0.8/zshot/linker/linker_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_ensemble/linker_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_ensemble/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.291703 zshot-0.0.8/zshot/linker/linker_regen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_regen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_regen/linker_regen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_regen/trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_regen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_smxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/linker/linker_tars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.291703 zshot-0.0.8/zshot/mentions_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/mentions_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_flair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_smxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_tars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.291703 zshot-0.0.8/zshot/mentions_extractor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/utils/ExtractorType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/mentions_extractor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/pipeline_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.291703 zshot-0.0.8/zshot/relation_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/relation_extractor_zsrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/relations_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.295703 zshot-0.0.8/zshot/relation_extractor/zsrc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/zsrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/zsrc/data_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/zsrc/decide_entity_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/relation_extractor/zsrc/zero_shot_rel_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.295703 zshot-0.0.8/zshot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.295703 zshot-0.0.8/zshot/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/evaluation/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.295703 zshot-0.0.8/zshot/tests/linker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/linker/test_ensemble_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/linker/test_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/linker/test_regen_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/linker/test_smxm_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/linker/test_tars_linker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.295703 zshot-0.0.8/zshot/tests/mentions_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/mentions_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/mentions_extractor/test_flair_mentions_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/mentions_extractor/test_mention_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/mentions_extractor/test_smxm_mentions_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/mentions_extractor/test_spacy_mentions_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/mentions_extractor/test_tars_mentions_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.299703 zshot-0.0.8/zshot/tests/relations_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/relations_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/relations_extractor/test_relations_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/test_zshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.299703 zshot-0.0.8/zshot/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/utils/test_displacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/utils/test_ensembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.299703 zshot-0.0.8/zshot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/alignment_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.299703 zshot-0.0.8/zshot/utils/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/data_models/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/data_models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/data_models/relation_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/data_models/span.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.299703 zshot-0.0.8/zshot/utils/displacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/displacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/displacy/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/displacy/displacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/displacy/relations_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/displacy/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/ensembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.303703 zshot-0.0.8/zshot/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.303703 zshot-0.0.8/zshot/utils/models/smxm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/smxm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/smxm/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/smxm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/smxm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.303703 zshot-0.0.8/zshot/utils/models/tars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/tars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/utils/models/tars/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-29 16:50:30.000000 zshot-0.0.8/zshot/zshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:50:42.279703 zshot-0.0.8/zshot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-06-29 16:50:42.000000 zshot-0.0.8/zshot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-29 16:50:42.000000 zshot-0.0.8/zshot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:50:42.000000 zshot-0.0.8/zshot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:50:42.000000 zshot-0.0.8/zshot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 16:50:42.000000 zshot-0.0.8/zshot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 16:50:42.000000 zshot-0.0.8/zshot.egg-info/top_level.txt
```

### Comparing `zshot-0.0.7/LICENSE` & `zshot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/PKG-INFO` & `zshot-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zshot
-Version: 0.0.7
+Version: 0.0.8
 Summary: Zero and Few shot named entity recognition
 Home-page: https://ibm.github.io/zshot
 Author: IBM Research
 Author-email: 
 License: MIT
 Keywords: NER Zero-Shot Few-Shot
 Description-Content-Type: text/markdown
@@ -215,17 +215,32 @@
 >>> [is, similar, used, Business, Machines, materials]
 ```
 
 ### How to evaluate ZShot
 
 Evaluation is an important process to keep improving the performance of the models, that's why ZShot allows to evaluate the component with two predefined datasets: OntoNotes and MedMentions, in a Zero-Shot version in which the entities of the test and validation splits don't appear in the train set.  
 
-The package `evaluation` contains all the functionalities to evaluate the ZShot components. The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take as input the SpaCy `nlp` model and the dataset(s) and split(s) to evaluate. It will return a `str` containing a table with the results of the evaluation. For instance the evaluation of the ZShot custom component implemented above would be:
+The package `evaluation` contains all the functionalities to evaluate the ZShot components. The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take as input the SpaCy `nlp` model and the dataset to evaluate. It will return a `str` containing a table with the results of the evaluation. For instance the evaluation of the TARS linker in ZShot for the *Ontonotes validation* set would be:
 
 ```python
-from zshot.evaluation.zshot_evaluate import evaluate
-from datasets import Split
+import spacy
+
+from zshot import PipelineConfig
+from zshot.linker import LinkerTARS
+from zshot.evaluation.dataset import load_ontonotes_zs
+from zshot.evaluation.zshot_evaluate import evaluate, prettify_evaluate_report
+from zshot.evaluation.metrics.seqeval.seqeval import Seqeval
+
+ontonotes_zs = load_ontonotes_zs('validation')
+
+
+nlp = spacy.blank("en")
+nlp_config = PipelineConfig(
+    linker=LinkerTARS(),
+    entities=ontonotes_zs.entities
+)
+
+nlp.add_pipe("zshot", config=nlp_config, last=True)
 
-evaluation = evaluate(new_nlp, datasets="ontonotes", 
-                      splits=[Split.VALIDATION])
-print(evaluation)
+evaluation = evaluate(nlp, ontonotes_zs, metric=Seqeval())
+prettify_evaluate_report(evaluation)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zshot Version: 0.0.7 Summary: Zero and Few shot
+Metadata-Version: 2.1 Name: zshot Version: 0.0.8 Summary: Zero and Few shot
 named entity recognition Home-page: https://ibm.github.io/zshot Author: IBM
 Research Author-email: License: MIT Keywords: NER Zero-Shot Few-Shot
 Description-Content-Type: text/markdown License-File: LICENSE
                   [https://ibm.github.io/zshot/img/graph.png]
                               ****** Zshot ******
           Zero and Few shot named entity & relationships recognition
 [Tutorials] [https://img.shields.io/pypi/v/zshot] [https://img.shields.io/pypi/
@@ -126,13 +126,18 @@
 used, Business, Machines, materials] ``` ### How to evaluate ZShot Evaluation
 is an important process to keep improving the performance of the models, that's
 why ZShot allows to evaluate the component with two predefined datasets:
 OntoNotes and MedMentions, in a Zero-Shot version in which the entities of the
 test and validation splits don't appear in the train set. The package
 `evaluation` contains all the functionalities to evaluate the ZShot components.
 The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take
-as input the SpaCy `nlp` model and the dataset(s) and split(s) to evaluate. It
-will return a `str` containing a table with the results of the evaluation. For
-instance the evaluation of the ZShot custom component implemented above would
-be: ```python from zshot.evaluation.zshot_evaluate import evaluate from
-datasets import Split evaluation = evaluate(new_nlp, datasets="ontonotes",
-splits=[Split.VALIDATION]) print(evaluation) ```
+as input the SpaCy `nlp` model and the dataset to evaluate. It will return a
+`str` containing a table with the results of the evaluation. For instance the
+evaluation of the TARS linker in ZShot for the *Ontonotes validation* set would
+be: ```python import spacy from zshot import PipelineConfig from zshot.linker
+import LinkerTARS from zshot.evaluation.dataset import load_ontonotes_zs from
+zshot.evaluation.zshot_evaluate import evaluate, prettify_evaluate_report from
+zshot.evaluation.metrics.seqeval.seqeval import Seqeval ontonotes_zs =
+load_ontonotes_zs('validation') nlp = spacy.blank("en") nlp_config =
+PipelineConfig( linker=LinkerTARS(), entities=ontonotes_zs.entities )
+nlp.add_pipe("zshot", config=nlp_config, last=True) evaluation = evaluate(nlp,
+ontonotes_zs, metric=Seqeval()) prettify_evaluate_report(evaluation) ```
```

### Comparing `zshot-0.0.7/README.md` & `zshot-0.0.8/zshot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: zshot
+Version: 0.0.8
+Summary: Zero and Few shot named entity recognition
+Home-page: https://ibm.github.io/zshot
+Author: IBM Research
+Author-email: 
+License: MIT
+Keywords: NER Zero-Shot Few-Shot
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
   
   <img height="170x" src="https://ibm.github.io/zshot/img/graph.png" />
   
   <h1>Zshot</h1>
 
   <p>
@@ -203,17 +215,32 @@
 >>> [is, similar, used, Business, Machines, materials]
 ```
 
 ### How to evaluate ZShot
 
 Evaluation is an important process to keep improving the performance of the models, that's why ZShot allows to evaluate the component with two predefined datasets: OntoNotes and MedMentions, in a Zero-Shot version in which the entities of the test and validation splits don't appear in the train set.  
 
-The package `evaluation` contains all the functionalities to evaluate the ZShot components. The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take as input the SpaCy `nlp` model and the dataset(s) and split(s) to evaluate. It will return a `str` containing a table with the results of the evaluation. For instance the evaluation of the ZShot custom component implemented above would be:
+The package `evaluation` contains all the functionalities to evaluate the ZShot components. The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take as input the SpaCy `nlp` model and the dataset to evaluate. It will return a `str` containing a table with the results of the evaluation. For instance the evaluation of the TARS linker in ZShot for the *Ontonotes validation* set would be:
 
 ```python
-from zshot.evaluation.zshot_evaluate import evaluate
-from datasets import Split
+import spacy
+
+from zshot import PipelineConfig
+from zshot.linker import LinkerTARS
+from zshot.evaluation.dataset import load_ontonotes_zs
+from zshot.evaluation.zshot_evaluate import evaluate, prettify_evaluate_report
+from zshot.evaluation.metrics.seqeval.seqeval import Seqeval
+
+ontonotes_zs = load_ontonotes_zs('validation')
+
+
+nlp = spacy.blank("en")
+nlp_config = PipelineConfig(
+    linker=LinkerTARS(),
+    entities=ontonotes_zs.entities
+)
+
+nlp.add_pipe("zshot", config=nlp_config, last=True)
 
-evaluation = evaluate(new_nlp, datasets="ontonotes", 
-                      splits=[Split.VALIDATION])
-print(evaluation)
+evaluation = evaluate(nlp, ontonotes_zs, metric=Seqeval())
+prettify_evaluate_report(evaluation)
 ```
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: zshot Version: 0.0.8 Summary: Zero and Few shot
+named entity recognition Home-page: https://ibm.github.io/zshot Author: IBM
+Research Author-email: License: MIT Keywords: NER Zero-Shot Few-Shot
+Description-Content-Type: text/markdown License-File: LICENSE
                   [https://ibm.github.io/zshot/img/graph.png]
                               ****** Zshot ******
           Zero and Few shot named entity & relationships recognition
 [Tutorials] [https://img.shields.io/pypi/v/zshot] [https://img.shields.io/pypi/
                            dm/zshot] [Build] [Build]
 **Documentation**: https://ibm.github.io/zshot **Source Code**: https://
 github.com/IBM/zshot Zshot is a highly customisable framework for performing
@@ -122,13 +126,18 @@
 used, Business, Machines, materials] ``` ### How to evaluate ZShot Evaluation
 is an important process to keep improving the performance of the models, that's
 why ZShot allows to evaluate the component with two predefined datasets:
 OntoNotes and MedMentions, in a Zero-Shot version in which the entities of the
 test and validation splits don't appear in the train set. The package
 `evaluation` contains all the functionalities to evaluate the ZShot components.
 The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take
-as input the SpaCy `nlp` model and the dataset(s) and split(s) to evaluate. It
-will return a `str` containing a table with the results of the evaluation. For
-instance the evaluation of the ZShot custom component implemented above would
-be: ```python from zshot.evaluation.zshot_evaluate import evaluate from
-datasets import Split evaluation = evaluate(new_nlp, datasets="ontonotes",
-splits=[Split.VALIDATION]) print(evaluation) ```
+as input the SpaCy `nlp` model and the dataset to evaluate. It will return a
+`str` containing a table with the results of the evaluation. For instance the
+evaluation of the TARS linker in ZShot for the *Ontonotes validation* set would
+be: ```python import spacy from zshot import PipelineConfig from zshot.linker
+import LinkerTARS from zshot.evaluation.dataset import load_ontonotes_zs from
+zshot.evaluation.zshot_evaluate import evaluate, prettify_evaluate_report from
+zshot.evaluation.metrics.seqeval.seqeval import Seqeval ontonotes_zs =
+load_ontonotes_zs('validation') nlp = spacy.blank("en") nlp_config =
+PipelineConfig( linker=LinkerTARS(), entities=ontonotes_zs.entities )
+nlp.add_pipe("zshot", config=nlp_config, last=True) evaluation = evaluate(nlp,
+ontonotes_zs, metric=Seqeval()) prettify_evaluate_report(evaluation) ```
```

### Comparing `zshot-0.0.7/setup.py` & `zshot-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,19 @@
       packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
       include_package_data=True,
       zip_safe=False,
       install_requires=[
           "spacy>=3.4.1",
           "requests>=2.28",
           "tqdm>=4.62.3",
-          "setuptools~=60.0.0",  # Needed to install dynamic packages from source (e.g. Blink)
+          "setuptools>=65.5.1",  # Needed to install dynamic packages from source (e.g. Blink)
           "prettytable>=3.4",
-          "torch>=1",
+          "torch>=1,<2",
           "transformers>=4.20",
-          "datasets>=2.3.0",
+          "datasets>=2.9.1",
           "evaluate>=0.3.0",
           "seqeval>=1.2.2",
       ],
       entry_points="""
       # -*- Entry points: -*-
       """,
       )
```

### Comparing `zshot-0.0.7/zshot/evaluation/dataset/dataset.py` & `zshot-0.0.8/zshot/evaluation/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/dataset/med_mentions/entities.py` & `zshot-0.0.8/zshot/evaluation/dataset/med_mentions/entities.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/dataset/med_mentions/med_mentions.py` & `zshot-0.0.8/zshot/evaluation/dataset/med_mentions/med_mentions.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/dataset/med_mentions/utils.py` & `zshot-0.0.8/zshot/evaluation/dataset/med_mentions/utils.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/dataset/ontonotes/entities.py` & `zshot-0.0.8/zshot/evaluation/dataset/ontonotes/entities.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/dataset/ontonotes/onto_notes.py` & `zshot-0.0.8/zshot/evaluation/dataset/ontonotes/onto_notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         if label == 'O' or label[2:] in TRIVIAL_CLASSES or label[2:] not in CLASSES_PER_SPLIT[split]:
             sentence['named_entities'][i] = 0
     return sentence
 
 
 def load_ontonotes_zs(split: Optional[Union[str, Split]] = None, **kwargs) -> Union[Dict[DatasetWithEntities,
                                                                                          Dataset], Dataset]:
-    dataset_zs = load_dataset("conll2012_ontonotesv5", "english_v12", split=split, ignore_verifications=True, **kwargs)
+    dataset_zs = load_dataset("conll2012_ontonotesv5", "english_v12",
+                              split=split, verification_mode='no_checks', **kwargs)
     if split:
         ontonotes_zs = preprocess_spit(dataset_zs, get_simple_split(split))
     else:
         ontonotes_zs = DatasetDict()
         for split in dataset_zs:
             ontonotes_zs[split] = preprocess_spit(dataset_zs[split], split)
     return ontonotes_zs
```

### Comparing `zshot-0.0.7/zshot/evaluation/evaluator.py` & `zshot-0.0.8/zshot/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/metrics/rel_eval.py` & `zshot-0.0.8/zshot/evaluation/metrics/rel_eval.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/metrics/seqeval/seqeval.py` & `zshot-0.0.8/zshot/evaluation/metrics/seqeval/seqeval.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/pipeline.py` & `zshot-0.0.8/zshot/evaluation/pipeline.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/evaluation/run_evaluation.py` & `zshot-0.0.8/zshot/evaluation/run_evaluation.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         mentions_extractors = list(MENTION_EXTRACTORS.keys())
     else:
         mentions_extractors = [args.mentions_extractor]
 
     if args.linker == "all":
         linkers = list(LINKERS.keys())
     else:
-        linkers = [args.linker]
+        linkers = args.linker.split(',')
 
     if args.mode == "full":
         if linkers:
             for linker in linkers:
                 if linker not in END2END:
                     for mentions_extractor in mentions_extractors:
                         configs[f"{mentions_extractor}_{linker}"] = PipelineConfig(
```

### Comparing `zshot-0.0.7/zshot/evaluation/zshot_evaluate.py` & `zshot-0.0.8/zshot/evaluation/zshot_evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Dict
+from typing import Optional, Union, Dict, List
 
 import spacy
 from datasets import Dataset
 from evaluate import EvaluationModule
 from prettytable import PrettyTable
 
 from zshot.evaluation.evaluator import ZeroShotTokenClassificationEvaluator, MentionsExtractorEvaluator
@@ -30,15 +30,15 @@
         results['linker'] = linker_evaluator.compute(pipe, dataset, metric=metric)
     if nlp.get_pipe("zshot").mentions_extractor:
         pipe = MentionsExtractorPipeline(nlp, batch_size)
         results['mentions_extractor'] = mentions_extractor_evaluator.compute(pipe, dataset, metric=metric)
     return results
 
 
-def prettify_evaluate_report(evaluation: Dict, name: str = "", decimals: int = 4) -> list[PrettyTable]:
+def prettify_evaluate_report(evaluation: Dict, name: str = "", decimals: int = 4) -> List[PrettyTable]:
     """
     Convert an evaluation report Dict to a formatted string
     :param evaluation: The evaluation report dict
     :param name: Reference name
     :param decimals: Number of decimals to show
     :return: Formatted evaluation table as string, for each component
     """
```

### Comparing `zshot-0.0.7/zshot/linker/linker.py` & `zshot-0.0.8/zshot/linker/linker.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/linker/linker_blink.py` & `zshot-0.0.8/zshot/linker/linker_blink.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/linker/linker_regen/linker_regen.py` & `zshot-0.0.8/zshot/linker/linker_regen/linker_regen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Iterator, Optional, Union, List
 
+import torch
 from spacy.tokens import Doc
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 
+from zshot.config import MODELS_CACHE_PATH
 from zshot.linker.linker import Linker
 from zshot.linker.linker_regen.trie import Trie
 from zshot.linker.linker_regen.utils import create_input
 from zshot.utils.data_models import Entity, Span
 
 MODEL_NAME = "ibm/regen-disambiguation"
 
@@ -47,21 +49,22 @@
                     for e in entities
                 ]
             )
 
     def load_models(self):
         """ Load Model """
         if self.model is None:
-            self.model = AutoModelForSeq2SeqLM.from_pretrained(MODEL_NAME)
+            self.model = AutoModelForSeq2SeqLM.from_pretrained(MODEL_NAME, cache_dir=MODELS_CACHE_PATH)
         self.load_tokenizer()
 
     def load_tokenizer(self):
         """ Load Tokenizer"""
         if self.tokenizer is None:
-            self.tokenizer = AutoTokenizer.from_pretrained(MODEL_NAME, model_max_length=1024)
+            self.tokenizer = AutoTokenizer.from_pretrained(MODEL_NAME, model_max_length=1024,
+                                                           cache_dir=MODELS_CACHE_PATH)
 
     def restrict_decode_vocab(self, _, prefix_beam):
         """ Restrict the posibilities of the Beam search to force the text generation """
         return self.trie.postfix(prefix_beam.tolist())
 
     def predict(self, docs: Iterator[Doc], batch_size: Optional[Union[int, None]] = None) -> List[List[Span]]:
         """
@@ -90,38 +93,45 @@
                                   max_length=self.max_input_len,
                                   start_delimiter=START_ENT_TOKEN,
                                   end_delimiter=END_ENT_TOKEN,
                                   ) for d in data_to_link]
         if not sentences:
             return []
 
-        input_args = {
-            k: v
-            for k, v in self.tokenizer.batch_encode_plus(
-                sentences, padding=True, return_tensors="pt"
-            ).items()
-        }
-
-        outputs = self.model.generate(
-            **input_args,
-            min_length=0,
-            max_length=self.max_output_len,
-            num_beams=self.num_beams,
-            num_return_sequences=1,
-            output_scores=True,
-            return_dict_in_generate=True,
-            prefix_allowed_tokens_fn=None
-            if self.trie is None
-            else self.restrict_decode_vocab,
-        )
+        sequences = []
+        scores = []
+        for sent in sentences:
+            input_args = {
+                k: v
+                for k, v in self.tokenizer.batch_encode_plus(
+                    [sent], padding=True, return_tensors="pt"
+                ).items()
+            }
+
+            outputs = self.model.generate(
+                **input_args,
+                min_length=0,
+                max_length=self.max_output_len,
+                num_beams=self.num_beams,
+                num_return_sequences=min(self.num_beams, len(self.entities)) if self.entities else self.num_beams,
+                output_scores=True,
+                return_dict_in_generate=True,
+                prefix_allowed_tokens_fn=None
+                if self.trie is None
+                else self.restrict_decode_vocab,
+            )
 
-        docs_pred = {}
+            tmp_scores = torch.nn.Softmax()(outputs.sequences_scores)
+            sequences.append(outputs.sequences[torch.argmax(tmp_scores)])
+            scores.append(max(tmp_scores.cpu().numpy().tolist()))
 
-        for data, out, score in zip(data_to_link, outputs.sequences, outputs.sequences_scores):
+        docs_pred = {}
+        for data, out, score in zip(data_to_link, sequences, scores):
             doc_id = data['id']
             mention = docs[doc_id]._.mentions[data['mention_id']]
             label = self.tokenizer.decode(out, skip_special_tokens=True)
             if doc_id not in docs_pred:
                 docs_pred[doc_id] = []
+
             docs_pred[doc_id].append(Span(mention.start, mention.end, label=label,
-                                          score=score.detach().numpy().tolist()))
+                                          score=score))
         return [val for key, val in sorted(docs_pred.items(), reverse=False)]
```

### Comparing `zshot-0.0.7/zshot/linker/linker_regen/trie.py` & `zshot-0.0.8/zshot/linker/linker_regen/trie.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/linker/linker_regen/utils.py` & `zshot-0.0.8/zshot/linker/linker_regen/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import pickle
 from typing import Dict, List
 
-import pytest
 from huggingface_hub import hf_hub_download
 
 from zshot.linker.linker_regen.trie import Trie
 from zshot.utils.data_models import Span
 
 REPO_ID = "ibm/regen-disambiguation"
 TRIE_FILE_NAME = "wikipedia_trie.pkl"
@@ -21,15 +20,14 @@
         end_delimiter_index = sent_list.index(end_delimiter)
         start_delimiter_index = sent_list.index(start_delimiter)
         half_context = (max_length - (end_delimiter_index - start_delimiter_index)) // 2
         left_index = max(0, start_delimiter_index - half_context)
         right_index = min(len(sent_list), end_delimiter_index + half_context + (
             half_context - (start_delimiter_index - left_index)))
         left_index = left_index - max(0, (half_context - (right_index - end_delimiter_index)))
-        print(len(sent_list[left_index:right_index]))
         return " ".join(sent_list[left_index:right_index])
 
 
 def load_wikipedia_trie() -> Trie:
     """
     Load the wikipedia trie from the HB hub
     :return: The Wikipedia trie
@@ -38,15 +36,14 @@
                                           repo_type='model',
                                           filename=TRIE_FILE_NAME)
     with open(wikipedia_trie_file, "rb") as f:
         wikipedia_trie = pickle.load(f)
     return wikipedia_trie
 
 
-@pytest.mark.skip(reason="Too expensive to run on every commit")
 def load_wikipedia_mapping() -> Dict[str, str]:
     """
     Load the wikipedia trie from the HB hub
     :return: The Wikipedia trie
     """
     wikipedia_map = hf_hub_download(repo_id=REPO_ID,
                                     repo_type='model',
```

### Comparing `zshot-0.0.7/zshot/linker/linker_smxm.py` & `zshot-0.0.8/zshot/linker/linker_smxm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterator, List, Optional, Union
 
 from spacy.tokens import Doc
 from transformers import BertTokenizerFast
 
+from zshot.config import MODELS_CACHE_PATH
 from zshot.linker.linker import Linker
 from zshot.utils.data_models import Span
 from zshot.utils.models.smxm.model import BertTaggerMultiClass
 from zshot.utils.models.smxm.utils import (
     get_entities_names_descriptions,
     smxm_predict
 )
@@ -17,30 +18,30 @@
 class LinkerSMXM(Linker):
     """ SMXM linker """
 
     def __init__(self, model_name=ONTONOTES_MODEL_NAME):
         super().__init__()
 
         self.tokenizer = BertTokenizerFast.from_pretrained(
-            "bert-large-cased", truncation_side="left"
+            "bert-large-cased", truncation_side="left", cache_dir=MODELS_CACHE_PATH
         )
 
         self.model_name = model_name
         self.model = None
 
     @property
     def is_end2end(self) -> bool:
         """ SMXM is end2end model"""
         return True
 
     def load_models(self):
         """ Load SMXM model """
         if self.model is None:
             self.model = BertTaggerMultiClass.from_pretrained(
-                self.model_name, output_hidden_states=True
+                self.model_name, output_hidden_states=True, cache_dir=MODELS_CACHE_PATH
             ).to(self.device)
 
     def predict(self, docs: Iterator[Doc], batch_size: Optional[Union[int, None]] = None) -> List[List[Span]]:
         """
         Perform the entity prediction
         :param docs: A list of spacy Document
         :param batch_size: The batch size
```

### Comparing `zshot-0.0.7/zshot/linker/linker_tars.py` & `zshot-0.0.8/zshot/linker/linker_tars.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,47 +31,47 @@
         self.task = None
 
     def set_kg(self, entities: Iterator[Entity]):
         """ Set new entities in the model
 
         :param entities: New entities to use
         """
-        old_entities = self._entities
+        old_entities = self.entities
         super().set_kg(entities)
+        self.flat_entities()
         if old_entities != entities:
-            self.flat_entities()
-            self.task = f'zshot.ner.{hash(tuple(self._entities))}'
+            self.task = f'zshot.ner.{hash(tuple(self.entities))}'
             if not self.model:
                 self.load_models()
             self.model.add_and_switch_to_new_task(self.task,
-                                                  self._entities, label_type='ner')
+                                                  self.entities, label_type='ner')
 
     def flat_entities(self):
         """ As TARS use only the labels, take just the name of the entities and not the description """
-        if isinstance(self._entities, dict):
-            self._entities = list(self._entities.keys())
-        if isinstance(self._entities, list):
-            self._entities = [e.name if type(e) == Entity else e for e in self._entities]
-        if self._entities is None:
+        if isinstance(self.entities, dict):
+            self._entities = list(self.entities.keys())
+        if isinstance(self.entities, list):
+            self._entities = [e.name if type(e) == Entity else e for e in self.entities]
+        if self.entities is None:
             self._entities = []
 
     def load_models(self):
         """ Load TARS model if its not initialized"""
         if not self.model:
             from flair.models import TARSTagger
             self.model = TARSTagger.load('tars-ner')
 
             if not self.entities:
                 self.model.switch_to_task(self.default_entities)
                 self.task = self.default_entities
             else:
                 self.flat_entities()
-                self.task = f'zshot.ner.{hash(tuple(self._entities))}'
+                self.task = f'zshot.ner.{hash(tuple(self.entities))}'
                 self.model.add_and_switch_to_new_task(self.task,
-                                                      self._entities, label_type='ner')
+                                                      self.entities, label_type='ner')
 
     def predict(self, docs: Iterator[Doc], batch_size: Optional[Union[int, None]] = None) -> List[List[Span]]:
         """
         Perform the entity prediction
         :param docs: A list of spacy Document
         :param batch_size: The batch size
         :return: List Spans for each Document in docs
```

### Comparing `zshot-0.0.7/zshot/mentions_extractor/mentions_extractor.py` & `zshot-0.0.8/zshot/mentions_extractor/mentions_extractor.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_flair.py` & `zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_flair.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_smxm.py` & `zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_smxm.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_spacy.py` & `zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_spacy.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/mentions_extractor/mentions_extractor_tars.py` & `zshot-0.0.8/zshot/mentions_extractor/mentions_extractor_tars.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/pipeline_config.py` & `zshot-0.0.8/zshot/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/relation_extractor/relation_extractor_zsrc.py` & `zshot-0.0.8/zshot/relation_extractor/relation_extractor_zsrc.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/relation_extractor/relations_extractor.py` & `zshot-0.0.8/zshot/relation_extractor/relations_extractor.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/relation_extractor/zsrc/data_helper.py` & `zshot-0.0.8/zshot/relation_extractor/zsrc/data_helper.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/relation_extractor/zsrc/decide_entity_order.py` & `zshot-0.0.8/zshot/relation_extractor/zsrc/decide_entity_order.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/relation_extractor/zsrc/zero_shot_rel_class.py` & `zshot-0.0.8/zshot/relation_extractor/zsrc/zero_shot_rel_class.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/config.py` & `zshot-0.0.8/zshot/tests/config.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/evaluation/test_datasets.py` & `zshot-0.0.8/zshot/tests/evaluation/test_datasets.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/evaluation/test_evaluation.py` & `zshot-0.0.8/zshot/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/linker/test_linker.py` & `zshot-0.0.8/zshot/tests/linker/test_linker.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class DummyLinkerEnd2End(Linker):
 
     @property
     def is_end2end(self) -> bool:
         return True
 
     def predict(self, docs: Iterator[Doc], batch_size=None):
-        return [[Span(0, len(doc.text) - 1, label='label')] for doc in docs]
+        return [[Span(0, len(doc.text) - 1, label='label', score=0.9)] for doc in docs]
 
 
 class DummyLinkerWithEntities(Linker):
 
     def predict(self, docs: Iterator[Doc], batch_size=None):
         entities = self.entities
         return [
```

### Comparing `zshot-0.0.7/zshot/tests/linker/test_regen_linker.py` & `zshot-0.0.8/zshot/tests/mentions_extractor/test_spacy_mentions_extractor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,69 @@
-import gc
-import logging
-import shutil
-from pathlib import Path
-
-import pytest
 import spacy
 
-from zshot import PipelineConfig
-from zshot.linker.linker_regen.linker_regen import LinkerRegen
-from zshot.linker.linker_regen.trie import Trie
-from zshot.linker.linker_regen.utils import load_wikipedia_trie, spans_to_wikipedia
 from zshot.mentions_extractor import MentionsExtractorSpacy
-from zshot.tests.config import EX_DOCS, EX_ENTITIES
-from zshot.tests.mentions_extractor.test_mention_extractor import DummyMentionsExtractor
-from zshot.utils.data_models import Span
-
-logger = logging.getLogger(__name__)
-
-
-@pytest.fixture(scope="module", autouse=True)
-def teardown():
-    logger.warning("Starting regen tests")
-    yield True
-    logger.warning("Removing cache")
-    shutil.rmtree(f"{Path.home()}/.cache/huggingface", ignore_errors=True)
-    shutil.rmtree(f"{Path.home()}/.cache/zshot", ignore_errors=True)
-    gc.collect()
-
-
-def test_regen_linker():
-    nlp = spacy.blank("en")
-    config = PipelineConfig(
-        mentions_extractor=DummyMentionsExtractor(),
-        linker=LinkerRegen(),
-        entities=EX_ENTITIES
-    )
-    nlp.add_pipe("zshot", config=config, last=True)
-    assert "zshot" in nlp.pipe_names
+from zshot.mentions_extractor.mentions_extractor_spacy import ExtractorType
+from zshot.tests.config import EX_DOCS
+from zshot import PipelineConfig
+
+
+def test_spacy_ner_mentions_extractor():
+    nlp = spacy.load("en_core_web_sm")
+
+    config_zshot = PipelineConfig(mentions_extractor=MentionsExtractorSpacy(ExtractorType.NER))
+    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    assert "zshot" in nlp.pipe_names and "ner" in nlp.pipe_names
 
     doc = nlp(EX_DOCS[1])
-    assert len(doc.ents) > 0
-    del nlp.get_pipe('zshot').mentions_extractor, nlp.get_pipe('zshot').entities, nlp.get_pipe('zshot').nlp
-    del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.trie, \
-        nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
-    nlp.remove_pipe('zshot')
-    del doc, nlp, config
+    assert doc.ents == ()
+    assert len(doc._.mentions) > 0
+    nlp = None
 
 
-def test_regen_linker_pipeline():
+def test_custom_spacy_mentions_extractor():
     nlp = spacy.load("en_core_web_sm")
-    config = PipelineConfig(
-        mentions_extractor=MentionsExtractorSpacy(),
-        linker=LinkerRegen(),
-        entities=EX_ENTITIES
-    )
-    nlp.add_pipe("zshot", config=config, last=True)
-    assert "zshot" in nlp.pipe_names
 
-    docs = [doc for doc in nlp.pipe(EX_DOCS)]
-    assert all(len(doc.ents) > 0 for doc in docs)
-    del nlp.get_pipe('zshot').mentions_extractor, nlp.get_pipe('zshot').entities, nlp.get_pipe('zshot').nlp
-    del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.trie, \
-        nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
-    nlp.remove_pipe('zshot')
-    del docs, nlp, config
-
-
-def test_regen_linker_wikification():
-    nlp = spacy.blank("en")
-    trie = Trie()
-    trie.add([794, 536, 1])
-    trie.add([794, 357, 1])
-    config = PipelineConfig(
-        mentions_extractor=DummyMentionsExtractor(),
-        linker=LinkerRegen(trie=trie),
-    )
-    nlp.add_pipe("zshot", config=config, last=True)
-    assert "zshot" in nlp.pipe_names
+    custom_component = MentionsExtractorSpacy(ExtractorType.NER)
+    config_zshot = PipelineConfig(mentions_extractor=custom_component, disable_default_ner=False)
+    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    assert "zshot" in nlp.pipe_names and "ner" in nlp.pipe_names
 
     doc = nlp(EX_DOCS[1])
-    assert len(doc.ents) > 0
-    del nlp.get_pipe('zshot').mentions_extractor, nlp.get_pipe('zshot').entities, nlp.get_pipe('zshot').nlp
-    del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.trie, \
-        nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
-    nlp.remove_pipe('zshot')
-    del doc, nlp, config
-
-
-def test_load_wikipedia_trie():
-    trie = load_wikipedia_trie()
-    assert len(list(trie.trie_dict.keys())) == 6952
-
-
-def test_span_to_wiki():
-    s = Span(label="Surfing", start=0, end=10)
-    wiki_links = spans_to_wikipedia([s])
-    assert len(wiki_links) > 0
-    assert wiki_links[0].startswith("https://en.wikipedia.org/wiki?curid=")
+    assert doc.ents == ()
+    assert len(doc._.mentions) > 0
+    nlp = None
+
+
+def test_spacy_pos_mentions_extractor():
+    nlp = spacy.load("en_core_web_sm")
+
+    config_zshot = PipelineConfig(mentions_extractor=MentionsExtractorSpacy(ExtractorType.POS))
+    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    assert "zshot" in nlp.pipe_names and "ner" not in nlp.pipe_names
+    doc = nlp(EX_DOCS[1])
+    assert doc.ents == ()
+    assert len(doc._.mentions) > 0
+    nlp = None
+
+
+def test_spacy_ner_mentions_extractor_pipeline():
+    nlp = spacy.load("en_core_web_sm")
+
+    config_zshot = PipelineConfig(mentions_extractor=MentionsExtractorSpacy(ExtractorType.NER))
+    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    assert "zshot" in nlp.pipe_names and "ner" in nlp.pipe_names
+    docs = [doc for doc in nlp.pipe(EX_DOCS)]
+    assert all(doc.ents == () for doc in docs)
+    assert all(len(doc._.mentions) > 0 for doc in docs)
+    nlp = None
+
+
+def test_spacy_pos_mentions_extractor_pipeline():
+    nlp = spacy.load("en_core_web_sm")
+
+    config_zshot = PipelineConfig(mentions_extractor=MentionsExtractorSpacy(ExtractorType.POS))
+    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    assert "zshot" in nlp.pipe_names and "ner" not in nlp.pipe_names
+    docs = [doc for doc in nlp.pipe(EX_DOCS)]
+    assert all(doc.ents == () for doc in docs)
+    assert all(len(doc._.mentions) > 0 for doc in docs)
+    nlp = None
```

### Comparing `zshot-0.0.7/zshot/tests/linker/test_smxm_linker.py` & `zshot-0.0.8/zshot/tests/linker/test_smxm_linker.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shutil
 from pathlib import Path
 
 import pytest
 import spacy
 
 from zshot import PipelineConfig, Linker
-from zshot.linker import LinkerSMXM
+from zshot.linker import LinkerSMXM, LinkerEnsemble
 from zshot.tests.config import EX_DOCS, EX_ENTITIES
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="module", autouse=True)
 def teardown():
@@ -37,33 +37,19 @@
         entities=EX_ENTITIES
     )
     nlp.add_pipe("zshot", config=smxm_config, last=True)
     assert "zshot" in nlp.pipe_names
 
     doc = nlp(EX_DOCS[1])
     assert len(doc.ents) > 0
-    del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
-    nlp.remove_pipe('zshot')
-    del doc, nlp, smxm_config
-
-
-def test_smxm_linker_pipeline():
-    nlp = spacy.blank("en")
-    smxm_config = PipelineConfig(
-        linker=LinkerSMXM(),
-        entities=EX_ENTITIES
-    )
-    nlp.add_pipe("zshot", config=smxm_config, last=True)
-    assert "zshot" in nlp.pipe_names
-
     docs = [doc for doc in nlp.pipe(EX_DOCS)]
     assert all(len(doc.ents) > 0 for doc in docs)
     del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
     nlp.remove_pipe('zshot')
-    del docs, nlp, smxm_config
+    del doc, nlp, smxm_config
 
 
 def test_smxm_linker_no_entities():
     nlp = spacy.blank("en")
     smxm_config = PipelineConfig(
         linker=LinkerSMXM(),
         entities=[]
@@ -72,7 +58,20 @@
     assert "zshot" in nlp.pipe_names
 
     doc = nlp(EX_DOCS[1])
     assert len(doc.ents) == 0
     del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
     nlp.remove_pipe('zshot')
     del doc, nlp, smxm_config
+
+
+def test_ensemble_smxm_linker():
+    nlp = spacy.blank("en")
+    nlp.add_pipe("zshot", config=PipelineConfig(
+        entities=EX_ENTITIES,
+        linker=LinkerEnsemble(
+            threshold=0.25
+        )
+    ), last=True)
+    doc = nlp(EX_DOCS[1])
+    assert len(doc.ents) > 0
+    del doc, nlp
```

### Comparing `zshot-0.0.7/zshot/tests/linker/test_tars_linker.py` & `zshot-0.0.8/zshot/tests/linker/test_regen_linker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,100 @@
 import gc
-import pkgutil
+import logging
+import shutil
+from pathlib import Path
 
 import pytest
 import spacy
 
-from zshot import PipelineConfig, Linker
-from zshot.linker import LinkerTARS
+from zshot import PipelineConfig
+from zshot.linker.linker_regen.linker_regen import LinkerRegen
+from zshot.linker.linker_regen.trie import Trie
+from zshot.linker.linker_regen.utils import load_wikipedia_trie, spans_to_wikipedia, create_input
 from zshot.tests.config import EX_DOCS, EX_ENTITIES
+from zshot.tests.mentions_extractor.test_mention_extractor import DummyMentionsExtractor
+from zshot.utils.data_models import Span
 
-OVERLAP_TEXT = "Senator McConnell in addition to this the New York Times editors wrote in reaction to the " \
-               "Supreme Court 's decision striking down the military tribunal set up to private detainees " \
-               "being held in Guantanamo bay it is far more than a narrow ruling on the issue of military courts . " \
-               "It is an important and welcome reaffirmation That even in times of war the law is what the " \
-               "constitution the statuette books and the Geneva convention say it is . " \
-               "Not what the President wants it to be /."
-INCOMPLETE_SPANS_TEXT = "-LSB- -LSB- They attacked small bridges and small districts , " \
-                        "and generally looted these stations . -RSB- -RSB-"
+logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="module", autouse=True)
 def teardown():
+    logger.warning("Starting regen tests")
     yield True
+    logger.warning("Removing cache")
+    shutil.rmtree(f"{Path.home()}/.cache/huggingface", ignore_errors=True)
+    shutil.rmtree(f"{Path.home()}/.cache/zshot", ignore_errors=True)
     gc.collect()
 
 
-def test_tars_download():
-    linker = LinkerTARS()
-    linker.load_models()
-    assert isinstance(linker, Linker)
-    del linker.model, linker
-
-
-def test_tars_end2end_with_entities():
-    if not pkgutil.find_loader("flair"):
-        return
+def test_regen_linker():
     nlp = spacy.blank("en")
-
-    config_zshot = PipelineConfig(linker=LinkerTARS(), entities=EX_ENTITIES)
-    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    config = PipelineConfig(
+        mentions_extractor=DummyMentionsExtractor(),
+        linker=LinkerRegen(),
+        entities=EX_ENTITIES
+    )
+    nlp.add_pipe("zshot", config=config, last=True)
     assert "zshot" in nlp.pipe_names
-    doc = nlp(EX_DOCS[1])
-    assert doc.ents != ()
-    del nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
-    nlp.remove_pipe('zshot')
-    del nlp, config_zshot
 
-
-def test_tars_end2end_pipeline_with_entities():
-    if not pkgutil.find_loader("flair"):
-        return
-    nlp = spacy.blank("en")
-
-    config_zshot = PipelineConfig(linker=LinkerTARS(), entities=EX_ENTITIES)
-    nlp.add_pipe("zshot", config=config_zshot, last=True)
-    assert "zshot" in nlp.pipe_names
+    doc = nlp(EX_DOCS[1])
+    assert len(doc.ents) > 0
+    doc = nlp("")
+    assert len(doc.ents) == 0
     docs = [doc for doc in nlp.pipe(EX_DOCS)]
-    assert all(doc.ents != () for doc in docs)
-    del nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
+    assert all(len(doc.ents) > 0 for doc in docs)
+    del nlp.get_pipe('zshot').mentions_extractor, nlp.get_pipe('zshot').entities, nlp.get_pipe('zshot').nlp
+    del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.trie, \
+        nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
     nlp.remove_pipe('zshot')
-    del nlp, config_zshot
+    del doc, nlp, config
 
 
-def test_tars_end2end_overlap():
-    if not pkgutil.find_loader("flair"):
-        return
+def test_regen_linker_wikification():
     nlp = spacy.blank("en")
-
-    config_zshot = PipelineConfig(linker=LinkerTARS(), entities=["company", "location", "organic compound"])
-    nlp.add_pipe("zshot", config=config_zshot, last=True)
+    trie = Trie()
+    trie.add([794, 536, 1])
+    trie.add([794, 357, 1])
+    config = PipelineConfig(
+        mentions_extractor=DummyMentionsExtractor(),
+        linker=LinkerRegen(trie=trie),
+    )
+    nlp.add_pipe("zshot", config=config, last=True)
     assert "zshot" in nlp.pipe_names
-    doc = nlp(OVERLAP_TEXT)
+
+    doc = nlp(EX_DOCS[1])
     assert len(doc.ents) > 0
-    del nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
+    del nlp.get_pipe('zshot').mentions_extractor, nlp.get_pipe('zshot').entities, nlp.get_pipe('zshot').nlp
+    del nlp.get_pipe('zshot').linker.tokenizer, nlp.get_pipe('zshot').linker.trie, \
+        nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
     nlp.remove_pipe('zshot')
-    del nlp, config_zshot
+    del doc, nlp, config
 
 
-def test_tars_end2end_incomplete_spans():
-    if not pkgutil.find_loader("flair"):
-        return
-    nlp = spacy.blank("en")
-
-    config_zshot = PipelineConfig(linker=LinkerTARS())
-    nlp.add_pipe("zshot", config=config_zshot, last=True)
-    assert "zshot" in nlp.pipe_names
-    doc = nlp(INCOMPLETE_SPANS_TEXT)
-    assert len(doc.ents) > 0
-    del nlp.get_pipe('zshot').linker.model, nlp.get_pipe('zshot').linker
-    nlp.remove_pipe('zshot')
-    del nlp, config_zshot
+@pytest.mark.skip(reason="Too expensive to run on every commit")
+def test_load_wikipedia_trie():
+    trie = load_wikipedia_trie()
+    assert len(list(trie.trie_dict.keys())) == 6952
+
+
+@pytest.mark.skip(reason="Too expensive to run on every commit")
+def test_span_to_wiki():
+    s = Span(label="Surfing", start=0, end=10)
+    wiki_links = spans_to_wikipedia([s])
+    assert len(wiki_links) > 0
+    assert wiki_links[0].startswith("https://en.wikipedia.org/wiki?curid=")
+
+
+def test_create_input():
+    start_delimiter = "[START]"
+    end_delimiter = "[END]"
+    max_length = 10
+
+    times_rep = 6
+    sentence = "[START]" + " test" * times_rep + " [END]"
+    input_sentence = create_input(sentence, max_length, start_delimiter, end_delimiter)
+    assert input_sentence == sentence
+    times_rep = 12
+    sentence = "[START]" + " test" * times_rep + " [END]"
+    input_sentence = create_input(sentence, max_length, start_delimiter, end_delimiter)
+    assert input_sentence == " ".join(["test" for i in range(9)])
```

### Comparing `zshot-0.0.7/zshot/tests/mentions_extractor/test_flair_mentions_extractor.py` & `zshot-0.0.8/zshot/tests/mentions_extractor/test_flair_mentions_extractor.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/mentions_extractor/test_mention_extractor.py` & `zshot-0.0.8/zshot/tests/mentions_extractor/test_mention_extractor.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/mentions_extractor/test_smxm_mentions_extractor.py` & `zshot-0.0.8/zshot/tests/mentions_extractor/test_smxm_mentions_extractor.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/mentions_extractor/test_tars_mentions_extractor.py` & `zshot-0.0.8/zshot/tests/mentions_extractor/test_tars_mentions_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,10 +79,10 @@
         return
     nlp = spacy.blank("en")
 
     config_zshot = PipelineConfig(mentions_extractor=MentionsExtractorTARS())
     nlp.add_pipe("zshot", config=config_zshot, last=True)
     assert "zshot" in nlp.pipe_names
     doc = nlp(INCOMPLETE_SPANS_TEXT)
-    assert len(doc._.mentions) > 0
+    assert len(doc._.mentions) == 0
     nlp.remove_pipe('zshot')
     del doc, nlp
```

### Comparing `zshot-0.0.7/zshot/tests/relations_extractor/test_relations_extractor.py` & `zshot-0.0.8/zshot/tests/relations_extractor/test_relations_extractor.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/test_zshot.py` & `zshot-0.0.8/zshot/tests/test_zshot.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/utils/test_displacy.py` & `zshot-0.0.8/zshot/tests/utils/test_displacy.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/tests/utils/test_utils.py` & `zshot-0.0.8/zshot/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/alignment_utils.py` & `zshot-0.0.8/zshot/utils/alignment_utils.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/data_models/relation_span.py` & `zshot-0.0.8/zshot/utils/data_models/relation_span.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/displacy/displacy.py` & `zshot-0.0.8/zshot/utils/displacy/displacy.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/displacy/relations_render.py` & `zshot-0.0.8/zshot/utils/displacy/relations_render.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/displacy/templates.py` & `zshot-0.0.8/zshot/utils/displacy/templates.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/file_utils.py` & `zshot-0.0.8/zshot/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/models/smxm/data.py` & `zshot-0.0.8/zshot/utils/models/smxm/data.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/models/smxm/model.py` & `zshot-0.0.8/zshot/utils/models/smxm/model.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/utils/models/smxm/utils.py` & `zshot-0.0.8/zshot/utils/models/smxm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                         "They have no insurance on their cars. What else would you like? Whether holding an international cultural event "
                         "or setting the city's cultural policies, she always asks for the participation or input of other cities and counties.",
         )
         entities.insert(0, neg_ent)
 
     entity_labels = [e.name for e in entities]
     entity_descriptions = [e.description for e in entities]
+    entities.pop(0)
 
     return entity_labels, entity_descriptions
 
 
 def smxm_predict(model, tokenizer, sentences, entity_labels, entity_descriptions, batch_size):
     encoded_data, max_sentence_tokens = encode_data(
         sentences, entity_labels, entity_descriptions, tokenizer
```

### Comparing `zshot-0.0.7/zshot/utils/models/tars/utils.py` & `zshot-0.0.8/zshot/utils/models/tars/utils.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot/zshot.py` & `zshot-0.0.8/zshot/zshot.py`

 * *Files identical despite different names*

### Comparing `zshot-0.0.7/zshot.egg-info/PKG-INFO` & `zshot-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: zshot
-Version: 0.0.7
-Summary: Zero and Few shot named entity recognition
-Home-page: https://ibm.github.io/zshot
-Author: IBM Research
-Author-email: 
-License: MIT
-Keywords: NER Zero-Shot Few-Shot
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   
   <img height="170x" src="https://ibm.github.io/zshot/img/graph.png" />
   
   <h1>Zshot</h1>
 
   <p>
@@ -215,17 +203,32 @@
 >>> [is, similar, used, Business, Machines, materials]
 ```
 
 ### How to evaluate ZShot
 
 Evaluation is an important process to keep improving the performance of the models, that's why ZShot allows to evaluate the component with two predefined datasets: OntoNotes and MedMentions, in a Zero-Shot version in which the entities of the test and validation splits don't appear in the train set.  
 
-The package `evaluation` contains all the functionalities to evaluate the ZShot components. The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take as input the SpaCy `nlp` model and the dataset(s) and split(s) to evaluate. It will return a `str` containing a table with the results of the evaluation. For instance the evaluation of the ZShot custom component implemented above would be:
+The package `evaluation` contains all the functionalities to evaluate the ZShot components. The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take as input the SpaCy `nlp` model and the dataset to evaluate. It will return a `str` containing a table with the results of the evaluation. For instance the evaluation of the TARS linker in ZShot for the *Ontonotes validation* set would be:
 
 ```python
-from zshot.evaluation.zshot_evaluate import evaluate
-from datasets import Split
+import spacy
+
+from zshot import PipelineConfig
+from zshot.linker import LinkerTARS
+from zshot.evaluation.dataset import load_ontonotes_zs
+from zshot.evaluation.zshot_evaluate import evaluate, prettify_evaluate_report
+from zshot.evaluation.metrics.seqeval.seqeval import Seqeval
+
+ontonotes_zs = load_ontonotes_zs('validation')
+
+
+nlp = spacy.blank("en")
+nlp_config = PipelineConfig(
+    linker=LinkerTARS(),
+    entities=ontonotes_zs.entities
+)
+
+nlp.add_pipe("zshot", config=nlp_config, last=True)
 
-evaluation = evaluate(new_nlp, datasets="ontonotes", 
-                      splits=[Split.VALIDATION])
-print(evaluation)
+evaluation = evaluate(nlp, ontonotes_zs, metric=Seqeval())
+prettify_evaluate_report(evaluation)
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: zshot Version: 0.0.7 Summary: Zero and Few shot
-named entity recognition Home-page: https://ibm.github.io/zshot Author: IBM
-Research Author-email: License: MIT Keywords: NER Zero-Shot Few-Shot
-Description-Content-Type: text/markdown License-File: LICENSE
                   [https://ibm.github.io/zshot/img/graph.png]
                               ****** Zshot ******
           Zero and Few shot named entity & relationships recognition
 [Tutorials] [https://img.shields.io/pypi/v/zshot] [https://img.shields.io/pypi/
                            dm/zshot] [Build] [Build]
 **Documentation**: https://ibm.github.io/zshot **Source Code**: https://
 github.com/IBM/zshot Zshot is a highly customisable framework for performing
@@ -126,13 +122,18 @@
 used, Business, Machines, materials] ``` ### How to evaluate ZShot Evaluation
 is an important process to keep improving the performance of the models, that's
 why ZShot allows to evaluate the component with two predefined datasets:
 OntoNotes and MedMentions, in a Zero-Shot version in which the entities of the
 test and validation splits don't appear in the train set. The package
 `evaluation` contains all the functionalities to evaluate the ZShot components.
 The main function is `zshot.evaluation.zshot_evaluate.evaluate`, that will take
-as input the SpaCy `nlp` model and the dataset(s) and split(s) to evaluate. It
-will return a `str` containing a table with the results of the evaluation. For
-instance the evaluation of the ZShot custom component implemented above would
-be: ```python from zshot.evaluation.zshot_evaluate import evaluate from
-datasets import Split evaluation = evaluate(new_nlp, datasets="ontonotes",
-splits=[Split.VALIDATION]) print(evaluation) ```
+as input the SpaCy `nlp` model and the dataset to evaluate. It will return a
+`str` containing a table with the results of the evaluation. For instance the
+evaluation of the TARS linker in ZShot for the *Ontonotes validation* set would
+be: ```python import spacy from zshot import PipelineConfig from zshot.linker
+import LinkerTARS from zshot.evaluation.dataset import load_ontonotes_zs from
+zshot.evaluation.zshot_evaluate import evaluate, prettify_evaluate_report from
+zshot.evaluation.metrics.seqeval.seqeval import Seqeval ontonotes_zs =
+load_ontonotes_zs('validation') nlp = spacy.blank("en") nlp_config =
+PipelineConfig( linker=LinkerTARS(), entities=ontonotes_zs.entities )
+nlp.add_pipe("zshot", config=nlp_config, last=True) evaluation = evaluate(nlp,
+ontonotes_zs, metric=Seqeval()) prettify_evaluate_report(evaluation) ```
```

### Comparing `zshot-0.0.7/zshot.egg-info/SOURCES.txt` & `zshot-0.0.8/zshot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 zshot/evaluation/metrics/seqeval/__init__.py
 zshot/evaluation/metrics/seqeval/seqeval.py
 zshot/linker/__init__.py
 zshot/linker/linker.py
 zshot/linker/linker_blink.py
 zshot/linker/linker_smxm.py
 zshot/linker/linker_tars.py
+zshot/linker/linker_ensemble/__init__.py
+zshot/linker/linker_ensemble/linker_ensemble.py
+zshot/linker/linker_ensemble/utils.py
 zshot/linker/linker_regen/__init__.py
 zshot/linker/linker_regen/linker_regen.py
 zshot/linker/linker_regen/trie.py
 zshot/linker/linker_regen/utils.py
 zshot/mentions_extractor/__init__.py
 zshot/mentions_extractor/mentions_extractor.py
 zshot/mentions_extractor/mentions_extractor_flair.py
@@ -57,31 +60,34 @@
 zshot/tests/__init__.py
 zshot/tests/config.py
 zshot/tests/test_zshot.py
 zshot/tests/evaluation/__init__.py
 zshot/tests/evaluation/test_datasets.py
 zshot/tests/evaluation/test_evaluation.py
 zshot/tests/linker/__init__.py
+zshot/tests/linker/test_ensemble_linker.py
 zshot/tests/linker/test_linker.py
 zshot/tests/linker/test_regen_linker.py
 zshot/tests/linker/test_smxm_linker.py
 zshot/tests/linker/test_tars_linker.py
 zshot/tests/mentions_extractor/__init__.py
 zshot/tests/mentions_extractor/test_flair_mentions_extractor.py
 zshot/tests/mentions_extractor/test_mention_extractor.py
 zshot/tests/mentions_extractor/test_smxm_mentions_extractor.py
 zshot/tests/mentions_extractor/test_spacy_mentions_extractor.py
 zshot/tests/mentions_extractor/test_tars_mentions_extractor.py
 zshot/tests/relations_extractor/__init__.py
 zshot/tests/relations_extractor/test_relations_extractor.py
 zshot/tests/utils/__init__.py
 zshot/tests/utils/test_displacy.py
+zshot/tests/utils/test_ensembler.py
 zshot/tests/utils/test_utils.py
 zshot/utils/__init__.py
 zshot/utils/alignment_utils.py
+zshot/utils/ensembler.py
 zshot/utils/file_utils.py
 zshot/utils/data_models/__init__.py
 zshot/utils/data_models/entity.py
 zshot/utils/data_models/relation.py
 zshot/utils/data_models/relation_span.py
 zshot/utils/data_models/span.py
 zshot/utils/displacy/__init__.py
```

