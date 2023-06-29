# Comparing `tmp/adaseq-0.6.3.tar.gz` & `tmp/adaseq-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adaseq-0.6.3.tar", last modified: Mon Apr 24 06:03:35 2023, max compression
+gzip compressed data, was "dist/adaseq-0.6.4.tar", last modified: Thu Jun 29 06:06:26 2023, max compression
```

## Comparing `adaseq-0.6.3.tar` & `adaseq-0.6.4.tar`

### file list

```diff
@@ -1,132 +1,137 @@
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/
--rw-r--r--   0 pangda   (1345362) users      (100)    11416 2022-12-14 08:58:36.000000 adaseq-0.6.3/LICENSE
--rw-r--r--   0 pangda   (1345362) users      (100)     5906 2023-04-24 06:07:40.000000 adaseq-0.6.3/PKG-INFO
--rw-r--r--   0 pangda   (1345362) users      (100)     5526 2023-04-24 03:08:57.000000 adaseq-0.6.3/README.md
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/
--rw-r--r--   0 pangda   (1345362) users      (100)      283 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/__init__.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/commands/
--rw-r--r--   0 pangda   (1345362) users      (100)      844 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/commands/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4674 2023-02-16 06:14:41.000000 adaseq-0.6.3/adaseq/commands/pretrain.py
--rw-r--r--   0 pangda   (1345362) users      (100)      360 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/commands/subcommand.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3448 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/commands/test.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9019 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/commands/train.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/data/
--rw-r--r--   0 pangda   (1345362) users      (100)      155 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1969 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/batch.py
--rw-r--r--   0 pangda   (1345362) users      (100)      284 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/data/constant.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/data/data_collators/
--rw-r--r--   0 pangda   (1345362) users      (100)      539 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/data/data_collators/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5403 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/data_collators/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1777 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)      645 2023-01-12 08:59:17.000000 adaseq-0.6.3/adaseq/data/data_collators/pretraining_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)      703 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1275 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1651 2023-02-20 09:45:46.000000 adaseq-0.6.3/adaseq/data/data_collators/twostage_data_collator_with_padding.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/data/dataset_builders/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/data/dataset_builders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4771 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_builders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4079 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/dataset_builders/entity_typing_dataset_builder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     7721 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py
--rw-r--r--   0 pangda   (1345362) users      (100)    10006 2023-04-24 04:01:26.000000 adaseq-0.6.3/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4485 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/
--rw-r--r--   0 pangda   (1345362) users      (100)      139 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1143 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3234 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9864 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_manager.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/data/preprocessors/
--rw-r--r--   0 pangda   (1345362) users      (100)      602 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/data/preprocessors/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     7010 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/preprocessors/multilabel_typing_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)    10258 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/data/preprocessors/nlp_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5000 2023-01-12 08:59:17.000000 adaseq-0.6.3/adaseq/data/preprocessors/pretraining_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1439 2023-01-11 09:41:17.000000 adaseq-0.6.3/adaseq/data/preprocessors/relation_extraction_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3828 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/data/preprocessors/sequence_labeling_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1483 2023-01-11 09:41:17.000000 adaseq-0.6.3/adaseq/data/preprocessors/span_extraction_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3744 2023-02-20 09:45:46.000000 adaseq-0.6.3/adaseq/data/preprocessors/twostage_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2650 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/data/span_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)      948 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/tokenizer.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1678 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/data/utils.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/exporters/
--rw-r--r--   0 pangda   (1345362) users      (100)       76 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/exporters/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)      605 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/exporters/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1886 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/exporters/sequence_labeling_model_exporter.py
--rw-r--r--   0 pangda   (1345362) users      (100)      327 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/main.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4004 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/metainfo.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/metrics/
--rw-r--r--   0 pangda   (1345362) users      (100)      352 2023-02-16 06:13:38.000000 adaseq-0.6.3/adaseq/metrics/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9133 2023-02-16 06:16:11.000000 adaseq-0.6.3/adaseq/metrics/pretraining_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3188 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/relation_extraction_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4339 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/sequence_labeling_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4468 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/span_extraction_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8629 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/typing_metric.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/models/
--rw-r--r--   0 pangda   (1345362) users      (100)      515 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/models/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9420 2023-04-24 03:48:13.000000 adaseq-0.6.3/adaseq/models/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     6735 2023-02-20 09:45:46.000000 adaseq-0.6.3/adaseq/models/biaffine_ner_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9185 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/models/global_pointer_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)    18041 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/models/multilabel_typing_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8812 2023-02-16 07:59:33.000000 adaseq-0.6.3/adaseq/models/pretraining_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4045 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/models/relation_extraction_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8045 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/models/sequence_labeling_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)    11244 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/models/twostage_ner_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2304 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/models/utils.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/modules/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2018 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/biaffine.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/decoders/
--rw-r--r--   0 pangda   (1345362) users      (100)      250 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/decoders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4237 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/modules/decoders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)    46589 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/decoders/crf.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1959 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/decoders/mlm_head.py
--rw-r--r--   0 pangda   (1345362) users      (100)    12649 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/modules/decoders/pairwise_crf.py
--rw-r--r--   0 pangda   (1345362) users      (100)     6471 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/modules/decoders/partial_crf.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1190 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/dropouts.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/embedders/
--rw-r--r--   0 pangda   (1345362) users      (100)      191 2023-01-10 11:56:59.000000 adaseq-0.6.3/adaseq/modules/embedders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2227 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/embedders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5482 2023-02-08 11:54:02.000000 adaseq-0.6.3/adaseq/modules/embedders/embedding.py
--rw-r--r--   0 pangda   (1345362) users      (100)    17440 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/modules/embedders/transformer_embedder.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/encoders/
--rw-r--r--   0 pangda   (1345362) users      (100)      208 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1854 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5109 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/pytorch_rnn_encoder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3070 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/span_encoder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     7663 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/losses.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4024 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/scalar_mix.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9730 2022-12-30 08:44:17.000000 adaseq-0.6.3/adaseq/modules/util.py
--rw-r--r--   0 pangda   (1345362) users      (100)      547 2023-03-16 03:16:27.000000 adaseq-0.6.3/adaseq/ms_patch.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/pipelines/
--rw-r--r--   0 pangda   (1345362) users      (100)      173 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/pipelines/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1728 2023-01-11 07:11:36.000000 adaseq-0.6.3/adaseq/pipelines/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2413 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/pipelines/sequence_labeling_pipeline.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1760 2023-01-10 12:12:52.000000 adaseq-0.6.3/adaseq/pipelines/span_based_ner_pipeline.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/training/
--rw-r--r--   0 pangda   (1345362) users      (100)      207 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/training/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)      621 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/training/default_config.py
--rw-r--r--   0 pangda   (1345362) users      (100)     6339 2023-02-13 12:10:14.000000 adaseq-0.6.3/adaseq/training/default_trainer.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/training/hooks/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/training/hooks/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2987 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/training/hooks/text_logger_hook.py
--rw-r--r--   0 pangda   (1345362) users      (100)      961 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/training/lr_scheduler.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8422 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/training/optimizer.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3282 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/training/typing_trainer.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/utils/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/utils/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)      710 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/utils/checks.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1006 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/utils/common_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)       87 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/utils/constant.py
--rw-r--r--   0 pangda   (1345362) users      (100)      214 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/utils/file_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)      667 2023-02-16 06:13:37.000000 adaseq-0.6.3/adaseq/utils/hub_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4888 2023-01-31 06:40:19.000000 adaseq-0.6.3/adaseq/utils/logging.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3478 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/utils/yaml.py
--rw-r--r--   0 pangda   (1345362) users      (100)       72 2023-04-24 04:00:39.000000 adaseq-0.6.3/adaseq/version.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq.egg-info/
--rw-r--r--   0 pangda   (1345362) users      (100)     5906 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/PKG-INFO
--rw-r--r--   0 pangda   (1345362) users      (100)     3946 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/SOURCES.txt
--rw-r--r--   0 pangda   (1345362) users      (100)        1 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/dependency_links.txt
--rw-r--r--   0 pangda   (1345362) users      (100)       44 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/entry_points.txt
--rw-r--r--   0 pangda   (1345362) users      (100)      114 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/requires.txt
--rw-r--r--   0 pangda   (1345362) users      (100)        7 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/top_level.txt
--rw-r--r--   0 pangda   (1345362) users      (100)      412 2022-12-14 08:58:38.000000 adaseq-0.6.3/pyproject.toml
--rw-r--r--   0 pangda   (1345362) users      (100)       38 2023-04-24 06:07:40.000000 adaseq-0.6.3/setup.cfg
--rw-r--r--   0 pangda   (1345362) users      (100)     4724 2022-12-22 15:49:06.000000 adaseq-0.6.3/setup.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/
+-rw-r--r--   0 pangda   (1345362) users      (100)    11416 2022-12-14 08:58:36.000000 adaseq-0.6.4/LICENSE
+-rw-r--r--   0 pangda   (1345362) users      (100)     5906 2023-06-29 06:11:09.000000 adaseq-0.6.4/PKG-INFO
+-rw-r--r--   0 pangda   (1345362) users      (100)     5526 2023-05-06 07:59:03.000000 adaseq-0.6.4/README.md
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:07.000000 adaseq-0.6.4/adaseq/
+-rw-r--r--   0 pangda   (1345362) users      (100)      283 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/__init__.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:07.000000 adaseq-0.6.4/adaseq/commands/
+-rw-r--r--   0 pangda   (1345362) users      (100)      844 2022-12-14 08:58:36.000000 adaseq-0.6.4/adaseq/commands/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4674 2023-02-16 06:14:41.000000 adaseq-0.6.4/adaseq/commands/pretrain.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      360 2022-12-14 08:58:36.000000 adaseq-0.6.4/adaseq/commands/subcommand.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3448 2022-12-21 02:38:01.000000 adaseq-0.6.4/adaseq/commands/test.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9019 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/commands/train.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:07.000000 adaseq-0.6.4/adaseq/data/
+-rw-r--r--   0 pangda   (1345362) users      (100)      155 2022-12-21 02:38:01.000000 adaseq-0.6.4/adaseq/data/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1969 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/data/batch.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      284 2023-02-16 06:22:26.000000 adaseq-0.6.4/adaseq/data/constant.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:07.000000 adaseq-0.6.4/adaseq/data/data_collators/
+-rw-r--r--   0 pangda   (1345362) users      (100)      642 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/data/data_collators/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5403 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/data/data_collators/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1860 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      645 2023-01-12 08:59:17.000000 adaseq-0.6.4/adaseq/data/data_collators/pretraining_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      703 2022-12-14 08:58:36.000000 adaseq-0.6.4/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1275 2022-12-21 02:38:01.000000 adaseq-0.6.4/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1651 2023-02-20 09:45:46.000000 adaseq-0.6.4/adaseq/data/data_collators/twostage_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2094 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/data/data_collators/word_extraction_data_collator_with_padding.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:07.000000 adaseq-0.6.4/adaseq/data/dataset_builders/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.4/adaseq/data/dataset_builders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4771 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/data/dataset_builders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4079 2022-12-21 02:38:01.000000 adaseq-0.6.4/adaseq/data/dataset_builders/entity_typing_dataset_builder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     7721 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9605 2023-05-06 07:58:21.000000 adaseq-0.6.4/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4485 2022-12-21 02:38:01.000000 adaseq-0.6.4/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:08.000000 adaseq-0.6.4/adaseq/data/dataset_dumpers/
+-rw-r--r--   0 pangda   (1345362) users      (100)      139 2022-12-14 08:58:36.000000 adaseq-0.6.4/adaseq/data/dataset_dumpers/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1143 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/data/dataset_dumpers/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3234 2022-12-21 02:38:01.000000 adaseq-0.6.4/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9864 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/data/dataset_manager.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:08.000000 adaseq-0.6.4/adaseq/data/preprocessors/
+-rw-r--r--   0 pangda   (1345362) users      (100)      670 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/data/preprocessors/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     7357 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/data/preprocessors/multilabel_typing_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    10258 2023-02-16 06:22:26.000000 adaseq-0.6.4/adaseq/data/preprocessors/nlp_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5000 2023-01-12 08:59:17.000000 adaseq-0.6.4/adaseq/data/preprocessors/pretraining_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1439 2023-01-11 09:41:17.000000 adaseq-0.6.4/adaseq/data/preprocessors/relation_extraction_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     6802 2023-06-16 08:28:39.000000 adaseq-0.6.4/adaseq/data/preprocessors/sequence_labeling_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1545 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/data/preprocessors/span_extraction_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3744 2023-02-20 09:45:46.000000 adaseq-0.6.4/adaseq/data/preprocessors/twostage_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2938 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/data/preprocessors/word_extraction_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2650 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/data/span_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      948 2023-06-15 01:45:30.000000 adaseq-0.6.4/adaseq/data/tokenizer.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1678 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/data/utils.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:08.000000 adaseq-0.6.4/adaseq/exporters/
+-rw-r--r--   0 pangda   (1345362) users      (100)      156 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/exporters/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      605 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/exporters/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2056 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/exporters/multilabel_typing_model_exporter.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1886 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/exporters/sequence_labeling_model_exporter.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      327 2022-12-14 08:58:36.000000 adaseq-0.6.4/adaseq/main.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4202 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/metainfo.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:08.000000 adaseq-0.6.4/adaseq/metrics/
+-rw-r--r--   0 pangda   (1345362) users      (100)      352 2023-02-16 06:13:38.000000 adaseq-0.6.4/adaseq/metrics/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9133 2023-02-16 06:16:11.000000 adaseq-0.6.4/adaseq/metrics/pretraining_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3188 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/metrics/relation_extraction_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4339 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/metrics/sequence_labeling_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4468 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/metrics/span_extraction_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8963 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/metrics/typing_metric.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:08.000000 adaseq-0.6.4/adaseq/models/
+-rw-r--r--   0 pangda   (1345362) users      (100)      551 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/models/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9420 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/models/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8464 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/models/biaffine_ner_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9271 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/models/global_pointer_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    17606 2023-05-06 07:59:03.000000 adaseq-0.6.4/adaseq/models/multilabel_typing_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8812 2023-02-16 07:59:33.000000 adaseq-0.6.4/adaseq/models/pretraining_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4045 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/models/relation_extraction_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8795 2023-06-29 03:26:25.000000 adaseq-0.6.4/adaseq/models/sequence_labeling_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    11244 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/models/twostage_ner_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2304 2023-01-12 08:59:18.000000 adaseq-0.6.4/adaseq/models/utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    11912 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/models/w2ner_model.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/modules/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.4/adaseq/modules/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2018 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/modules/biaffine.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/modules/decoders/
+-rw-r--r--   0 pangda   (1345362) users      (100)      250 2023-01-12 08:59:18.000000 adaseq-0.6.4/adaseq/modules/decoders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4237 2022-12-14 08:58:37.000000 adaseq-0.6.4/adaseq/modules/decoders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    46589 2023-01-12 08:59:18.000000 adaseq-0.6.4/adaseq/modules/decoders/crf.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1959 2023-01-12 08:59:18.000000 adaseq-0.6.4/adaseq/modules/decoders/mlm_head.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    12649 2022-12-14 08:58:37.000000 adaseq-0.6.4/adaseq/modules/decoders/pairwise_crf.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     6471 2022-12-14 08:58:37.000000 adaseq-0.6.4/adaseq/modules/decoders/partial_crf.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1190 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/modules/dropouts.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/modules/embedders/
+-rw-r--r--   0 pangda   (1345362) users      (100)      191 2023-01-10 11:56:59.000000 adaseq-0.6.4/adaseq/modules/embedders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2227 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/modules/embedders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5482 2023-02-08 11:54:02.000000 adaseq-0.6.4/adaseq/modules/embedders/embedding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    18187 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/modules/embedders/transformer_embedder.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/modules/encoders/
+-rw-r--r--   0 pangda   (1345362) users      (100)      244 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/modules/encoders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1854 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/modules/encoders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1648 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/modules/encoders/cnn_encoder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5102 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/modules/encoders/pytorch_rnn_encoder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3070 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/modules/encoders/span_encoder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     7663 2023-01-12 08:59:18.000000 adaseq-0.6.4/adaseq/modules/losses.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4024 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/modules/scalar_mix.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9730 2022-12-30 08:44:17.000000 adaseq-0.6.4/adaseq/modules/util.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      547 2023-03-16 03:16:27.000000 adaseq-0.6.4/adaseq/ms_patch.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/pipelines/
+-rw-r--r--   0 pangda   (1345362) users      (100)      173 2023-02-16 06:22:26.000000 adaseq-0.6.4/adaseq/pipelines/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1728 2023-01-11 07:11:36.000000 adaseq-0.6.4/adaseq/pipelines/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2413 2023-02-16 06:22:26.000000 adaseq-0.6.4/adaseq/pipelines/sequence_labeling_pipeline.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1760 2023-01-10 12:12:52.000000 adaseq-0.6.4/adaseq/pipelines/span_based_ner_pipeline.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/training/
+-rw-r--r--   0 pangda   (1345362) users      (100)      207 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/training/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      621 2023-02-16 06:22:26.000000 adaseq-0.6.4/adaseq/training/default_config.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     6339 2023-02-13 12:10:14.000000 adaseq-0.6.4/adaseq/training/default_trainer.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/training/hooks/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.4/adaseq/training/hooks/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2987 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/training/hooks/text_logger_hook.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      961 2023-01-12 08:59:18.000000 adaseq-0.6.4/adaseq/training/lr_scheduler.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8422 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/training/optimizer.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3282 2023-02-16 06:13:36.000000 adaseq-0.6.4/adaseq/training/typing_trainer.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:09.000000 adaseq-0.6.4/adaseq/utils/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.4/adaseq/utils/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      710 2022-12-14 08:58:37.000000 adaseq-0.6.4/adaseq/utils/checks.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1006 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/utils/common_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)       87 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/utils/constant.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      214 2022-12-21 02:38:02.000000 adaseq-0.6.4/adaseq/utils/file_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      667 2023-02-16 06:13:37.000000 adaseq-0.6.4/adaseq/utils/hub_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4888 2023-01-31 06:40:19.000000 adaseq-0.6.4/adaseq/utils/logging.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3478 2023-05-06 07:58:53.000000 adaseq-0.6.4/adaseq/utils/yaml.py
+-rw-r--r--   0 pangda   (1345362) users      (100)       72 2023-06-29 06:10:22.000000 adaseq-0.6.4/adaseq/version.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-06-29 06:11:07.000000 adaseq-0.6.4/adaseq.egg-info/
+-rw-r--r--   0 pangda   (1345362) users      (100)     5906 2023-06-29 06:11:06.000000 adaseq-0.6.4/adaseq.egg-info/PKG-INFO
+-rw-r--r--   0 pangda   (1345362) users      (100)     4198 2023-06-29 06:11:06.000000 adaseq-0.6.4/adaseq.egg-info/SOURCES.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)        1 2023-06-29 06:11:06.000000 adaseq-0.6.4/adaseq.egg-info/dependency_links.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)       44 2023-06-29 06:11:06.000000 adaseq-0.6.4/adaseq.egg-info/entry_points.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)      106 2023-06-29 06:11:06.000000 adaseq-0.6.4/adaseq.egg-info/requires.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)        7 2023-06-29 06:11:06.000000 adaseq-0.6.4/adaseq.egg-info/top_level.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)      412 2022-12-14 08:58:38.000000 adaseq-0.6.4/pyproject.toml
+-rw-r--r--   0 pangda   (1345362) users      (100)       38 2023-06-29 06:11:09.000000 adaseq-0.6.4/setup.cfg
+-rw-r--r--   0 pangda   (1345362) users      (100)     4724 2022-12-22 15:49:06.000000 adaseq-0.6.4/setup.py
```

### Comparing `adaseq-0.6.3/LICENSE` & `adaseq-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/PKG-INFO` & `adaseq-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaseq
-Version: 0.6.3
+Version: 0.6.4
 Summary: AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 Home-page: https://github.com/modelscope/adaseq
 Author: Alibaba Damo Academy NLP foundation team
 License: Apache License 2.0
 Platform: any
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `adaseq-0.6.3/README.md` & `adaseq-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/commands/__init__.py` & `adaseq-0.6.4/adaseq/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/commands/pretrain.py` & `adaseq-0.6.4/adaseq/commands/pretrain.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/commands/test.py` & `adaseq-0.6.4/adaseq/commands/test.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/commands/train.py` & `adaseq-0.6.4/adaseq/commands/train.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/batch.py` & `adaseq-0.6.4/adaseq/data/batch.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/__init__.py` & `adaseq-0.6.4/adaseq/data/data_collators/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,7 +6,10 @@
 from .sequence_labeling_data_collator_with_padding import (
     SequenceLabelingDataCollatorWithPadding,
 )
 from .span_extraction_data_collator_with_padding import (
     SpanExtractionDataCollatorWithPadding,
 )
 from .twostage_data_collator_with_padding import TwostageDataCollatorWithPadding
+from .word_extraction_data_collator_with_padding import (
+    WordExtractionDataCollatorWithPadding,
+)
```

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/base.py` & `adaseq-0.6.4/adaseq/data/data_collators/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py` & `adaseq-0.6.4/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,24 @@
     def padding(self, batch: Dict[str, Any], **kwargs) -> Dict[str, Any]:
         """
         Padding a batch. In addition to the fields padded by base class DataCollatorWithPadding,
         'mention_boundary'、'type_ids'、'mention_mask' are padded here.
         """
 
         max_span_count = max([len(x[0]) for x in batch['mention_boundary']])
