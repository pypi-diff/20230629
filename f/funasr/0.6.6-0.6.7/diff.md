# Comparing `tmp/funasr-0.6.6.tar.gz` & `tmp/funasr-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.6.6.tar", last modified: Wed Jun 28 08:08:12 2023, max compression
+gzip compressed data, was "funasr-0.6.7.tar", last modified: Thu Jun 29 12:15:05 2023, max compression
```

## Comparing `funasr-0.6.6.tar` & `funasr-0.6.7.tar`

### file list

```diff
@@ -1,441 +1,441 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.286918 funasr-0.6.6/
--rw-r--r--   0 zhifu      (502) staff       (20)     9951 2023-06-28 08:08:12.286351 funasr-0.6.6/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     8951 2023-06-27 04:52:41.000000 funasr-0.6.6/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:10.250689 funasr-0.6.6/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:10.345993 funasr-0.6.6/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    69796 2023-06-26 06:18:54.000000 funasr-0.6.6/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    70907 2023-06-27 08:57:43.000000 funasr-0.6.6/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.6/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    11802 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17893 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14489 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8085 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     4991 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    10058 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.6.6/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3458 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9526 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6614 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12260 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.600920 funasr-0.6.6/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.6/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16902 2023-06-28 08:07:26.000000 funasr-0.6.6/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8714 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_model_from_file.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1907 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_streaming_iterator.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7941 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_sv_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.603512 funasr-0.6.6/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15818 2023-06-27 08:57:43.000000 funasr-0.6.6/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.605248 funasr-0.6.6/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.643055 funasr-0.6.6/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10803 2023-06-27 08:57:43.000000 funasr-0.6.6/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.688556 funasr-0.6.6/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.6/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.6.6/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.692982 funasr-0.6.6/funasr/datasets/small_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.6.6/funasr/datasets/small_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/datasets/small_datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9834 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/datasets/small_datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/datasets/small_datasets/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    33183 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/datasets/small_datasets/preprocessor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/datasets/small_datasets/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.693627 funasr-0.6.6/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11128 2023-06-28 06:45:37.000000 funasr-0.6.6/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.730580 funasr-0.6.6/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.6/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.731804 funasr-0.6.6/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.6/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.6/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.733550 funasr-0.6.6/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.6/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.6/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.764625 funasr-0.6.6/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.6/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.6/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.765410 funasr-0.6.6/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.6/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.768162 funasr-0.6.6/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.6/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.794872 funasr-0.6.6/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.6/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.797366 funasr-0.6.6/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6006 2023-06-27 03:21:23.000000 funasr-0.6.6/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.799193 funasr-0.6.6/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.834041 funasr-0.6.6/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.6.6/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.834402 funasr-0.6.6/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.6.6/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.873008 funasr-0.6.6/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.941084 funasr-0.6.6/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.6.6/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:11.999058 funasr-0.6.6/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.6.6/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.6.6/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15723 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11845 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18965 2023-06-19 09:03:43.000000 funasr-0.6.6/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51733 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-06-20 01:57:45.000000 funasr-0.6.6/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.007419 funasr-0.6.6/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    45056 2023-06-27 03:21:23.000000 funasr-0.6.6/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.6/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.6/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.6/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.009093 funasr-0.6.6/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.6/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.6/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.6.6/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.046747 funasr-0.6.6/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12621 2023-06-21 03:15:06.000000 funasr-0.6.6/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.047622 funasr-0.6.6/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.6/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.6/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.048439 funasr-0.6.6/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.6/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.049823 funasr-0.6.6/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.050359 funasr-0.6.6/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.051606 funasr-0.6.6/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.052275 funasr-0.6.6/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.074601 funasr-0.6.6/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.6/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.076483 funasr-0.6.6/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.6/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.113122 funasr-0.6.6/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.6/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.113827 funasr-0.6.6/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.6/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/modules/eend_ola/encoder_decoder_attractor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.189530 funasr-0.6.6/funasr/modules/eend_ola/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.6.6/funasr/modules/eend_ola/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.6.6/funasr/modules/eend_ola/utils/losses.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.6.6/funasr/modules/eend_ola/utils/power.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7317 2023-03-29 08:06:18.000000 funasr-0.6.6/funasr/modules/eend_ola/utils/report.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.6/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.191529 funasr-0.6.6/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.6/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.6/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.6/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.6/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.197030 funasr-0.6.6/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.198279 funasr-0.6.6/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.199443 funasr-0.6.6/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.6.6/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.200695 funasr-0.6.6/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.200965 funasr-0.6.6/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.6/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.201134 funasr-0.6.6/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.6/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.201860 funasr-0.6.6/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.6/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.202920 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.208150 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.228646 funasr-0.6.6/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.244720 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.247409 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1588 2023-06-19 11:16:01.000000 funasr-0.6.6/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.249576 funasr-0.6.6/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.250927 funasr-0.6.6/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.267213 funasr-0.6.6/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.6.6/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    58550 2023-06-19 09:03:43.000000 funasr-0.6.6/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21358 2023-06-19 09:03:43.000000 funasr-0.6.6/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.269879 funasr-0.6.6/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.272199 funasr-0.6.6/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.6/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.273856 funasr-0.6.6/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.6.6/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.6/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.283127 funasr-0.6.6/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.6.6/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.6/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.6/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.6/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.6/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.6/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.6/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.6.6/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-28 06:44:46.000000 funasr-0.6.6/funasr/utils/runtime_sdk_download_tool.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.6/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.6/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.6.6/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.6/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-28 08:07:53.000000 funasr-0.6.6/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:10.252357 funasr-0.6.6/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     9951 2023-06-28 08:08:09.000000 funasr-0.6.6/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    14008 2023-06-28 08:08:10.000000 funasr-0.6.6/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-28 08:08:09.000000 funasr-0.6.6/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-28 08:08:09.000000 funasr-0.6.6/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-28 08:08:10.000000 funasr-0.6.6/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-28 08:08:12.287008 funasr-0.6.6/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-06-26 13:46:26.000000 funasr-0.6.6/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-28 08:08:12.285676 funasr-0.6.6/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26773 2023-06-15 09:10:12.000000 funasr-0.6.6/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.6/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.6/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.6/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.6.6/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-06-28 08:07:26.000000 funasr-0.6.6/tests/test_tp_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.6.6/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.666676 funasr-0.6.7/
+-rw-r--r--   0 zhifu      (502) staff       (20)     9928 2023-06-29 12:15:05.666372 funasr-0.6.7/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     8951 2023-06-27 04:52:41.000000 funasr-0.6.7/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.487311 funasr-0.6.7/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.498405 funasr-0.6.7/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    67983 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    70592 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.7/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.7/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9687 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17782 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12149 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.503637 funasr-0.6.7/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.7/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16902 2023-06-28 08:07:26.000000 funasr-0.6.7/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_model_from_file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_streaming_iterator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_sv_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.505104 funasr-0.6.7/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.505808 funasr-0.6.7/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3713 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.507103 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10803 2023-06-27 08:57:43.000000 funasr-0.6.7/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.509391 funasr-0.6.7/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    30602 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.529864 funasr-0.6.7/funasr/datasets/small_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.6.7/funasr/datasets/small_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/preprocessor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/datasets/small_datasets/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.530511 funasr-0.6.7/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-06-29 12:09:00.000000 funasr-0.6.7/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.531951 funasr-0.6.7/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.532789 funasr-0.6.7/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.7/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.7/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.534201 funasr-0.6.7/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.7/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.536199 funasr-0.6.7/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.7/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.536764 funasr-0.6.7/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.7/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.538705 funasr-0.6.7/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.7/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.539154 funasr-0.6.7/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.540695 funasr-0.6.7/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.541946 funasr-0.6.7/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.545554 funasr-0.6.7/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.546162 funasr-0.6.7/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.6.7/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.547738 funasr-0.6.7/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.555668 funasr-0.6.7/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.559513 funasr-0.6.7/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40753 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75359 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15642 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100258 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35177 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.586384 funasr-0.6.7/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.7/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.7/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.588618 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3552 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56207 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.592475 funasr-0.6.7/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.594162 funasr-0.6.7/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.7/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.7/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.594892 funasr-0.6.7/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.7/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.596061 funasr-0.6.7/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.597231 funasr-0.6.7/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.598892 funasr-0.6.7/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.599703 funasr-0.6.7/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.610655 funasr-0.6.7/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.7/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.613101 funasr-0.6.7/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.7/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.615469 funasr-0.6.7/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.7/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.616278 funasr-0.6.7/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/modules/eend_ola/encoder_decoder_attractor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.617730 funasr-0.6.7/funasr/modules/eend_ola/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/losses.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/power.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/report.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.7/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.620128 funasr-0.6.7/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.7/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.7/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.7/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.622062 funasr-0.6.7/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.623607 funasr-0.6.7/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.624840 funasr-0.6.7/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.6.7/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.625684 funasr-0.6.7/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.626000 funasr-0.6.7/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.626193 funasr-0.6.7/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.626954 funasr-0.6.7/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.7/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.627674 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.630318 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.634317 funasr-0.6.7/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.635686 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.638018 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1588 2023-06-19 11:16:01.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.640696 funasr-0.6.7/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.642276 funasr-0.6.7/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.646782 funasr-0.6.7/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72548 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    57686 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.650432 funasr-0.6.7/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.652998 funasr-0.6.7/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.654812 funasr-0.6.7/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.7/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38470 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.663687 funasr-0.6.7/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.6.7/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-06-29 11:59:56.000000 funasr-0.6.7/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.7/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.7/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.6.7/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-29 10:01:51.000000 funasr-0.6.7/funasr/utils/runtime_sdk_download_tool.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.7/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.6.7/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-29 12:03:04.000000 funasr-0.6.7/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.488333 funasr-0.6.7/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     9928 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    14008 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      774 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-29 12:15:05.666742 funasr-0.6.7/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-06-29 09:20:46.000000 funasr-0.6.7/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.665938 funasr-0.6.7/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26773 2023-06-15 09:10:12.000000 funasr-0.6.7/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.7/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.7/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.7/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.6.7/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-06-28 08:07:26.000000 funasr-0.6.7/tests/test_tp_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.6.7/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.6.6/PKG-INFO` & `funasr-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.6
+Version: 0.6.7
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: train
-Provides-Extra: recipe
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
 
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.6 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.7 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
-Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
-Extra: test Provides-Extra: doc [//]: # (
+Provides-Extra: train Provides-Extra: all Provides-Extra: test Provides-Extra:
+doc [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
```

### Comparing `funasr-0.6.6/README.md` & `funasr-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.6.7/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/asr_infer.py` & `funasr-0.6.7/funasr/bin/asr_infer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import requests
 import torch
 from packaging.version import parse as V
-from typeguard import check_argument_types
-from typeguard import check_return_type
-from  funasr.build_utils.build_model_from_file import build_model_from_file
+from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
 from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 from funasr.modules.beam_search.beam_search import BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
 from funasr.modules.beam_search.beam_search_sa_asr import Hypothesis as HypothesisSAASR
 from funasr.modules.beam_search.beam_search_transducer import BeamSearchTransducer
@@ -74,15 +72,14 @@
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
             streaming: bool = False,
             frontend_conf: dict = None,
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
@@ -188,15 +185,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
@@ -244,15 +240,14 @@
 
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
 
-        assert check_return_type(results)
         return results
 
 
 class Speech2TextParaformer:
     """Speech2Text class
 
     Examples:
@@ -284,15 +279,14 @@
             penalty: float = 0.0,
             nbest: int = 1,
             frontend_conf: dict = None,
             hotword_list_or_file: str = None,
             decoding_ind: int = 0,
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device, mode="paraformer"
         )
         frontend = None
@@ -409,15 +403,14 @@
 
         Args:
                 speech: Input speech data
         Returns:
                 text, token, token_int, hyp
 
         """
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
@@ -512,15 +505,14 @@
                 if isinstance(self.asr_model, BiCifParaformer):
                     _, timestamp = ts_prediction_lfr6_standard(us_alphas[i][:enc_len[i] * 3],
                                                                us_peaks[i][:enc_len[i] * 3],
                                                                copy.copy(token),
                                                                vad_offset=begin_time)
                 results.append((text, token, token_int, hyp, timestamp, enc_len_batch_total, lfr_factor))
 
-        # assert check_return_type(results)
         return results
 
     def generate_hotwords_list(self, hotword_list_or_file):
         def load_seg_dict(seg_dict_file):
             seg_dict = {}
             assert isinstance(seg_dict_file, str)
             with open(seg_dict_file, "r", encoding="utf8") as f:
@@ -652,15 +644,14 @@
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
             frontend_conf: dict = None,
             hotword_list_or_file: str = None,
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device, mode="paraformer"
         )
         frontend = None
@@ -772,15 +763,14 @@
 
         Args:
                 speech: Input speech data
         Returns:
                 text, token, token_int, hyp
 
         """
-        assert check_argument_types()
         results = []
         cache_en = cache["encoder"]
         if speech.shape[1] < 16 * 60 and cache_en["is_final"]:
             if cache_en["start_idx"] == 0:
                 return []
             cache_en["tail_chunk"] = True
             feats = cache_en["feats"]
@@ -867,15 +857,14 @@
                     elif re.match('^[a-zA-Z]+$', item):
                         postprocessed_result += item + " "
                     else:
                         postprocessed_result += item
 
                 results.append(postprocessed_result)
 
-        # assert check_return_type(results)
         return results
 
 
 class Speech2TextUniASR:
     """Speech2Text class
 
     Examples:
@@ -908,15 +897,14 @@
             nbest: int = 1,
             token_num_relax: int = 1,
             decoding_ind: int = 0,
             decoding_mode: str = "model1",
             frontend_conf: dict = None,
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device, mode="uniasr"
         )
         frontend = None
@@ -1032,15 +1020,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
@@ -1100,15 +1087,14 @@
 
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
 
-        assert check_return_type(results)
         return results
 
 
 class Speech2TextMFCCA:
     """Speech2Text class
 
     Examples:
@@ -1139,15 +1125,14 @@
             lm_weight: float = 1.0,
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
             streaming: bool = False,
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
 
@@ -1244,15 +1229,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
-        assert check_argument_types()
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
         if (speech.dim() == 3):
             speech = torch.squeeze(speech, 2)
         # speech = speech.unsqueeze(0).to(getattr(torch, self.dtype))
         speech = speech.to(getattr(torch, self.dtype))
@@ -1294,15 +1278,14 @@
 
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
 
-        assert check_return_type(results)
         return results
 
 
 class Speech2TextTransducer:
     """Speech2Text class for Transducer models.
     Args:
         asr_train_config: ASR model training config path.
@@ -1351,15 +1334,14 @@
             left_context: int = 32,
             right_context: int = 0,
             display_partial_hypotheses: bool = False,
     ) -> None:
         """Construct a Speech2Text object."""
         super().__init__()
 
-        assert check_argument_types()
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
 
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
@@ -1530,15 +1512,14 @@
     def simu_streaming_decode(self, speech: Union[torch.Tensor, np.ndarray]) -> List[HypothesisTransducer]:
         """Speech2Text call.
         Args:
             speech: Speech data. (S)
         Returns:
             nbest_hypothesis: N-best hypothesis.
         """
-        assert check_argument_types()
 
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             speech = torch.unsqueeze(speech, axis=0)
             speech_lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
@@ -1562,15 +1543,14 @@
     def __call__(self, speech: Union[torch.Tensor, np.ndarray]) -> List[HypothesisTransducer]:
         """Speech2Text call.
         Args:
             speech: Speech data. (S)
         Returns:
             nbest_hypothesis: N-best hypothesis.
         """
-        assert check_argument_types()
 
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             speech = torch.unsqueeze(speech, axis=0)
             speech_lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
@@ -1604,44 +1584,17 @@
 
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
 
-            assert check_return_type(results)
 
         return results
 
-    @staticmethod
-    def from_pretrained(
-            model_tag: Optional[str] = None,
-            **kwargs: Optional[Any],
-    ) -> Speech2Text:
-        """Build Speech2Text instance from the pretrained model.
-        Args:
-            model_tag: Model tag of the pretrained models.
-        Return:
-            : Speech2Text instance.
-        """
-        if model_tag is not None:
-            try:
-                from espnet_model_zoo.downloader import ModelDownloader
-
-            except ImportError:
-                logging.error(
-                    "`espnet_model_zoo` is not installed. "
-                    "Please install via `pip install -U espnet_model_zoo`."
-                )
-                raise
-            d = ModelDownloader()
-            kwargs.update(**d.download_and_unpack(model_tag))
-
-        return Speech2TextTransducer(**kwargs)
-
 
 class Speech2TextSAASR:
     """Speech2Text class
 
     Examples:
         >>> import soundfile
         >>> speech2text = Speech2TextSAASR("asr_config.yml", "asr.pb")
@@ -1671,15 +1624,14 @@
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
             streaming: bool = False,
             frontend_conf: dict = None,
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
@@ -1789,15 +1741,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             text, text_id, token, token_int, hyp
 
         """
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if isinstance(profile, np.ndarray):
             profile = torch.tensor(profile)
@@ -1882,9 +1833,8 @@
 
             text_id = '$'.join(spk_list)
 
             assert len(text) == len(text_id)
 
             results.append((text, text_id, token, token_int, hyp))
 
-        assert check_return_type(results)
         return results
```

### Comparing `funasr-0.6.6/funasr/bin/asr_inference_launch.py` & `funasr-0.6.7/funasr/bin/asr_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing import Union
 
 import numpy as np
 import torch
 import torchaudio
 import soundfile
 import yaml
-from typeguard import check_argument_types
 
 from funasr.bin.asr_infer import Speech2Text
 from funasr.bin.asr_infer import Speech2TextMFCCA
 from funasr.bin.asr_infer import Speech2TextParaformer, Speech2TextParaformerOnline
 from funasr.bin.asr_infer import Speech2TextSAASR
 from funasr.bin.asr_infer import Speech2TextTransducer
 from funasr.bin.asr_infer import Speech2TextUniASR
@@ -76,15 +75,14 @@
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
         mc: bool = False,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
