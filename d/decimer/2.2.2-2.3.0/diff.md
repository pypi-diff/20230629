# Comparing `tmp/decimer-2.2.2.tar.gz` & `tmp/decimer-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decimer-2.2.2.tar", last modified: Thu Mar 30 13:30:14 2023, max compression
+gzip compressed data, was "decimer-2.3.0.tar", last modified: Thu Jun 29 14:56:52 2023, max compression
```

## Comparing `decimer-2.2.2.tar` & `decimer-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,66 @@
-drwxr-xr-x   0 kohulanrajan   (501) staff       (20)        0 2023-03-30 13:30:14.812044 decimer-2.2.2/
-drwxr-xr-x   0 kohulanrajan   (501) staff       (20)        0 2023-03-30 13:30:14.810092 decimer-2.2.2/DECIMER/
--rw-r--r--   0 kohulanrajan   (501) staff       (20)    15813 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/DECIMER_EfficinetNetV2_Transfomer_Trainer.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     2500 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/Efficient_Net_encoder.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     4468 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/Predictor_EfficientNet2.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     6394 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/Repack_model.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)    15395 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/Transformer_decoder.py
-drwxr-xr-x   0 kohulanrajan   (501) staff       (20)        0 2023-03-30 13:30:14.810356 decimer-2.2.2/DECIMER/Utils/
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     2856 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/Utils/Create_TFrecord_From_pickles.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     4120 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/Utils/Create_image_tokenizer.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)      736 2023-03-30 11:21:51.000000 decimer-2.2.2/DECIMER/__init__.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)    11764 2023-03-30 11:21:35.000000 decimer-2.2.2/DECIMER/config.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     3195 2023-03-27 12:50:43.000000 decimer-2.2.2/DECIMER/decimer.py
-drwxr-xr-x   0 kohulanrajan   (501) staff       (20)        0 2023-03-30 13:30:14.810929 decimer-2.2.2/DECIMER/efficientnetv2/
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     8998 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/efficientnetv2/effnetv2_configs.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)    24008 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/efficientnetv2/effnetv2_model.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)    10270 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/efficientnetv2/hparams.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)    20655 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/efficientnetv2/utils.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     1452 2023-03-27 12:50:02.000000 decimer-2.2.2/DECIMER/utils.py
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     1070 2023-03-27 12:50:02.000000 decimer-2.2.2/LICENSE
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     8661 2023-03-30 13:30:14.811905 decimer-2.2.2/PKG-INFO
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     7708 2023-03-27 12:50:02.000000 decimer-2.2.2/README.md
-drwxr-xr-x   0 kohulanrajan   (501) staff       (20)        0 2023-03-30 13:30:14.811489 decimer-2.2.2/decimer.egg-info/
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     8661 2023-03-30 13:30:14.000000 decimer-2.2.2/decimer.egg-info/PKG-INFO
--rw-r--r--   0 kohulanrajan   (501) staff       (20)      690 2023-03-30 13:30:14.000000 decimer-2.2.2/decimer.egg-info/SOURCES.txt
--rw-r--r--   0 kohulanrajan   (501) staff       (20)        1 2023-03-30 13:30:14.000000 decimer-2.2.2/decimer.egg-info/dependency_links.txt
--rw-r--r--   0 kohulanrajan   (501) staff       (20)       65 2023-03-30 13:30:14.000000 decimer-2.2.2/decimer.egg-info/requires.txt
--rw-r--r--   0 kohulanrajan   (501) staff       (20)        8 2023-03-30 13:30:14.000000 decimer-2.2.2/decimer.egg-info/top_level.txt
--rw-r--r--   0 kohulanrajan   (501) staff       (20)       38 2023-03-30 13:30:14.812080 decimer-2.2.2/setup.cfg
--rw-r--r--   0 kohulanrajan   (501) staff       (20)     1476 2023-03-30 11:22:20.000000 decimer-2.2.2/setup.py
-drwxr-xr-x   0 kohulanrajan   (501) staff       (20)        0 2023-03-30 13:30:14.811609 decimer-2.2.2/tests/
--rw-r--r--   0 kohulanrajan   (501) staff       (20)      313 2023-03-27 12:50:43.000000 decimer-2.2.2/tests/test_functions.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.601411 decimer-2.3.0/
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.593411 decimer-2.3.0/.github/
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     3380 2023-06-29 14:09:35.000000 decimer-2.3.0/.github/ISSUE_TEMPLATE/Bug_Report.yml
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/.github/workflows/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      919 2023-06-29 14:09:35.000000 decimer-2.3.0/.github/workflows/Check_errors.yml
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1817 2023-06-29 14:09:35.000000 decimer-2.3.0/.gitignore
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      474 2023-06-29 14:09:35.000000 decimer-2.3.0/.readthedocs.yml
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/Benchmark/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1054 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/README.md
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      169 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/TEST.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     2735 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/distort_images.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     3390 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/evaluate_benchmarks.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1029 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/run_decimer_save_results.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/Benchmark/test_images/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     4743 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/test_images/DECIMER_test_0.png
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    12486 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/test_images/DECIMER_test_1.png
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    30464 2023-06-29 14:09:35.000000 decimer-2.3.0/Benchmark/test_images/github_issue_test.png
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      575 2023-06-29 14:09:35.000000 decimer-2.3.0/CITATION.cff
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     5244 2023-06-29 14:09:35.000000 decimer-2.3.0/CODE_OF_CONDUCT.md
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/DECIMER/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    15813 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/DECIMER_EfficinetNetV2_Transfomer_Trainer.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     2500 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/Efficient_Net_encoder.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     4468 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/Predictor_EfficientNet2.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     6678 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/Repack_model.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    15395 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/Transformer_decoder.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/DECIMER/Utils/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     2856 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/Utils/Create_TFrecord_From_pickles.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     4120 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/Utils/Create_image_tokenizer.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      736 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/__init__.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    12200 2023-06-29 14:09:43.000000 decimer-2.3.0/DECIMER/config.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     3195 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/decimer.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/DECIMER/efficientnetv2/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     8998 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/efficientnetv2/effnetv2_configs.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    24008 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/efficientnetv2/effnetv2_model.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    10270 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/efficientnetv2/hparams.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    20655 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/efficientnetv2/utils.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1452 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER/utils.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)  2755120 2023-06-29 14:09:35.000000 decimer-2.3.0/DECIMER_V2.png
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1313 2023-06-29 14:09:35.000000 decimer-2.3.0/ISSUES.md
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1070 2023-06-29 14:09:35.000000 decimer-2.3.0/LICENSE
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     8726 2023-06-29 14:56:52.601411 decimer-2.3.0/PKG-INFO
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       64 2023-06-29 14:09:35.000000 decimer-2.3.0/Python_Requirements.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     7708 2023-06-29 14:09:35.000000 decimer-2.3.0/README.md
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.597411 decimer-2.3.0/Tests/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    24609 2023-06-29 14:09:35.000000 decimer-2.3.0/Tests/caffeine.png
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      313 2023-06-29 14:09:35.000000 decimer-2.3.0/Tests/test_functions.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.601411 decimer-2.3.0/decimer.egg-info/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     8726 2023-06-29 14:56:52.000000 decimer-2.3.0/decimer.egg-info/PKG-INFO
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1300 2023-06-29 14:56:52.000000 decimer-2.3.0/decimer.egg-info/SOURCES.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)        1 2023-06-29 14:56:52.000000 decimer-2.3.0/decimer.egg-info/dependency_links.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       65 2023-06-29 14:56:52.000000 decimer-2.3.0/decimer.egg-info/requires.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)        8 2023-06-29 14:56:52.000000 decimer-2.3.0/decimer.egg-info/top_level.txt
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.601411 decimer-2.3.0/docs/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      449 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/DECIMER.rst
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      634 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/Makefile
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-06-29 14:56:52.601411 decimer-2.3.0/docs/_static/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)  1736034 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/_static/DECIMER.gif
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     2981 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/conf.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1278 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/index.rst
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      800 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/make.bat
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       60 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/modules.rst
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      122 2023-06-29 14:09:35.000000 decimer-2.3.0/docs/requirements.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       38 2023-06-29 14:56:52.601411 decimer-2.3.0/setup.cfg
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1743 2023-06-29 14:09:35.000000 decimer-2.3.0/setup.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      952 2023-06-29 14:09:35.000000 decimer-2.3.0/tox.ini
```

### Comparing `decimer-2.2.2/DECIMER/DECIMER_EfficinetNetV2_Transfomer_Trainer.py` & `decimer-2.3.0/DECIMER/DECIMER_EfficinetNetV2_Transfomer_Trainer.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/Efficient_Net_encoder.py` & `decimer-2.3.0/DECIMER/Efficient_Net_encoder.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/Predictor_EfficientNet2.py` & `decimer-2.3.0/DECIMER/Predictor_EfficientNet2.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/Repack_model.py` & `decimer-2.3.0/DECIMER/Repack_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 import tensorflow as tf
 
 import pickle
 import Transformer_decoder
 import Efficient_Net_encoder
 import config