+        for type_ids in batch['type_ids']:
+            if len(type_ids) > 0:
+                type_num = len(type_ids[0])
+                break
         for i in range(len(batch['mention_boundary'])):
             difference = max_span_count - len(batch['mention_boundary'][i][0])
             if difference > 0:
                 batch['mention_boundary'][i][0] = batch['mention_boundary'][i][0] + [0] * difference
                 batch['mention_boundary'][i][1] = batch['mention_boundary'][i][1] + [0] * difference
-                batch['type_ids'][i] = (
-                    batch['type_ids'][i] + ([[0] * len(batch['type_ids'][i][0])]) * difference
-                )
+                batch['type_ids'][i] = batch['type_ids'][i] + ([[0] * type_num]) * difference
                 batch['mention_mask'][i] = batch['mention_mask'][i] + [0] * difference
         return batch
 
 
 @DATA_COLLATORS.register_module(module_name=DataCollators.multi_label_concat_typing_data_collator)
 class MultiLabelConcatTypingDataCollatorWithPadding(DataCollatorWithPadding):
     """Padding method for multilabel span concat typing dataset."""
```

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/pretraining_data_collator_with_padding.py` & `adaseq-0.6.4/adaseq/data/data_collators/pretraining_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py` & `adaseq-0.6.4/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py` & `adaseq-0.6.4/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/data_collators/twostage_data_collator_with_padding.py` & `adaseq-0.6.4/adaseq/data/data_collators/twostage_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_builders/base.py` & `adaseq-0.6.4/adaseq/data/dataset_builders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_builders/entity_typing_dataset_builder.py` & `adaseq-0.6.4/adaseq/data/dataset_builders/entity_typing_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py` & `adaseq-0.6.4/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py` & `adaseq-0.6.4/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 
-import ast
 import json
 from typing import Dict
 
 import datasets
 from datasets import Features, Value
 
 from adaseq.data.constant import PAD_LABEL
@@ -172,44 +171,36 @@
         is_end_included = corpus_config.get('is_end_included', False)
 
         with open(filepath, encoding='utf-8') as f:
             guid = 0
             for line in f:
                 if line.strip() == '':
                     continue
-                try:
-                    try:
-                        example = json.loads(line)
-                    except:
-                        example = ast.literal_eval(line)
-                    text = example[text_key]
-                    if isinstance(text, list):
-                        tokens = text
-                    elif isinstance(text, str):
-                        if tokenizer == 'char':
-                            tokens = list(text)
-                        elif tokenizer == 'blank':
-                            tokens = text.split(' ')
-                        else:
-                            raise RuntimeError
+                example = json.loads(line)
+                text = example[text_key]
+                if isinstance(text, list):
+                    tokens = text
+                elif isinstance(text, str):
+                    if tokenizer == 'char':
+                        tokens = list(text)
+                    elif tokenizer == 'blank':
+                        tokens = text.split(' ')
                     else:
-                        raise ValueError('Unsupported text input.')
-                    spans = []
-                    for span in example[spans_key]:
-                        if is_end_included:
-                            span['end'] += 1
-                        if 'word' in span:
-                            del span['word']
-                        if isinstance(span['type'], list):
-                            span['type'] = span['type'][0]
-                        spans.append(span)
-                    mask = [True] * len(tokens)
-                    yield guid, {'id': str(guid), 'tokens': tokens, 'spans': spans, 'mask': mask}
-                except:
-                    pass
+                        raise RuntimeError
+                else:
+                    raise ValueError('Unsupported text input.')
+                spans = []
+                for span in example[spans_key]:
+                    if is_end_included:
+                        span['end'] += 1
+                    if 'word' in span:
+                        del span['word']
+                    spans.append(span)
+                mask = [True] * len(tokens)
+                yield guid, {'id': str(guid), 'tokens': tokens, 'spans': spans, 'mask': mask}
                 guid += 1
 
     @classmethod
     def _load_cluener_file(cls, filepath, corpus_config):
         is_end_included = corpus_config.get('is_end_included', False)
 
         with open(filepath, encoding='utf-8') as f:
```