@@ -236,15 +234,14 @@
         num_workers: int = 1,
         output_dir: Optional[str] = None,
         timestamp_infer_config: Union[Path, str] = None,
         timestamp_model_file: Union[Path, str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
@@ -477,15 +474,14 @@
         time_stamp_writer: bool = True,
         punc_infer_config: Optional[str] = None,
         punc_model_file: Optional[str] = None,
         outputs_dict: Optional[bool] = True,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
@@ -745,15 +741,14 @@
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
         output_dir: Optional[str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
 
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
@@ -953,15 +948,14 @@
         num_workers: int = 1,
         token_num_relax: int = 1,
         decoding_ind: int = 0,
         decoding_mode: str = "model1",
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
@@ -1122,15 +1116,14 @@
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
@@ -1310,15 +1303,14 @@
         quantize_dtype: Dynamic quantization data type.
         streaming: Whether to perform chunk-by-chunk inference.
         chunk_size: Number of frames in chunk AFTER subsampling.
         left_context: Number of frames in left context AFTER subsampling.
         right_context: Number of frames in right context AFTER subsampling.
         display_partial_hypotheses: Whether to display partial hypotheses.
     """
-    assert check_argument_types()
 
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
@@ -1460,15 +1452,14 @@
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
         mc: bool = False,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
```

### Comparing `funasr-0.6.6/funasr/bin/asr_train.py` & `funasr-0.6.7/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/build_trainer.py` & `funasr-0.6.7/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/data2vec_train.py` & `funasr-0.6.7/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/diar_infer.py` & `funasr-0.6.7/funasr/bin/diar_infer.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import torch
 from scipy.ndimage import median_filter
 from torch.nn import functional as F
-from typeguard import check_argument_types
 
 from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.tasks.diar import DiarTask
 from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.torch_utils.device_funcs import to_device
 from funasr.utils.misc import statistic_model_parameters
 
@@ -41,15 +40,14 @@
     def __init__(
             self,
             diar_train_config: Union[Path, str] = None,
             diar_model_file: Union[Path, str] = None,
             device: str = "cpu",
             dtype: str = "float32",
     ):
-        assert check_argument_types()
 
         # 1. Build Diarization model
         diar_model, diar_train_args = build_model_from_file(
             config_file=diar_train_config,
             model_file=diar_model_file,
             device=device,
             task_name="diar",
@@ -84,15 +82,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             diarization results
 
         """
-        assert check_argument_types()
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
@@ -103,44 +100,14 @@
             feats_len = speech_lengths
         batch = {"speech": feats, "speech_lengths": feats_len}
         batch = to_device(batch, device=self.device)
         results = self.diar_model.estimate_sequential(**batch)
 
         return results
 
-    @staticmethod
-    def from_pretrained(
-            model_tag: Optional[str] = None,
-            **kwargs: Optional[Any],
-    ):
-        """Build Speech2Diarization instance from the pretrained model.
-
-        Args:
-            model_tag (Optional[str]): Model tag of the pretrained models.
-                Currently, the tags of espnet_model_zoo are supported.
-
-        Returns:
-            Speech2Diarization: Speech2Diarization instance.
-
-        """
-        if model_tag is not None:
-            try:
-                from espnet_model_zoo.downloader import ModelDownloader
-
-            except ImportError:
-                logging.error(
-                    "`espnet_model_zoo` is not installed. "
-                    "Please install via `pip install -U espnet_model_zoo`."
-                )
-                raise
-            d = ModelDownloader()
-            kwargs.update(**d.download_and_unpack(model_tag))
-
-        return Speech2DiarizationEEND(**kwargs)
-
 
 class Speech2DiarizationSOND:
     """Speech2Xvector class
 
     Examples:
         >>> import soundfile
         >>> import numpy as np
@@ -159,15 +126,14 @@
             device: Union[str, torch.device] = "cpu",
             batch_size: int = 1,
             dtype: str = "float32",
             streaming: bool = False,
             smooth_size: int = 83,
             dur_threshold: float = 10,
     ):
-        assert check_argument_types()
 
         # TODO: 1. Build Diarization model
         diar_model, diar_train_args = build_model_from_file(
             config_file=diar_train_config,
             model_file=diar_model_file,
             device=device,
             task_name="diar",
@@ -279,15 +245,14 @@
         Args:
             speech: Input speech data
             profile: Speaker profiles
         Returns:
             diarization results for each speaker
 
         """
-        assert check_argument_types()
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
         if isinstance(profile, np.ndarray):
             profile = torch.tensor(profile)
 
         # data: (Nsamples,) -> (1, Nsamples)
@@ -301,37 +266,7 @@
         # a. To device
         batch = to_device(batch, device=self.device)
 
         logits = self.diar_model.prediction_forward(**batch)
         results, pse_labels = self.post_processing(logits, profile.shape[1], output_format)
 
         return results, pse_labels
-
-    @staticmethod
-    def from_pretrained(
-            model_tag: Optional[str] = None,
-            **kwargs: Optional[Any],
-    ):
-        """Build Speech2Xvector instance from the pretrained model.
-
-        Args:
-            model_tag (Optional[str]): Model tag of the pretrained models.
-                Currently, the tags of espnet_model_zoo are supported.
-
-        Returns:
-            Speech2Xvector: Speech2Xvector instance.
-
-        """
-        if model_tag is not None:
-            try:
-                from espnet_model_zoo.downloader import ModelDownloader
-
-            except ImportError:
-                logging.error(
-                    "`espnet_model_zoo` is not installed. "
-                    "Please install via `pip install -U espnet_model_zoo`."
-                )
-                raise
-            d = ModelDownloader()
-            kwargs.update(**d.download_and_unpack(model_tag))
-
-        return Speech2DiarizationSOND(**kwargs)
```

### Comparing `funasr-0.6.6/funasr/bin/diar_inference_launch.py` & `funasr-0.6.7/funasr/bin/diar_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import soundfile
 import torch
 from scipy.signal import medfilt
-from typeguard import check_argument_types
 
 from funasr.bin.diar_infer import Speech2DiarizationSOND, Speech2DiarizationEEND
 from funasr.datasets.iterable_dataset import load_bytes
 from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
@@ -48,15 +47,14 @@
         smooth_size: int = 83,
         dur_threshold: int = 10,
         out_format: str = "vad",
         param_dict: Optional[dict] = None,
         mode: str = "sond",
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
@@ -229,15 +227,14 @@
         key_file: Optional[str] = None,
         model_tag: Optional[str] = None,
         allow_variable_data_keys: bool = True,
         streaming: bool = False,
         param_dict: Optional[dict] = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
```

### Comparing `funasr-0.6.6/funasr/bin/diar_train.py` & `funasr-0.6.7/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/lm_inference_launch.py` & `funasr-0.6.7/funasr/bin/lm_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import torch
 from torch.nn.parallel import data_parallel
-from typeguard import check_argument_types
 
 from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.datasets.preprocessor import LMPreprocessor
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
@@ -46,15 +45,14 @@
         allow_variable_data_keys: bool = False,
         split_with_space: Optional[bool] = False,
         seg_dict_file: Optional[str] = None,
         output_dir: Optional[str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
```

### Comparing `funasr-0.6.6/funasr/bin/lm_train.py` & `funasr-0.6.7/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/punc_infer.py` & `funasr-0.6.7/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/punc_inference_launch.py` & `funasr-0.6.7/funasr/bin/punc_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.bin.punc_infer import Text2Punc, Text2PuncVADRealtime
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
@@ -34,15 +33,14 @@
         key_file: Optional[str],
         train_config: Optional[str],
         model_file: Optional[str],
         output_dir: Optional[str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
@@ -114,15 +112,14 @@
         key_file: Optional[str],
         train_config: Optional[str],
         model_file: Optional[str],
         output_dir: Optional[str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
```

### Comparing `funasr-0.6.6/funasr/bin/punc_train.py` & `funasr-0.6.7/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/sa_asr_train.py` & `funasr-0.6.7/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/sv_inference_launch.py` & `funasr-0.6.7/funasr/bin/sv_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 from kaldiio import WriteHelper
-from typeguard import check_argument_types
 
 from funasr.bin.sv_infer import Speech2Xvector
 from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
@@ -42,15 +41,14 @@
         allow_variable_data_keys: bool = True,
         streaming: bool = False,
         embedding_node: str = "resnet1_dense",
         sv_threshold: float = 0.9465,
         param_dict: Optional[dict] = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
@@ -75,18 +73,15 @@
         sv_model_file=sv_model_file,
         device=device,
         dtype=dtype,
         streaming=streaming,
         embedding_node=embedding_node
     )
     logging.info("speech2xvector_kwargs: {}".format(speech2xvector_kwargs))
-    speech2xvector = Speech2Xvector.from_pretrained(
-        model_tag=model_tag,
-        **speech2xvector_kwargs,
-    )
+    speech2xvector = Speech2Xvector(**speech2xvector_kwargs)
     speech2xvector.sv_model.eval()
 
     def _forward(
             data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
             raw_inputs: Union[np.ndarray, torch.Tensor] = None,
             output_dir_v2: Optional[str] = None,
             param_dict: Optional[dict] = None,
```

### Comparing `funasr-0.6.6/funasr/bin/tokenize_text.py` & `funasr-0.6.7/funasr/bin/tokenize_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from collections import Counter
 import logging
 from pathlib import Path
 import sys
 from typing import List
 from typing import Optional
 
-from typeguard import check_argument_types
 
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.cleaner import TextCleaner
 from funasr.text.phoneme_tokenizer import g2p_choices
 from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
@@ -77,15 +76,14 @@
     vocabulary_size: int,
     remove_non_linguistic_symbols: bool,
     cutoff: int,
     add_symbol: List[str],
     cleaner: Optional[str],
     g2p: Optional[str],
 ):
-    assert check_argument_types()
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
     if input == "-":
         fin = sys.stdin
```

### Comparing `funasr-0.6.6/funasr/bin/tp_infer.py` & `funasr-0.6.7/funasr/bin/tp_infer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import logging
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.text.token_id_converter import TokenIDConverter
 from funasr.torch_utils.device_funcs import to_device
 
 
 class Speech2Timestamp:
@@ -22,15 +21,14 @@
             timestamp_infer_config: Union[Path, str] = None,
             timestamp_model_file: Union[Path, str] = None,
             timestamp_cmvn_file: Union[Path, str] = None,
             device: str = "cpu",
             dtype: str = "float32",
             **kwargs,
     ):
-        assert check_argument_types()
         # 1. Build ASR model
         tp_model, tp_train_args = build_model_from_file(
             timestamp_infer_config, timestamp_model_file, cmvn_file=None, device=device, task_name="asr", mode="tp"
         )
         if 'cuda' in device:
             tp_model = tp_model.cuda()  # force model to cuda
 
@@ -60,15 +58,14 @@
     @torch.no_grad()
     def __call__(
             self,
             speech: Union[torch.Tensor, np.ndarray],
             speech_lengths: Union[torch.Tensor, np.ndarray] = None,
             text_lengths: Union[torch.Tensor, np.ndarray] = None
     ):
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
```

### Comparing `funasr-0.6.6/funasr/bin/tp_inference_launch.py` & `funasr-0.6.7/funasr/bin/tp_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import os
 import sys
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 
 from funasr.bin.tp_infer import Speech2Timestamp
 from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.datasets.preprocessor import LMPreprocessor
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
@@ -43,15 +42,14 @@
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
         split_with_space: bool = True,
         seg_dict_file: Optional[str] = None,
         **kwargs,
 ):
-    assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
```

### Comparing `funasr-0.6.6/funasr/bin/train.py` & `funasr-0.6.7/funasr/bin/train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/bin/vad_infer.py` & `funasr-0.6.7/funasr/bin/vad_infer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 
 from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 from funasr.torch_utils.device_funcs import to_device
 
 
 class Speech2VadSegment:
@@ -38,15 +37,14 @@
             vad_model_file: Union[Path, str] = None,
             vad_cmvn_file: Union[Path, str] = None,
             device: str = "cpu",
             batch_size: int = 1,
             dtype: str = "float32",
             **kwargs,
     ):
-        assert check_argument_types()
 
         # 1. Build vad model
         vad_model, vad_infer_args = build_model_from_file(
             vad_infer_config, vad_model_file, None, device, task_name="vad"
         )
         frontend = None
         if vad_infer_args.frontend is not None:
@@ -72,15 +70,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             self.frontend.filter_length_max = math.inf
@@ -145,15 +142,14 @@
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
-        assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
         batch_size = speech.shape[0]
         segments = [[]] * batch_size
         if self.frontend is not None:
```

### Comparing `funasr-0.6.6/funasr/bin/vad_inference_launch.py` & `funasr-0.6.7/funasr/bin/vad_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 import json
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
@@ -43,15 +42,14 @@
         allow_variable_data_keys: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
         **kwargs,
 ):
-    assert check_argument_types()
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
@@ -144,15 +142,14 @@
         allow_variable_data_keys: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
         **kwargs,
 ):
-    assert check_argument_types()
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
```

### Comparing `funasr-0.6.6/funasr/build_utils/build_args.py` & `funasr-0.6.7/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_asr_model.py` & `funasr-0.6.7/funasr/build_utils/build_asr_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_dataloader.py` & `funasr-0.6.7/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_diar_model.py` & `funasr-0.6.7/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_distributed.py` & `funasr-0.6.7/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_lm_model.py` & `funasr-0.6.7/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_model.py` & `funasr-0.6.7/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_model_from_file.py` & `funasr-0.6.7/funasr/build_utils/build_model_from_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union
 
 import torch
 import yaml