+import utils
 
 print(tf.__version__)
 
 # Set GPU
 os.environ["CUDA_VISIBLE_DEVICES"] = "0"
 gpus = tf.config.experimental.list_physical_devices("GPU")
 for gpu in gpus:
     tf.config.experimental.set_memory_growth(gpu, True)
 
 # load assets
 tokenizer = pickle.load(open("tokenizer_TPU_Stereo.pkl", "rb"))
 max_length = pickle.load(open("max_length_TPU_Stereo.pkl", "rb"))
 
 # Image parameters
-IMG_EMB_DIM = (10, 10, 232)
+IMG_EMB_DIM = (16, 16, 232)
 IMG_EMB_DIM = (IMG_EMB_DIM[0] * IMG_EMB_DIM[1], IMG_EMB_DIM[2])
-IMG_SHAPE = (299, 299, 3)
+IMG_SHAPE = (512, 512, 3)
 PE_INPUT = IMG_EMB_DIM[0]
 IMG_SEQ_LEN, IMG_EMB_DEPTH = IMG_EMB_DIM
 D_MODEL = IMG_EMB_DEPTH
 
 # Network parameters
 N_LAYERS = 4
 D_MODEL = 512
@@ -80,14 +81,25 @@
 )
 ckpt_manager = tf.train.CheckpointManager(ckpt, checkpoint_path, max_to_keep=50)
 if ckpt_manager.latest_checkpoint:
     ckpt.restore(tf.train.latest_checkpoint(checkpoint_path))
     start_epoch = int(ckpt_manager.latest_checkpoint.split("-")[-1])
 
 