### Comparing `adaseq-0.6.3/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py` & `adaseq-0.6.4/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_dumpers/base.py` & `adaseq-0.6.4/adaseq/data/dataset_dumpers/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py` & `adaseq-0.6.4/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/dataset_manager.py` & `adaseq-0.6.4/adaseq/data/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/__init__.py` & `adaseq-0.6.4/adaseq/data/preprocessors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 )
 from .nlp_preprocessor import NLPPreprocessor
 from .pretraining_preprocessor import PretrainingPreprocessor
 from .relation_extraction_preprocessor import RelationExtractionPreprocessor
 from .sequence_labeling_preprocessor import SequenceLabelingPreprocessor
 from .span_extraction_preprocessor import SpanExtracionPreprocessor
 from .twostage_preprocessor import TwoStagePreprocessor
+from .word_extraction_preprocessor import WordExtracionPreprocessor
```

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/multilabel_typing_preprocessor.py` & `adaseq-0.6.4/adaseq/data/preprocessors/multilabel_typing_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from typing import Any, Dict
 
 import numpy as np
 from modelscope.preprocessors.builder import PREPROCESSORS
-from modelscope.utils.constant import Fields
+from modelscope.utils.constant import Fields, ModeKeys
 
 from adaseq.metainfo import Preprocessors
 
 from .nlp_preprocessor import NLPPreprocessor
 
 
 @PREPROCESSORS.register_module(
-    Fields.nlp, module_name=Preprocessors.multilabel_span_typing_preprocessor
+    group_key=Fields.nlp, module_name=Preprocessors.multilabel_span_typing_preprocessor
 )
 class MultiLabelSpanTypingPreprocessor(NLPPreprocessor):
     """Preprocessor for multilabel (aka multi-type) span typing task.
     span targets are processed into mention_boundary, type_ids.
     examples:
         span: {'start':1, 'end':2, 'type': ['PER']}
         processed: {'mention_boundary': [[1], [2]], 'type_ids':[1]}
@@ -32,24 +32,29 @@
         boundary_starts = []
         boundary_ends = []
         mention_mask = []
         for span in data['spans']:
             boundary_starts.append(span['start'])
             boundary_ends.append(span['end'] - 1)
             mention_mask.append(1)
-            type_ids = [self.label_to_id.get(x, -1) for x in span['type']]
-            padded_type_ids = [0] * len(self.label_to_id)
-            for t in type_ids:
-                if t != -1:
-                    padded_type_ids[t] = 1
-            mention_type_ids.append(padded_type_ids)
+            if 'type' in span:
+                type_ids = [self.label_to_id.get(x, -1) for x in span['type']]
+                padded_type_ids = [0] * len(self.label_to_id)
+                for t in type_ids:
+                    if t != -1:
+                        padded_type_ids[t] = 1
+                mention_type_ids.append(padded_type_ids)
 
         output['mention_boundary'] = [boundary_starts, boundary_ends]
         output['mention_mask'] = mention_mask  # mask, 为了避开nlp_preprocessor对他做padding.
-        output['type_ids'] = mention_type_ids
+        if len(mention_type_ids) > 0:
+            output['type_ids'] = mention_type_ids
+        if self.mode == ModeKeys.INFERENCE:
+            output['mention_boundary'] = np.expand_dims(np.array(output['mention_boundary']), 0)
+            output['mention_mask'] = np.expand_dims(np.array(output['mention_mask']), 0)
         return output
 
 
 @PREPROCESSORS.register_module(
     Fields.nlp, module_name=Preprocessors.multilabel_concat_typing_preprocessor
 )
 class MultiLabelConcatTypingPreprocessor(NLPPreprocessor):
```

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/nlp_preprocessor.py` & `adaseq-0.6.4/adaseq/data/preprocessors/nlp_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/pretraining_preprocessor.py` & `adaseq-0.6.4/adaseq/data/preprocessors/pretraining_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/relation_extraction_preprocessor.py` & `adaseq-0.6.4/adaseq/data/preprocessors/relation_extraction_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/span_extraction_preprocessor.py` & `adaseq-0.6.4/adaseq/data/preprocessors/span_extraction_preprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,10 +31,12 @@
         length = len(output['tokens']['mask']) - 2 * int(self.add_special_tokens)
         # calculate span labels
         span_labels = np.zeros([length, length])
         for span in data['spans']:
             # self.label_to_id doesn't have non-entity label,
             # we set index 0 as non-entity label, so we add 1 to type_id
             type_id = self.label_to_id[span['type']] + 1