-from typeguard import check_argument_types
 
 from funasr.build_utils.build_model import build_model
 from funasr.models.base_model import FunASRModel
 
 
 def build_model_from_file(
         config_file: Union[Path, str] = None,
@@ -26,15 +25,14 @@
 
     Args:
         config_file: The yaml file saved when training.
         model_file: The model file saved when training.
         device: Device type, "cpu", "cuda", or "cuda:N".
 
     """
-    assert check_argument_types()
     if config_file is None:
         assert model_file is not None, (
             "The argument 'model_file' must be provided "
             "if the argument 'config_file' is not specified."
         )
         config_file = Path(model_file).parent / "config.yaml"
     else:
```

### Comparing `funasr-0.6.6/funasr/build_utils/build_optimizer.py` & `funasr-0.6.7/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_pretrain_model.py` & `funasr-0.6.7/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_punc_model.py` & `funasr-0.6.7/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_scheduler.py` & `funasr-0.6.7/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/build_utils/build_streaming_iterator.py` & `funasr-0.6.7/funasr/build_utils/build_streaming_iterator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from torch.utils.data import DataLoader
-from typeguard import check_argument_types
 
 from funasr.datasets.iterable_dataset import IterableESPnetDataset
 from funasr.datasets.small_datasets.collate_fn import CommonCollateFn
 from funasr.datasets.small_datasets.preprocessor import build_preprocess
 
 
 def build_streaming_iterator(
@@ -19,15 +18,14 @@
         num_workers: int = 1,
         use_collate_fn: bool = True,
         preprocess_fn=None,
         ngpu: int = 0,
         train: bool = False,
 ) -> DataLoader:
     """Build DataLoader using iterable dataset"""
-    assert check_argument_types()
 
     # preprocess
     if preprocess_fn is not None:
         preprocess_fn = preprocess_fn
     elif preprocess_args is not None:
         preprocess_args.task_name = task_name
         preprocess_fn = build_preprocess(preprocess_args, train)
```

### Comparing `funasr-0.6.6/funasr/build_utils/build_sv_model.py` & `funasr-0.6.7/funasr/build_utils/build_sv_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
 import torch
-from typeguard import check_return_type
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.base_model import FunASRModel
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.decoder.sv_decoder import DenseDecoder
@@ -250,9 +249,8 @@
     )
 
     # FIXME(kamo): Should be done in model?
     # 8. Initialize
     if args.init is not None:
         initialize(model, args.init)
 
-    assert check_return_type(model)
     return model
```

### Comparing `funasr-0.6.6/funasr/build_utils/build_trainer.py` & `funasr-0.6.7/funasr/build_utils/build_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing import Union
 
 import humanfriendly
 import oss2
 import torch
 import torch.nn
 import torch.optim
-from typeguard import check_argument_types
 
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 from funasr.main_funcs.average_nbest_models import average_nbest_models
 from funasr.models.base_model import FunASRModel
 from funasr.schedulers.abs_scheduler import AbsBatchStepScheduler
 from funasr.schedulers.abs_scheduler import AbsEpochStepScheduler
 from funasr.schedulers.abs_scheduler import AbsScheduler
@@ -114,15 +113,14 @@
         self.schedulers = schedulers
         self.train_dataloader = train_dataloader
         self.valid_dataloader = valid_dataloader
         self.distributed_option = distributed_option
 
     def build_options(self, args: argparse.Namespace) -> TrainerOptions:
         """Build options consumed by train(), eval()"""
-        assert check_argument_types()
         return build_dataclass(TrainerOptions, args)
 
     @classmethod
     def add_arguments(cls, parser: argparse.ArgumentParser):
         """Reserved for future development of another Trainer"""
         pass
 
@@ -152,15 +150,14 @@
             else:
                 scaler.load_state_dict(states["scaler"])
 
         logging.info(f"The training was resumed using {checkpoint}")
 
     def run(self) -> None:
         """Perform training. This method performs the main process of training."""
-        assert check_argument_types()
         # NOTE(kamo): Don't check the type more strictly as far trainer_options
         model = self.model
         optimizers = self.optimizers
         schedulers = self.schedulers
         train_dataloader = self.train_dataloader
         valid_dataloader = self.valid_dataloader
         trainer_options = self.trainer_options
@@ -518,15 +515,14 @@
             schedulers: Sequence[Optional[AbsScheduler]],
             scaler: Optional[GradScaler],
             reporter: SubReporter,
             summary_writer,
             options: TrainerOptions,
             distributed_option: DistributedOption,
     ) -> Tuple[bool, bool]:
-        assert check_argument_types()
 
         grad_noise = options.grad_noise
         accum_grad = options.accum_grad
         grad_clip = options.grad_clip
         grad_clip_type = options.grad_clip_type
         log_interval = options.log_interval
         # no_forward_run = options.no_forward_run
@@ -754,15 +750,14 @@
             self,
             model: torch.nn.Module,
             iterator: Iterable[Dict[str, torch.Tensor]],
             reporter: SubReporter,
             options: TrainerOptions,
             distributed_option: DistributedOption,
     ) -> None:
-        assert check_argument_types()
         ngpu = options.ngpu
         # no_forward_run = options.no_forward_run
         distributed = distributed_option.distributed
 
         model.eval()
 
         # [For distributed] Because iteration counts are not always equals between
```

### Comparing `funasr-0.6.6/funasr/build_utils/build_vad_model.py` & `funasr-0.6.7/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/collate_fn.py` & `funasr-0.6.7/funasr/datasets/collate_fn.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.modules.nets_utils import pad_list
 
 
 class CommonCollateFn:
     """Functor class of common_collate_fn()"""
 
     def __init__(
             self,
             float_pad_value: Union[float, int] = 0.0,
             int_pad_value: int = -32768,
             not_sequence: Collection[str] = (),
             max_sample_size=None
     ):
-        assert check_argument_types()
         self.float_pad_value = float_pad_value
         self.int_pad_value = int_pad_value
         self.not_sequence = set(not_sequence)
         self.max_sample_size = max_sample_size
 
     def __repr__(self):
         return (
@@ -49,15 +46,14 @@
         data: Collection[Tuple[str, Dict[str, np.ndarray]]],
         float_pad_value: Union[float, int] = 0.0,
         int_pad_value: int = -32768,
         not_sequence: Collection[str] = (),
 ) -> Tuple[List[str], Dict[str, torch.Tensor]]:
     """Concatenate ndarray-list to an array and convert to torch.Tensor.
     """
-    assert check_argument_types()
     uttids = [u for u, _ in data]
     data = [d for _, d in data]
 
     assert all(set(data[0]) == set(d) for d in data), "dict-keys mismatching"
     assert all(
         not k.endswith("_lengths") for k in data[0]
     ), f"*_lengths is reserved: {list(data[0])}"
@@ -75,15 +71,14 @@
         output[key] = tensor
 
         if key not in not_sequence:
             lens = torch.tensor([d[key].shape[0] for d in data], dtype=torch.long)
             output[key + "_lengths"] = lens
 
     output = (uttids, output)
-    assert check_return_type(output)
     return output
 
 def crop_to_max_size(feature, target_size):
     size = len(feature)
     diff = size - target_size
     if diff <= 0:
         return feature
@@ -95,15 +90,14 @@
 
 def clipping_collate_fn(
         data: Collection[Tuple[str, Dict[str, np.ndarray]]],
         max_sample_size=None,
         not_sequence: Collection[str] = (),
 ) -> Tuple[List[str], Dict[str, torch.Tensor]]:
     # mainly for pre-training
-    assert check_argument_types()
     uttids = [u for u, _ in data]
     data = [d for _, d in data]
 
     assert all(set(data[0]) == set(d) for d in data), "dict-keys mismatching"
     assert all(
         not k.endswith("_lengths") for k in data[0]
     ), f"*_lengths is reserved: {list(data[0])}"
@@ -127,9 +121,8 @@
         output[key] = tensor
 
         if key not in not_sequence:
             lens = torch.tensor([source.shape[0] for source in tensor], dtype=torch.long)
             output[key + "_lengths"] = lens
 
     output = (uttids, output)
-    assert check_return_type(output)
     return output
```

### Comparing `funasr-0.6.6/funasr/datasets/dataset.py` & `funasr-0.6.7/funasr/datasets/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,26 @@
 
 import h5py
 import humanfriendly
 import kaldiio
 import numpy as np
 import torch
 from torch.utils.data.dataset import Dataset
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.fileio.npy_scp import NpyScpReader
 from funasr.fileio.rand_gen_dataset import FloatRandomGenerateDataset
 from funasr.fileio.rand_gen_dataset import IntRandomGenerateDataset
 from funasr.fileio.read_text import load_num_sequence_text
 from funasr.fileio.read_text import read_2column_text
 from funasr.fileio.sound_scp import SoundScpReader
 from funasr.utils.sized_dict import SizedDict
 
 
 class AdapterForSoundScpReader(collections.abc.Mapping):
     def __init__(self, loader, dtype=None):
-        assert check_argument_types()
         self.loader = loader
         self.dtype = dtype
         self.rate = None
 
     def keys(self):
         return self.loader.keys()
 
@@ -280,15 +277,14 @@
         ] = None,
         float_dtype: str = "float32",
         int_dtype: str = "long",
         max_cache_size: Union[float, int, str] = 0.0,
         max_cache_fd: int = 0,
         dest_sample_rate: int = 16000,
     ):
-        assert check_argument_types()
         if len(path_name_type_list) == 0:
             raise ValueError(
                 '1 or more elements are required for "path_name_type_list"'
             )
 
         path_name_type_list = copy.deepcopy(path_name_type_list)
         self.preprocess = preprocess
@@ -375,15 +371,14 @@
         _mes += "("
         for name, (path, _type) in self.debug_info.items():
             _mes += f'\n  {name}: {{"path": "{path}", "type": "{_type}"}}'
         _mes += f"\n  preprocess: {self.preprocess})"
         return _mes
 
     def __getitem__(self, uid: Union[str, int]) -> Tuple[str, Dict[str, np.ndarray]]:
-        assert check_argument_types()
 
         # Change integer-id to string-id
         if isinstance(uid, int):
             d = next(iter(self.loader_dict.values()))
             uid = list(d)[uid]
 
         if self.cache is not None and uid in self.cache:
@@ -440,9 +435,8 @@
                 raise NotImplementedError(f"Not supported dtype: {value.dtype}")
             data[name] = value
 
         if self.cache is not None and self.cache.size < self.max_cache_size:
             self.cache[uid] = data
 
         retval = uid, data
-        assert check_return_type(retval)
         return retval
```

### Comparing `funasr-0.6.6/funasr/datasets/iterable_dataset.py` & `funasr-0.6.7/funasr/datasets/iterable_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import kaldiio
 import numpy as np
 import torch
 import torchaudio
 import soundfile
 from torch.utils.data.dataset import IterableDataset
-from typeguard import check_argument_types
 import os.path
 
 from funasr.datasets.dataset import ESPnetDataset
 
 
 SUPPORT_AUDIO_TYPE_SETS = ['flac', 'mp3', 'ogg', 'opus', 'wav', 'pcm']
 
@@ -117,15 +116,14 @@
             ] = None,
             float_dtype: str = "float32",
             fs: dict = None,
             mc: bool = False,
             int_dtype: str = "long",
             key_file: str = None,
     ):
-        assert check_argument_types()
         if len(path_name_type_list) == 0:
             raise ValueError(
                 '1 or more elements are required for "path_name_type_list"'
             )
 
         path_name_type_list = copy.deepcopy(path_name_type_list)
         self.preprocess = preprocess
```

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.6.7/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 from typing import Iterable
 from typing import List
 from typing import Union
 
 import sentencepiece as spm
 from torch.utils.data import DataLoader
-from typeguard import check_argument_types
 
 from funasr.datasets.large_datasets.dataset import Dataset
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 from funasr.text.abs_tokenizer import AbsTokenizer
 
 
 def read_symbol_table(symbol_table_file):
@@ -39,15 +38,14 @@
             value = s[1:]
             seg_dict[key] = " ".join(value)
     return seg_dict
 
 
 class SentencepiecesTokenizer(AbsTokenizer):
     def __init__(self, model: Union[Path, str]):
-        assert check_argument_types()
         self.model = str(model)
         self.sp = None
 
     def __repr__(self):
         return f'{self.__class__.__name__}(model="{self.model}")'
 
     def _build_sentence_piece_processor(self):
```

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.6.7/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.6.7/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/dataset.py` & `funasr-0.6.7/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.6.7/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.6.7/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.6.7/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.6.7/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.6.7/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.6.7/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/ms_dataset.py` & `funasr-0.6.7/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/datasets/preprocessor.py` & `funasr-0.6.7/funasr/datasets/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from typing import Iterable
 from typing import List
 from typing import Union
 
 import numpy as np
 import scipy.signal
 import soundfile
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.cleaner import TextCleaner
 from funasr.text.token_id_converter import TokenIDConverter
 
 
 class AbsPreprocessor(ABC):
@@ -264,15 +262,14 @@
                 )
         else:
             self.noises = None
 
     def _speech_process(
             self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, Union[str, np.ndarray]]:
-        assert check_argument_types()
         if self.speech_name in data:
             if self.train and (self.rirs is not None or self.noises is not None):
                 speech = data[self.speech_name]
                 nsamples = len(speech)
 
                 # speech: (Nmic, Time)
                 if speech.ndim == 1:
@@ -351,15 +348,14 @@
                     speech /= ma
                 data[self.speech_name] = speech
 
             if self.speech_volume_normalize is not None:
                 speech = data[self.speech_name]
                 ma = np.max(np.abs(speech))
                 data[self.speech_name] = speech * self.speech_volume_normalize / ma
-        assert check_return_type(data)
         return data
 
     def _text_process(
             self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         if self.text_name in data and self.tokenizer is not None:
             text = data[self.text_name]
@@ -368,21 +364,19 @@
                 tokens = text.strip().split(" ")
                 if self.seg_dict is not None:
                     tokens = seg_tokenize(tokens, self.seg_dict)
             else:
                 tokens = self.tokenizer.text2tokens(text)
             text_ints = self.token_id_converter.tokens2ids(tokens)
             data[self.text_name] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
     def __call__(
             self, uid: str, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
-        assert check_argument_types()
 
         data = self._speech_process(data)
         data = self._text_process(data)
         return data
 
 ## FIXME
 class LMPreprocessor(CommonPreprocessor):
@@ -441,15 +435,14 @@
                 tokens = text.strip().split(" ")
                 if self.seg_dict is not None:
                     tokens = seg_tokenize_wo_pattern(tokens, self.seg_dict)
             else:
                 tokens = self.tokenizer.text2tokens(text)
             text_ints = self.token_id_converter.tokens2ids(tokens)
             data[self.text_name] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
 
 class CommonPreprocessor_multi(AbsPreprocessor):
     def __init__(
             self,
             train: bool,
@@ -498,21 +491,19 @@
         for text_n in self.text_name:
             if text_n in data and self.tokenizer is not None:
                 text = data[text_n]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer.text2tokens(text)
                 text_ints = self.token_id_converter.tokens2ids(tokens)
                 data[text_n] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
     def __call__(
             self, uid: str, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
-        assert check_argument_types()
 
         if self.speech_name in data:
             # Nothing now: candidates:
             # - STFT
             # - Fbank
             # - CMVN
             # - Data augmentation
@@ -608,15 +599,14 @@
             text_name = self.text_name[i]
             if text_name in data and self.tokenizer[i] is not None:
                 text = data[text_name]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer[i].text2tokens(text)
                 text_ints = self.token_id_converter[i].tokens2ids(tokens)
                 data[text_name] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
 class CodeMixTokenizerCommonPreprocessor(CommonPreprocessor):
     def __init__(
             self,
             train: bool,
             token_type: str = None,
@@ -686,15 +676,14 @@
             if len(current_word) > 0:
                 words.append(current_word)
         return words
 
     def __call__(
             self, uid: str, data: Dict[str, Union[list, str, np.ndarray]]
     ) -> Dict[str, Union[list, np.ndarray]]:
-        assert check_argument_types()
         # Split words.
         if isinstance(data[self.text_name], str):
             split_text = self.split_words(data[self.text_name])
         else:
             split_text = data[self.text_name]
         data[self.text_name] = " ".join(split_text)
         data = self._speech_process(data)
```

### Comparing `funasr-0.6.6/funasr/datasets/small_datasets/collate_fn.py` & `funasr-0.6.7/funasr/datasets/small_datasets/collate_fn.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.modules.nets_utils import pad_list
 
 
 class CommonCollateFn:
     """Functor class of common_collate_fn()"""
 
     def __init__(
             self,
             float_pad_value: Union[float, int] = 0.0,
             int_pad_value: int = -32768,
             not_sequence: Collection[str] = (),
             max_sample_size=None
     ):
-        assert check_argument_types()
         self.float_pad_value = float_pad_value
         self.int_pad_value = int_pad_value
         self.not_sequence = set(not_sequence)
         self.max_sample_size = max_sample_size
 
     def __repr__(self):
         return (
@@ -49,15 +46,14 @@
         data: Collection[Tuple[str, Dict[str, np.ndarray]]],
         float_pad_value: Union[float, int] = 0.0,
         int_pad_value: int = -32768,
         not_sequence: Collection[str] = (),
 ) -> Tuple[List[str], Dict[str, torch.Tensor]]:
     """Concatenate ndarray-list to an array and convert to torch.Tensor.
     """
-    assert check_argument_types()
     uttids = [u for u, _ in data]
     data = [d for _, d in data]
 
     assert all(set(data[0]) == set(d) for d in data), "dict-keys mismatching"
     assert all(
         not k.endswith("_lengths") for k in data[0]
     ), f"*_lengths is reserved: {list(data[0])}"
@@ -75,15 +71,14 @@
         output[key] = tensor
 
         if key not in not_sequence:
             lens = torch.tensor([d[key].shape[0] for d in data], dtype=torch.long)
             output[key + "_lengths"] = lens
 
     output = (uttids, output)
-    assert check_return_type(output)
     return output
 
 def crop_to_max_size(feature, target_size):
     size = len(feature)
     diff = size - target_size
     if diff <= 0:
         return feature
```

### Comparing `funasr-0.6.6/funasr/datasets/small_datasets/dataset.py` & `funasr-0.6.7/funasr/datasets/small_datasets/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,21 @@
 from typing import Mapping
 from typing import Union, List, Tuple
 
 import kaldiio
 import numpy as np
 import torch
 from torch.utils.data.dataset import Dataset
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.fileio.npy_scp import NpyScpReader
 from funasr.fileio.sound_scp import SoundScpReader
 
 
 class AdapterForSoundScpReader(collections.abc.Mapping):
     def __init__(self, loader, dtype=None):
-        assert check_argument_types()
         self.loader = loader
         self.dtype = dtype
         self.rate = None
 
     def keys(self):
         return self.loader.keys()
 
@@ -108,15 +105,14 @@
             ] = None,
             float_dtype: str = "float32",
             int_dtype: str = "long",
             dest_sample_rate: int = 16000,
             speed_perturb: Union[list, tuple] = None,
             mode: str = "train",
     ):
-        assert check_argument_types()
         if len(path_name_type_list) == 0:
             raise ValueError(
                 '1 or more elements are required for "path_name_type_list"'
             )
 
         path_name_type_list = copy.deepcopy(path_name_type_list)
         self.preprocess = preprocess
@@ -203,15 +199,14 @@
         _mes += "("
         for name, (path, _type) in self.debug_info.items():
             _mes += f'\n  {name}: {{"path": "{path}", "type": "{_type}"}}'
         _mes += f"\n  preprocess: {self.preprocess})"
         return _mes
 
     def __getitem__(self, uid: Union[str, int]) -> Tuple[str, Dict[str, np.ndarray]]:
-        assert check_argument_types()
 
         # Change integer-id to string-id
         if isinstance(uid, int):
             d = next(iter(self.loader_dict.values()))
             uid = list(d)[uid]
 
         data = {}
@@ -261,9 +256,8 @@
             elif value.dtype.kind == "i":
                 value = value.astype(self.int_dtype)
             else:
                 raise NotImplementedError(f"Not supported dtype: {value.dtype}")
             data[name] = value
 
         retval = uid, data
-        assert check_return_type(retval)
         return retval
```

### Comparing `funasr-0.6.6/funasr/datasets/small_datasets/length_batch_sampler.py` & `funasr-0.6.7/funasr/datasets/small_datasets/length_batch_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterator
 from typing import List
 from typing import Dict
 from typing import Tuple
 from typing import Union
 
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import load_num_sequence_text
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class LengthBatchSampler(AbsSampler):
     def __init__(
@@ -17,15 +16,14 @@
         shape_files: Union[Tuple[str, ...], List[str], Dict],
         min_batch_size: int = 1,
         sort_in_batch: str = "descending",
         sort_batch: str = "ascending",
         drop_last: bool = False,
         padding: bool = True,
     ):
-        assert check_argument_types()
         assert batch_bins > 0
         if sort_batch != "ascending" and sort_batch != "descending":
             raise ValueError(
                 f"sort_batch must be ascending or descending: {sort_batch}"
             )
         if sort_in_batch != "descending" and sort_in_batch != "ascending":
             raise ValueError(
```

### Comparing `funasr-0.6.6/funasr/datasets/small_datasets/preprocessor.py` & `funasr-0.6.7/funasr/datasets/small_datasets/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from typing import Iterable
 from typing import List
 from typing import Union
 
 import numpy as np
 import scipy.signal
 import soundfile
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.cleaner import TextCleaner
 from funasr.text.token_id_converter import TokenIDConverter
 
 
 class AbsPreprocessor(ABC):
@@ -256,15 +254,14 @@
                 )
         else:
             self.noises = None
 
     def _speech_process(
             self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, Union[str, np.ndarray]]:
-        assert check_argument_types()
         if self.speech_name in data:
             if self.train and (self.rirs is not None or self.noises is not None):
                 speech = data[self.speech_name]
                 nsamples = len(speech)
 
                 # speech: (Nmic, Time)
                 if speech.ndim == 1:
@@ -343,15 +340,14 @@
                     speech /= ma
                 data[self.speech_name] = speech
 
             if self.speech_volume_normalize is not None:
                 speech = data[self.speech_name]
                 ma = np.max(np.abs(speech))
                 data[self.speech_name] = speech * self.speech_volume_normalize / ma
-        assert check_return_type(data)
         return data
 
     def _text_process(
             self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         if self.text_name in data and self.tokenizer is not None:
             text = data[self.text_name]
@@ -361,21 +357,19 @@
                 if self.seg_dict is not None:
                     tokens = forward_segment("".join(tokens), self.seg_dict)
                     tokens = seg_tokenize(tokens, self.seg_dict)
             else:
                 tokens = self.tokenizer.text2tokens(text)
             text_ints = self.token_id_converter.tokens2ids(tokens)
             data[self.text_name] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
     def __call__(
             self, uid: str, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
-        assert check_argument_types()
 
         data = self._speech_process(data)
         data = self._text_process(data)
         return data
 
 
 ## FIXME
@@ -435,15 +429,14 @@
                 tokens = text.strip().split(" ")
                 if self.seg_dict is not None:
                     tokens = seg_tokenize_wo_pattern(tokens, self.seg_dict)
             else:
                 tokens = self.tokenizer.text2tokens(text)
             text_ints = self.token_id_converter.tokens2ids(tokens)
             data[self.text_name] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
 
 class CommonPreprocessor_multi(AbsPreprocessor):
     def __init__(
             self,
             train: bool,
@@ -492,21 +485,19 @@
         for text_n in self.text_name:
             if text_n in data and self.tokenizer is not None:
                 text = data[text_n]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer.text2tokens(text)
                 text_ints = self.token_id_converter.tokens2ids(tokens)
                 data[text_n] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
     def __call__(
             self, uid: str, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
-        assert check_argument_types()
 
         if self.speech_name in data:
             # Nothing now: candidates:
             # - STFT
             # - Fbank
             # - CMVN
             # - Data augmentation
@@ -602,15 +593,14 @@
             text_name = self.text_name[i]
             if text_name in data and self.tokenizer[i] is not None:
                 text = data[text_name]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer[i].text2tokens(text)
                 text_ints = self.token_id_converter[i].tokens2ids(tokens)
                 data[text_name] = np.array(text_ints, dtype=np.int64)
-        assert check_return_type(data)
         return data
 
 
 class CodeMixTokenizerCommonPreprocessor(CommonPreprocessor):
     def __init__(
             self,
             train: bool,
@@ -681,15 +671,14 @@
             if len(current_word) > 0:
                 words.append(current_word)
         return words
 
     def __call__(
             self, uid: str, data: Dict[str, Union[list, str, np.ndarray]]
     ) -> Dict[str, Union[list, np.ndarray]]:
-        assert check_argument_types()
         # Split words.
         if isinstance(data[self.text_name], str):
             split_text = self.split_words(data[self.text_name])
         else:
             split_text = data[self.text_name]
         data[self.text_name] = " ".join(split_text)
         data = self._speech_process(data)
```

### Comparing `funasr-0.6.6/funasr/datasets/small_datasets/sequence_iter_factory.py` & `funasr-0.6.7/funasr/datasets/small_datasets/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/export_model.py` & `funasr-0.6.7/funasr/export/export_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 from typing import Union, Dict
 from pathlib import Path
-from typeguard import check_argument_types
 
 import os
 import logging
 import torch
 
 from funasr.export.models import get_model
 import numpy as np
 import random
-from funasr.utils.types import str2bool
+from funasr.utils.types import str2bool, str2triple_str
 # torch_version = float(".".join(torch.__version__.split(".")[:2]))
 # assert torch_version > 1.9
 
 class ModelExport:
     def __init__(
         self,
         cache_dir: Union[Path, str] = None,
@@ -22,15 +21,14 @@
         device: str = "cpu",
         quant: bool = True,
         fallback_num: int = 0,
         audio_in: str = None,
         calib_num: int = 200,
         model_revision: str = None,
     ):
-        assert check_argument_types()
         self.set_all_random_seed(0)
 
         self.cache_dir = cache_dir
         self.export_config = dict(
             feats_dim=560,
             onnx=False,
         )
@@ -190,14 +188,15 @@
             config = os.path.join(model_dir, 'config.yaml')
             model_file = os.path.join(model_dir, 'model.pb')
             cmvn_file = os.path.join(model_dir, 'am.mvn')
             model, asr_train_args = ASRTask.build_model_from_file(
                 config, model_file, cmvn_file, 'cpu'
             )
             self.frontend = model.frontend
+            self.export_config["feats_dim"] = 560
         elif mode.startswith('offline'):
             from funasr.tasks.vad import VADTask
             config = os.path.join(model_dir, 'vad.yaml')
             model_file = os.path.join(model_dir, 'vad.pb')
             cmvn_file = os.path.join(model_dir, 'vad.mvn')
             
             model, vad_infer_args = VADTask.build_model_from_file(
@@ -261,15 +260,16 @@
                     nodes_to_exclude=nodes_to_exclude,
                 )
 
 
 if __name__ == '__main__':
     import argparse
     parser = argparse.ArgumentParser()
-    parser.add_argument('--model-name', type=str, required=True)
+    # parser.add_argument('--model-name', type=str, required=True)
+    parser.add_argument('--model-name', type=str, action="append", required=True, default=[])
     parser.add_argument('--export-dir', type=str, required=True)
     parser.add_argument('--type', type=str, default='onnx', help='["onnx", "torch"]')
     parser.add_argument('--device', type=str, default='cpu', help='["cpu", "cuda"]')
     parser.add_argument('--quantize', type=str2bool, default=False, help='export quantized model')
     parser.add_argument('--fallback-num', type=int, default=0, help='amp fallback number')
     parser.add_argument('--audio_in', type=str, default=None, help='["wav", "wav.scp"]')
     parser.add_argument('--calib_num', type=int, default=200, help='calib max num')
@@ -282,8 +282,10 @@
         device=args.device,
         quant=args.quantize,
         fallback_num=args.fallback_num,
         audio_in=args.audio_in,
         calib_num=args.calib_num,
         model_revision=args.model_revision,
     )
-    export_model.export(args.model_name)
+    for model_name in args.model_name:
+        print("export model: {}".format(model_name))
+        export_model.export(model_name)
```

### Comparing `funasr-0.6.6/funasr/export/models/CT_Transformer.py` & `funasr-0.6.7/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/__init__.py` & `funasr-0.6.7/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.6.7/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.6.7/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.6.7/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/e2e_vad.py` & `funasr-0.6.7/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.6.7/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.6.7/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.6.7/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/modules/decoder_layer.py` & `funasr-0.6.7/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/modules/encoder_layer.py` & `funasr-0.6.7/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/modules/feedforward.py` & `funasr-0.6.7/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/modules/multihead_att.py` & `funasr-0.6.7/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/models/predictor/cif.py` & `funasr-0.6.7/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/test/test_onnx.py` & `funasr-0.6.7/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/test/test_onnx_punc.py` & `funasr-0.6.7/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.6.7/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/test/test_onnx_vad.py` & `funasr-0.6.7/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/export/utils/torch_function.py` & `funasr-0.6.7/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/fileio/datadir_writer.py` & `funasr-0.6.7/funasr/fileio/datadir_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from pathlib import Path
 from typing import Union
 import warnings
 
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 
 class DatadirWriter:
     """Writer class to create kaldi like data directory.
 
     Examples:
         >>> with DatadirWriter("output") as writer:
@@ -16,40 +14,36 @@
         ...     # Write "uttidA some/where/a.wav"
         ...     subwriter["uttidA"] = "some/where/a.wav"
         ...     subwriter["uttidB"] = "some/where/b.wav"
 
     """
 
     def __init__(self, p: Union[Path, str]):
-        assert check_argument_types()
         self.path = Path(p)
         self.chilidren = {}
         self.fd = None
         self.has_children = False
         self.keys = set()
 
     def __enter__(self):
         return self
 
     def __getitem__(self, key: str) -> "DatadirWriter":
-        assert check_argument_types()
         if self.fd is not None:
             raise RuntimeError("This writer points out a file")
 
         if key not in self.chilidren:
             w = DatadirWriter((self.path / key))
             self.chilidren[key] = w
             self.has_children = True
 
         retval = self.chilidren[key]
-        assert check_return_type(retval)
         return retval
 
     def __setitem__(self, key: str, value: str):
-        assert check_argument_types()
         if self.has_children:
             raise RuntimeError("This writer points out a directory")
         if key in self.keys:
             warnings.warn(f"Duplicated: {key}")
 
         if self.fd is None:
             self.path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `funasr-0.6.6/funasr/fileio/npy_scp.py` & `funasr-0.6.7/funasr/fileio/npy_scp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import collections.abc
 from pathlib import Path
 from typing import Union
 
 import numpy as np
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import read_2column_text
 
 
 class NpyScpWriter:
     """Writer class for a scp file of numpy file.
 
@@ -21,15 +20,14 @@
         >>> writer = NpyScpWriter('./data/', './data/feat.scp')
         >>> writer['aa'] = numpy_array
         >>> writer['bb'] = numpy_array
 
     """
 
     def __init__(self, outdir: Union[Path, str], scpfile: Union[Path, str]):
-        assert check_argument_types()
         self.dir = Path(outdir)
         self.dir.mkdir(parents=True, exist_ok=True)
         scpfile = Path(scpfile)
         scpfile.parent.mkdir(parents=True, exist_ok=True)
         self.fscp = scpfile.open("w", encoding="utf-8")
 
         self.data = {}
@@ -69,15 +67,14 @@
 
         >>> reader = NpyScpReader('npy.scp')
         >>> array = reader['key1']
 
     """
 
     def __init__(self, fname: Union[Path, str]):
-        assert check_argument_types()
         self.fname = Path(fname)
         self.data = read_2column_text(fname)
 
     def get_path(self, key):
         return self.data[key]
 
     def __getitem__(self, key) -> np.ndarray:
```

### Comparing `funasr-0.6.6/funasr/fileio/rand_gen_dataset.py` & `funasr-0.6.7/funasr/fileio/rand_gen_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import collections
 from pathlib import Path
 from typing import Union
 
 import numpy as np
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import load_num_sequence_text
 
 
 class FloatRandomGenerateDataset(collections.abc.Mapping):
     """Generate float array from shape.txt.
 
@@ -25,15 +24,14 @@
 
     def __init__(
         self,
         shape_file: Union[Path, str],
         dtype: Union[str, np.dtype] = "float32",
         loader_type: str = "csv_int",
     ):
-        assert check_argument_types()
         shape_file = Path(shape_file)
         self.utt2shape = load_num_sequence_text(shape_file, loader_type)
         self.dtype = np.dtype(dtype)
 
     def __iter__(self):
         return iter(self.utt2shape)
 
@@ -64,15 +62,14 @@
         self,
         shape_file: Union[Path, str],
         low: int,
         high: int = None,
         dtype: Union[str, np.dtype] = "int64",
         loader_type: str = "csv_int",
     ):
-        assert check_argument_types()
         shape_file = Path(shape_file)
         self.utt2shape = load_num_sequence_text(shape_file, loader_type)
         self.dtype = np.dtype(dtype)
         self.low = low
         self.high = high
 
     def __iter__(self):
```

### Comparing `funasr-0.6.6/funasr/fileio/read_text.py` & `funasr-0.6.7/funasr/fileio/read_text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import logging
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Union
 
-from typeguard import check_argument_types
 
 
 def read_2column_text(path: Union[Path, str]) -> Dict[str, str]:
     """Read a text file having 2 column as dict object.
 
     Examples:
         wav.scp:
             key1 /some/path/a.wav
             key2 /some/path/b.wav
 
         >>> read_2column_text('wav.scp')
         {'key1': '/some/path/a.wav', 'key2': '/some/path/b.wav'}
 
     """
-    assert check_argument_types()
 
     data = {}
     with Path(path).open("r", encoding="utf-8") as f:
         for linenum, line in enumerate(f, 1):
             sps = line.rstrip().split(maxsplit=1)
             if len(sps) == 1:
                 k, v = sps[0], ""
@@ -43,15 +41,14 @@
     Examples:
         key1 1 2 3
         key2 34 5 6
 
         >>> d = load_num_sequence_text('text')
         >>> np.testing.assert_array_equal(d["key1"], np.array([1, 2, 3]))
     """
-    assert check_argument_types()
     if loader_type == "text_int":
         delimiter = " "
         dtype = int
     elif loader_type == "text_float":
         delimiter = " "
         dtype = float
     elif loader_type == "csv_int":
```

### Comparing `funasr-0.6.6/funasr/fileio/sound_scp.py` & `funasr-0.6.7/funasr/fileio/sound_scp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 from typing import List, Tuple, Union
 
 import random
 import numpy as np
 import soundfile
 import librosa
-from typeguard import check_argument_types
 
 import torch
 import torchaudio
 
 from funasr.fileio.read_text import read_2column_text
 
 def soundfile_read(
@@ -102,15 +101,14 @@
         fname,
         dtype=np.int16,
         always_2d: bool = False,
         normalize: bool = False,
         dest_sample_rate: int = 16000,
         speed_perturb: Union[list, tuple] = None,
     ):
-        assert check_argument_types()
         self.fname = fname
         self.dtype = dtype
         self.always_2d = always_2d
         self.normalize = normalize
         self.data = read_2column_text(fname)
         self.dest_sample_rate = dest_sample_rate
         self.speed_perturb = speed_perturb
@@ -175,15 +173,14 @@
     def __init__(
         self,
         outdir: Union[Path, str],
         scpfile: Union[Path, str],
         format="wav",
         dtype=None,
     ):
-        assert check_argument_types()
         self.dir = Path(outdir)
         self.dir.mkdir(parents=True, exist_ok=True)
         scpfile = Path(scpfile)
         scpfile.parent.mkdir(parents=True, exist_ok=True)
         self.fscp = scpfile.open("w", encoding="utf-8")
         self.format = format
         self.dtype = dtype
```

### Comparing `funasr-0.6.6/funasr/iterators/chunk_iter_factory.py` & `funasr-0.6.7/funasr/iterators/chunk_iter_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import List
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 from funasr.iterators.sequence_iter_factory import SequenceIterFactory
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class ChunkIterFactory(AbsIterFactory):
@@ -47,15 +46,14 @@
         num_samples_per_epoch: int = None,
         seed: int = 0,
         shuffle: bool = False,
         num_workers: int = 0,
         collate_fn=None,
         pin_memory: bool = False,
     ):