+def detokenize_output(predicted_array):
+    outputs = [tokenizer.index_word[i] for i in predicted_array[0].numpy()]
+    prediction = (
+        "".join([str(elem) for elem in outputs])
+        .replace("<start>", "")
+        .replace("<end>", "")
+    )
+
+    return prediction
+
+
 class DECIMER_Predictor(tf.Module):
     """This is a class which takes care of inference. It loads the saved checkpoint and the necessary
     tokenizers. The inference begins with the start token (<start>) and ends when the end token(<end>)
     is met. This class can only work with tf.Tensor objects. The strings shoul gets transformed into np.arrays
     before feeding them into this class.
     """
 
@@ -112,18 +124,17 @@
 
         Args:
             Decoded_image (tf.Tensor[tf.int32]): Input array in tf.Eagertensor format.
 
         Returns:
             output (tf.Tensor[tf.int64]): predicted output as an array.
         """
-
         assert isinstance(Decoded_image, tf.Tensor)
         if len(Decoded_image.shape) == 0:
-            Decoded_image = Decoded_image[tf.newaxis]
+            sentence = Decoded_image[tf.newaxis]
 
         _image_batch = tf.expand_dims(Decoded_image, 0)
         _image_embedding = encoder(_image_batch, training=False)
 
         start_token = tf.cast(
             tf.convert_to_tensor([tokenizer.word_index["<start>"]]), tf.int32
         )
```

### Comparing `decimer-2.2.2/DECIMER/Transformer_decoder.py` & `decimer-2.3.0/DECIMER/Transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/Utils/Create_TFrecord_From_pickles.py` & `decimer-2.3.0/DECIMER/Utils/Create_TFrecord_From_pickles.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/Utils/Create_image_tokenizer.py` & `decimer-2.3.0/DECIMER/Utils/Create_image_tokenizer.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/__init__.py` & `decimer-2.3.0/DECIMER/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-DECIMER V2.2.2 Python Package.
+DECIMER V2.3.0 Python Package.
 ============================
 
 This repository contains DECIMER-V2,Deep lEarning for Chemical ImagE Recognition) project
 was launched to address the OCSR problem with the latest computational intelligence methods
 to provide an automated open-source software solution.
 
 
@@ -19,15 +19,15 @@
 print(SMILES)
 
 For comments, bug reports or feature ideas,
 please raise a issue on the Github repository.
 
 """
 