+            if span['end'] > length:
+                continue
             span_labels[span['start']][span['end'] - 1] = type_id
         output['span_labels'] = span_labels
         return output
```

### Comparing `adaseq-0.6.3/adaseq/data/preprocessors/twostage_preprocessor.py` & `adaseq-0.6.4/adaseq/data/preprocessors/twostage_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/span_utils.py` & `adaseq-0.6.4/adaseq/data/span_utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/tokenizer.py` & `adaseq-0.6.4/adaseq/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/data/utils.py` & `adaseq-0.6.4/adaseq/data/utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/exporters/base.py` & `adaseq-0.6.4/adaseq/exporters/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/exporters/sequence_labeling_model_exporter.py` & `adaseq-0.6.4/adaseq/exporters/sequence_labeling_model_exporter.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/metainfo.py` & `adaseq-0.6.4/adaseq/metainfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     biaffine_ner_model = 'biaffine-ner-model'
     relation_extraction_model = 'relation-extraction-model'
     multilabel_concat_typing_model = 'multilabel-concat-typing-model'
     multilabel_span_typing_model = 'multilabel-span-typing-model'
     multilabel_concat_typing_model_mcce_s = 'multilabel-concat-typing-model-mcce-s'
     pretraining_model = 'pretraining-model'
     twostage_ner_model = 'twostage-ner-model'