-        assert check_argument_types()
         assert all(len(x) == 1 for x in batches), "batch-size must be 1"
 
         self.per_sample_iter_factory = SequenceIterFactory(
             dataset=dataset,
             batches=batches,
             num_iters_per_epoch=num_samples_per_epoch,
             seed=seed,
```

### Comparing `funasr-0.6.6/funasr/iterators/multiple_iter_factory.py` & `funasr-0.6.7/funasr/iterators/multiple_iter_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import logging
 from typing import Callable
 from typing import Collection
 from typing import Iterator
 
 import numpy as np
-from typeguard import check_argument_types
 
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 
 
 class MultipleIterFactory(AbsIterFactory):
     def __init__(
         self,
         build_funcs: Collection[Callable[[], AbsIterFactory]],
         seed: int = 0,
         shuffle: bool = False,
     ):
-        assert check_argument_types()
         self.build_funcs = list(build_funcs)
         self.seed = seed
         self.shuffle = shuffle
 
     def build_iter(self, epoch: int, shuffle: bool = None) -> Iterator:
         if shuffle is None:
             shuffle = self.shuffle
```

### Comparing `funasr-0.6.6/funasr/iterators/sequence_iter_factory.py` & `funasr-0.6.7/funasr/iterators/sequence_iter_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any
 from typing import Sequence
 from typing import Union
 
 import numpy as np
 from torch.utils.data import DataLoader
-from typeguard import check_argument_types
 
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class RawSampler(AbsSampler):
     def __init__(self, batches):
@@ -42,15 +41,14 @@
         num_iters_per_epoch: int = None,
         seed: int = 0,
         shuffle: bool = False,
         num_workers: int = 0,
         collate_fn=None,
         pin_memory: bool = False,
     ):
-        assert check_argument_types()
 
         if not isinstance(batches, AbsSampler):
             self.sampler = RawSampler(batches)
         else:
             self.sampler = batches
 
         self.dataset = dataset
```

### Comparing `funasr-0.6.6/funasr/layers/complex_utils.py` & `funasr-0.6.7/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/layers/global_mvn.py` & `funasr-0.6.7/funasr/layers/global_mvn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.inversible_interface import InversibleInterface
 
 
 class GlobalMVN(AbsNormalize, InversibleInterface):
@@ -24,15 +23,14 @@
     def __init__(
         self,
         stats_file: Union[Path, str],
         norm_means: bool = True,
         norm_vars: bool = True,
         eps: float = 1.0e-20,
     ):
-        assert check_argument_types()
         super().__init__()
         self.norm_means = norm_means
         self.norm_vars = norm_vars
         self.eps = eps
         stats_file = Path(stats_file)
 
         self.stats_file = stats_file