-__version__ = "2.2.2"
+__version__ = "2.3.0"
 
 __all__ = [
     "DECIMER",
 ]
 
 
 from .decimer import predict_SMILES
```

### Comparing `decimer-2.2.2/DECIMER/config.py` & `decimer-2.3.0/DECIMER/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,153 +1,142 @@
 # Network configuration file
 import tensorflow as tf
 import efficientnet.tfkeras as efn
 import DECIMER.Efficient_Net_encoder
 import DECIMER.Transformer_decoder
 from PIL import Image, ImageEnhance
 from pillow_heif import register_heif_opener
+from pathlib import Path
 import numpy as np
 import io
 import cv2
 import pystow
-import pathlib
 import zipfile
 
+
 TARGET_DTYPE = tf.float32
 
 
 def resize_byratio(image):
     """
     This function takes a Pillow Image object and will resize the image by 512 x 512
     To upscale or to downscale the image LANCZOS resampling method is used.
     with the new pillow version the antialias is turned on when using LANCZOS.
-    ___
-    im: PIL.Image
-    ___
-    output: PIL.Image
+    Args: PIL.Image
+    Returns: PIL.Image
     """
     maxwidth = 512
     ratio = maxwidth / max(image.width, image.height)
     new_size = int((float(image.width) * ratio)), int((float(image.height) * ratio))
     resized_image = image.resize(new_size, resample=Image.LANCZOS)
     return resized_image
 
 
-def central_square_image(im):
+def central_square_image(image):
     """
     This function takes a Pillow Image object and will add white padding
     so that the image has a square shape with the width/height of the longest side
     of the original image.
-    ___
-    im: PIL.Image
-    ___
-    output: PIL.Image
+    Args: PIL.Image
+    Returns: PIL.Image
     """
-    max_wh = int(1.2 * max(im.size))
+    max_wh = int(1.2 * max(image.size))
     # If the new image is smaller than 299x299, then let's paste it into an empty image
     # of that size instead of distorting it later while resizing.
     if max_wh < 512:
         max_wh = 512
-    new_im = Image.new(im.mode, (max_wh, max_wh), "white")
+    new_im = Image.new(image.mode, (max_wh, max_wh), "white")
     paste_pos = (
-        int((new_im.size[0] - im.size[0]) / 2),
-        int((new_im.size[1] - im.size[1]) / 2),
+        int((new_im.size[0] - image.size[0]) / 2),
+        int((new_im.size[1] - image.size[1]) / 2),
     )
-    new_im.paste(im, paste_pos)
+    new_im.paste(image, paste_pos)
     return new_im
 
 