+    w2ner_model = 'w2ner-model'
 
 
 class Embedders:
     """Names for different embedders"""
 
     embedding = 'embedding'
     transformer_embedder = 'transformer-embedder'
@@ -57,14 +58,15 @@
 class Encoders:
     """Names for different encoders"""
 
     span_encoder = 'span-encoder'
     gru_encoder = 'gru'
     rnn_encoder = 'rnn'
     lstm_encoder = 'lstm'
+    cnn_encoder = 'cnn'
 
 
 class Decoders:
     """Names for different decoders"""
 
     crf = 'crf'
     partial_crf = 'partial-crf'
@@ -81,26 +83,28 @@
     relation_extraction_preprocessor = 'relation-extraction-preprocessor'
     span_extraction_preprocessor = 'span-extraction-preprocessor'
     multilabel_span_typing_preprocessor = 'multilabel-span-typing-preprocessor'
     multilabel_concat_typing_preprocessor = 'multilabel-concat-typing-preprocessor'
     multilabel_concat_typing_mcce_preprocessor = 'multilabel-concat-typing-mcce-preprocessor'
     pretraining_preprocessor = 'pretraining-preprocessor'
     twostage_preprocessor = 'twostage-preprocessor'
+    word_extraction_preprocessor = 'word-extraction-preprocessor'
 
 
 class DataCollators:
     """Names for different data_collators"""
 
     data_collator_with_padding = 'DataCollatorWithPadding'
     sequence_labeling_data_collator = 'SequenceLabelingDataCollatorWithPadding'
     span_extraction_data_collator = 'SpanExtractionDataCollatorWithPadding'
     multi_label_span_typing_data_collator = 'MultiLabelSpanTypingDataCollatorWithPadding'
     multi_label_concat_typing_data_collator = 'MultiLabelConcatTypingDataCollatorWithPadding'
     pretraining_data_collator = 'PretrainingDataCollatorWithPadding'
     twostage_data_collator = 'TwostageDataCollatorWithPadding'
+    word_extraction_data_collator = 'WordExtractionDataCollatorWithPadding'
 
 
 class Trainers:
     """Names for different trainers"""
 
     default_trainer = 'default-trainer'
     typing_trainer = 'typing-trainer'
```

### Comparing `adaseq-0.6.3/adaseq/metrics/pretraining_metric.py` & `adaseq-0.6.4/adaseq/metrics/pretraining_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/metrics/relation_extraction_metric.py` & `adaseq-0.6.4/adaseq/metrics/relation_extraction_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/metrics/sequence_labeling_metric.py` & `adaseq-0.6.4/adaseq/metrics/sequence_labeling_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/metrics/span_extraction_metric.py` & `adaseq-0.6.4/adaseq/metrics/span_extraction_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/metrics/typing_metric.py` & `adaseq-0.6.4/adaseq/metrics/typing_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,18 +112,26 @@
         super().__init__(*args, **kwargs)
         self.scorer = SetScore()
 
     def add(self, outputs: Dict, inputs: Dict):  # noqa: D102
         predicts = outputs['predicts']
         pred_results = list()
         ground_truths = list()
-        for i, meta in enumerate(inputs['meta']):
-            for j, s in enumerate(meta['spans']):
-                pred_results.append(predicts[i][j])
-                ground_truths.append(set(s['type']))
+        for i, golden_type_ids in enumerate(inputs['type_ids']):
+            for j in range(len(golden_type_ids)):
+
+                def one_hot_to_list(in_tensor):
+                    id_list = set((np.where(in_tensor.detach().cpu() == 1)[0]))
+                    return id_list
+
+                ground_truths.append(one_hot_to_list(golden_type_ids[j]))
+                if j < len(predicts[i]):
+                    pred_results.append(one_hot_to_list(predicts[i][j]))
+                else:
+                    pred_results.append(set([]))
         self.scorer.update(ground_truths, pred_results)
 
     def evaluate(self):  # noqa: D102
         score_detail = self.scorer.result()
         scores = {}
         scores[MetricKeys.PRECISION] = score_detail['macro_p']
         scores[MetricKeys.RECALL] = score_detail['macro_r']
```

### Comparing `adaseq-0.6.3/adaseq/models/__init__.py` & `adaseq-0.6.4/adaseq/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,7 +7,8 @@
     MultiLabelConcatTypingModelMCCES,
     MultiLabelSpanTypingModel,
 )
 from .pretraining_model import PretrainingModel
 from .relation_extraction_model import RelationExtractionModel
 from .sequence_labeling_model import SequenceLabelingModel
 from .twostage_ner_model import TwoStageNERModel
+from .w2ner_model import W2NerModel
```

### Comparing `adaseq-0.6.3/adaseq/models/base.py` & `adaseq-0.6.4/adaseq/models/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/models/biaffine_ner_model.py` & `adaseq-0.6.4/adaseq/models/biaffine_ner_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,23 +26,25 @@
     def __init__(
         self,
         id_to_label: Union[Dict[int, str], List[str]],
         embedder: Optional[Union[Embedder, Dict]] = None,
         encoder: Optional[Union[Encoder, Dict[str, Any]]] = None,
         biaffine_ffnn_size: int = -1,
         biaffine_bias: bool = True,
+        multi_label: bool = False,
         flat_ner: bool = True,
         dropout: float = 0.0,
         word_dropout: bool = False,
         **kwargs
     ):
         super().__init__(**kwargs)
         self.id_to_label = id_to_label
         self.num_labels = len(id_to_label) + 1  # leave 0 as non-entity label
         self.flat_ner = flat_ner
+        self.multi_label = multi_label
 
         if isinstance(embedder, Embedder):
             self.embedder = embedder
         else:
             self.embedder = Embedder.from_config(embedder, **kwargs)
         hidden_size = self.embedder.get_output_dim()
 