```

### Comparing `funasr-0.6.6/funasr/layers/label_aggregation.py` & `funasr-0.6.7/funasr/layers/label_aggregation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import torch
-from typeguard import check_argument_types
 from typing import Optional
 from typing import Tuple
 
 from funasr.modules.nets_utils import make_pad_mask
 
 
 class LabelAggregate(torch.nn.Module):
     def __init__(
         self,
         win_length: int = 512,
         hop_length: int = 128,
         center: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
 
         self.win_length = win_length
         self.hop_length = hop_length
         self.center = center
 
     def extra_repr(self):
```

### Comparing `funasr-0.6.6/funasr/layers/log_mel.py` & `funasr-0.6.7/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/layers/mask_along_axis.py` & `funasr-0.6.7/funasr/layers/mask_along_axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import math
 import torch
-from typeguard import check_argument_types
 from typing import Sequence
 from typing import Union
 
 
 def mask_along_axis(
     spec: torch.Tensor,
     spec_lengths: torch.Tensor,
@@ -143,15 +142,14 @@
     def __init__(
         self,
         mask_width_range: Union[int, Sequence[int]] = (0, 30),
         num_mask: int = 2,
         dim: Union[int, str] = "time",
         replace_with_zero: bool = True,
     ):
-        assert check_argument_types()
         if isinstance(mask_width_range, int):
             mask_width_range = (0, mask_width_range)
         if len(mask_width_range) != 2:
             raise TypeError(
                 f"mask_width_range must be a tuple of int and int values: "
                 f"{mask_width_range}",
             )
@@ -210,15 +208,14 @@
     def __init__(
         self,
         mask_width_ratio_range: Union[float, Sequence[float]] = (0.0, 0.05),
         num_mask: int = 2,
         dim: Union[int, str] = "time",
         replace_with_zero: bool = True,
     ):
-        assert check_argument_types()
         if isinstance(mask_width_ratio_range, float):
             mask_width_ratio_range = (0.0, mask_width_ratio_range)
         if len(mask_width_ratio_range) != 2:
             raise TypeError(
                 f"mask_width_ratio_range must be a tuple of float and float values: "
                 f"{mask_width_ratio_range}",
             )
@@ -279,15 +276,14 @@
         self,
         mask_width_range: Union[int, Sequence[int]] = (0, 30),
         num_mask: int = 2,
         dim: Union[int, str] = "time",
         replace_with_zero: bool = True,
         lfr_rate: int = 1,
     ):
-        assert check_argument_types()
         if isinstance(mask_width_range, int):
             mask_width_range = (0, mask_width_range)
         if len(mask_width_range) != 2:
             raise TypeError(
                 f"mask_width_range must be a tuple of int and int values: "
                 f"{mask_width_range}",
             )
```

### Comparing `funasr-0.6.6/funasr/layers/sinc_conv.py` & `funasr-0.6.7/funasr/layers/sinc_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 #  2020, Technische Universität München;  Ludwig Kürzinger
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 """Sinc convolutions."""
 import math
 import torch
-from typeguard import check_argument_types
 from typing import Union
 
 
 class LogCompression(torch.nn.Module):
     """Log Compression Activation.
 
     Activation function `log(abs(x) + 1)`.
@@ -67,15 +66,14 @@
             kernel_size: Sinc filter kernel size (needs to be an odd number).
             stride: See torch.nn.functional.conv1d.
             padding: See torch.nn.functional.conv1d.
             dilation: See torch.nn.functional.conv1d.
             window_func: Window function on the filter, one of ["hamming", "none"].
             fs (str, int, float): Sample rate of the input data
         """
-        assert check_argument_types()
         super().__init__()
         window_funcs = {
             "none": self.none_window,
             "hamming": self.hamming_window,
         }
         if window_func not in window_funcs:
             raise NotImplementedError(
@@ -204,15 +202,14 @@
             channels: Number of channels.
             fs: Sample rate.
 
         Returns:
             torch.Tensor: Filter start frequencíes.
             torch.Tensor: Filter stop frequencies.
         """
-        assert check_argument_types()
         # min and max bandpass edge frequencies
         min_frequency = torch.tensor(30.0)
         max_frequency = torch.tensor(fs * 0.5)
         frequencies = torch.linspace(
             cls.convert(min_frequency), cls.convert(max_frequency), channels + 2
         )
         frequencies = cls.invert(frequencies)
@@ -253,15 +250,14 @@
             channels: Number of channels.
             fs: Sample rate.
 
         Returns:
             torch.Tensor: Filter start frequencíes.
             torch.Tensor: Filter stop frequencíes.
         """
-        assert check_argument_types()
         # min and max BARK center frequencies by approximation
         min_center_frequency = torch.tensor(70.0)
         max_center_frequency = torch.tensor(fs * 0.45)
         center_frequencies = torch.linspace(
             cls.convert(min_center_frequency),
             cls.convert(max_center_frequency),
             channels,
```

### Comparing `funasr-0.6.6/funasr/layers/stft.py` & `funasr-0.6.7/funasr/layers/stft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from distutils.version import LooseVersion
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
 from torch_complex.tensor import ComplexTensor
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.layers.complex_utils import is_complex
 from funasr.layers.inversible_interface import InversibleInterface
 import librosa
 import numpy as np
 
@@ -26,15 +25,14 @@
         win_length: int = None,
         hop_length: int = 128,
         window: Optional[str] = "hann",
         center: bool = True,
         normalized: bool = False,
         onesided: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
         self.n_fft = n_fft
         if win_length is None:
             self.win_length = n_fft
         else:
             self.win_length = win_length
         self.hop_length = hop_length
```

### Comparing `funasr-0.6.6/funasr/layers/time_warp.py` & `funasr-0.6.7/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/layers/utterance_mvn.py` & `funasr-0.6.7/funasr/layers/utterance_mvn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import Tuple
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.layers.abs_normalize import AbsNormalize
 
 
 class UtteranceMVN(AbsNormalize):
     def __init__(
         self,
         norm_means: bool = True,
         norm_vars: bool = False,
         eps: float = 1.0e-20,
     ):
-        assert check_argument_types()
         super().__init__()
         self.norm_means = norm_means
         self.norm_vars = norm_vars
         self.eps = eps
 
     def extra_repr(self):
         return f"norm_means={self.norm_means}, norm_vars={self.norm_vars}"
```

### Comparing `funasr-0.6.6/funasr/losses/label_smoothing_loss.py` & `funasr-0.6.7/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/main_funcs/average_nbest_models.py` & `funasr-0.6.7/funasr/main_funcs/average_nbest_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Sequence
 from typing import Union
 import warnings
 import os
 from io import BytesIO
 
 import torch
-from typeguard import check_argument_types
 from typing import Collection
 
 from funasr.train.reporter import Reporter
 
 
 @torch.no_grad()
 def average_nbest_models(
@@ -30,15 +29,14 @@
         output_dir: The directory contains the model file for each epoch
         reporter: Reporter instance
         best_model_criterion: Give criterions to decide the best model.
             e.g. [("valid", "loss", "min"), ("train", "acc", "max")]
         nbest: Number of best model files to be averaged
         suffix: A suffix added to the averaged model file name
     """
-    assert check_argument_types()
     if isinstance(nbest, int):
         nbests = [nbest]
     else:
         nbests = list(nbest)
     if len(nbests) == 0:
         warnings.warn("At least 1 nbest values are required")
         nbests = [1]
```

### Comparing `funasr-0.6.6/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.6.7/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/main_funcs/collect_stats.py` & `funasr-0.6.7/funasr/main_funcs/collect_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import torch
 from torch.nn.parallel import data_parallel
 from torch.utils.data import DataLoader
-from typeguard import check_argument_types
 
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.fileio.npy_scp import NpyScpWriter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
 from funasr.models.base_model import FunASRModel
 
@@ -33,15 +32,14 @@
     """Perform on collect_stats mode.
 
     Running for deriving the shape information from data
     and gathering statistics.
     This method is used before executing train().
 
     """
-    assert check_argument_types()
 
     npy_scp_writers = {}
     for itr, mode in zip([train_iter, valid_iter], ["train", "valid"]):
         if log_interval is None:
             try:
                 log_interval = max(len(itr) // 20, 10)
             except TypeError:
```

### Comparing `funasr-0.6.6/funasr/main_funcs/pack_funcs.py` & `funasr-0.6.7/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/ctc.py` & `funasr-0.6.7/funasr/models/ctc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 import torch
 import torch.nn.functional as F
-from typeguard import check_argument_types
 
 
 class CTC(torch.nn.Module):
     """CTC module.
 
     Args:
         odim: dimension of outputs
@@ -21,15 +20,14 @@
         odim: int,
         encoder_output_size: int,
         dropout_rate: float = 0.0,
         ctc_type: str = "builtin",
         reduce: bool = True,
         ignore_nan_grad: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
         eprojs = encoder_output_size
         self.dropout_rate = dropout_rate
         self.ctc_lo = torch.nn.Linear(eprojs, odim)
         self.ctc_type = ctc_type
         self.ignore_nan_grad = ignore_nan_grad
 
@@ -37,19 +35,14 @@
             self.ctc_loss = torch.nn.CTCLoss(reduction="none")
         elif self.ctc_type == "warpctc":
             import warpctc_pytorch as warp_ctc
 
             if ignore_nan_grad:
                 logging.warning("ignore_nan_grad option is not supported for warp_ctc")
             self.ctc_loss = warp_ctc.CTCLoss(size_average=True, reduce=reduce)
-
-        elif self.ctc_type == "gtnctc":
-            from espnet.nets.pytorch_backend.gtn_ctc import GTNCTCLossFunction
-
-            self.ctc_loss = GTNCTCLossFunction.apply
         else:
             raise ValueError(
                 f'ctc_type must be "builtin" or "warpctc": {self.ctc_type}'
             )
 
         self.reduce = reduce
```

### Comparing `funasr-0.6.6/funasr/models/data2vec.py` & `funasr-0.6.7/funasr/models/data2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from contextlib import contextmanager
 from distutils.version import LooseVersion
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.torch_utils.device_funcs import force_gatherable
@@ -36,15 +35,14 @@
             self,
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
             preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
     ):
-        assert check_argument_types()
 
         super().__init__()
 
         self.frontend = frontend
         self.specaug = specaug
         self.normalize = normalize
         self.preencoder = preencoder
```

### Comparing `funasr-0.6.6/funasr/models/decoder/contextual_decoder.py` & `funasr-0.6.7/funasr/models/decoder/contextual_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import torch
 import torch.nn as nn
 import numpy as np
 
 from funasr.modules.streaming_utils import utils as myutils
 from funasr.models.decoder.transformer_decoder import BaseTransformerDecoder
-from typeguard import check_argument_types
 
 from funasr.modules.attention import MultiHeadedAttentionSANMDecoder, MultiHeadedAttentionCrossAtt
 from funasr.modules.embedding import PositionalEncoding
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.positionwise_feed_forward import PositionwiseFeedForwardDecoderSANM
 from funasr.modules.repeat import repeat
 from funasr.models.decoder.sanm_decoder import DecoderLayerSANM, ParaformerSANMDecoder
@@ -122,15 +121,14 @@
         pos_enc_class=PositionalEncoding,
         normalize_before: bool = True,
         concat_after: bool = False,
         att_layer_num: int = 6,
         kernel_size: int = 21,
         sanm_shfit: int = 0,
     ):
-        assert check_argument_types()
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             dropout_rate=dropout_rate,
             positional_dropout_rate=positional_dropout_rate,
             input_layer=input_layer,
             use_output_layer=use_output_layer,
```

### Comparing `funasr-0.6.6/funasr/models/decoder/rnn_decoder.py` & `funasr-0.6.7/funasr/models/decoder/rnn_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import random
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.nets_utils import to_device
 from funasr.modules.rnn.attentions import initial_att
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.utils.get_default_kwargs import get_default_kwargs
 
@@ -93,15 +92,14 @@
         dropout: float = 0.0,
         context_residual: bool = False,
         replace_sos: bool = False,
         num_encs: int = 1,
         att_conf: dict = get_default_kwargs(build_attention_list),
     ):
         # FIXME(kamo): The parts of num_spk should be refactored more more more
-        assert check_argument_types()
         if rnn_type not in {"lstm", "gru"}:
             raise ValueError(f"Not supported: rnn_type={rnn_type}")
 
         super().__init__()
         eprojs = encoder_output_size
         self.dtype = rnn_type
         self.dunits = hidden_size
```

### Comparing `funasr-0.6.6/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.6.7/funasr/models/decoder/rnnt_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """RNN decoder definition for Transducer models."""
 
 from typing import List, Optional, Tuple
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.modules.beam_search.beam_search_transducer import Hypothesis
 from funasr.models.specaug.specaug import SpecAug
 
 class RNNTDecoder(torch.nn.Module):
     """RNN decoder module.
 
@@ -34,15 +33,14 @@
         embed_dropout_rate: float = 0.0,
         embed_pad: int = 0,
         use_embed_mask: bool = False,
     ) -> None:
         """Construct a RNNDecoder object."""
         super().__init__()
 
-        assert check_argument_types()
 
         if rnn_type not in ("lstm", "gru"):
             raise ValueError(f"Not supported: rnn_type={rnn_type}")
 
         self.embed = torch.nn.Embedding(vocab_size, embed_size, padding_idx=embed_pad)
         self.dropout_embed = torch.nn.Dropout(p=embed_dropout_rate)
```

### Comparing `funasr-0.6.6/funasr/models/decoder/sanm_decoder.py` & `funasr-0.6.7/funasr/models/decoder/sanm_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import torch
 import torch.nn as nn
 import numpy as np
 
 from funasr.modules.streaming_utils import utils as myutils
 from funasr.models.decoder.transformer_decoder import BaseTransformerDecoder
-from typeguard import check_argument_types
 
 from funasr.modules.attention import MultiHeadedAttentionSANMDecoder, MultiHeadedAttentionCrossAtt
 from funasr.modules.embedding import PositionalEncoding
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.positionwise_feed_forward import PositionwiseFeedForwardDecoderSANM
 from funasr.modules.repeat import repeat
 
@@ -177,15 +176,14 @@
             sanm_shfit: int = None,
             concat_embeds: bool = False,
             attention_dim: int = None,
             tf2torch_tensor_name_prefix_torch: str = "decoder",
             tf2torch_tensor_name_prefix_tf: str = "seq2seq/decoder",
             embed_tensor_name_prefix_tf: str = None,
     ):
-        assert check_argument_types()
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             dropout_rate=dropout_rate,
             positional_dropout_rate=positional_dropout_rate,
             input_layer=input_layer,
             use_output_layer=use_output_layer,
@@ -834,15 +832,14 @@
         concat_after: bool = False,
         att_layer_num: int = 6,
         kernel_size: int = 21,
         sanm_shfit: int = 0,
         tf2torch_tensor_name_prefix_torch: str = "decoder",
         tf2torch_tensor_name_prefix_tf: str = "seq2seq/decoder",
     ):
-        assert check_argument_types()
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             dropout_rate=dropout_rate,
             positional_dropout_rate=positional_dropout_rate,
             input_layer=input_layer,
             use_output_layer=use_output_layer,
```

### Comparing `funasr-0.6.6/funasr/models/decoder/sv_decoder.py` & `funasr-0.6.7/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/decoder/transformer_decoder.py` & `funasr-0.6.7/funasr/models/decoder/transformer_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Any
 from typing import List
 from typing import Sequence
 from typing import Tuple
 
 import torch
 from torch import nn
-from typeguard import check_argument_types
 
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.modules.attention import MultiHeadedAttention
 from funasr.modules.attention import CosineDistanceAttention
 from funasr.modules.dynamic_conv import DynamicConvolution
 from funasr.modules.dynamic_conv2d import DynamicConvolution2D
 from funasr.modules.embedding import PositionalEncoding
@@ -180,15 +179,14 @@
             dropout_rate: float = 0.1,
             positional_dropout_rate: float = 0.1,
             input_layer: str = "embed",
             use_output_layer: bool = True,
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
         attention_dim = encoder_output_size
 
         if input_layer == "embed":
             self.embed = torch.nn.Sequential(
                 torch.nn.Embedding(vocab_size, attention_dim),
                 pos_enc_class(attention_dim, positional_dropout_rate),
@@ -369,15 +367,14 @@
             src_attention_dropout_rate: float = 0.0,
             input_layer: str = "embed",
             use_output_layer: bool = True,
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
     ):
-        assert check_argument_types()
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             dropout_rate=dropout_rate,
             positional_dropout_rate=positional_dropout_rate,
             input_layer=input_layer,
             use_output_layer=use_output_layer,
@@ -424,15 +421,14 @@
             input_layer: str = "embed",
             use_output_layer: bool = True,
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
             embeds_id: int = -1,
     ):
-        assert check_argument_types()
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             dropout_rate=dropout_rate,
             positional_dropout_rate=positional_dropout_rate,
             input_layer=input_layer,
             use_output_layer=use_output_layer,
@@ -536,15 +532,14 @@
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
             conv_wshare: int = 4,
             conv_kernel_length: Sequence[int] = (11, 11, 11, 11, 11, 11),
             conv_usebias: int = False,
     ):
-        assert check_argument_types()
         if len(conv_kernel_length) != num_blocks:
             raise ValueError(
                 "conv_kernel_length must have equal number of values to num_blocks: "
                 f"{len(conv_kernel_length)} != {num_blocks}"
             )
         super().__init__(
             vocab_size=vocab_size,
@@ -598,15 +593,14 @@
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
             conv_wshare: int = 4,
             conv_kernel_length: Sequence[int] = (11, 11, 11, 11, 11, 11),
             conv_usebias: int = False,
     ):
-        assert check_argument_types()
         if len(conv_kernel_length) != num_blocks:
             raise ValueError(
                 "conv_kernel_length must have equal number of values to num_blocks: "
                 f"{len(conv_kernel_length)} != {num_blocks}"
             )
         super().__init__(
             vocab_size=vocab_size,
@@ -660,15 +654,14 @@
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
             conv_wshare: int = 4,
             conv_kernel_length: Sequence[int] = (11, 11, 11, 11, 11, 11),
             conv_usebias: int = False,
     ):
-        assert check_argument_types()
         if len(conv_kernel_length) != num_blocks:
             raise ValueError(
                 "conv_kernel_length must have equal number of values to num_blocks: "
                 f"{len(conv_kernel_length)} != {num_blocks}"
             )
         super().__init__(
             vocab_size=vocab_size,
@@ -722,15 +715,14 @@
             pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
             conv_wshare: int = 4,
             conv_kernel_length: Sequence[int] = (11, 11, 11, 11, 11, 11),
             conv_usebias: int = False,
     ):
-        assert check_argument_types()
         if len(conv_kernel_length) != num_blocks:
             raise ValueError(
                 "conv_kernel_length must have equal number of values to num_blocks: "
                 f"{len(conv_kernel_length)} != {num_blocks}"
             )
         super().__init__(
             vocab_size=vocab_size,
@@ -777,15 +769,14 @@
         positional_dropout_rate: float = 0.1,
         input_layer: str = "embed",
         use_asr_output_layer: bool = True,
         use_spk_output_layer: bool = True,
         pos_enc_class=PositionalEncoding,
         normalize_before: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
         attention_dim = encoder_output_size
 
         if input_layer == "embed":
             self.embed = torch.nn.Sequential(
                 torch.nn.Embedding(vocab_size, attention_dim),
                 pos_enc_class(attention_dim, positional_dropout_rate),
@@ -951,15 +942,14 @@
         input_layer: str = "embed",
         use_asr_output_layer: bool = True,
         use_spk_output_layer: bool = True,
         pos_enc_class=PositionalEncoding,
         normalize_before: bool = True,
         concat_after: bool = False,
     ):
-        assert check_argument_types()
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             spker_embedding_dim=spker_embedding_dim,
             dropout_rate=dropout_rate,
             positional_dropout_rate=positional_dropout_rate,
             input_layer=input_layer,
```

### Comparing `funasr-0.6.6/funasr/models/e2e_asr.py` & `funasr-0.6.7/funasr/models/e2e_asr.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.losses.label_smoothing_loss import (
     LabelSmoothingLoss,  # noqa: H301
 )
 from funasr.models.ctc import CTC
 from funasr.models.decoder.abs_decoder import AbsDecoder
@@ -61,15 +60,14 @@
             report_wer: bool = True,
             sym_space: str = "<space>",
             sym_blank: str = "<blank>",
             extract_feats_in_collect_stats: bool = True,
             preencoder: Optional[AbsPreEncoder] = None,
             postencoder: Optional[AbsPostEncoder] = None,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.blank_id = 0
         self.sos = 1
```

### Comparing `funasr-0.6.6/funasr/models/e2e_asr_common.py` & `funasr-0.6.7/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.6.7/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 import numpy as np
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.models.ctc import CTC
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
@@ -69,15 +68,14 @@
         use_decoder_embedding: bool = False,
         crit_attn_weight: float = 0.0,
         crit_attn_smooth: float = 0.0,
         bias_encoder_dropout_rate: float = 0.0,
         preencoder: Optional[AbsPreEncoder] = None,
         postencoder: Optional[AbsPostEncoder] = None,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
         vocab_size=vocab_size,
         token_list=token_list,
         frontend=frontend,
```

### Comparing `funasr-0.6.6/funasr/models/e2e_asr_mfcca.py` & `funasr-0.6.7/funasr/models/e2e_asr_mfcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 import logging
 import torch
-from typeguard import check_argument_types
 
 from funasr.modules.e2e_asr_common import ErrorCalculator
 from funasr.modules.nets_utils import th_accuracy
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.losses.label_smoothing_loss import (
     LabelSmoothingLoss,  # noqa: H301
 )
@@ -61,15 +60,14 @@
             length_normalized_loss: bool = False,
             report_cer: bool = True,
             report_wer: bool = True,
             sym_space: str = "<space>",
             sym_blank: str = "<blank>",
             preencoder: Optional[AbsPreEncoder] = None,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert rnnt_decoder is None, "Not implemented"
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.sos = vocab_size - 1
         self.eos = vocab_size - 1
```

### Comparing `funasr-0.6.6/funasr/models/e2e_asr_paraformer.py` & `funasr-0.6.7/funasr/models/e2e_asr_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
 import random
 import numpy as np
-from typeguard import check_argument_types
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.losses.label_smoothing_loss import (
     LabelSmoothingLoss,  # noqa: H301
 )
 from funasr.models.ctc import CTC
 from funasr.models.decoder.abs_decoder import AbsDecoder
@@ -76,15 +75,14 @@
             predictor_bias: int = 0,
             sampling_ratio: float = 0.2,
             share_embedding: bool = False,
             preencoder: Optional[AbsPreEncoder] = None,
             postencoder: Optional[AbsPostEncoder] = None,
             use_1st_decoder_loss: bool = False,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.blank_id = blank_id
         self.sos = vocab_size - 1 if sos is None else sos
@@ -641,15 +639,14 @@
             sampling_ratio: float = 0.2,
             decoder_attention_chunk_type: str = 'chunk',
             share_embedding: bool = False,
             preencoder: Optional[AbsPreEncoder] = None,
             postencoder: Optional[AbsPostEncoder] = None,
             use_1st_decoder_loss: bool = False,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
             token_list=token_list,
             frontend=frontend,
@@ -1251,15 +1248,14 @@
             sampling_ratio: float = 0.2,
             embeds_id: int = 2,
             embeds_loss_weight: float = 0.0,
             embed_dims: int = 768,
             preencoder: Optional[AbsPreEncoder] = None,
             postencoder: Optional[AbsPostEncoder] = None,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
             token_list=token_list,
             frontend=frontend,
@@ -1524,15 +1520,14 @@
             predictor=None,
             predictor_weight: float = 0.0,
             predictor_bias: int = 0,
             sampling_ratio: float = 0.2,
             preencoder: Optional[AbsPreEncoder] = None,
             postencoder: Optional[AbsPostEncoder] = None,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
             token_list=token_list,
             frontend=frontend,
@@ -1802,15 +1797,14 @@
             inner_dim: int = 256,
             bias_encoder_type: str = 'lstm',
             label_bracket: bool = False,
             use_decoder_embedding: bool = False,
             preencoder: Optional[AbsPreEncoder] = None,
             postencoder: Optional[AbsPostEncoder] = None,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
             token_list=token_list,
             frontend=frontend,
```

### Comparing `funasr-0.6.6/funasr/models/e2e_asr_transducer.py` & `funasr-0.6.7/funasr/models/e2e_asr_transducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 
 import logging
 from contextlib import contextmanager
 from typing import Dict, List, Optional, Tuple, Union
 
 import torch
 from packaging.version import parse as V
-from typeguard import check_argument_types
-
+from funasr.losses.label_smoothing_loss import (
+    LabelSmoothingLoss,  # noqa: H301
+)
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.decoder.abs_decoder import AbsDecoder as AbsAttDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.modules.nets_utils import get_transducer_task_io
+from funasr.modules.nets_utils import th_accuracy
+from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.models.base_model import FunASRModel
 
 if V(torch.__version__) >= V("1.6.0"):
     from torch.cuda.amp import autocast
 else:
@@ -78,16 +81,14 @@
         report_cer: bool = True,
         report_wer: bool = True,
         extract_feats_in_collect_stats: bool = True,
     ) -> None:
         """Construct an ESPnetASRTransducerModel object."""
         super().__init__()
 
-        assert check_argument_types()
-
         # The following labels ID are reserved: 0 (blank) and vocab_size - 1 (sos/eos)
         self.blank_id = 0
         self.vocab_size = vocab_size
         self.ignore_id = ignore_id
         self.token_list = token_list.copy()
 
         self.sym_space = sym_space
@@ -538,16 +539,14 @@
         extract_feats_in_collect_stats: bool = True,
         lsm_weight: float = 0.0,
         length_normalized_loss: bool = False,
     ) -> None:
         """Construct an ESPnetASRTransducerModel object."""
         super().__init__()
 
-        assert check_argument_types()
-
         # The following labels ID are reserved: 0 (blank) and vocab_size - 1 (sos/eos)
         self.blank_id = 0
 
         if sym_sos in token_list:
             self.sos = token_list.index(sym_sos)
         else:
             self.sos = vocab_size - 1
@@ -705,15 +704,15 @@
                 u_len,
             )
 
         if self.use_auxiliary_lm_loss:
             loss_lm = self._calc_lm_loss(decoder_out, target)
 
         loss_trans = loss_trans_utt + loss_trans_chunk
-        loss_ctc = loss_ctc + loss_ctc_chunk 
+        loss_ctc = loss_ctc + loss_ctc_chunk
         loss_ctc = loss_att + loss_att_chunk
 
         loss = (
             self.transducer_weight * loss_trans
             + self.auxiliary_ctc_weight * loss_ctc
             + self.auxiliary_att_weight * loss_att
             + self.auxiliary_lm_loss_weight * loss_lm
@@ -1010,8 +1009,8 @@
         loss_att = self.criterion_att(decoder_out, ys_out_pad)
         acc_att = th_accuracy(
             decoder_out.view(-1, self.vocab_size),
             ys_out_pad,
             ignore_label=self.ignore_id,
         )
 
-        return loss_att, acc_att
+        return loss_att, acc_att
```

### Comparing `funasr-0.6.6/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.6.7/funasr/models/e2e_diar_eend_ola.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from distutils.version import LooseVersion
 from typing import Dict
 from typing import Tuple
 
 import numpy as np
 import torch
 import torch.nn as  nn
-from typeguard import check_argument_types
 
 from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
 from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
 from funasr.modules.eend_ola.utils.power import generate_mapping_dict
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.models.base_model import FunASRModel
@@ -44,15 +43,14 @@
             encoder_decoder_attractor: EncoderDecoderAttractor,
             n_units: int = 256,
             max_n_speaker: int = 8,
             attractor_loss_weight: float = 1.0,
             mapping_dict=None,
             **kwargs,
     ):
-        assert check_argument_types()
 
         super().__init__()
         self.frontend = frontend
         self.enc = encoder
         self.eda = encoder_decoder_attractor
         self.attractor_loss_weight = attractor_loss_weight
         self.max_n_speaker = max_n_speaker
```

### Comparing `funasr-0.6.6/funasr/models/e2e_diar_sond.py` & `funasr-0.6.7/funasr/models/e2e_diar_sond.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import Dict
 from typing import Optional
 from typing import Tuple, List
 
 import numpy as np
 import torch
 from torch.nn import functional as F
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import to_device
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.specaug.abs_specaug import AbsSpecAug
@@ -62,15 +61,14 @@
         label_aggregator: Optional[torch.nn.Module] = None,
         normalize_speech_speaker: bool = False,
         ignore_id: int = -1,
         speaker_discrimination_loss_weight: float = 1.0,
         inter_score_loss_weight: float = 0.0,
         inputs_type: str = "raw",
     ):
-        assert check_argument_types()
 
         super().__init__()
 
         self.encoder = encoder
         self.speaker_encoder = speaker_encoder
         self.ci_scorer = ci_scorer
         self.cd_scorer = cd_scorer
```

### Comparing `funasr-0.6.6/funasr/models/e2e_sa_asr.py` & `funasr-0.6.7/funasr/models/e2e_sa_asr.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
 import torch.nn.functional as F
-from typeguard import check_argument_types
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.losses.label_smoothing_loss import (
     LabelSmoothingLoss, NllLoss  # noqa: H301
 )
 from funasr.models.ctc import CTC
 from funasr.models.decoder.abs_decoder import AbsDecoder
@@ -63,15 +62,14 @@
             length_normalized_loss: bool = False,
             report_cer: bool = True,
             report_wer: bool = True,
             sym_space: str = "<space>",
             sym_blank: str = "<blank>",
             extract_feats_in_collect_stats: bool = True,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.blank_id = 0
         self.sos = 1
```

### Comparing `funasr-0.6.6/funasr/models/e2e_sv.py` & `funasr-0.6.7/funasr/models/e2e_sv.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.losses.label_smoothing_loss import (
     LabelSmoothingLoss,  # noqa: H301
 )
 from funasr.models.ctc import CTC
 from funasr.models.decoder.abs_decoder import AbsDecoder
@@ -52,15 +51,14 @@
             normalize: Optional[AbsNormalize],
             preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
             postencoder: Optional[AbsPostEncoder],
             pooling_layer: torch.nn.Module,
             decoder: AbsDecoder,
     ):
-        assert check_argument_types()
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.vocab_size = vocab_size
         self.token_list = token_list.copy()
 
         self.frontend = frontend
```

### Comparing `funasr-0.6.6/funasr/models/e2e_tp.py` & `funasr-0.6.7/funasr/models/e2e_tp.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
 import numpy as np
-from typeguard import check_argument_types
 
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.predictor.cif import mae_loss
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.modules.nets_utils import make_pad_mask, pad_list
 from funasr.torch_utils.device_funcs import force_gatherable
@@ -38,15 +37,14 @@
             self,
             frontend: Optional[AbsFrontend],
             encoder: AbsEncoder,
             predictor: CifPredictorV3,
             predictor_bias: int = 0,
             token_list=None,
     ):
-        assert check_argument_types()
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
 
         self.frontend = frontend
         self.encoder = encoder
         self.encoder.interctc_use_conditioning = False
```

### Comparing `funasr-0.6.6/funasr/models/e2e_uni_asr.py` & `funasr-0.6.7/funasr/models/e2e_uni_asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
-from typeguard import check_argument_types
 
 from funasr.models.e2e_asr_common import ErrorCalculator
 from funasr.modules.nets_utils import th_accuracy
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.losses.label_smoothing_loss import (
     LabelSmoothingLoss,  # noqa: H301
 )
@@ -78,15 +77,14 @@
         loss_weight_model1: float = 0.5,
         enable_maas_finetune: bool = False,
         freeze_encoder2: bool = False,
         preencoder: Optional[AbsPreEncoder] = None,
         postencoder: Optional[AbsPostEncoder] = None,
         encoder1_encoder2_joint_training: bool = True,
     ):
-        assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
         self.blank_id = 0
         self.sos = 1
         self.eos = 2
```

### Comparing `funasr-0.6.6/funasr/models/e2e_vad.py` & `funasr-0.6.7/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/encoder/conformer_encoder.py` & `funasr-0.6.7/funasr/models/encoder/conformer_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import Dict
 
 import torch
 from torch import nn
-from typeguard import check_argument_types
 
 from funasr.models.ctc import CTC
 from funasr.modules.attention import (
     MultiHeadedAttention,  # noqa: H301
     RelPositionMultiHeadedAttention,  # noqa: H301
     RelPositionMultiHeadedAttentionChunk,
     LegacyRelPositionMultiHeadedAttention,  # noqa: H301
@@ -529,15 +528,14 @@
             zero_triu: bool = False,
             cnn_module_kernel: int = 31,
             padding_idx: int = -1,
             interctc_layer_idx: List[int] = [],
             interctc_use_conditioning: bool = False,
             stochastic_depth_rate: Union[float, List[float]] = 0.0,
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if rel_pos_type == "legacy":
             if pos_enc_layer_type == "rel_pos":
                 pos_enc_layer_type = "legacy_rel_pos"
             if selfattention_layer_type == "rel_selfattn":
@@ -939,15 +937,14 @@
         default_chunk_size: int = 16,
         jitter_range: int = 4,
         subsampling_factor: int = 1,
     ) -> None:
         """Construct an Encoder object."""
         super().__init__()
 
-        assert check_argument_types()
 
         self.embed = StreamingConvInput(
             input_size,
             output_size,
             subsampling_factor,
             vgg_like=embed_vgg_like,
             output_size=output_size,
```

### Comparing `funasr-0.6.6/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.6.7/funasr/models/encoder/data2vec_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import math
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
-from typeguard import check_argument_types
 
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.modules.data2vec.data_utils import compute_mask_indices
 from funasr.modules.data2vec.ema_module import EMAModule
 from funasr.modules.data2vec.grad_multiply import GradMultiply
 from funasr.modules.data2vec.wav2vec2 import (
     ConvFeatureExtractionModel,
@@ -93,15 +92,14 @@
             min_pred_var: float = 0.01,
             # Loss
             loss_beta: float = 0.0,
             loss_scale: float = None,
             # FP16 optimization
             required_seq_len_multiple: int = 2,
     ):
-        assert check_argument_types()
         super().__init__()
 
         # ConvFeatureExtractionModel
         self.conv_feature_layers = conv_feature_layers
         feature_enc_layers = eval(conv_feature_layers)
         self.extractor_embed = feature_enc_layers[-1][0]
         self.feature_extractor = ConvFeatureExtractionModel(
```

### Comparing `funasr-0.6.6/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.6.7/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.6.7/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.6.7/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.6.7/funasr/models/encoder/mfcca_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 from typing import Tuple
 
 import logging
 import torch
 from torch import nn
 
-from typeguard import check_argument_types
 
 from funasr.models.encoder.encoder_layer_mfcca import EncoderLayer
 from funasr.modules.nets_utils import get_activation
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.attention import (
     MultiHeadedAttention,  # noqa: H301
     RelPositionMultiHeadedAttention,  # noqa: H301
@@ -157,15 +156,14 @@
             selfattention_layer_type: str = "rel_selfattn",
             activation_type: str = "swish",
             use_cnn_module: bool = True,
             zero_triu: bool = False,
             cnn_module_kernel: int = 31,
             padding_idx: int = -1,
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if rel_pos_type == "legacy":
             if pos_enc_layer_type == "rel_pos":
                 pos_enc_layer_type = "legacy_rel_pos"
             if selfattention_layer_type == "rel_selfattn":
```

### Comparing `funasr-0.6.6/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 import logging
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
-from typeguard import check_argument_types
 import numpy as np
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.layer_norm import LayerNorm
 from funasr.models.encoder.abs_encoder import AbsEncoder
 import math
 from funasr.modules.repeat import repeat
 
@@ -86,15 +85,14 @@
             out_residual=False,
             include_batchnorm=False,
             regularization_weight=0.0,
             stride=1,
             tf2torch_tensor_name_prefix_torch: str = "speaker_encoder",
             tf2torch_tensor_name_prefix_tf: str = "EAND/speaker_encoder",
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = num_units
 
         self.num_layers = num_layers
         self.input_units = input_units
         self.num_units = num_units
         self.kernel_size = kernel_size
```

### Comparing `funasr-0.6.6/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 import logging
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
-from typeguard import check_argument_types
 import numpy as np
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.layer_norm import LayerNorm
 from funasr.models.encoder.abs_encoder import AbsEncoder
 import math
 from funasr.modules.repeat import repeat
 from funasr.modules.multi_layer_conv import FsmnFeedForward
```

### Comparing `funasr-0.6.6/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 import logging
 import torch
 import torch.nn as nn
 from funasr.modules.streaming_utils.chunk_utilis import overlap_chunk
-from typeguard import check_argument_types
 import numpy as np
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.attention import MultiHeadSelfAttention, MultiHeadedAttentionSANM
 from funasr.modules.embedding import SinusoidalPositionEncoder
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.multi_layer_conv import Conv1dLinear
 from funasr.modules.multi_layer_conv import MultiLayeredConv1d
@@ -140,15 +139,14 @@
         padding_idx: int = -1,
         interctc_layer_idx: List[int] = [],
         interctc_use_conditioning: bool = False,
         tf2torch_tensor_name_prefix_torch: str = "encoder",
         tf2torch_tensor_name_prefix_tf: str = "seq2seq/encoder",
         out_units=None,
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
```

### Comparing `funasr-0.6.6/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.6.7/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/encoder/rnn_encoder.py` & `funasr-0.6.7/funasr/models/encoder/rnn_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.rnn.encoders import RNN
 from funasr.modules.rnn.encoders import RNNP
 from funasr.models.encoder.abs_encoder import AbsEncoder
 
 
@@ -33,15 +32,14 @@
         use_projection: bool = True,
         num_layers: int = 4,
         hidden_size: int = 320,
         output_size: int = 320,
         dropout: float = 0.0,
         subsample: Optional[Sequence[int]] = (2, 2, 1, 1),
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
         self.rnn_type = rnn_type
         self.bidirectional = bidirectional
         self.use_projection = use_projection
 
         if rnn_type not in {"lstm", "gru"}:
```

### Comparing `funasr-0.6.6/funasr/models/encoder/sanm_encoder.py` & `funasr-0.6.7/funasr/models/encoder/sanm_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Tuple
 from typing import Union
 import logging
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from funasr.modules.streaming_utils.chunk_utilis import overlap_chunk
-from typeguard import check_argument_types
 import numpy as np
 from funasr.torch_utils.device_funcs import to_device
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.attention import MultiHeadedAttention, MultiHeadedAttentionSANM, MultiHeadedAttentionSANMwithMask
 from funasr.modules.embedding import SinusoidalPositionEncoder, StreamSinusoidalPositionEncoder
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.multi_layer_conv import Conv1dLinear
@@ -147,15 +146,14 @@
         interctc_use_conditioning: bool = False,
         kernel_size : int = 11,
         sanm_shfit : int = 0,
         selfattention_layer_type: str = "sanm",
         tf2torch_tensor_name_prefix_torch: str = "encoder",
         tf2torch_tensor_name_prefix_tf: str = "seq2seq/encoder",
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
@@ -597,15 +595,14 @@
             stride: Union[int, Sequence[int]] = (10,),
             pad_left: Union[int, Sequence[int]] = (0,),
             encoder_att_look_back_factor: Union[int, Sequence[int]] = (1,),
             decoder_att_look_back_factor: Union[int, Sequence[int]] = (1,),
             tf2torch_tensor_name_prefix_torch: str = "encoder",
             tf2torch_tensor_name_prefix_tf: str = "seq2seq/encoder",
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
@@ -1056,15 +1053,14 @@
         padding_idx: int = -1,
         interctc_layer_idx: List[int] = [],
         interctc_use_conditioning: bool = False,
         kernel_size : int = 11,
         sanm_shfit : int = 0,
         selfattention_layer_type: str = "sanm",
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
```

### Comparing `funasr-0.6.6/funasr/models/encoder/transformer_encoder.py` & `funasr-0.6.7/funasr/models/encoder/transformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import torch
 from torch import nn
-from typeguard import check_argument_types
 import logging
 
 from funasr.models.ctc import CTC
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.modules.attention import MultiHeadedAttention
 from funasr.modules.embedding import PositionalEncoding
 from funasr.modules.layer_norm import LayerNorm
@@ -185,15 +184,14 @@
             concat_after: bool = False,
             positionwise_layer_type: str = "linear",
             positionwise_conv_kernel_size: int = 1,
             padding_idx: int = -1,
             interctc_layer_idx: List[int] = [],
             interctc_use_conditioning: bool = False,
     ):
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
```

### Comparing `funasr-0.6.6/funasr/models/frontend/default.py` & `funasr-0.6.7/funasr/models/frontend/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Tuple
 from typing import Union
 import logging
 import humanfriendly
 import numpy as np
 import torch
 from torch_complex.tensor import ComplexTensor
-from typeguard import check_argument_types
 
 from funasr.layers.log_mel import LogMel
 from funasr.layers.stft import Stft
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.modules.frontends.frontend import Frontend
 from funasr.utils.get_default_kwargs import get_default_kwargs
 from funasr.modules.nets_utils import make_pad_mask
@@ -36,15 +35,14 @@
             fmin: int = None,
             fmax: int = None,
             htk: bool = False,
             frontend_conf: Optional[dict] = get_default_kwargs(Frontend),
             apply_stft: bool = True,
             use_channel: int = None,
     ):
-        assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
 
         # Deepcopy (In general, dict shouldn't be used as default arg)
         frontend_conf = copy.deepcopy(frontend_conf)
         self.hop_length = hop_length
@@ -163,15 +161,14 @@
             apply_stft: bool = True,
             use_channel: int = None,
             lfr_m: int = 1,
             lfr_n: int = 1,
             cmvn_file: str = None,
             mc: bool = True
     ):
-        assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
 
         # Deepcopy (In general, dict shouldn't be used as default arg)
         frontend_conf = copy.deepcopy(frontend_conf)
         if win_length is None and hop_length is None:
```

### Comparing `funasr-0.6.6/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.6.7/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/frontend/fused.py` & `funasr-0.6.7/funasr/models/frontend/fused.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.s3prl import S3prlFrontend
 import numpy as np
 import torch
-from typeguard import check_argument_types
 from typing import Tuple
 
 
 class FusedFrontends(AbsFrontend):
     def __init__(
         self, frontends=None, align_method="linear_projection", proj_dim=100, fs=16000
     ):
 
-        assert check_argument_types()
         super().__init__()
         self.align_method = (
             align_method  # fusing method : linear_projection only for now
         )
         self.proj_dim = proj_dim  # dim of the projection done on each frontend
         self.frontends = []  # list of the frontends to combine
```

### Comparing `funasr-0.6.6/funasr/models/frontend/s3prl.py` & `funasr-0.6.7/funasr/models/frontend/s3prl.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from argparse import Namespace
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import humanfriendly
 import torch
-from typeguard import check_argument_types
 
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.modules.frontends.frontend import Frontend
 from funasr.modules.nets_utils import pad_list
 from funasr.utils.get_default_kwargs import get_default_kwargs
 
 
@@ -33,15 +32,14 @@
     def __init__(
             self,
             fs: Union[int, str] = 16000,
             frontend_conf: Optional[dict] = get_default_kwargs(Frontend),
             download_dir: str = None,
             multilayer_feature: bool = False,
     ):
-        assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
 
         if download_dir is not None:
             torch.hub.set_dir(download_dir)
```

### Comparing `funasr-0.6.6/funasr/models/frontend/wav_frontend.py` & `funasr-0.6.7/funasr/models/frontend/wav_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Part of the implementation is borrowed from espnet/espnet.
 from typing import Tuple
 
 import numpy as np
 import torch
 import torchaudio.compliance.kaldi as kaldi
 from torch.nn.utils.rnn import pad_sequence
-from typeguard import check_argument_types
 
 import funasr.models.frontend.eend_ola_feature as eend_ola_feature
 from funasr.models.frontend.abs_frontend import AbsFrontend
 
 
 def load_cmvn(cmvn_file):
     with open(cmvn_file, 'r', encoding='utf-8') as f:
@@ -91,15 +90,14 @@
             filter_length_max: int = -1,
             lfr_m: int = 1,
             lfr_n: int = 1,
             dither: float = 1.0,
             snip_edges: bool = True,
             upsacle_samples: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
         self.fs = fs
         self.window = window
         self.n_mels = n_mels
         self.frame_length = frame_length
         self.frame_shift = frame_shift
         self.filter_length_min = filter_length_min
@@ -223,15 +221,14 @@
             filter_length_max: int = -1,
             lfr_m: int = 1,
             lfr_n: int = 1,
             dither: float = 1.0,
             snip_edges: bool = True,
             upsacle_samples: bool = True,
     ):
-        assert check_argument_types()
         super().__init__()
         self.fs = fs
         self.window = window
         self.n_mels = n_mels
         self.frame_length = frame_length
         self.frame_shift = frame_shift
         self.frame_sample_length = int(self.frame_length * self.fs / 1000)
@@ -462,15 +459,14 @@
             self,
             fs: int = 16000,
             frame_length: int = 25,
             frame_shift: int = 10,
             lfr_m: int = 1,
             lfr_n: int = 1,
     ):
-        assert check_argument_types()
         super().__init__()
         self.fs = fs
         self.frame_length = frame_length
         self.frame_shift = frame_shift
         self.lfr_m = lfr_m
         self.lfr_n = lfr_n
         self.n_mels = 23
```

### Comparing `funasr-0.6.6/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.6.7/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/frontend/windowing.py` & `funasr-0.6.7/funasr/models/frontend/windowing.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #  2020, Technische Universität München;  Ludwig Kürzinger
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 """Sliding Window for raw audio input data."""
 
 from funasr.models.frontend.abs_frontend import AbsFrontend
 import torch
-from typeguard import check_argument_types
 from typing import Tuple
 
 
 class SlidingWindow(AbsFrontend):
     """Sliding Window.
     Provides a sliding window over a batched continuous raw audio tensor.
     Optionally, provides padding (Currently not implemented).
@@ -34,15 +33,14 @@
         Args:
             win_length: Length of frame.
             hop_length: Relative starting point of next frame.
             channels: Number of input channels.
             padding: Padding (placeholder, currently not implemented).
             fs:  Sampling rate (placeholder for compatibility, not used).
         """
-        assert check_argument_types()
         super().__init__()
         self.fs = fs
         self.win_length = win_length
         self.hop_length = hop_length
         self.channels = channels
         self.padding = padding
```

### Comparing `funasr-0.6.6/funasr/models/joint_net/joint_network.py` & `funasr-0.6.7/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/pooling/statistic_pooling.py` & `funasr-0.6.7/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.6.7/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #  2021, University of Stuttgart;  Pavel Denisov
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 """Hugging Face Transformers PostEncoder."""
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
-from typeguard import check_argument_types
 from typing import Tuple
 
 import copy
 import logging
 import torch
 
 try:
@@ -26,15 +25,14 @@
 
     def __init__(
         self,
         input_size: int,
         model_name_or_path: str,
     ):
         """Initialize the module."""
-        assert check_argument_types()
         super().__init__()
 
         if not is_transformers_available:
             raise ImportError(
                 "`transformers` is not available. Please install it via `pip install"
                 " transformers` or `cd /path/to/espnet/tools && . ./activate_python.sh"
                 " && ./installers/install_transformers.sh`."
```

### Comparing `funasr-0.6.6/funasr/models/predictor/cif.py` & `funasr-0.6.7/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/preencoder/linear.py` & `funasr-0.6.7/funasr/models/preencoder/linear.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python3
 #  2021, Carnegie Mellon University;  Xuankai Chang
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 """Linear Projection."""
 
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
-from typeguard import check_argument_types
 from typing import Tuple
 
 import torch
 
 
 class LinearProjection(AbsPreEncoder):
     """Linear Projection Preencoder."""
 
     def __init__(
         self,
         input_size: int,
         output_size: int,
     ):
         """Initialize the module."""
-        assert check_argument_types()
         super().__init__()
 
         self.output_dim = output_size
         self.linear_out = torch.nn.Linear(input_size, output_size)
 
     def forward(
         self, input: torch.Tensor, input_lengths: torch.Tensor
```

### Comparing `funasr-0.6.6/funasr/models/preencoder/sinc.py` & `funasr-0.6.7/funasr/models/preencoder/sinc.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from collections import OrderedDict
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.layers.sinc_conv import LogCompression
 from funasr.layers.sinc_conv import SincConv
 import humanfriendly
 import torch
-from typeguard import check_argument_types
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 
 class LightweightSincConvs(AbsPreEncoder):
     """Lightweight Sinc Convolutions.
@@ -56,15 +55,14 @@
             in_channels: Number of input channels.
             out_channels: Number of output channels (for each input channel).
             activation_type: Choice of activation function.
             dropout_type: Choice of dropout function.
             windowing_type: Choice of windowing function.
             scale_type:  Choice of filter-bank initialization scale.
         """
-        assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
         self.fs = fs
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.activation_type = activation_type
@@ -264,15 +262,14 @@
     ):
         """Initialize.
 
         Args:
             dropout_probability: Dropout probability.
             shape (tuple, list): Shape of input tensors.
         """
-        assert check_argument_types()
         super().__init__()
         if shape is None:
             shape = (0, 2, 1)
         self.dropout = torch.nn.Dropout2d(dropout_probability)
         self.shape = (shape,)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
```

### Comparing `funasr-0.6.6/funasr/models/seq_rnn_lm.py` & `funasr-0.6.7/funasr/models/seq_rnn_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Sequential implementation of Recurrent Neural Network Language Model."""
 from typing import Tuple
 from typing import Union
 
 import torch
 import torch.nn as nn
-from typeguard import check_argument_types
 from funasr.train.abs_model import AbsLM
 
 
 class SequentialRNNLM(AbsLM):
     """Sequential RNNLM.
 
     See also:
@@ -23,15 +22,14 @@
         nhid: int = None,
         nlayers: int = 2,
         dropout_rate: float = 0.0,
         tie_weights: bool = False,
         rnn_type: str = "lstm",
         ignore_id: int = 0,
     ):
-        assert check_argument_types()
         super().__init__()
 
         ninp = unit
         if nhid is None:
             nhid = unit
         rnn_type = rnn_type.upper()
```

### Comparing `funasr-0.6.6/funasr/models/specaug/specaug.py` & `funasr-0.6.7/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/target_delay_transformer.py` & `funasr-0.6.7/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/transformer_lm.py` & `funasr-0.6.7/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/models/vad_realtime_transformer.py` & `funasr-0.6.7/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/add_sos_eos.py` & `funasr-0.6.7/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/attention.py` & `funasr-0.6.7/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.6.7/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.6.7/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/beam_search/beam_search.py` & `funasr-0.6.7/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.6.7/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.6.7/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/data2vec/data_utils.py` & `funasr-0.6.7/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/data2vec/ema_module.py` & `funasr-0.6.7/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.6.7/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/data2vec/quant_noise.py` & `funasr-0.6.7/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/data2vec/utils.py` & `funasr-0.6.7/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.6.7/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/dynamic_conv.py` & `funasr-0.6.7/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/dynamic_conv2d.py` & `funasr-0.6.7/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/e2e_asr_common.py` & `funasr-0.6.7/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/eend_ola/encoder.py` & `funasr-0.6.7/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.6.7/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/eend_ola/utils/losses.py` & `funasr-0.6.7/funasr/modules/eend_ola/utils/losses.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/eend_ola/utils/power.py` & `funasr-0.6.7/funasr/modules/eend_ola/utils/power.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/eend_ola/utils/report.py` & `funasr-0.6.7/funasr/modules/eend_ola/utils/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import numpy as np
 import time
 import torch
-from eend.utils.power import create_powerlabel
+from funasr.modules.eend_ola.utils.power import create_powerlabel
 from itertools import combinations
 
 metrics = [
     ('diarization_error', 'speaker_scored', 'DER'),
     ('speech_miss', 'speech_scored', 'SAD_MR'),
     ('speech_falarm', 'speech_scored', 'SAD_FR'),
     ('speaker_miss', 'speaker_scored', 'MI'),
```

### Comparing `funasr-0.6.6/funasr/modules/embedding.py` & `funasr-0.6.7/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/frontends/beamformer.py` & `funasr-0.6.7/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.6.7/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.6.7/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/frontends/feature_transform.py` & `funasr-0.6.7/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/frontends/frontend.py` & `funasr-0.6.7/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/frontends/mask_estimator.py` & `funasr-0.6.7/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/layer_norm.py` & `funasr-0.6.7/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/lightconv.py` & `funasr-0.6.7/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/lightconv2d.py` & `funasr-0.6.7/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/mask.py` & `funasr-0.6.7/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/multi_layer_conv.py` & `funasr-0.6.7/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/nets_utils.py` & `funasr-0.6.7/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/positionwise_feed_forward.py` & `funasr-0.6.7/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/repeat.py` & `funasr-0.6.7/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/rnn/argument.py` & `funasr-0.6.7/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/rnn/attentions.py` & `funasr-0.6.7/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/rnn/decoders.py` & `funasr-0.6.7/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/rnn/encoders.py` & `funasr-0.6.7/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/scorers/ctc.py` & `funasr-0.6.7/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.6.7/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/scorers/length_bonus.py` & `funasr-0.6.7/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/scorers/scorer_interface.py` & `funasr-0.6.7/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.6.7/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.6.7/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/streaming_utils/utils.py` & `funasr-0.6.7/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/subsampling.py` & `funasr-0.6.7/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/modules/subsampling_without_posenc.py` & `funasr-0.6.7/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/optimizers/fairseq_adam.py` & `funasr-0.6.7/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/optimizers/sgd.py` & `funasr-0.6.7/funasr/optimizers/sgd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import torch
-from typeguard import check_argument_types
 
 
 class SGD(torch.optim.SGD):
     """Thin inheritance of torch.optim.SGD to bind the required arguments, 'lr'
 
     Note that
     the arguments of the optimizer invoked by AbsTask.main()
@@ -17,15 +16,14 @@
         params,
         lr: float = 0.1,
         momentum: float = 0.0,
         dampening: float = 0.0,
         weight_decay: float = 0.0,
         nesterov: bool = False,
     ):