-def delete_empty_borders(im):
+def delete_empty_borders(image):
     """This function takes a Pillow Image object, converts it to grayscale and
     deletes white space at the borders.
-    ___
-    im: PIL.Image
-    ___
-    output: PIL.Image
+    Args: PIL.Image
+    Returns: PIL.Image
     """
-    im = np.asarray(im.convert("L"))
-    mask = im > 200
+    image = np.asarray(image.convert("L"))
+    mask = image > 200
     rows = np.flatnonzero((~mask).sum(axis=1))
     cols = np.flatnonzero((~mask).sum(axis=0))
-    crop = im[rows.min() : rows.max() + 1, cols.min() : cols.max() + 1]
+    crop = image[rows.min() : rows.max() + 1, cols.min() : cols.max() + 1]
     return Image.fromarray(crop)
 
 
-def PIL_im_to_BytesIO(im):
+def PIL_im_to_BytesIO(image):
     """
     Convert pillow image to io.BytesIO object
-    ___
-    im: PIL.Image
-    ___
-    Output: io.BytesIO object with the image data
+    Args: PIL.Image
+    Returns: io.BytesIO object with the image data
     """
     output = io.BytesIO()
-    im.save(output, format="PNG")
+    image.save(output, format="PNG")
     return output
 
 
 def HEIF_to_pillow(image_path: str):
     """
     Converts Apple's HEIF format to useful pillow object
-    ___
-    image_path (str): path of input image
-    ___
-    Output: PIL.Image
+    Returns: image_path (str): path of input image
+    Returns: PIL.Image
     """
     register_heif_opener()
 
     heif_file = Image.open(image_path).convert("RGBA")
     return heif_file
 
 
 def remove_transparent(image_path: str):
     """
     Removes the transparent layer from a PNG image with an alpha channel
-    ___
-    image_path (str): path of input image
-    ___
-    Output: PIL.Image
+    Args: image_path (str): path of input image
+    Returns: PIL.Image
     """
-    if pathlib.Path(image_path).suffix == ".HEIC":
-        png = HEIF_to_pillow(image_path)
-    else:
+    try:
         png = Image.open(image_path).convert("RGBA")
+    except Exception as e:
+        if type(e).__name__ == "UnidentifiedImageError":
+            png = HEIF_to_pillow(image_path)
+        else:
+            print(e)
+            raise Exception
 
     background = Image.new("RGBA", png.size, (255, 255, 255))
 
     alpha_composite = Image.alpha_composite(background, png)
 
     return alpha_composite
 
 
 def get_bnw_image(image):
     """
     converts images to black and white
-    ___
-    image: PIL.Image
-    ___
-    Output: PIL.Image
+    Args: PIL.Image
+    Returns: PIL.Image
     """
 
     im_np = np.asarray(image)
     grayscale = cv2.cvtColor(im_np, cv2.COLOR_BGR2GRAY)
     # (thresh, im_bw) = cv2.threshold(grayscale, 128, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
     im_pil = Image.fromarray(grayscale)
     enhancer = ImageEnhance.Contrast(im_pil)
-    im_output = enhancer.enhance(1.2)
+    im_output = enhancer.enhance(1.8)
     return im_output
 
 
 def increase_contrast(image):
     """
     This function increases the contrast of an image input.
-    ___
-    image: PIL.Image
-    ___
-    Output: PIL.Image
+    Args: PIL.Image
+    Returns: PIL.Image
     """
 
     # Get brightness range
     min = np.min(image)
     max = np.max(image)
 
     # Use LUT to convert image values
@@ -159,35 +148,41 @@
     # Apply LUT and return image
     return Image.fromarray(LUT[image])
 
 
 def get_resize(image):
     """
     This function used to decide how to resize a given image without losing much information.
-    ___
-    image: PIL.Image
-    ___
-    Output: PIL.Image
+    Args: PIL.Image
+    Returns: PIL.Image
     """
-
     width, height = image.size
 
     # Checks the image size and resizes using the LANCOS image resampling
     if (width == height) and (width < 512):
         image = image.resize((512, 512), resample=Image.LANCZOS)