@@ -53,15 +55,15 @@
                 self.encoder = encoder
             else:
                 self.encoder = Encoder.from_config(encoder)
             assert hidden_size == self.encoder.get_input_dim()
             hidden_size = self.encoder.get_output_dim()
 
         self.scorer = BiaffineScorer(
-            hidden_size, biaffine_ffnn_size, self.num_labels, biaffine_bias
+            hidden_size, biaffine_ffnn_size, self.num_labels * (1 + int(multi_label)), biaffine_bias
         )
 
         self.use_dropout = dropout > 0.0
         if self.use_dropout:
             if word_dropout:
                 self.dropout = WordDropout(dropout)
             else:
@@ -86,15 +88,14 @@
         mask = get_tokens_mask(tokens, x.size(1))
 
         if self.use_dropout:
             x = self.dropout(x)
 
         if self.encoder is not None:
             x = self.encoder(x, mask)
-
             if self.use_dropout:
                 x = self.dropout(x)
 
         span_scores = self.scorer(x)
         outputs = {'span_scores': span_scores}
 
         if self.training and span_labels is not None:
@@ -108,34 +109,63 @@
     def _calculate_loss(
         self, span_scores: torch.Tensor, span_labels: torch.LongTensor, mask: torch.BoolTensor
     ) -> torch.Tensor:
         """
         span_labels : (batch_size, seq_len, seq_len)
         span_scores : (batch_size, seq_len, seq_len, num_classes)
         """
-        label_mask = torch.triu(mask.unsqueeze(-1).expand_as(span_labels).clone())
-        loss = nn.functional.cross_entropy(
-            span_scores.reshape(-1, self.num_labels),
-            span_labels.masked_fill(~label_mask, -100).reshape(-1),
-        )
+        if self.multi_label:  # TODO why?
+            new_scores = span_scores.view(-1, 2)
+            new_labels = nn.functional.one_hot(span_labels, self.num_labels)
+            mi_mask = torch.triu(mask.unsqueeze(-1).expand_as(span_labels).clone())
+            en_mask = mi_mask.unsqueeze(-1).expand_as(new_labels).clone()
+            use_labels = new_labels.masked_fill(~en_mask, -100).view(-1)
+            loss = nn.functional.cross_entropy(new_scores, use_labels)
+        else:
+            label_mask = torch.triu(mask.unsqueeze(-1).expand_as(span_labels).clone())
+            loss = nn.functional.cross_entropy(
+                span_scores.reshape(-1, self.num_labels),
+                span_labels.masked_fill(~label_mask, -100).reshape(-1),
+            )
         return loss
 
     def decode(self, span_scores, mask):
         """
         :param span_scores: (b, t, t, c)
         :param mask: (b, t)
         :return:
         """
+        batch_size, t_shape = span_scores.shape[0], span_scores.shape[1]
         lengths = mask.sum(-1).tolist()
-        # (b, t, t)
-        type_idxs = span_scores.detach().argmax(dim=-1)
-        # (b, t, t)
-        span_max_score = (
-            span_scores.detach().gather(dim=-1, index=type_idxs.unsqueeze(-1)).squeeze(-1)
-        )
+        # mult = self.multi_label and not self.flat_ner
+        if not self.multi_label:
+            # (b, t, t)
+            type_idxs = span_scores.detach().argmax(dim=-1)
+            # (b, t, t)
+            span_max_score = (
+                span_scores.detach().gather(dim=-1, index=type_idxs.unsqueeze(-1)).squeeze(-1)
+            )
+        else:
+            binary_scores = span_scores.detach().view(-1, 2)  # (b*t*t*c, 2)
+            # if not mult:
+            #     new_span_scores = binary_scores[..., 1].view(-1, t_shape, t_shape, self.num_labels)
+            #     assert new_span_scores.shape[0] == batch_size
+            #     type_idxs = new_span_scores.argmax(dim=-1)
+            #     span_max_score = (
+            #         new_span_scores.gather(dim=-1, index=type_idxs.unsqueeze(-1)).squeeze(1)
+            #     )
+            # else:
+            #     cur = binary_scores.argmax(dim=-1).view(-1, self.num_labels)
+
+            # use the second dim as span_scores
+            span_scores = binary_scores[..., 1].view(-1, t_shape, t_shape, self.num_labels)
+            assert span_scores.shape[0] == batch_size
+            type_idxs = span_scores.argmax(dim=-1)
+            span_max_score = span_scores.gather(dim=-1, index=type_idxs.unsqueeze(-1)).squeeze(1)
+
         final = []
         for span_score, tids, l in zip(span_max_score, type_idxs, lengths):
             cands = []
             for s in range(l):
                 for e in range(s, l):
                     type_id = tids[s, e].item()
                     if type_id > 0:
```

### Comparing `adaseq-0.6.3/adaseq/models/global_pointer_model.py` & `adaseq-0.6.4/adaseq/models/global_pointer_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         span_labels: Optional[torch.LongTensor] = None,
         meta: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:  # noqa
         """TODO: docstring"""
         entity_score = self._forward(tokens)
         if self.training:
             onehot = nn.functional.one_hot(span_labels, self.num_classes)
+            # we choose the indexes from 1, so the label_id does not need to minus 1.
             label_matrix = onehot.permute(0, 3, 1, 2)[:, 1:, ...]
             loss = self._calculate_loss(entity_score, label_matrix)
             outputs = {'entity_score': entity_score, 'loss': loss}
         else:
             predicts = self.decode(entity_score)
             outputs = {'entity_score': entity_score, 'predicts': predicts}
         return outputs
```

### Comparing `adaseq-0.6.3/adaseq/models/multilabel_typing_model.py` & `adaseq-0.6.4/adaseq/models/multilabel_typing_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             self.embedder = Embedder.from_config(embedder)
 
         self.span_encoder = SpanEncoder(
             self.embedder.get_output_dim(), span_encoder_method, **kwargs
         )
         self.linear_input_dim = self.span_encoder.output_dim
 
-        self.id_to_label = id_to_label
+        self.id_to_label = {int(k): v for k, v in id_to_label.items()}
         self.num_labels = len(id_to_label)
         self.linear = nn.Linear(self.linear_input_dim, self.num_labels)
 
         self.use_dropout = dropout > 0.0
         if self.use_dropout:
             if word_dropout:
                 self.dropout = WordDropout(dropout)
@@ -110,15 +110,16 @@
         # B x M -> B*M x 1
         logits = self._forward(tokens, mention_boundary)
         mask = mention_mask.reshape(-1).unsqueeze(-1)
         if self.training:
             loss = self._calculate_loss(logits, type_ids, mask)
             outputs = {'logits': logits, 'loss': loss}
         else:
-            batch_size, max_mention_per_sent = type_ids.shape[0:2]  # TODO: no supervision
+            batch_size = tokens['input_ids'].shape[0]
+            max_mention_per_sent = mention_boundary.shape[2]
             logits = logits.reshape(batch_size, max_mention_per_sent, -1)
             predicts = self.classify(logits, mask)
             outputs = {'logits': logits, 'predicts': predicts}
         return outputs
 
     def _forward(self, tokens: Dict[str, Any], mention_boundary: torch.LongTensor) -> torch.Tensor:
         # B*M x K
@@ -157,27 +158,15 @@
 
     def classify(self, logits, mention_mask):  # noqa: D102
         if self.loss_function_type == 'BCE':
             logits = self.sigmoid(logits)  # B*M x L
             predicts = torch.where(logits > self.class_threshold, 1, 0)  # B*M x L
         else:
             raise ValueError('Unsupported loss %s', self.loss_function_type)