-        assert check_argument_types()
         super().__init__(
             params,
             lr=lr,
             momentum=momentum,
             dampening=dampening,
             weight_decay=weight_decay,
             nesterov=nesterov,
```

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/demo.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- encoding: utf-8 -*-
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
 import numpy as np
-from typeguard import check_argument_types
 import kaldi_native_fbank as knf
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
@@ -24,15 +23,14 @@
             frame_length: int = 25,
             frame_shift: int = 10,
             lfr_m: int = 1,
             lfr_n: int = 1,
             dither: float = 1.0,
             **kwargs,
     ) -> None:
-        check_argument_types()
 
         opts = knf.FbankOptions()
         opts.frame_opts.samp_freq = fs
         opts.frame_opts.dither = dither
         opts.frame_opts.window_type = window
         opts.frame_opts.frame_shift_ms = float(frame_shift)
         opts.frame_opts.frame_length_ms = float(frame_length)
```

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 import pickle
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
 import numpy as np
 import yaml
 
-from typeguard import check_argument_types
 
 import warnings
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
 class TokenIDConverter():
     def __init__(self, token_list: Union[List, str],
                  ):
-        check_argument_types()
 
         self.token_list = token_list
         self.unk_symbol = token_list[-1]
         self.token2id = {v: i for i, v in enumerate(self.token_list)}
         self.unk_id = self.token2id[self.unk_symbol]
 
 
@@ -47,15 +45,14 @@
 class CharTokenizer():
     def __init__(
         self,
         symbol_value: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
         remove_non_linguistic_symbols: bool = False,
     ):
-        check_argument_types()
 
         self.space_symbol = space_symbol
         self.non_linguistic_symbols = self.load_symbols(symbol_value)
         self.remove_non_linguistic_symbols = remove_non_linguistic_symbols
 
     @staticmethod
     def load_symbols(value: Union[Path, str, Iterable[str]] = None) -> Set:
```

### Comparing `funasr-0.6.6/funasr/runtime/python/libtorch/setup.py` & `funasr-0.6.7/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- encoding: utf-8 -*-
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 import copy
 
 import numpy as np
-from typeguard import check_argument_types
 import kaldi_native_fbank as knf
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
@@ -25,15 +24,14 @@
             frame_length: int = 25,
             frame_shift: int = 10,
             lfr_m: int = 1,
             lfr_n: int = 1,
             dither: float = 1.0,
             **kwargs,
     ) -> None:
-        check_argument_types()
 
         opts = knf.FbankOptions()
         opts.frame_opts.samp_freq = fs
         opts.frame_opts.dither = dither
         opts.frame_opts.window_type = window
         opts.frame_opts.frame_shift_ms = float(frame_shift)
         opts.frame_opts.frame_length_ms = float(frame_length)
```

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
 import numpy as np
 import yaml
 from onnxruntime import (GraphOptimizationLevel, InferenceSession,
                          SessionOptions, get_available_providers, get_device)
-from typeguard import check_argument_types
 
 import warnings
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
 class TokenIDConverter():
     def __init__(self, token_list: Union[List, str],
                  ):
-        check_argument_types()
 
         self.token_list = token_list
         self.unk_symbol = token_list[-1]
         self.token2id = {v: i for i, v in enumerate(self.token_list)}
         self.unk_id = self.token2id[self.unk_symbol]
 
 
@@ -48,15 +46,14 @@
 class CharTokenizer():
     def __init__(
         self,
         symbol_value: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
         remove_non_linguistic_symbols: bool = False,
     ):
-        check_argument_types()
 
         self.space_symbol = space_symbol
         self.non_linguistic_symbols = self.load_symbols(symbol_value)
         self.remove_non_linguistic_symbols = remove_non_linguistic_symbols
 
     @staticmethod
     def load_symbols(value: Union[Path, str, Iterable[str]] = None) -> Set:
```

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.6.7/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/samplers/build_batch_sampler.py` & `funasr-0.6.7/funasr/samplers/build_batch_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import List
 from typing import Dict
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.samplers.abs_sampler import AbsSampler
 from funasr.samplers.folded_batch_sampler import FoldedBatchSampler
 from funasr.samplers.length_batch_sampler import LengthBatchSampler
 from funasr.samplers.num_elements_batch_sampler import NumElementsBatchSampler
 from funasr.samplers.sorted_batch_sampler import SortedBatchSampler
 from funasr.samplers.unsorted_batch_sampler import UnsortedBatchSampler
@@ -100,15 +98,14 @@
         sort_batch:
         drop_last:
         min_batch_size:  Used for "numel" or "folded" mode
         fold_lengths: Used for "folded" mode
         padding: Whether sequences are input as a padded tensor or not.
             used for "numel" mode
     """
-    assert check_argument_types()
     if len(shape_files) == 0:
         raise ValueError("No shape file are given")
 
     if type == "unsorted":
         retval = UnsortedBatchSampler(
             batch_size=batch_size, key_file=shape_files[0], drop_last=drop_last
         )
@@ -160,9 +157,8 @@
             drop_last=drop_last,
             padding=padding,
             min_batch_size=min_batch_size,
         )
 
     else:
         raise ValueError(f"Not supported: {type}")
-    assert check_return_type(retval)
     return retval
```

### Comparing `funasr-0.6.6/funasr/samplers/folded_batch_sampler.py` & `funasr-0.6.7/funasr/samplers/folded_batch_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterator
 from typing import List
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import load_num_sequence_text
 from funasr.fileio.read_text import read_2column_text
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class FoldedBatchSampler(AbsSampler):
@@ -19,15 +18,14 @@
         fold_lengths: Sequence[int],
         min_batch_size: int = 1,
         sort_in_batch: str = "descending",
         sort_batch: str = "ascending",
         drop_last: bool = False,
         utt2category_file: str = None,
     ):
-        assert check_argument_types()
         assert batch_size > 0
         if sort_batch != "ascending" and sort_batch != "descending":
             raise ValueError(
                 f"sort_batch must be ascending or descending: {sort_batch}"
             )
         if sort_in_batch != "descending" and sort_in_batch != "ascending":
             raise ValueError(
```

### Comparing `funasr-0.6.6/funasr/samplers/length_batch_sampler.py` & `funasr-0.6.7/funasr/samplers/length_batch_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterator
 from typing import List
 from typing import Dict
 from typing import Tuple
 from typing import Union
 
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import load_num_sequence_text
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class LengthBatchSampler(AbsSampler):
     def __init__(
@@ -17,15 +16,14 @@
         shape_files: Union[Tuple[str, ...], List[str], Dict],
         min_batch_size: int = 1,
         sort_in_batch: str = "descending",
         sort_batch: str = "ascending",
         drop_last: bool = False,
         padding: bool = True,
     ):
-        assert check_argument_types()
         assert batch_bins > 0
         if sort_batch != "ascending" and sort_batch != "descending":
             raise ValueError(
                 f"sort_batch must be ascending or descending: {sort_batch}"
             )
         if sort_in_batch != "descending" and sort_in_batch != "ascending":
             raise ValueError(
```

### Comparing `funasr-0.6.6/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.6.7/funasr/samplers/num_elements_batch_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterator
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import numpy as np
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import load_num_sequence_text
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class NumElementsBatchSampler(AbsSampler):
     def __init__(
@@ -17,15 +16,14 @@
         shape_files: Union[Tuple[str, ...], List[str]],
         min_batch_size: int = 1,
         sort_in_batch: str = "descending",
         sort_batch: str = "ascending",
         drop_last: bool = False,
         padding: bool = True,
     ):
-        assert check_argument_types()
         assert batch_bins > 0
         if sort_batch != "ascending" and sort_batch != "descending":
             raise ValueError(
                 f"sort_batch must be ascending or descending: {sort_batch}"
             )
         if sort_in_batch != "descending" and sort_in_batch != "ascending":
             raise ValueError(
```

### Comparing `funasr-0.6.6/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.6.7/funasr/samplers/sorted_batch_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from typing import Iterator
 from typing import Tuple
 
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import load_num_sequence_text
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class SortedBatchSampler(AbsSampler):
     """BatchSampler with sorted samples by length.
@@ -22,15 +21,14 @@
         self,
         batch_size: int,
         shape_file: str,
         sort_in_batch: str = "descending",
         sort_batch: str = "ascending",
         drop_last: bool = False,
     ):
-        assert check_argument_types()
         assert batch_size > 0
         self.batch_size = batch_size
         self.shape_file = shape_file
         self.sort_in_batch = sort_in_batch
         self.sort_batch = sort_batch
         self.drop_last = drop_last
```

### Comparing `funasr-0.6.6/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.6.7/funasr/samplers/unsorted_batch_sampler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from typing import Iterator
 from typing import Tuple
 