-
     elif width >= 512 or height >= 512:
         return image
-
     else:
         image = resize_byratio(image)
 
     return image
 
 
+def increase_brightness(image):
+    """
+    This function adjusts the brightness of the given image.
+    Args: PIL.Image
+    Returns: PIL.Image
+    """
+    enhancer = ImageEnhance.Brightness(image)
+    image = enhancer.enhance(1.6)
+    return image
+
+
 def decode_image(image_path: str):
     """
     Loads an image and preprocesses the input image in several steps to get the image ready for DECIMER input.
 
     Args:
         image_path (str): path of input image
 
@@ -196,14 +191,15 @@
     """
     img = remove_transparent(image_path)
     img = increase_contrast(img)
     img = get_bnw_image(img)
     img = get_resize(img)
     img = delete_empty_borders(img)
     img = central_square_image(img)
+    img = increase_brightness(img)
     img = PIL_im_to_BytesIO(img)
     img = tf.image.decode_png(img.getvalue(), channels=3)
     img = tf.image.resize(img, (512, 512), method="gaussian", antialias=True)
     img = efn.preprocess_input(img)
     return img
 
 
@@ -378,7 +374,10 @@
         print("Downloading trained model to " + str(model_path))
         model_path = pystow.ensure("DECIMER-V2", url=model_url)
         print(model_path)
     if verbose > 0:
         print("... done downloading trained model!")
         with zipfile.ZipFile(model_path.as_posix(), "r") as zip_ref:
             zip_ref.extractall(model_path.parent.as_posix())
+        # Delete zipfile after downloading
+        if Path(model_path).exists():
+            Path(model_path).unlink()
```

### Comparing `decimer-2.2.2/DECIMER/decimer.py` & `decimer-2.3.0/DECIMER/decimer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 for gpu in gpus:
     tf.config.experimental.set_memory_growth(gpu, True)
 
 # Set path
 default_path = pystow.join("DECIMER-V2")
 
 # model download location
-model_url = "https://zenodo.org/record/7624994/files/models.zip"
+model_url = "https://zenodo.org/record/8093783/files/models.zip"
 model_path = str(default_path) + "/DECIMER_model/"
 
 # download models to a default location
 if (
     os.path.exists(model_path)
-    and os.stat(model_path + "/saved_model.pb").st_size != 28425789
+    and os.stat(model_path + "/saved_model.pb").st_size != 28073658
 ):
     shutil.rmtree(model_path)
     config.download_trained_weights(model_url, default_path)
 elif not os.path.exists(model_path):
     config.download_trained_weights(model_url, default_path)
 
 # Load important pickle files which consists the tokenizers and the maxlength setting
```

### Comparing `decimer-2.2.2/DECIMER/efficientnetv2/effnetv2_configs.py` & `decimer-2.3.0/DECIMER/efficientnetv2/effnetv2_configs.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/efficientnetv2/effnetv2_model.py` & `decimer-2.3.0/DECIMER/efficientnetv2/effnetv2_model.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/efficientnetv2/hparams.py` & `decimer-2.3.0/DECIMER/efficientnetv2/hparams.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/efficientnetv2/utils.py` & `decimer-2.3.0/DECIMER/efficientnetv2/utils.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/DECIMER/utils.py` & `decimer-2.3.0/DECIMER/utils.py`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/LICENSE` & `decimer-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/PKG-INFO` & `decimer-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: decimer
-Version: 2.2.2
-Summary: DECIMER 2.0: Deep Learning for Chemical Image Recognition using Efficient-Net V2 + Transformer
+Version: 2.3.0
+Summary: DECIMER 2.3: Deep Learning for Chemical Image Recognition using Efficient-Net V2 + Transformer
 Home-page: https://github.com/Kohulan/DECIMER-Image_Transformer
 Author: Kohulan Rajan
 Author-email: kohulan.rajan@uni-jena.de
-Maintainer: Kohulan Rajan
-Maintainer-email: kohulan.rajan@uni-jena.de
+Maintainer: Kohulan Rajan, Otto Brinkhaus 
+Maintainer-email: kohulan.rajan@uni-jena.de, otto.brinkhaus@uni-jena.de
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -139,7 +140,9 @@
 - A web application implementation is available at [decimer.ai](https://decimer.ai), implemented by [Otto Brinkhaus](https://github.com/OBrink)
 
 
 ## Research Group
 [![GitHub Logo](https://github.com/Kohulan/DECIMER-Image-to-SMILES/blob/master/assets/CheminfGit.png)](https://cheminf.uni-jena.de)
 
 ![Alt](https://repobeats.axiom.co/api/embed/bf532b7ac0d34137bdea8fbb82986828f86de065.svg "Repobeats analytics image")
+
+
```