-
-        predicts = predicts.detach().cpu().numpy()
-        batch_mention_mask = mention_mask.detach().cpu().numpy()
-        batch_mentions = []
-        for prediction, mask in zip(predicts, batch_mention_mask):
-            mentions = []
-            for pred, flag in zip(prediction, mask):
-                if flag == 1:
-                    types = set(self.id_to_label[i] for i, p in enumerate(pred) if p == 1)
-                    mentions.append(types)
-            batch_mentions.append(mentions)
-
-        return batch_mentions
+        return predicts * mention_mask
 
 
 @MODELS.register_module(Tasks.entity_typing, module_name=Models.multilabel_concat_typing_model)
 class MultiLabelConcatTypingModel(Model):
     """Concat based Single Mention MultiLabel Entity Typing model
 
     This model is used for single mention multilabel entity typing tasks.
```

### Comparing `adaseq-0.6.3/adaseq/models/pretraining_model.py` & `adaseq-0.6.4/adaseq/models/pretraining_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/models/relation_extraction_model.py` & `adaseq-0.6.4/adaseq/models/relation_extraction_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/models/sequence_labeling_model.py` & `adaseq-0.6.4/adaseq/models/sequence_labeling_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         word_dropout: bool = False,
         use_crf: Optional[bool] = True,
         multiview: Optional[bool] = False,
         temperature: Optional[float] = 1.0,
         mv_loss_type: Optional[str] = 'kl',
         mv_interpolation: Optional[float] = 0.5,
         partial: Optional[bool] = False,
+        chunk: Optional[bool] = False,
         **kwargs
     ) -> None:
         super().__init__(**kwargs)
         self.id_to_label = id_to_label
         self.num_labels = len(id_to_label)
 
         if isinstance(embedder, Embedder):
@@ -91,29 +92,42 @@
         else:
             self.loss_fn = nn.CrossEntropyLoss(reduction='mean', ignore_index=PAD_LABEL_ID)
 
         self.multiview = multiview
         self.mv_loss_type = mv_loss_type
         self.temperature = temperature
         self.mv_interpolation = mv_interpolation
+        self.chunk = chunk
 
     def forward(
         self,
         tokens: Dict[str, Any],
         label_ids: Optional[torch.LongTensor] = None,
         meta: Optional[Dict[str, Any]] = None,
         origin_tokens: Optional[Dict[str, Any]] = None,
         origin_mask: Optional[torch.Tensor] = None,
     ) -> Dict[str, Any]:
         """
         TODO docstring
         """
-        logits = self._forward(tokens)
 
-        crf_mask = get_tokens_mask(tokens, logits.size(1)) if origin_mask is None else origin_mask
+        if self.chunk:
+            self._flatten(tokens)
+            logits = self._forward(tokens)
+            logits = logits.view(len(meta), -1, logits.size(-2), logits.size(-1)).max(dim=1)[0]
+            logits = logits[:, : label_ids.size(1), :]
+            crf_mask = (
+                get_tokens_mask(tokens, logits.size(1)) if origin_mask is None else origin_mask
+            )
+
+        else:
+            logits = self._forward(tokens)
+            crf_mask = (
+                get_tokens_mask(tokens, logits.size(1)) if origin_mask is None else origin_mask
+            )
 
         if self.training and label_ids is not None:
             loss = self._calculate_loss(logits, label_ids, crf_mask)
 
             if self.multiview and origin_tokens is not None:  # for multiview training
                 origin_view_logits = self._forward(origin_tokens)
                 origin_size = origin_view_logits.size(1 if origin_view_logits.dim() == 3 else 0)
@@ -207,7 +221,16 @@
         self, logits: torch.Tensor, mask: torch.Tensor
     ) -> Union[List, torch.LongTensor]:
         if self.use_crf:
             predicts = self.crf.decode(logits, mask=mask).squeeze(0)
         else:
             predicts = logits.argmax(-1)
         return predicts
+
+    def _flatten(
+        self,
+        tokens: Dict[str, Any],
+    ):
+        fields = set(tokens.keys())
+        for field in fields:
+            if len(tokens[field].size()) > 2:
+                tokens[field] = tokens[field].flatten(0, 1)
```

### Comparing `adaseq-0.6.3/adaseq/models/twostage_ner_model.py` & `adaseq-0.6.4/adaseq/models/twostage_ner_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/models/utils.py` & `adaseq-0.6.4/adaseq/models/utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/biaffine.py` & `adaseq-0.6.4/adaseq/modules/biaffine.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/decoders/base.py` & `adaseq-0.6.4/adaseq/modules/decoders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/decoders/crf.py` & `adaseq-0.6.4/adaseq/modules/decoders/crf.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/decoders/mlm_head.py` & `adaseq-0.6.4/adaseq/modules/decoders/mlm_head.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/decoders/pairwise_crf.py` & `adaseq-0.6.4/adaseq/modules/decoders/pairwise_crf.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/decoders/partial_crf.py` & `adaseq-0.6.4/adaseq/modules/decoders/partial_crf.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/dropouts.py` & `adaseq-0.6.4/adaseq/modules/dropouts.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/embedders/base.py` & `adaseq-0.6.4/adaseq/modules/embedders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/embedders/embedding.py` & `adaseq-0.6.4/adaseq/modules/embedders/embedding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/embedders/transformer_embedder.py` & `adaseq-0.6.4/adaseq/modules/embedders/transformer_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,18 @@
         `torch.Tensor`
             Shape: `[batch_size, num_wordpieces or num_orig_tokens, embedding_size]`.
         """
         # first encode sub-token level representations
         encoded = self.encode(input_ids, attention_mask, token_type_ids)  # type: ignore
         if offsets is not None:
             # then reconstruct token-level ones by offsets