-from typeguard import check_argument_types
 
 from funasr.fileio.read_text import read_2column_text
 from funasr.samplers.abs_sampler import AbsSampler
 
 
 class UnsortedBatchSampler(AbsSampler):
     """BatchSampler with constant batch-size.
@@ -24,15 +23,14 @@
     def __init__(
         self,
         batch_size: int,
         key_file: str,
         drop_last: bool = False,
         utt2category_file: str = None,
     ):
-        assert check_argument_types()
         assert batch_size > 0
         self.batch_size = batch_size
         self.key_file = key_file
         self.drop_last = drop_last
 
         # utt2shape:
         #    uttA <anything is o.k>
```

### Comparing `funasr-0.6.6/funasr/schedulers/abs_scheduler.py` & `funasr-0.6.7/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/schedulers/noam_lr.py` & `funasr-0.6.7/funasr/schedulers/noam_lr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Noam learning rate scheduler module."""
 from typing import Union
 import warnings
 
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
-from typeguard import check_argument_types
 
 from funasr.schedulers.abs_scheduler import AbsBatchStepScheduler
 
 
 class NoamLR(_LRScheduler, AbsBatchStepScheduler):
     """The LR scheduler proposed by Noam
 
@@ -27,15 +26,14 @@
     def __init__(
         self,
         optimizer: torch.optim.Optimizer,
         model_size: Union[int, float] = 320,
         warmup_steps: Union[int, float] = 25000,
         last_epoch: int = -1,
     ):
-        assert check_argument_types()
         self.model_size = model_size
         self.warmup_steps = warmup_steps
 
         lr = list(optimizer.param_groups)[0]["lr"]
         new_lr = self.lr_for_WarmupLR(lr)
         warnings.warn(
             f"NoamLR is deprecated. "
```

### Comparing `funasr-0.6.6/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.6.7/funasr/schedulers/tri_stage_scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 # LICENSE file in the root directory of this source tree.
 
 import math
 from typing import Optional, List
 
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
-from typeguard import check_argument_types
 
 from funasr.schedulers.abs_scheduler import AbsBatchStepScheduler
 
 
 class TriStageLR(_LRScheduler, AbsBatchStepScheduler):
     def __init__(
             self,
             optimizer: torch.optim.Optimizer,
             last_epoch: int = -1,
             phase_ratio: Optional[List[float]] = None,
             init_lr_scale: float = 0.01,
             final_lr_scale: float = 0.01,
     ):
-        assert check_argument_types()
         self.optimizer = optimizer
         self.last_epoch = last_epoch
         self.phase_ratio = phase_ratio
         self.init_lr_scale = init_lr_scale
         self.final_lr_scale = final_lr_scale
         self.optimizer_lr = self.optimizer.defaults["lr"]
```

### Comparing `funasr-0.6.6/funasr/schedulers/warmup_lr.py` & `funasr-0.6.7/funasr/schedulers/warmup_lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Warm up learning rate scheduler module."""
 from typing import Union
 
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
-from typeguard import check_argument_types
 
 from funasr.schedulers.abs_scheduler import AbsBatchStepScheduler
 
 
 class WarmupLR(_LRScheduler, AbsBatchStepScheduler):
     """The WarmupLR scheduler
 
@@ -26,15 +25,14 @@
 
     def __init__(
         self,
         optimizer: torch.optim.Optimizer,
         warmup_steps: Union[int, float] = 25000,
         last_epoch: int = -1,
     ):
-        assert check_argument_types()
         self.warmup_steps = warmup_steps
 
         # __init__() must be invoked before setting field
         # because step() is also invoked in __init__()
         super().__init__(optimizer, last_epoch)
 
     def __repr__(self):
```

### Comparing `funasr-0.6.6/funasr/tasks/abs_task.py` & `funasr-0.6.7/funasr/tasks/abs_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 import torch.distributed as dist
 import torch.multiprocessing
 import torch.nn
 import torch.optim
 import yaml
 from funasr.models.base_model import FunASRModel
 from torch.utils.data import DataLoader
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr import __version__
 from funasr.datasets.dataset import AbsDataset
 from funasr.datasets.dataset import DATA_TYPES
 from funasr.datasets.dataset import ESPnetDataset
 from funasr.datasets.iterable_dataset import IterableESPnetDataset
 from funasr.iterators.abs_iter_factory import AbsIterFactory
@@ -265,15 +263,14 @@
     @abstractmethod
     def build_model(cls, args: argparse.Namespace) -> FunASRModel:
         raise NotImplementedError
 
 
     @classmethod
     def get_parser(cls) -> config_argparse.ArgumentParser:
-        assert check_argument_types()
 
         class ArgumentDefaultsRawTextHelpFormatter(
             argparse.RawTextHelpFormatter,
             argparse.ArgumentDefaultsHelpFormatter,
         ):
             pass
 
@@ -955,15 +952,14 @@
             default=None,
             help="oss bucket.",
         )
 
         cls.trainer.add_arguments(parser)
         cls.add_task_arguments(parser)
 
-        assert check_return_type(parser)
         return parser
 
     @classmethod
     def build_optimizers(
             cls,
             args: argparse.Namespace,
             model: torch.nn.Module,
@@ -1003,15 +999,14 @@
         def get_class_type(name: str, classes: dict):
             _cls = classes.get(name)
             if _cls is None:
                 raise ValueError(f"must be one of {list(classes)}: {name}")
             return _cls
 
         # This method is used only for --print_config
-        assert check_argument_types()
         parser = cls.get_parser()
         args, _ = parser.parse_known_args()
         config = vars(args)
         # Excludes the options not to be shown
         for k in AbsTask.exclude_opts():
             config.pop(k)
 
@@ -1043,15 +1038,14 @@
                 conf.update(config[f"{name}_conf"])
                 # and set it again
                 config[f"{name}_conf"] = conf
         return config
 
     @classmethod
     def check_required_command_args(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if hasattr(args, "required"):
             for k in vars(args):
                 if "-" in k:
                     raise RuntimeError(f'Use "_" instead of "-": parser.get_parser("{k}")')
 
             required = ", ".join(
                 f"--{a}" for a in args.required if getattr(args, a) is None
@@ -1073,15 +1067,14 @@
             cls,
             dataset: Union[AbsDataset, IterableESPnetDataset],
             allow_variable_data_keys: bool,
             train: bool,
             inference: bool = False,
     ) -> None:
         """Check if the dataset satisfy the requirement of current Task"""
-        assert check_argument_types()
         mes = (
             f"If you intend to use an additional input, modify "
             f'"{cls.__name__}.required_data_names()" or '
             f'"{cls.__name__}.optional_data_names()". '
             f"Otherwise you need to set --allow_variable_data_keys true "
         )
 
@@ -1100,22 +1093,20 @@
                     raise RuntimeError(
                         f"The data-name must be one of {task_keys} "
                         f'for {cls.__name__}: "{k}" is not allowed.\n{mes}'
                     )
 
     @classmethod
     def print_config(cls, file=sys.stdout) -> None:
-        assert check_argument_types()
         # Shows the config: e.g. python train.py asr --print_config
         config = cls.get_default_config()
         file.write(yaml_no_alias_safe_dump(config, indent=4, sort_keys=False))
 
     @classmethod
     def main(cls, args: argparse.Namespace = None, cmd: Sequence[str] = None):
-        assert check_argument_types()
         print(get_commandline_args(), file=sys.stderr)
         if args is None:
             parser = cls.get_parser()
             args = parser.parse_args(cmd)
         args.version = __version__
         if args.pretrain_path is not None:
             raise RuntimeError("--pretrain_path is deprecated. Use --init_param")
@@ -1144,15 +1135,14 @@
         args.batch_type = "length"
         args.oss_bucket = None
         args.input_size = None
         cls.main_worker(args)
 
     @classmethod
     def main_worker(cls, args: argparse.Namespace):
-        assert check_argument_types()
 
         # 0. Init distributed process
         distributed_option = build_dataclass(DistributedOption, args)
         # Setting distributed_option.dist_rank, etc.
         if args.use_pai:
             distributed_option.init_options_pai()
         elif not args.simple_ddp:
@@ -1552,15 +1542,14 @@
         and the rest of samples for the originally epoch are left for the next epoch.
         e.g. If The number of mini-batches equals to 4, the following two are same:
 
         - 1 epoch without "--num_iters_per_epoch"
         - 4 epoch with "--num_iters_per_epoch" == 4
 
         """
-        assert check_argument_types()
         iter_options = cls.build_iter_options(args, distributed_option, mode)
 
         # Overwrite iter_options if any kwargs is given
         if kwargs is not None:
             for k, v in kwargs.items():
                 setattr(iter_options, k, v)
 
@@ -1585,15 +1574,14 @@
         else:
             raise RuntimeError(f"Not supported: iterator_type={args.iterator_type}")
 
     @classmethod
     def build_sequence_iter_factory(
             cls, args: argparse.Namespace, iter_options: IteratorOptions, mode: str
     ) -> AbsIterFactory:
-        assert check_argument_types()
 
         if hasattr(args, "frontend_conf"):
             if args.frontend_conf is not None and "fs" in args.frontend_conf:
                 dest_sample_rate = args.frontend_conf["fs"]
             else:
                 dest_sample_rate = 16000
         else:
@@ -1679,15 +1667,14 @@
     @classmethod
     def build_chunk_iter_factory(
             cls,
             args: argparse.Namespace,
             iter_options: IteratorOptions,
             mode: str,
     ) -> AbsIterFactory:
-        assert check_argument_types()
 
         dataset = ESPnetDataset(
             iter_options.data_path_and_name_and_type,
             float_dtype=args.train_dtype,
             preprocess=iter_options.preprocess_fn,
             max_cache_size=iter_options.max_cache_size,
             max_cache_fd=iter_options.max_cache_fd,
@@ -1784,15 +1771,14 @@
         """
         raise NotImplementedError
 
     @classmethod
     def build_multiple_iter_factory(
             cls, args: argparse.Namespace, distributed_option: DistributedOption, mode: str
     ):
-        assert check_argument_types()
         iter_options = cls.build_iter_options(args, distributed_option, mode)
         assert len(iter_options.data_path_and_name_and_type) > 0, len(
             iter_options.data_path_and_name_and_type
         )
 
         # 1. Sanity check
         num_splits = None
@@ -1881,15 +1867,14 @@
             dtype: str = np.float32,
             num_workers: int = 1,
             allow_variable_data_keys: bool = False,
             ngpu: int = 0,
             inference: bool = False,
     ) -> DataLoader:
         """Build DataLoader using iterable dataset"""
-        assert check_argument_types()
         # For backward compatibility for pytorch DataLoader
         if collate_fn is not None:
             kwargs = dict(collate_fn=collate_fn)
         else:
             kwargs = {}
 
         dataset = IterableESPnetDataset(
@@ -1931,15 +1916,14 @@
 
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
```

### Comparing `funasr-0.6.6/funasr/tasks/asr.py` & `funasr-0.6.7/funasr/tasks/asr.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 import yaml
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.ctc import CTC
@@ -487,23 +485,21 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
         return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 token_type=args.token_type,
                 token_list=args.token_list,
                 bpemodel=args.bpemodel,
                 non_linguistic_symbols=args.non_linguistic_symbols if hasattr(args, "non_linguistic_symbols") else None,
@@ -525,15 +521,14 @@
                 else "13_15",
                 speech_volume_normalize=args.speech_volume_normalize
                 if hasattr(args, "rir_scp")
                 else None,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
@@ -544,20 +539,18 @@
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -654,15 +647,14 @@
             **args.model_conf,
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
 
 class ASRTaskUniASR(ASRTask):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
@@ -697,15 +689,14 @@
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -834,15 +825,14 @@
             **args.model_conf,
         )
 
         # 12. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
@@ -856,15 +846,14 @@
 
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
@@ -971,15 +960,14 @@
     # ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -1081,15 +1069,14 @@
             **args.model_conf,
         )
 
         # 11. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
@@ -1103,15 +1090,14 @@
 
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
@@ -1206,15 +1192,14 @@
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -1304,15 +1289,14 @@
             **args.model_conf,
         )
 
         # 11. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
 
 class ASRTaskAligner(ASRTaskParaformer):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
@@ -1329,15 +1313,14 @@
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -1384,15 +1367,14 @@
             **args.model_conf,
         )
 
         # 11. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("speech", "text")
@@ -1421,15 +1403,14 @@
         """Required data depending on task mode.
         Args:
             cls: ASRTransducerTask object.
             args: Task arguments.
         Return:
             model: ASR Transducer model.
         """
-        assert check_argument_types()
 
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
@@ -1520,15 +1501,14 @@
         # 8. Initialize model
         if args.init is not None:
             raise NotImplementedError(
                 "Currently not supported.",
                 "Initialization part will be reworked in a short future.",
             )
 
-        #assert check_return_type(model)
 
         return model
 
 
 class ASRTaskSAASR(ASRTask):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
@@ -1555,15 +1535,14 @@
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -1641,9 +1620,8 @@
             **args.model_conf,
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
```

### Comparing `funasr-0.6.6/funasr/tasks/data2vec.py` & `funasr-0.6.7/funasr/tasks/data2vec.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.data2vec import Data2VecPretrainModel
@@ -252,22 +250,20 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         return CommonCollateFn(clipping=True)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 bpemodel=args.bpemodel,
                 non_linguistic_symbols=args.non_linguistic_symbols,
                 text_cleaner=args.cleaner,
                 g2p_type=args.g2p,
@@ -285,15 +281,14 @@
                 else "13_15",
                 speech_volume_normalize=args.speech_volume_normalize
                 if hasattr(args, "rir_scp")
                 else None,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         # for pre-training
@@ -301,20 +296,18 @@
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
 
         # 1. frontend
         if args.input_size is None:
             # Extract features in the model
             frontend_class = frontend_choices.get_class(args.frontend)
             frontend = frontend_class(**args.frontend_conf)
             input_size = frontend.output_size()
@@ -368,9 +361,8 @@
             encoder=encoder,
         )
 
         # 7. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
```

### Comparing `funasr-0.6.6/funasr/tasks/diar.py` & `funasr-0.6.7/funasr/tasks/diar.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 import yaml
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.label_aggregation import LabelAggregate
 from funasr.layers.utterance_mvn import UtteranceMVN
@@ -340,23 +338,21 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
         return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 token_type=args.token_type,
                 token_list=args.token_list,
                 bpemodel=None,
                 non_linguistic_symbols=None,
@@ -378,15 +374,14 @@
                 else "13_15",
                 speech_volume_normalize=args.speech_volume_normalize
                 if hasattr(args, "rir_scp")
                 else None,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
@@ -397,20 +392,18 @@
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -501,15 +494,14 @@
             **args.model_conf,
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
@@ -524,15 +516,14 @@
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             cmvn_file: The cmvn file for front-end
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
@@ -760,23 +751,21 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
         return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         # if args.use_preprocessor:
         #     retval = CommonPreprocessor(
         #         train=train,
         #         token_type=args.token_type,
         #         token_list=args.token_list,
         #         bpemodel=None,
         #         non_linguistic_symbols=None,
@@ -798,15 +787,14 @@
         #         else "13_15",
         #         speech_volume_normalize=args.speech_volume_normalize
         #         if hasattr(args, "rir_scp")
         #         else None,
         #     )
         # else:
         #     retval = None
-        # assert check_return_type(retval)
         return None
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
@@ -817,20 +805,18 @@
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
 
         # 1. frontend
         if args.input_size is None or args.frontend == "wav_frontend_mel23":
             # Extract features in the model
             frontend_class = frontend_choices.get_class(args.frontend)
             if args.frontend == 'wav_frontend':
                 frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
@@ -861,15 +847,14 @@
             **args.model_conf,
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
@@ -884,15 +869,14 @@
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             cmvn_file: The cmvn file for front-end
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
```

### Comparing `funasr-0.6.6/funasr/tasks/lm.py` & `funasr-0.6.7/funasr/tasks/lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.train.abs_model import AbsLM
 from funasr.train.abs_model import LanguageModel
 from funasr.models.seq_rnn_lm import SequentialRNNLM
 from funasr.models.transformer_lm import TransformerLM
@@ -48,15 +46,14 @@
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def add_task_arguments(cls, parser: argparse.ArgumentParser):
         # NOTE(kamo): Use '_' instead of '-' to avoid confusion
-        assert check_argument_types()
         group = parser.add_argument_group(description="Task related")
 
         # NOTE(kamo): add_arguments(..., required=True) can't be used
         # to provide --print_config mode. Instead of it, do as
         required = parser.get_default("required")
         # required += ["token_list"]
 
@@ -126,45 +123,41 @@
             default=None,
             help="Specify g2p method if --token_type=phn",
         )
 
         for class_choices in cls.class_choices_list:
             class_choices.add_arguments(group)
 
-        assert check_return_type(parser)
         return parser
 
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         return CommonCollateFn(int_pad_value=0)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 token_type=args.token_type,
                 token_list=args.token_list,
                 bpemodel=args.bpemodel,
                 text_cleaner=args.cleaner,
                 g2p_type=args.g2p,
                 non_linguistic_symbols=args.non_linguistic_symbols,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("text",)
@@ -175,15 +168,14 @@
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace) -> LanguageModel:
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # "args" is saved as it is in a yaml file by BaseTask.main().
             # Overwriting token_list to keep it as "portable".
             args.token_list = token_list.copy()
```

### Comparing `funasr-0.6.6/funasr/tasks/punctuation.py` & `funasr-0.6.7/funasr/tasks/punctuation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import PuncTrainTokenizerCommonPreprocessor
 from funasr.train.abs_model import PunctuationModel
 from funasr.models.target_delay_transformer import TargetDelayTransformer
 from funasr.models.vad_realtime_transformer import VadRealtimeTransformer
 from funasr.tasks.abs_task import AbsTask
@@ -43,15 +41,14 @@
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def add_task_arguments(cls, parser: argparse.ArgumentParser):
         # NOTE(kamo): Use '_' instead of '-' to avoid confusion
-        assert check_argument_types()
         group = parser.add_argument_group(description="Task related")
 
         # NOTE(kamo): add_arguments(..., required=True) can't be used
         # to provide --print_config mode. Instead of it, do as
         required = parser.get_default("required")
 
         group.add_argument(
@@ -122,32 +119,29 @@
         )
 
         for class_choices in cls.class_choices_list:
             # Append --<name> and --<name>_conf.
             # e.g. --encoder and --encoder_conf
             class_choices.add_arguments(group)
 
-        assert check_return_type(parser)
         return parser
 
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         return CommonCollateFn(int_pad_value=0)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         token_types = [args.token_type, args.token_type]
         token_lists = [args.token_list, args.punc_list]
         bpemodels = [args.bpemodel, args.bpemodel]
         text_names = ["text", "punc"]
         if args.use_preprocessor:
             retval = PuncTrainTokenizerCommonPreprocessor(
                 train=train,
@@ -157,15 +151,14 @@
                 text_cleaner=args.cleaner,
                 g2p_type=args.g2p,
                 text_name = text_names,
                 non_linguistic_symbols=args.non_linguistic_symbols,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("text", "punc")
@@ -178,15 +171,14 @@
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("vad",)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace) -> PunctuationModel:
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # "args" is saved as it is in a yaml file by BaseTask.main().
             # Overwriting token_list to keep it as "portable".
             args.token_list = token_list.copy()
@@ -219,9 +211,8 @@
         model = PunctuationModel(punc_model=punc, vocab_size=vocab_size, punc_weight=punc_weight_list, **args.model_conf)
 
         # FIXME(kamo): Should be done in model?
         # 3. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
```

### Comparing `funasr-0.6.6/funasr/tasks/sa_asr.py` & `funasr-0.6.7/funasr/tasks/sa_asr.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 import yaml
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.ctc import CTC
@@ -441,23 +439,21 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
         return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 token_type=args.token_type,
                 token_list=args.token_list,
                 bpemodel=args.bpemodel,
                 non_linguistic_symbols=args.non_linguistic_symbols,
@@ -479,15 +475,14 @@
                 else "13_15",
                 speech_volume_normalize=args.speech_volume_normalize
                 if hasattr(args, "rir_scp")
                 else None,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
@@ -498,20 +493,18 @@
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -615,9 +608,8 @@
             **args.model_conf,
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
```

### Comparing `funasr-0.6.6/funasr/tasks/sv.py` & `funasr-0.6.7/funasr/tasks/sv.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 import yaml
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.e2e_asr import ASRModel
@@ -269,23 +267,21 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
         return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 token_type=None,
                 token_list=None,
                 bpemodel=None,
                 non_linguistic_symbols=None,
@@ -305,15 +301,14 @@
                 else "13_15",
                 speech_volume_normalize=args.speech_volume_normalize
                 if hasattr(args, "rir_scp")
                 else None,
             )
         else:
             retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
@@ -326,20 +321,18 @@
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
         if inference:
             retval = ("ref_speech",)
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace) -> ESPnetSVModel:
-        assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
@@ -445,15 +438,14 @@
         )
 
         # FIXME(kamo): Should be done in model?
         # 8. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
-        assert check_return_type(model)
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
@@ -468,15 +460,14 @@
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             cmvn_file: The cmvn file for front-end
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
```

### Comparing `funasr-0.6.6/funasr/tasks/vad.py` & `funasr-0.6.7/funasr/tasks/vad.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 import yaml
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
 from funasr.models.e2e_vad import E2EVadModel
 from funasr.models.encoder.fsmn_encoder import FSMN
@@ -188,23 +186,21 @@
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
-        assert check_argument_types()
         # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
         return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
         # if args.use_preprocessor:
         #    retval = CommonPreprocessor(
         #        train=train,
         #        # NOTE(kamo): Check attribute existence for backward compatibility
         #        rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
         #        rir_apply_prob=args.rir_apply_prob
         #        if hasattr(args, "rir_apply_prob")
@@ -219,15 +215,14 @@
         #        speech_volume_normalize=args.speech_volume_normalize
         #        if hasattr(args, "rir_scp")
         #        else None,
         #    )
         # else:
         #    retval = None
         retval = None
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
@@ -238,20 +233,18 @@
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
-        assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
         # 4. Encoder
         encoder_class = encoder_choices.get_class(args.encoder)
         encoder = encoder_class(**args.encoder_conf)
 
         # 5. Build model
         try:
             model_class = model_choices.get_class(args.model)
@@ -293,15 +286,14 @@
 
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
             device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
-        assert check_argument_types()
         if config_file is None:
             assert model_file is not None, (
                 "The argument 'model_file' must be provided "
                 "if the argument 'config_file' is not specified."
             )
             config_file = Path(model_file).parent / "config.yaml"
         else:
```

### Comparing `funasr-0.6.6/funasr/text/build_tokenizer.py` & `funasr-0.6.7/funasr/text/build_tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 from typing import Iterable
 from typing import Union
 
-from typeguard import check_argument_types
 
 from funasr.text.abs_tokenizer import AbsTokenizer
 from funasr.text.char_tokenizer import CharTokenizer
 from funasr.text.phoneme_tokenizer import PhonemeTokenizer
 from funasr.text.sentencepiece_tokenizer import SentencepiecesTokenizer
 from funasr.text.word_tokenizer import WordTokenizer
 
@@ -17,15 +16,14 @@
     non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
     remove_non_linguistic_symbols: bool = False,
     space_symbol: str = "<space>",
     delimiter: str = None,
     g2p_type: str = None,
 ) -> AbsTokenizer:
     """A helper function to instantiate Tokenizer"""
-    assert check_argument_types()
     if token_type == "bpe":
         if bpemodel is None:
             raise ValueError('bpemodel is required if token_type = "bpe"')
 
         if remove_non_linguistic_symbols:
             raise RuntimeError(
                 "remove_non_linguistic_symbols is not implemented for token_type=bpe"
```

### Comparing `funasr-0.6.6/funasr/text/char_tokenizer.py` & `funasr-0.6.7/funasr/text/char_tokenizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from pathlib import Path
 from typing import Iterable
 from typing import List
 from typing import Union
 import warnings
 
-from typeguard import check_argument_types
 
 from funasr.text.abs_tokenizer import AbsTokenizer
 
 
 class CharTokenizer(AbsTokenizer):
     def __init__(
         self,
         non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
         remove_non_linguistic_symbols: bool = False,
     ):
-        assert check_argument_types()
         self.space_symbol = space_symbol
         if non_linguistic_symbols is None:
             self.non_linguistic_symbols = set()
         elif isinstance(non_linguistic_symbols, (Path, str)):
             non_linguistic_symbols = Path(non_linguistic_symbols)
             try:
                 with non_linguistic_symbols.open("r", encoding="utf-8") as f:
```

### Comparing `funasr-0.6.6/funasr/text/cleaner.py` & `funasr-0.6.7/funasr/text/cleaner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Collection
 
 from jaconv import jaconv
 import tacotron_cleaner.cleaners
-from typeguard import check_argument_types
 
 try:
     from vietnamese_cleaner import vietnamese_cleaners
 except ImportError:
     vietnamese_cleaners = None
 
 
@@ -17,15 +16,14 @@
         >>> cleaner = TextCleaner("tacotron")
         >>> cleaner("(Hello-World);   &  jr. & dr.")
         'HELLO WORLD, AND JUNIOR AND DOCTOR'
 
     """
 
     def __init__(self, cleaner_types: Collection[str] = None):
-        assert check_argument_types()
 
         if cleaner_types is None:
             self.cleaner_types = []
         elif isinstance(cleaner_types, str):
             self.cleaner_types = [cleaner_types]
         else:
             self.cleaner_types = list(cleaner_types)
```

### Comparing `funasr-0.6.6/funasr/text/korean_cleaner.py` & `funasr-0.6.7/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/text/phoneme_tokenizer.py` & `funasr-0.6.7/funasr/text/phoneme_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import List
 from typing import Optional
 from typing import Union
 import warnings
 
 # import g2p_en
 import jamo
-from typeguard import check_argument_types
 
 from funasr.text.abs_tokenizer import AbsTokenizer
 
 
 g2p_choices = [
     None,
     "g2p_en",
@@ -361,15 +360,14 @@
     def __init__(
         self,
         g2p_type: Union[None, str],
         non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
         remove_non_linguistic_symbols: bool = False,
     ):
-        assert check_argument_types()
         if g2p_type is None:
             self.g2p = split_by_space
         elif g2p_type == "g2p_en":
             self.g2p = G2p_en(no_space=False)
         elif g2p_type == "g2p_en_no_space":
             self.g2p = G2p_en(no_space=True)
         elif g2p_type == "pyopenjtalk":
```

### Comparing `funasr-0.6.6/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.6.7/funasr/text/sentencepiece_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from pathlib import Path
 from typing import Iterable
 from typing import List
 from typing import Union
 
 import sentencepiece as spm
-from typeguard import check_argument_types
 
 from funasr.text.abs_tokenizer import AbsTokenizer
 
 
 class SentencepiecesTokenizer(AbsTokenizer):
     def __init__(self, model: Union[Path, str]):
-        assert check_argument_types()
         self.model = str(model)
         # NOTE(kamo):
         # Don't build SentencePieceProcessor in __init__()
         # because it's not picklable and it may cause following error,
         # "TypeError: can't pickle SwigPyObject objects",
         # when giving it as argument of "multiprocessing.Process()".
         self.sp = None
```

### Comparing `funasr-0.6.6/funasr/text/token_id_converter.py` & `funasr-0.6.7/funasr/text/token_id_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Union
 
 import numpy as np
-from typeguard import check_argument_types
 
 
 class TokenIDConverter:
     def __init__(
         self,
         token_list: Union[Path, str, Iterable[str]],
         unk_symbol: str = "<unk>",
     ):
-        assert check_argument_types()
 
         if isinstance(token_list, (Path, str)):
             token_list = Path(token_list)
             self.token_list_repr = str(token_list)
             self.token_list: List[str] = []
 
             with token_list.open("r", encoding="utf-8") as f:
```

### Comparing `funasr-0.6.6/funasr/text/word_tokenizer.py` & `funasr-0.6.7/funasr/text/word_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from pathlib import Path
 from typing import Iterable
 from typing import List
 from typing import Union
 import warnings
 
-from typeguard import check_argument_types
 
 from funasr.text.abs_tokenizer import AbsTokenizer
 
 
 class WordTokenizer(AbsTokenizer):
     def __init__(
         self,
         delimiter: str = None,
         non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
         remove_non_linguistic_symbols: bool = False,
     ):
-        assert check_argument_types()
         self.delimiter = delimiter
 
         if not remove_non_linguistic_symbols and non_linguistic_symbols is not None:
             warnings.warn(
                 "non_linguistic_symbols is only used "
                 "when remove_non_linguistic_symbols = True"
             )
```

### Comparing `funasr-0.6.6/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.6.7/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/torch_utils/device_funcs.py` & `funasr-0.6.7/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/torch_utils/forward_adaptor.py` & `funasr-0.6.7/funasr/torch_utils/forward_adaptor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import torch
-from typeguard import check_argument_types
 
 
 class ForwardAdaptor(torch.nn.Module):
     """Wrapped module to parallelize specified method
 
     torch.nn.DataParallel parallelizes only "forward()"
     and, maybe, the method having the other name can't be applied
@@ -17,15 +16,14 @@
         >>> model = ForwardAdaptor(model, "foo")
         >>> model = torch.nn.DataParallel(model, device_ids=[0, 1])
         >>> x = torch.randn(2, 10)
         >>> model(x)
     """
 
     def __init__(self, module: torch.nn.Module, name: str):
-        assert check_argument_types()
         super().__init__()
         self.module = module
         self.name = name
         if not hasattr(module, name):
             raise ValueError(f"{module} doesn't have {name}")
 
     def forward(self, *args, **kwargs):
```

### Comparing `funasr-0.6.6/funasr/torch_utils/initialize.py` & `funasr-0.6.7/funasr/torch_utils/initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python3
 
 """Initialize modules for espnet2 neural networks."""
 
 import math
 import torch
-from typeguard import check_argument_types
 
 
 def initialize(model: torch.nn.Module, init: str):
     """Initialize weights of a neural network module.
 
     Parameters are initialized using the given method or distribution.
 
     Custom initialization routines can be implemented into submodules
     as function `espnet_initialization_fn` within the custom module.
 
     Args:
         model: Target.
         init: Method of initialization.
     """
-    assert check_argument_types()
 
     if init == "chainer":
         # 1. lecun_normal_init_parameters
         for p in model.parameters():
             data = p.data
             if data.dim() == 1:
                 # bias
```

### Comparing `funasr-0.6.6/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.6.7/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/torch_utils/model_summary.py` & `funasr-0.6.7/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/torch_utils/recursive_op.py` & `funasr-0.6.7/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/train/abs_model.py` & `funasr-0.6.7/funasr/train/abs_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from funasr.modules.scorers.scorer_interface import BatchScorerInterface
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import torch
 import torch.nn.functional as F
-from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.models.base_model import FunASRModel
 
 class AbsLM(torch.nn.Module, BatchScorerInterface, ABC):
     """The abstract LM class
@@ -30,15 +29,14 @@
         self, input: torch.Tensor, hidden: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         raise NotImplementedError
 
 
 class LanguageModel(FunASRModel):
     def __init__(self, lm: AbsLM, vocab_size: int, ignore_id: int = 0):
-        assert check_argument_types()
         super().__init__()
         self.lm = lm
         self.sos = 1
         self.eos = 2
 
         # ignore_id may be assumed as 0, shared with CTC-blank symbol for ASR.
         self.ignore_id = ignore_id
@@ -150,15 +148,14 @@
     ) -> Dict[str, torch.Tensor]:
         return {}
 
 
 class PunctuationModel(FunASRModel):
     
     def __init__(self, punc_model: torch.nn.Module, vocab_size: int, ignore_id: int = 0, punc_weight: list = None):
-        assert check_argument_types()
         super().__init__()
         self.punc_model = punc_model
         self.punc_weight = torch.Tensor(punc_weight)
         self.sos = 1
         self.eos = 2
         
         # ignore_id may be assumed as 0, shared with CTC-blank symbol for ASR.
```

### Comparing `funasr-0.6.6/funasr/train/class_choices.py` & `funasr-0.6.7/funasr/train/class_choices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import Mapping
 from typing import Optional
 from typing import Tuple
 
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 from funasr.utils.nested_dict_action import NestedDictAction
 from funasr.utils.types import str_or_none
 
 
 class ClassChoices:
     """Helper class to manage the options for variable objects and its configuration.
@@ -36,15 +34,14 @@
         self,
         name: str,
         classes: Mapping[str, type],
         type_check: type = None,
         default: str = None,
         optional: bool = False,
     ):
-        assert check_argument_types()
         self.name = name
         self.base_type = type_check
         self.classes = {k.lower(): v for k, v in classes.items()}
         if "none" in self.classes or "nil" in self.classes or "null" in self.classes:
             raise ValueError('"none", "nil", and "null" are reserved.')
         if type_check is not None:
             for v in self.classes.values():
@@ -60,20 +57,18 @@
         retval = tuple(self.classes)
         if self.optional:
             return retval + (None,)
         else:
             return retval
 
     def get_class(self, name: Optional[str]) -> Optional[type]:
-        assert check_argument_types()
         if name is None or (self.optional and name.lower() == ("none", "null", "nil")):
             retval = None
         elif name.lower() in self.classes:
             class_obj = self.classes[name]
-            assert check_return_type(class_obj)
             retval = class_obj
         else:
             raise ValueError(
                 f"--{self.name} must be one of {self.choices()}: "
                 f"--{self.name} {name.lower()}"
             )
```

### Comparing `funasr-0.6.6/funasr/train/distributed_utils.py` & `funasr-0.6.7/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/train/reporter.py` & `funasr-0.6.7/funasr/train/reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,44 +14,39 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import humanfriendly
 import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
 
 Num = Union[float, int, complex, torch.Tensor, np.ndarray]
 
 _reserved = {"time", "total_count"}
 
 
 def to_reported_value(v: Num, weight: Num = None) -> "ReportedValue":
-    assert check_argument_types()
     if isinstance(v, (torch.Tensor, np.ndarray)):
         if np.prod(v.shape) != 1:
             raise ValueError(f"v must be 0 or 1 dimension: {len(v.shape)}")
         v = v.item()
 
     if isinstance(weight, (torch.Tensor, np.ndarray)):
         if np.prod(weight.shape) != 1:
             raise ValueError(f"weight must be 0 or 1 dimension: {len(weight.shape)}")
         weight = weight.item()
 
     if weight is not None:
         retval = WeightedAverage(v, weight)
     else:
         retval = Average(v)
-    assert check_return_type(retval)
     return retval
 
 
 def aggregate(values: Sequence["ReportedValue"]) -> Num:
-    assert check_argument_types()
 
     for v in values:
         if not isinstance(v, type(values[0])):
             raise ValueError(
                 f"Can't use different Reported type together: "
                 f"{type(v)} != {type(values[0])}"
             )
@@ -82,15 +77,14 @@
                 retval = sum_value / sum_weights
         else:
             warnings.warn("No valid stats found")
             retval = np.nan
 
     else:
         raise NotImplementedError(f"type={type(values[0])}")
-    assert check_return_type(retval)
     return retval
 
 
 def wandb_get_prefix(key: str):
     if key.startswith("valid"):
         return "valid/"
     if key.startswith("train"):
@@ -118,15 +112,14 @@
 class SubReporter:
     """This class is used in Reporter.
 
     See the docstring of Reporter for the usage.
     """
 
     def __init__(self, key: str, epoch: int, total_count: int):
-        assert check_argument_types()
         self.key = key
         self.epoch = epoch
         self.start_time = time.perf_counter()
         self.stats = defaultdict(list)
         self._finished = False
         self.total_count = total_count
         self.count = 0
@@ -156,15 +149,14 @@
         self._seen_keys_in_the_step = set()
 
     def register(
             self,
             stats: Dict[str, Optional[Union[Num, Dict[str, Num]]]],
             weight: Num = None,
     ) -> None:
-        assert check_argument_types()
         if self._finished:
             raise RuntimeError("Already finished")
         if len(self._seen_keys_in_the_step) == 0:
             # Increment count as the first register in this step
             self.total_count += 1
             self.count += 1
 
@@ -289,15 +281,14 @@
         ...     for batch in iterator:
         ...         stats = dict(loss=0.2)
         ...         sub_reporter.register(stats)
 
     """
 
     def __init__(self, epoch: int = 0):
-        assert check_argument_types()
         if epoch < 0:
             raise ValueError(f"epoch must be 0 or more: {epoch}")
         self.epoch = epoch
         # stats: Dict[int, Dict[str, Dict[str, float]]]
         # e.g. self.stats[epoch]['train']['loss']
         self.stats = {}
```

### Comparing `funasr-0.6.6/funasr/train/trainer.py` & `funasr-0.6.7/funasr/train/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import oss2
 from io import BytesIO
 import os
 import numpy as np
 import torch
 import torch.nn
 import torch.optim
-from typeguard import check_argument_types
 
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 from funasr.main_funcs.average_nbest_models import average_nbest_models
 from funasr.main_funcs.calculate_all_attentions import calculate_all_attentions
 from funasr.schedulers.abs_scheduler import AbsBatchStepScheduler
 from funasr.schedulers.abs_scheduler import AbsEpochStepScheduler
 from funasr.schedulers.abs_scheduler import AbsScheduler
@@ -123,15 +122,14 @@
 
     def __init__(self):
         raise RuntimeError("This class can't be instantiated.")
 
     @classmethod
     def build_options(cls, args: argparse.Namespace) -> TrainerOptions:
         """Build options consumed by train(), eval()"""
-        assert check_argument_types()
         return build_dataclass(TrainerOptions, args)
 
     @classmethod
     def add_arguments(cls, parser: argparse.ArgumentParser):
         """Reserved for future development of another Trainer"""
         pass
 
@@ -184,15 +182,14 @@
         schedulers: Sequence[Optional[AbsScheduler]],
         train_iter_factory: AbsIterFactory,
         valid_iter_factory: AbsIterFactory,
         trainer_options,
         distributed_option: DistributedOption,
     ) -> None:
         """Perform training. This method performs the main process of training."""
-        assert check_argument_types()
         # NOTE(kamo): Don't check the type more strictly as far trainer_options
         assert is_dataclass(trainer_options), type(trainer_options)
         assert len(optimizers) == len(schedulers), (len(optimizers), len(schedulers))
 
         if isinstance(trainer_options.keep_nbest_models, int):
             keep_nbest_models = [trainer_options.keep_nbest_models]
         else:
@@ -547,15 +544,14 @@
         schedulers: Sequence[Optional[AbsScheduler]],
         scaler: Optional[GradScaler],
         reporter: SubReporter,
         summary_writer,
         options: TrainerOptions,
         distributed_option: DistributedOption,
     ) -> Tuple[bool, bool]:
-        assert check_argument_types()
 
         grad_noise = options.grad_noise
         accum_grad = options.accum_grad
         grad_clip = options.grad_clip
         grad_clip_type = options.grad_clip_type
         log_interval = options.log_interval
         no_forward_run = options.no_forward_run
@@ -841,15 +837,14 @@
         cls,
         model: torch.nn.Module,
         iterator: Iterable[Dict[str, torch.Tensor]],
         reporter: SubReporter,
         options: TrainerOptions,
         distributed_option: DistributedOption,
     ) -> None:
-        assert check_argument_types()
         ngpu = options.ngpu
         no_forward_run = options.no_forward_run
         distributed = distributed_option.distributed
 
         model.eval()
 
         # [For distributed] Because iteration counts are not always equals between
```

### Comparing `funasr-0.6.6/funasr/utils/asr_env_checking.py` & `funasr-0.6.7/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/asr_utils.py` & `funasr-0.6.7/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/cli_utils.py` & `funasr-0.6.7/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/compute_eer.py` & `funasr-0.6.7/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/compute_min_dcf.py` & `funasr-0.6.7/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/compute_wer.py` & `funasr-0.6.7/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/config_argparse.py` & `funasr-0.6.7/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/get_default_kwargs.py` & `funasr-0.6.7/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/griffin_lim.py` & `funasr-0.6.7/funasr/utils/griffin_lim.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # Copyright 2019 Tomoki Hayashi
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 import logging
 
 from distutils.version import LooseVersion
 from functools import partial
-from typeguard import check_argument_types
 from typing import Optional
 
 import librosa
 import numpy as np
 import torch
 
 EPS = 1e-10
@@ -134,15 +133,14 @@
             win_length: Window length in points.
             window: Window function type.
             f_min: Minimum frequency to analyze.
             f_max: Maximum frequency to analyze.
             griffin_lim_iters: The number of iterations.
 
         """
-        assert check_argument_types()
         self.fs = fs
         self.logmel2linear = (
             partial(
                 logmel2linear, fs=fs, n_fft=n_fft, n_mels=n_mels, fmin=fmin, fmax=fmax
             )
             if n_mels is not None
             else None
```

### Comparing `funasr-0.6.6/funasr/utils/job_runner.py` & `funasr-0.6.7/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/misc.py` & `funasr-0.6.7/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/modelscope_param.py` & `funasr-0.6.7/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/modelscope_utils.py` & `funasr-0.6.7/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/nested_dict_action.py` & `funasr-0.6.7/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/postprocess_utils.py` & `funasr-0.6.7/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/prepare_data.py` & `funasr-0.6.7/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/runtime_sdk_download_tool.py` & `funasr-0.6.7/funasr/utils/runtime_sdk_download_tool.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/sized_dict.py` & `funasr-0.6.7/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/timestamp_tools.py` & `funasr-0.6.7/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/types.py` & `funasr-0.6.7/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/vad_utils.py` & `funasr-0.6.7/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr/utils/wav_utils.py` & `funasr-0.6.7/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr.egg-info/PKG-INFO` & `funasr-0.6.7/funasr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.6
+Version: 0.6.7
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: train
-Provides-Extra: recipe
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
 
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.6 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.7 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
-Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
-Extra: test Provides-Extra: doc [//]: # (
+Provides-Extra: train Provides-Extra: all Provides-Extra: test Provides-Extra:
+doc [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
```

### Comparing `funasr-0.6.6/funasr.egg-info/SOURCES.txt` & `funasr-0.6.7/funasr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/funasr.egg-info/requires.txt` & `funasr-0.6.7/funasr.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 setuptools>=38.5.1
-typeguard==2.13.3
+typeguard>=3.0.1
 humanfriendly
 scipy>=1.4.1
 librosa
-jamo==0.4.1
+jamo
 PyYAML>=5.1.2
-soundfile>=0.11.0
+soundfile>=0.10.2
 h5py>=2.10.0
 kaldiio>=2.17.0
 torch_complex
 nltk>=3.4.5
 sentencepiece
-pypinyin<=0.44.0
+pypinyin>=0.44.0
 espnet_tts_frontend
 pytorch_wpe
 editdistance>=0.5.2
-tensorboard==1.15
+tensorboard
 g2p
 oss2
 edit-distance
 textgrid
-protobuf==3.20.0
+protobuf
 
 [all]
 torch_optimizer
 fairscale
 transformers
-editdistance==0.5.2
+editdistance
 wandb
-espnet_model_zoo
 
 [doc]
-Jinja2<3.1
-Sphinx==2.1.2
+Jinja2
+Sphinx
 sphinx-rtd-theme>=0.2.4
 sphinx-argparse>=0.2.5
-commonmark==0.8.1
+commonmark
 recommonmark>=0.4.0
 nbsphinx>=0.4.2
 sphinx-markdown-tables>=0.0.12
-
-[recipe]
-espnet_model_zoo
+configargparse>=1.2.1
 
 [test]
 pytest>=3.3.0
 pytest-timeouts>=1.2.1
 pytest-pythonpath>=0.7.3
 pytest-cov>=2.7.1
 hacking>=2.0.0
 mock>=2.0.0
 pycodestyle
 jsondiff<2.0.0,>=1.2.0
 flake8>=3.7.8
 flake8-docstrings>=1.3.1
 black
-editdistance==0.5.2
+editdistance
 wandb
 
 [train]
-editdistance==0.5.2
+editdistance
 wandb
```

### Comparing `funasr-0.6.6/setup.py` & `funasr-0.6.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,59 @@
 #!/usr/bin/env python3
 
 """FunASR setup script."""
 
 import os
 
-from distutils.version import LooseVersion
 from setuptools import find_packages
 from setuptools import setup
 
 
 requirements = {
     "install": [
         "setuptools>=38.5.1",
-        # "configargparse>=1.2.1",
-        "typeguard==2.13.3",
+        "typeguard>=3.0.1",
         "humanfriendly",
         "scipy>=1.4.1",
-        # "filelock",
         "librosa",
-        "jamo==0.4.1",  # For kss
+        "jamo",  # For kss
         "PyYAML>=5.1.2",
-        "soundfile>=0.11.0",
+        "soundfile>=0.10.2",
         "h5py>=2.10.0",
         "kaldiio>=2.17.0",
         "torch_complex",
         "nltk>=3.4.5",
         # ASR
         "sentencepiece",
-        # "ctc-segmentation<1.8,>=1.6.6",
         # TTS
-        # "pyworld>=0.2.10",
-        "pypinyin<=0.44.0",
+        "pypinyin>=0.44.0",
         "espnet_tts_frontend",
         # ENH
-        # "ci_sdr",
         "pytorch_wpe",
         "editdistance>=0.5.2",
-        "tensorboard==1.15",
+        "tensorboard",
         "g2p",
         # PAI
         "oss2",
-        # "kaldi-native-fbank",
-        # timestamp
         "edit-distance",
-        # textgrid
         "textgrid",
-        "protobuf==3.20.0",
+        "protobuf",
     ],
     # train: The modules invoked when training only.
     "train": [
-        # "pillow>=6.1.0",
-        "editdistance==0.5.2",
+        "editdistance",
         "wandb",
     ],
-    # recipe: The modules actually are not invoked in the main module of funasr,
-    #         but are invoked for the python scripts in each recipe
-    "recipe": [
-        "espnet_model_zoo",
-        # "gdown",
-        # "resampy",
-        # "pysptk>=0.1.17",
-        # "morfessor",  # for zeroth-korean
-        # "youtube_dl",  # for laborotv
-        # "nnmnkwii",
-        # "museval>=0.2.1",
-        # "pystoi>=0.2.2",
-        # "mir-eval>=0.6",
-        # "fastdtw",
-        # "nara_wpe>=0.0.5",
-        # "sacrebleu>=1.5.1",
-    ],
     # all: The modules should be optionally installled due to some reason.
     #      Please consider moving them to "install" occasionally
-    # NOTE(kamo): The modules in "train" and "recipe" are appended into "all"
     "all": [
         # NOTE(kamo): Append modules requiring specific pytorch version or torch>1.3.0
         "torch_optimizer",
         "fairscale",
         "transformers",
-        # "gtn==0.0.0",
     ],
     "setup": [
         "numpy",
         "pytest-runner",
     ],
     "test": [
         "pytest>=3.3.0",
@@ -94,25 +65,26 @@
         "pycodestyle",
         "jsondiff<2.0.0,>=1.2.0",
         "flake8>=3.7.8",
         "flake8-docstrings>=1.3.1",
         "black",
     ],
     "doc": [
-        "Jinja2<3.1",
-        "Sphinx==2.1.2",
+        "Jinja2",
+        "Sphinx",
         "sphinx-rtd-theme>=0.2.4",
         "sphinx-argparse>=0.2.5",
-        "commonmark==0.8.1",
+        "commonmark",
         "recommonmark>=0.4.0",
         "nbsphinx>=0.4.2",
         "sphinx-markdown-tables>=0.0.12",
+        "configargparse>=1.2.1"
     ],
 }
-requirements["all"].extend(requirements["train"] + requirements["recipe"])
+requirements["all"].extend(requirements["train"])
 requirements["test"].extend(requirements["train"])
 
 install_requires = requirements["install"]
 setup_requires = requirements["setup"]
 tests_require = requirements["test"]
 extras_require = {
     k: v for k, v in requirements.items() if k not in ["install", "setup"]
@@ -147,8 +119,8 @@
         "Programming Language :: Python :: 3.9",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Operating System :: POSIX :: Linux",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-)
+)
```

### Comparing `funasr-0.6.6/tests/test_asr_inference_pipeline.py` & `funasr-0.6.7/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.6.7/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/tests/test_lm_pipeline.py` & `funasr-0.6.7/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/tests/test_punctuation_pipeline.py` & `funasr-0.6.7/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/tests/test_sv_inference_pipeline.py` & `funasr-0.6.7/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/tests/test_tp_pipeline.py` & `funasr-0.6.7/tests/test_tp_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.6/tests/test_vad_inference_pipeline.py` & `funasr-0.6.7/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