### Comparing `decimer-2.2.2/README.md` & `decimer-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `decimer-2.2.2/decimer.egg-info/PKG-INFO` & `decimer-2.3.0/decimer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: decimer
-Version: 2.2.2
-Summary: DECIMER 2.0: Deep Learning for Chemical Image Recognition using Efficient-Net V2 + Transformer
+Version: 2.3.0
+Summary: DECIMER 2.3: Deep Learning for Chemical Image Recognition using Efficient-Net V2 + Transformer
 Home-page: https://github.com/Kohulan/DECIMER-Image_Transformer
 Author: Kohulan Rajan
 Author-email: kohulan.rajan@uni-jena.de
-Maintainer: Kohulan Rajan
-Maintainer-email: kohulan.rajan@uni-jena.de
+Maintainer: Kohulan Rajan, Otto Brinkhaus 
+Maintainer-email: kohulan.rajan@uni-jena.de, otto.brinkhaus@uni-jena.de
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -139,7 +140,9 @@
 - A web application implementation is available at [decimer.ai](https://decimer.ai), implemented by [Otto Brinkhaus](https://github.com/OBrink)
 
 
 ## Research Group
 [![GitHub Logo](https://github.com/Kohulan/DECIMER-Image-to-SMILES/blob/master/assets/CheminfGit.png)](https://cheminf.uni-jena.de)
 
 ![Alt](https://repobeats.axiom.co/api/embed/bf532b7ac0d34137bdea8fbb82986828f86de065.svg "Repobeats analytics image")
+
+
```

### Comparing `decimer-2.2.2/setup.py` & `decimer-2.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 #!/usr/bin/env python
 
 import setuptools
+import platform
+
+if (
+    platform.processor() == "arm" or platform.processor() == "i386"
+) and platform.system() == "Darwin":
+    tensorflow_os = "tensorflow-macos>=2.10.0"
+else:
+    tensorflow_os = "tensorflow==2.12.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="decimer",
-    version="2.2.2",
+    version="2.3.0",
     author="Kohulan Rajan",
     author_email="kohulan.rajan@uni-jena.de",
-    maintainer="Kohulan Rajan",
-    maintainer_email="kohulan.rajan@uni-jena.de",
-    description="DECIMER 2.0: Deep Learning for Chemical Image Recognition using Efficient-Net V2 + Transformer",
+    maintainer="Kohulan Rajan, Otto Brinkhaus ",
+    maintainer_email="kohulan.rajan@uni-jena.de, otto.brinkhaus@uni-jena.de",
+    description="DECIMER 2.3: Deep Learning for Chemical Image Recognition using Efficient-Net V2 + Transformer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kohulan/DECIMER-Image_Transformer",
     packages=setuptools.find_packages(),
     license="MIT",
     install_requires=[
-        "tensorflow==2.10.1",
+        tensorflow_os,
         "opencv-python",
         "pystow",
         "pillow-heif",
         "efficientnet",
     ],
     package_data={"DECIMER": ["repack/*.*", "efficientnetv2/*.*", "Utils/*.*"]},
     classifiers=[
```