-            encoded = self.reconstruct(encoded, offsets)
+            if 'pieces2word' in kwargs:
+                encoded = self.reconstruct(encoded, offsets, kwargs['pieces2word'])
+            else:
+                encoded = self.reconstruct(encoded, offsets)
 
         if has_special_tokens is not None:
             if self.drop_special_tokens and has_special_tokens.bool()[0]:
                 encoded = encoded[:, 1:-1]  # So far, we only consider [CLS] and [SEP]
         return encoded
 
     def encode(
@@ -229,15 +232,20 @@
             hidden_states = transformer_output.hidden_states[1:]
             embeddings = self._scalar_mix(hidden_states)
         else:
             embeddings = transformer_output.last_hidden_state
 
         return embeddings
 
-    def reconstruct(self, embeddings: torch.Tensor, offsets: torch.LongTensor) -> torch.Tensor:
+    def reconstruct(
+        self,
+        embeddings: torch.Tensor,
+        offsets: torch.LongTensor,
+        pieces2word: Optional[torch.LongTensor] = None,
+    ) -> torch.Tensor:
         """
         # Parameters
 
         input_ids: `torch.LongTensor`
             Shape: [batch_size, num_wordpieces].
         offsets: `torch.LongTensor`
             Shape: [batch_size, num_orig_tokens, 2].
@@ -284,14 +292,22 @@
             # Find the average of sub-tokens embeddings by dividing `span_embedding_sum` by `span_embedding_len`
             # Shape: (batch_size, num_orig_tokens, embedding_size)
             orig_embeddings = span_embeddings_sum / torch.clamp_min(span_embeddings_len, 1)
 
             # All the places where the span length is zero, write in zeros.
             orig_embeddings[(span_embeddings_len == 0).expand(orig_embeddings.shape)] = 0
 
+        # If "sub_token_mode" is set to "w2max", return the max embedding of all sub-tokens of a word in mode of w2ner.
+        elif self.sub_token_mode == 'w2max':
+            min_value = torch.min(embeddings).item()
+            length = pieces2word.size(1)
+            bert_embeds = embeddings.contiguous().unsqueeze(1).expand(-1, length, -1, -1)
+            bert_embeds = torch.masked_fill(bert_embeds, pieces2word.eq(0).unsqueeze(-1), min_value)
+            orig_embeddings, _ = torch.max(bert_embeds, dim=2)
+
         # If invalid "sub_token_mode" is provided, throw error
         else:
             raise ValueError(f"Do not recognise 'sub_token_mode' {self.sub_token_mode}")
 
         return orig_embeddings
```

### Comparing `adaseq-0.6.3/adaseq/modules/encoders/base.py` & `adaseq-0.6.4/adaseq/modules/encoders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/encoders/pytorch_rnn_encoder.py` & `adaseq-0.6.4/adaseq/modules/encoders/pytorch_rnn_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     def get_input_dim(self) -> int:
         return self._module.input_size
 
     def get_output_dim(self) -> int:
         return self._module.hidden_size * (1 + int(self._module.bidirectional))
 
     def forward(
-        self,
-        inputs: torch.Tensor,
-        mask: Optional[torch.BoolTensor] = None,
+        self, inputs: torch.Tensor, mask: Optional[torch.BoolTensor] = None, **kwargs
     ) -> torch.Tensor:
         """
         inputs: `torch.Tensor`
             Shape: [batch_size, max_length, input_dim].
         mask: `torch.BoolTensor`
             Shape: [batch_size, max_length].
```

### Comparing `adaseq-0.6.3/adaseq/modules/encoders/span_encoder.py` & `adaseq-0.6.4/adaseq/modules/encoders/span_encoder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/losses.py` & `adaseq-0.6.4/adaseq/modules/losses.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/scalar_mix.py` & `adaseq-0.6.4/adaseq/modules/scalar_mix.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/modules/util.py` & `adaseq-0.6.4/adaseq/modules/util.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/ms_patch.py` & `adaseq-0.6.4/adaseq/ms_patch.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/pipelines/base.py` & `adaseq-0.6.4/adaseq/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/pipelines/sequence_labeling_pipeline.py` & `adaseq-0.6.4/adaseq/pipelines/sequence_labeling_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/pipelines/span_based_ner_pipeline.py` & `adaseq-0.6.4/adaseq/pipelines/span_based_ner_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/training/default_config.py` & `adaseq-0.6.4/adaseq/training/default_config.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/training/default_trainer.py` & `adaseq-0.6.4/adaseq/training/default_trainer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/training/hooks/text_logger_hook.py` & `adaseq-0.6.4/adaseq/training/hooks/text_logger_hook.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/training/lr_scheduler.py` & `adaseq-0.6.4/adaseq/training/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/training/optimizer.py` & `adaseq-0.6.4/adaseq/training/optimizer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/training/typing_trainer.py` & `adaseq-0.6.4/adaseq/training/typing_trainer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/utils/checks.py` & `adaseq-0.6.4/adaseq/utils/checks.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/utils/common_utils.py` & `adaseq-0.6.4/adaseq/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/utils/hub_utils.py` & `adaseq-0.6.4/adaseq/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/utils/logging.py` & `adaseq-0.6.4/adaseq/utils/logging.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq/utils/yaml.py` & `adaseq-0.6.4/adaseq/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.3/adaseq.egg-info/PKG-INFO` & `adaseq-0.6.4/adaseq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaseq
-Version: 0.6.3
+Version: 0.6.4
 Summary: AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 Home-page: https://github.com/modelscope/adaseq
 Author: Alibaba Damo Academy NLP foundation team
 License: Apache License 2.0
 Platform: any
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `adaseq-0.6.3/adaseq.egg-info/SOURCES.txt` & `adaseq-0.6.4/adaseq.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 adaseq/data/data_collators/__init__.py
 adaseq/data/data_collators/base.py
 adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py
 adaseq/data/data_collators/pretraining_data_collator_with_padding.py
 adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py
 adaseq/data/data_collators/span_extraction_data_collator_with_padding.py
 adaseq/data/data_collators/twostage_data_collator_with_padding.py
+adaseq/data/data_collators/word_extraction_data_collator_with_padding.py
 adaseq/data/dataset_builders/__init__.py
 adaseq/data/dataset_builders/base.py
 adaseq/data/dataset_builders/entity_typing_dataset_builder.py
 adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py
 adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py
 adaseq/data/dataset_builders/relation_extraction_dataset_builder.py
 adaseq/data/dataset_dumpers/__init__.py
@@ -45,16 +46,18 @@
 adaseq/data/preprocessors/multilabel_typing_preprocessor.py
 adaseq/data/preprocessors/nlp_preprocessor.py
 adaseq/data/preprocessors/pretraining_preprocessor.py
 adaseq/data/preprocessors/relation_extraction_preprocessor.py
 adaseq/data/preprocessors/sequence_labeling_preprocessor.py
 adaseq/data/preprocessors/span_extraction_preprocessor.py
 adaseq/data/preprocessors/twostage_preprocessor.py
+adaseq/data/preprocessors/word_extraction_preprocessor.py
 adaseq/exporters/__init__.py
 adaseq/exporters/base.py
+adaseq/exporters/multilabel_typing_model_exporter.py
 adaseq/exporters/sequence_labeling_model_exporter.py
 adaseq/metrics/__init__.py
 adaseq/metrics/pretraining_metric.py
 adaseq/metrics/relation_extraction_metric.py
 adaseq/metrics/sequence_labeling_metric.py
 adaseq/metrics/span_extraction_metric.py
 adaseq/metrics/typing_metric.py
@@ -64,14 +67,15 @@
 adaseq/models/global_pointer_model.py
 adaseq/models/multilabel_typing_model.py
 adaseq/models/pretraining_model.py
 adaseq/models/relation_extraction_model.py
 adaseq/models/sequence_labeling_model.py
 adaseq/models/twostage_ner_model.py
 adaseq/models/utils.py
+adaseq/models/w2ner_model.py
 adaseq/modules/__init__.py
 adaseq/modules/biaffine.py
 adaseq/modules/dropouts.py
 adaseq/modules/losses.py
 adaseq/modules/scalar_mix.py
 adaseq/modules/util.py
 adaseq/modules/decoders/__init__.py
@@ -82,14 +86,15 @@
 adaseq/modules/decoders/partial_crf.py
 adaseq/modules/embedders/__init__.py
 adaseq/modules/embedders/base.py
 adaseq/modules/embedders/embedding.py
 adaseq/modules/embedders/transformer_embedder.py
 adaseq/modules/encoders/__init__.py
 adaseq/modules/encoders/base.py
+adaseq/modules/encoders/cnn_encoder.py
 adaseq/modules/encoders/pytorch_rnn_encoder.py
 adaseq/modules/encoders/span_encoder.py
 adaseq/pipelines/__init__.py
 adaseq/pipelines/base.py
 adaseq/pipelines/sequence_labeling_pipeline.py
 adaseq/pipelines/span_based_ner_pipeline.py
 adaseq/training/__init__.py
```

### Comparing `adaseq-0.6.3/setup.py` & `adaseq-0.6.4/setup.py`

 * *Files identical despite different names*

