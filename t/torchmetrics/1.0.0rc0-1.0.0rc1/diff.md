# Comparing `tmp/torchmetrics-1.0.0rc0.tar.gz` & `tmp/torchmetrics-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmetrics-1.0.0rc0.tar", last modified: Thu May  4 08:32:42 2023, max compression
+gzip compressed data, was "torchmetrics-1.0.0rc1.tar", last modified: Thu Jun 29 07:21:23 2023, max compression
```

## Comparing `torchmetrics-1.0.0rc0.tar` & `torchmetrics-1.0.0rc1.tar`

### file list

```diff
@@ -1,315 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.616968 torchmetrics-1.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (122)    57735 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)    11352 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14423 2023-05-04 08:32:42.616968 torchmetrics-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12618 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.580968 torchmetrics-1.0.0rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/audio.txt
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/audio_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/classification_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/detection.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/detection_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/doctest.txt
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/image.txt
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/image_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/integrate.txt
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/multimodal.txt
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/nominal_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/text.txt
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/text_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements/visual.txt
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 08:32:42.620968 torchmetrics-1.0.0rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)    10482 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.572968 torchmetrics-1.0.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.580968 torchmetrics-1.0.0rc0/src/torchmetrics/
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20446 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.580968 torchmetrics-1.0.0rc0/src/torchmetrics/audio/
--rw-r--r--   0 runner    (1001) docker     (122)     1417 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     7053 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (122)     6220 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10268 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8283 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.584968 torchmetrics-1.0.0rc0/src/torchmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (122)     6508 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22429 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)    24174 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)    24496 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (122)    13382 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (122)    21540 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    12445 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (122)    17743 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    50096 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (122)    13732 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)    23104 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (122)    15194 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (122)    19471 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (122)    25306 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    44737 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    31828 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    16414 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)    25037 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    28089 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (122)    22633 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (122)    18488 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (122)    24239 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/classification/stat_scores.py
--rw-r--r--   0 runner    (1001) docker     (122)    27056 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.588968 torchmetrics-1.0.0rc0/src/torchmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13103 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)    40481 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.588968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/
--rw-r--r--   0 runner    (1001) docker     (122)     9383 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.588968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/
--rw-r--r--   0 runner    (1001) docker     (122)     1397 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     4883 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (122)     7998 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (122)     9500 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4265 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.592968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19949 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)    23489 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)    23096 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    16818 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (122)    11568 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (122)    27890 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (122)    11726 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    35583 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (122)    16824 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)    20746 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (122)    12314 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (122)    16462 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (122)    11430 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (122)    17938 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    35029 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    44124 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)    21068 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    26597 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (122)    18560 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (122)    22285 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (122)    49417 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.592968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/_panoptic_quality_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)     7903 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.596968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9254 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     4962 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (122)     4544 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     6488 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    15609 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.596968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/
--rw-r--r--   0 runner    (1001) docker     (122)     6009 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/alex.pth
--rw-r--r--   0 runner    (1001) docker     (122)    10811 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/squeeze.pth
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/vgg.pth
--rw-r--r--   0 runner    (1001) docker     (122)     5948 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4527 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (122)     4322 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (122)    21491 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (122)     6820 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/uqi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.596968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/multimodal/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.596968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7377 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6924 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     7151 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.596968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/cosine.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3174 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/minkowski.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.600968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (122)    15067 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     4367 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     6636 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.604968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.604968 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13994 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    20940 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7575 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (122)    26029 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (122)    17582 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (122)    17031 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    11800 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/helper_embedding_metric.py
--rw-r--r--   0 runner    (1001) docker     (122)    27937 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (122)    21939 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (122)    13088 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     9892 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (122)    23216 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.608968 torchmetrics-1.0.0rc0/src/torchmetrics/image/
--rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8942 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (122)    18782 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (122)     9038 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/inception.py
--rw-r--r--   0 runner    (1001) docker     (122)    14543 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/kid.py
--rw-r--r--   0 runner    (1001) docker     (122)     8044 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/lpip.py
--rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (122)    17135 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (122)    48424 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.608968 torchmetrics-1.0.0rc0/src/torchmetrics/multimodal/
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6642 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.608968 torchmetrics-1.0.0rc0/src/torchmetrics/nominal/
--rw-r--r--   0 runner    (1001) docker     (122)      909 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5928 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6228 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.612969 torchmetrics-1.0.0rc0/src/torchmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5312 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (122)     6589 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8352 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     7330 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     5889 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.612969 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9390 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     5938 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (122)     5937 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    16598 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     5903 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.616968 torchmetrics-1.0.0rc0/src/torchmetrics/text/
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8333 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    13939 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10472 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6357 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (122)    10137 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (122)     9393 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (122)     6742 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5208 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.616968 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      986 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34594 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/compute.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5863 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    12694 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/utilities/prints.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.616968 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8494 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/bootstrapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     7154 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/classwise.py
--rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (122)     9090 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (122)    14623 2023-05-04 08:32:39.000000 torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 08:32:42.580968 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14423 2023-05-04 08:32:42.000000 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11955 2023-05-04 08:32:42.000000 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 08:32:42.000000 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 08:32:42.000000 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-05-04 08:32:42.000000 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-04 08:32:42.000000 torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.411015 torchmetrics-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)    59995 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (122)    11352 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14423 2023-06-29 07:21:23.411015 torchmetrics-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12618 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.363009 torchmetrics-1.0.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/audio.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/audio_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/classification_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/detection.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/detection_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/doctest.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/image.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/image_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/integrate.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/multimodal.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/nominal_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/text.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/text_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements/visual.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 07:21:23.411015 torchmetrics-1.0.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10482 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.359009 torchmetrics-1.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.363009 torchmetrics-1.0.0rc1/src/torchmetrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8519 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25794 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.367009 torchmetrics-1.0.0rc1/src/torchmetrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6930 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10354 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.371010 torchmetrics-1.0.0rc1/src/torchmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)     6508 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22507 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24174 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24504 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16947 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13382 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20779 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12439 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17743 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50135 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13732 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23104 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15194 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19471 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16756 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25306 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44771 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31828 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16414 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25037 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28089 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22672 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18488 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24233 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/classification/stat_scores.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28697 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.375010 torchmetrics-1.0.0rc1/src/torchmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13103 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42258 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.375010 torchmetrics-1.0.0rc1/src/torchmetrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)     9451 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.375010 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4883 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9935 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9544 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4265 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.379011 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19836 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23489 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23096 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16811 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11565 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27882 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11726 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35505 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16824 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20633 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12314 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16566 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12297 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17938 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35008 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44120 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21068 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26597 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18470 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22285 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49419 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.379011 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/_panoptic_quality_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7903 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.383011 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9254 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5675 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4544 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6468 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15605 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.383011 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/
+-rw-r--r--   0 runner    (1001) docker     (122)     6009 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/alex.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    10811 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/squeeze.pth
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/vgg.pth
+-rw-r--r--   0 runner    (1001) docker     (122)     5948 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4527 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4322 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21491 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6859 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/uqi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.383011 torchmetrics-1.0.0rc1/src/torchmetrics/functional/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.383011 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7377 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6924 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7151 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.387012 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3174 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/minkowski.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.391012 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15169 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.391012 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.395013 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13994 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21026 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7573 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26029 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17557 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17030 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11809 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/helper_embedding_metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27937 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21951 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13118 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9892 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23230 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.399013 torchmetrics-1.0.0rc1/src/torchmetrics/image/
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18782 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9034 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/inception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14539 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/kid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8075 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17135 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50879 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.399013 torchmetrics-1.0.0rc1/src/torchmetrics/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6615 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.399013 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5928 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6228 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.403014 torchmetrics-1.0.0rc1/src/torchmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5312 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6589 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8352 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7330 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5889 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.403014 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9210 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5938 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5937 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16598 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5903 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.407014 torchmetrics-1.0.0rc1/src/torchmetrics/text/
+-rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8249 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13999 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10472 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6357 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10137 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9393 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6742 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5208 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.407014 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34594 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/compute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12681 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/utilities/prints.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.411015 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8473 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7161 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/running.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14623 2023-06-29 07:21:20.000000 torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:21:23.367009 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14423 2023-06-29 07:21:23.000000 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12205 2023-06-29 07:21:23.000000 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 07:21:23.000000 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 07:21:23.000000 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-29 07:21:23.000000 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-29 07:21:23.000000 torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/top_level.txt
```

### Comparing `torchmetrics-1.0.0rc0/CHANGELOG.md` & `torchmetrics-1.0.0rc1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 **Note: we move fast, but still we preserve 0.1 version (one feature release) back compatibility.**
 
 
 ## [unreleased] - 2022-MM-DD
 
 ### Added
 
+- Added new global arg `compute_with_cache` to control caching behaviour after `compute` method ([#1754](https://github.com/Lightning-AI/torchmetrics/pull/1754))
+
+
+- Added `ComplexScaleInvariantSignalNoiseRatio` for audio package ([#1785](https://github.com/Lightning-AI/torchmetrics/pull/1785))
+
+
+- Added `Running` wrapper for calculate running statistics ([#1752](https://github.com/Lightning-AI/torchmetrics/pull/1752))
+
+
 - Added`RelativeAverageSpectralError` and `RootMeanSquaredErrorUsingSlidingWindow` to image package ([#816](https://github.com/PyTorchLightning/metrics/pull/816))
 
 
 - Added support for `SpecificityAtSensitivity` Metric ([#1432](https://github.com/Lightning-AI/metrics/pull/1432))
 
 
 - Added support for plotting of metrics through `.plot()` method (
@@ -34,14 +43,15 @@
     [#1623](https://github.com/Lightning-AI/metrics/pull/1623),
     [#1638](https://github.com/Lightning-AI/metrics/pull/1638),
     [#1631](https://github.com/Lightning-AI/metrics/pull/1631),
     [#1650](https://github.com/Lightning-AI/metrics/pull/1650),
     [#1639](https://github.com/Lightning-AI/metrics/pull/1639),
     [#1660](https://github.com/Lightning-AI/metrics/pull/1660),
     [#1682](https://github.com/Lightning-AI/torchmetrics/pull/1682),
+    [#1786](https://github.com/Lightning-AI/torchmetrics/pull/1786),
 )
 
 
 - Added support for plotting of audio metrics through `.plot()` method ([#1434](https://github.com/Lightning-AI/metrics/pull/1434))
 
 
 - Added `classes` to output from `MAP` metric ([#1419](https://github.com/Lightning-AI/metrics/pull/1419))
@@ -95,16 +105,25 @@
 - Added multiple metrics to detection package ([#1284](https://github.com/Lightning-AI/metrics/pull/1284))
   * `IntersectionOverUnion`
   * `GeneralizedIntersectionOverUnion`
   * `CompleteIntersectionOverUnion`
   * `DistanceIntersectionOverUnion`
 
 
+- Added `MultitaskWrapper` to wrapper package ([#1762](https://github.com/Lightning-AI/torchmetrics/pull/1762))
+
+
+- Added `RelativeSquaredError` metric to regression package ([#1765](https://github.com/Lightning-AI/torchmetrics/pull/1765))
+
+
 ### Changed
 
+- Changed `permutation_invariant_training` to allow using a `'permutation-wise'` metric function ([#1794](https://github.com/Lightning-AI/metrics/pull/1794))
+
+
 - Changed `update_count` and `update_called` from private to public methods ([#1370](https://github.com/Lightning-AI/metrics/pull/1370))
 
 
 - Raise exception for invalid kwargs in Metric base class ([#1427](https://github.com/Lightning-AI/metrics/pull/1427))
 
 
 - Extend `EnumStr` raising `ValueError` for invalid value ([#1479](https://github.com/Lightning-AI/metrics/pull/1479))
@@ -171,14 +190,44 @@
 
 - Fixed `max_det_threshold` in MAP detection ([#1712](https://github.com/Lightning-AI/torchmetrics/pull/1712))
 
 
 - Fixed states being saved in metrics that use `register_buffer` ([#1728](https://github.com/Lightning-AI/torchmetrics/pull/1728))
 
 
+- Fixed states not being correctly synced and device transfered in `MeanAveragePrecision` for `iou_type="segm"` ([#1763](https://github.com/Lightning-AI/torchmetrics/pull/1763))
+
+
+- Fixed use of `prefix` and `postfix` in nested `MetricCollection` ([#1773](https://github.com/Lightning-AI/torchmetrics/pull/1773))
+
+
+- Fixed `ax` plotting logging in `MetricCollection ([#1783](https://github.com/Lightning-AI/torchmetrics/pull/1783))
+
+
+- Fixed lookup for punkt sources being downloaded in `RougeScore` ([#1789](https://github.com/Lightning-AI/torchmetrics/pull/1789))
+
+
+- Fixed integration with lightning for `CompositionalMetric` ([#1761](https://github.com/Lightning-AI/torchmetrics/pull/1761))
+
+
+- Fixed several bugs in `SpectralDistortionIndex` metric ([#1808](https://github.com/Lightning-AI/torchmetrics/pull/1808))
+
+
+- Fixed bug for corner cases in `MatthewsCorrCoef` ([#1812](https://github.com/Lightning-AI/torchmetrics/pull/1812))
+
+
+- Fixed support for half precision in `PearsonCorrCoef` ([#1819](https://github.com/Lightning-AI/torchmetrics/pull/1819))
+
+
+- Fixed number of bugs related to `average="macro"` in classification metrics ([#1821](https://github.com/Lightning-AI/torchmetrics/pull/1821))
+
+
+- Fixed off-by-one issue when `ignore_index = num_classes + 1` in Multiclass-jaccard ([#1860](https://github.com/Lightning-AI/torchmetrics/pull/1860))
+
+
 ## [0.11.4] - 2023-03-10
 
 ### Fixed
 
 - Fixed evaluation of `R2Score` with near constant target ([#1576](https://github.com/Lightning-AI/metrics/pull/1576))
 - Fixed dtype conversion when metric is submodule ([#1583](https://github.com/Lightning-AI/metrics/pull/1583))
 - Fixed bug related to `top_k>1` and `ignore_index!=None` in `StatScores` based metrics ([#1589](https://github.com/Lightning-AI/metrics/pull/1589))
```

### Comparing `torchmetrics-1.0.0rc0/CITATION.cff` & `torchmetrics-1.0.0rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/LICENSE` & `torchmetrics-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/MANIFEST.in` & `torchmetrics-1.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/PKG-INFO` & `torchmetrics-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -37,41 +37,41 @@
 Provides-Extra: visual
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc0/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc1/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
   <a href="#implementing-your-own-module-metric">Implementing a metric</a> •
   <a href="#build-in-metrics">Built-in metrics</a> •
-  <a href="https://torchmetrics.readthedocs.io/en/v1.0.0.rc0">Docs</a> •
+  <a href="https://torchmetrics.readthedocs.io/en/v1.0.0.rc1">Docs</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 ______________________________________________________________________
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchmetrics)](https://pypi.org/project/torchmetrics/)
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI Status](https://pepy.tech/badge/torchmetrics)](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing - complete](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.0.rc0)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.0.rc0)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.0.rc0/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.0.rc1)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.0.rc1)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.0.rc1/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -306,15 +306,15 @@
 acc = torchmetrics.functional.classification.multiclass_accuracy(
     preds, target, num_classes=5
 )
 ```
 
 ### Covered domains and example metrics
 
-In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.0.rc0all-metrics.html), which
+In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.0.rc1all-metrics.html), which
 convers the following domains:
 
 - Audio
 - Classification
 - Detection
 - Information Retrieval
 - Image
@@ -360,15 +360,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc0/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc1/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.0.0rc0/README.md` & `torchmetrics-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/setup.py` & `torchmetrics-1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/__about__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0.rc0"
+__version__ = "1.0.0.rc1"
 __author__ = "Lightning-AI et al."
 __author_email__ = "name@pytorchlightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2020-2023, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/torchmetrics"
 __docs__ = "PyTorch native Metrics"
 __docs_url__ = "https://torchmetrics.readthedocs.io/en/stable/"
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 r"""Root package info."""
 import logging as __logging
 import os
 
-from torchmetrics.__about__ import *  # noqa: F401, F403
+from torchmetrics.__about__ import *  # noqa: F403
 
 _logger = __logging.getLogger("torchmetrics")
 _logger.addHandler(__logging.StreamHandler())
 _logger.setLevel(__logging.INFO)
 
 _PACKAGE_ROOT = os.path.dirname(__file__)
 _PROJECT_ROOT = os.path.dirname(_PACKAGE_ROOT)
 
 from torchmetrics import functional  # noqa: E402
-from torchmetrics.aggregation import CatMetric, MaxMetric, MeanMetric, MinMetric, SumMetric  # noqa: E402
+from torchmetrics.aggregation import (  # noqa: E402
+    CatMetric,
+    MaxMetric,
+    MeanMetric,
+    MinMetric,
+    RunningMean,
+    RunningSum,
+    SumMetric,
+)
 from torchmetrics.audio._deprecated import _PermutationInvariantTraining as PermutationInvariantTraining  # noqa: E402
 from torchmetrics.audio._deprecated import (  # noqa: E402
     _ScaleInvariantSignalDistortionRatio as ScaleInvariantSignalDistortionRatio,
 )
 from torchmetrics.audio._deprecated import (  # noqa: E402
     _ScaleInvariantSignalNoiseRatio as ScaleInvariantSignalNoiseRatio,
 )
@@ -64,29 +72,36 @@
 from torchmetrics.image._deprecated import _SpectralDistortionIndex as SpectralDistortionIndex  # noqa: E402
 from torchmetrics.image._deprecated import (  # noqa: E402
     _StructuralSimilarityIndexMeasure as StructuralSimilarityIndexMeasure,
 )
 from torchmetrics.image._deprecated import _TotalVariation as TotalVariation  # noqa: E402
 from torchmetrics.image._deprecated import _UniversalImageQualityIndex as UniversalImageQualityIndex  # noqa: E402
 from torchmetrics.metric import Metric  # noqa: E402
-from torchmetrics.nominal import CramersV, PearsonsContingencyCoefficient, TheilsU, TschuprowsT  # noqa: E402
+from torchmetrics.nominal import (  # noqa: E402
+    CramersV,
+    FleissKappa,
+    PearsonsContingencyCoefficient,
+    TheilsU,
+    TschuprowsT,
+)
 from torchmetrics.regression import (  # noqa: E402
     ConcordanceCorrCoef,
     CosineSimilarity,
     ExplainedVariance,
     KendallRankCorrCoef,
     KLDivergence,
     LogCoshError,
     MeanAbsoluteError,
     MeanAbsolutePercentageError,
     MeanSquaredError,
     MeanSquaredLogError,
     MinkowskiDistance,
     PearsonCorrCoef,
     R2Score,
+    RelativeSquaredError,
     SpearmanCorrCoef,
     SymmetricMeanAbsolutePercentageError,
     TweedieDevianceScore,
     WeightedMeanAbsolutePercentageError,
 )
 from torchmetrics.retrieval._deprecated import _RetrievalFallOut as RetrievalFallOut  # noqa: E402
 from torchmetrics.retrieval._deprecated import _RetrievalHitRate as RetrievalHitRate  # noqa: E402
@@ -116,14 +131,15 @@
 from torchmetrics.text._deprecated import _WordInfoPreserved as WordInfoPreserved  # noqa: E402
 from torchmetrics.wrappers import (  # noqa: E402
     BootStrapper,
     ClasswiseWrapper,
     MetricTracker,
     MinMaxMetric,
     MultioutputWrapper,
+    MultitaskWrapper,
 )
 
 __all__ = [
     "functional",
     "Accuracy",
     "AUROC",
     "AveragePrecision",
@@ -143,14 +159,15 @@
     "TweedieDevianceScore",
     "ErrorRelativeGlobalDimensionlessSynthesis",
     "ExactMatch",
     "ExplainedVariance",
     "ExtendedEditDistance",
     "F1Score",
     "FBetaScore",
+    "FleissKappa",
     "HammingDistance",
     "HingeLoss",
     "JaccardIndex",
     "KendallRankCorrCoef",
     "KLDivergence",
     "LogCoshError",
     "MatchErrorRate",
@@ -160,32 +177,35 @@
     "MeanAbsolutePercentageError",
     "MeanMetric",
     "MeanSquaredError",
     "MeanSquaredLogError",
     "Metric",
     "MetricCollection",
     "MetricTracker",
+    "MinkowskiDistance",
     "MinMaxMetric",
     "MinMetric",
     "ModifiedPanopticQuality",
     "MultioutputWrapper",
+    "MultitaskWrapper",
     "MultiScaleStructuralSimilarityIndexMeasure",
     "PanopticQuality",
     "PearsonCorrCoef",
     "PearsonsContingencyCoefficient",
     "PermutationInvariantTraining",
     "Perplexity",
     "Precision",
     "PrecisionAtFixedRecall",
     "PrecisionRecallCurve",
     "PeakSignalNoiseRatio",
     "R2Score",
     "Recall",
     "RecallAtFixedPrecision",
     "RelativeAverageSpectralError",
+    "RelativeSquaredError",
     "RetrievalFallOut",
     "RetrievalHitRate",
     "RetrievalMAP",
     "RetrievalMRR",
     "RetrievalNormalizedDCG",
     "RetrievalPrecision",
     "RetrievalRecall",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/aggregation.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/aggregation.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from torch import Tensor
 
 from torchmetrics.metric import Metric
 from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.data import dim_zero_cat
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
+from torchmetrics.wrappers.running import Running
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["SumMetric.plot", "MeanMetric.plot", "MaxMetric.plot", "MinMetric.plot"]
 
 
 class BaseAggregator(Metric):
     """Base class for aggregation metrics.
@@ -86,15 +87,14 @@
                     raise ValueError(f"`nan_strategy` shall be float but you pass {self.nan_strategy}")
                 x[nans] = self.nan_strategy
 
         return x.float()
 
     def update(self, value: Union[float, Tensor]) -> None:
         """Overwrite in child class."""
-        pass
 
     def compute(self) -> Tensor:
         """Compute the aggregated value."""
         return self.value
 
 
 class MaxMetric(BaseAggregator):
@@ -564,7 +564,119 @@
             >>> metric = MeanMetric()
             >>> values = [ ]
             >>> for i in range(10):
             ...     values.append(metric([i, i+1]))
             >>> fig_, ax_ = metric.plot(values)
         """
         return self._plot(val, ax)
+
+
+class RunningMean(Running):
+    """Aggregate a stream of value into their mean over a running window.
+
+    Using this metric compared to `MeanMetric` allows for calculating metrics over a running window of values, instead
+    of the whole history of values. This is beneficial when you want to get a better estimate of the metric during
+    training and don't want to wait for the whole training to finish to get epoch level estimates.
+
+    As input to ``forward`` and ``update`` the metric accepts the following input
+
+    - ``value`` (:class:`~float` or :class:`~torch.Tensor`): a single float or an tensor of float values with
+      arbitary shape ``(...,)``.
+
+    As output of `forward` and `compute` the metric returns the following output
+
+    - ``agg`` (:class:`~torch.Tensor`): scalar float tensor with aggregated sum over all inputs received
+
+    Args:
+        window: The size of the running window.
+        nan_strategy: options:
+            - ``'error'``: if any `nan` values are encounted will give a RuntimeError
+            - ``'warn'``: if any `nan` values are encounted will give a warning and continue
+            - ``'ignore'``: all `nan` values are silently removed
+            - a float: if a float is provided will impude any `nan` values with this value
+
+        kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
+
+    Raises:
+        ValueError:
+            If ``nan_strategy`` is not one of ``error``, ``warn``, ``ignore`` or a float
+
+    Example:
+        >>> from torch import tensor
+        >>> from torchmetrics.aggregation import RunningMean
+        >>> metric = RunningMean(window=3)
+        >>> for i in range(6):
+        ...     current_val = metric(tensor([i]))
+        ...     running_val = metric.compute()
+        ...     total_val = tensor(sum(list(range(i+1)))) / (i+1)  # total mean over all samples
+        ...     print(f"{current_val=}, {running_val=}, {total_val=}")
+        current_val=tensor(0.), running_val=tensor(0.), total_val=tensor(0.)
+        current_val=tensor(1.), running_val=tensor(0.5000), total_val=tensor(0.5000)
+        current_val=tensor(2.), running_val=tensor(1.), total_val=tensor(1.)
+        current_val=tensor(3.), running_val=tensor(2.), total_val=tensor(1.5000)
+        current_val=tensor(4.), running_val=tensor(3.), total_val=tensor(2.)
+        current_val=tensor(5.), running_val=tensor(4.), total_val=tensor(2.5000)
+    """
+
+    def __init__(
+        self,
+        window: int = 5,
+        nan_strategy: Union[str, float] = "warn",
+        **kwargs: Any,
+    ) -> None:
+        super().__init__(base_metric=MeanMetric(nan_strategy=nan_strategy, **kwargs), window=window)
+
+
+class RunningSum(Running):
+    """Aggregate a stream of value into their sum over a running window.
+
+    Using this metric compared to `MeanMetric` allows for calculating metrics over a running window of values, instead
+    of the whole history of values. This is beneficial when you want to get a better estimate of the metric during
+    training and don't want to wait for the whole training to finish to get epoch level estimates.
+
+    As input to ``forward`` and ``update`` the metric accepts the following input
+
+    - ``value`` (:class:`~float` or :class:`~torch.Tensor`): a single float or an tensor of float values with
+      arbitary shape ``(...,)``.
+
+    As output of `forward` and `compute` the metric returns the following output
+
+    - ``agg`` (:class:`~torch.Tensor`): scalar float tensor with aggregated sum over all inputs received
+
+    Args:
+        window: The size of the running window.
+        nan_strategy: options:
+            - ``'error'``: if any `nan` values are encounted will give a RuntimeError
+            - ``'warn'``: if any `nan` values are encounted will give a warning and continue
+            - ``'ignore'``: all `nan` values are silently removed
+            - a float: if a float is provided will impude any `nan` values with this value
+
+        kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
+
+    Raises:
+        ValueError:
+            If ``nan_strategy`` is not one of ``error``, ``warn``, ``ignore`` or a float
+
+    Example:
+        >>> from torch import tensor
+        >>> from torchmetrics.aggregation import RunningSum
+        >>> metric = RunningSum(window=3)
+        >>> for i in range(6):
+        ...     current_val = metric(tensor([i]))
+        ...     running_val = metric.compute()
+        ...     total_val = tensor(sum(list(range(i+1))))  # total sum over all samples
+        ...     print(f"{current_val=}, {running_val=}, {total_val=}")
+        current_val=tensor(0.), running_val=tensor(0.), total_val=tensor(0)
+        current_val=tensor(1.), running_val=tensor(1.), total_val=tensor(1)
+        current_val=tensor(2.), running_val=tensor(3.), total_val=tensor(3)
+        current_val=tensor(3.), running_val=tensor(6.), total_val=tensor(6)
+        current_val=tensor(4.), running_val=tensor(9.), total_val=tensor(10)
+        current_val=tensor(5.), running_val=tensor(12.), total_val=tensor(15)
+    """
+
+    def __init__(
+        self,
+        window: int = 5,
+        nan_strategy: Union[str, float] = "warn",
+        **kwargs: Any,
+    ) -> None:
+        super().__init__(base_metric=SumMetric(nan_strategy=nan_strategy, **kwargs), window=window)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.audio.pit import PermutationInvariantTraining
 from torchmetrics.audio.sdr import ScaleInvariantSignalDistortionRatio, SignalDistortionRatio
-from torchmetrics.audio.snr import ScaleInvariantSignalNoiseRatio, SignalNoiseRatio
+from torchmetrics.audio.snr import (
+    ComplexScaleInvariantSignalNoiseRatio,
+    ScaleInvariantSignalNoiseRatio,
+    SignalNoiseRatio,
+)
 from torchmetrics.utilities.imports import _PESQ_AVAILABLE, _PYSTOI_AVAILABLE
 
 __all__ = [
     "PermutationInvariantTraining",
     "ScaleInvariantSignalDistortionRatio",
     "SignalDistortionRatio",
     "ScaleInvariantSignalNoiseRatio",
     "SignalNoiseRatio",
+    "ComplexScaleInvariantSignalNoiseRatio",
 ]
 
 if _PESQ_AVAILABLE:
-    from torchmetrics.audio.pesq import PerceptualEvaluationSpeechQuality  # noqa: F401
+    from torchmetrics.audio.pesq import PerceptualEvaluationSpeechQuality
 
     __all__.append("PerceptualEvaluationSpeechQuality")
 
 if _PYSTOI_AVAILABLE:
-    from torchmetrics.audio.stoi import ShortTimeObjectiveIntelligibility  # noqa: F401
+    from torchmetrics.audio.stoi import ShortTimeObjectiveIntelligibility
 
     __all__.append("ShortTimeObjectiveIntelligibility")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/_deprecated.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> from torchmetrics.functional import scale_invariant_signal_noise_ratio
     >>> _ = torch.manual_seed(42)
     >>> preds = torch.randn(3, 2, 5) # [batch, spk, time]
     >>> target = torch.randn(3, 2, 5) # [batch, spk, time]
-    >>> pit = _PermutationInvariantTraining(scale_invariant_signal_noise_ratio, 'max')
+    >>> pit = _PermutationInvariantTraining(scale_invariant_signal_noise_ratio,
+    ...     mode="speaker-wise", eval_func="max")
     >>> pit(preds, target)
     tensor(-2.1065)
     """
 
     def __init__(
         self,
         metric_func: Callable,
+        mode: Literal["speaker-wise", "permutation-wise"] = "speaker-wise",
         eval_func: Literal["max", "min"] = "max",
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("PermutationInvariantTraining", "audio")
-        return super().__init__(metric_func=metric_func, eval_func=eval_func, **kwargs)
+        super().__init__(metric_func=metric_func, mode=mode, eval_func=eval_func, **kwargs)
 
 
 class _ScaleInvariantSignalDistortionRatio(ScaleInvariantSignalDistortionRatio):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> target = tensor([3.0, -0.5, 2.0, 7.0])
@@ -44,15 +46,15 @@
 
     def __init__(
         self,
         zero_mean: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("ScaleInvariantSignalDistortionRatio", "audio")
-        return super().__init__(zero_mean=zero_mean, **kwargs)
+        super().__init__(zero_mean=zero_mean, **kwargs)
 
 
 class _ScaleInvariantSignalNoiseRatio(ScaleInvariantSignalNoiseRatio):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> target = tensor([3.0, -0.5, 2.0, 7.0])
@@ -63,15 +65,15 @@
     """
 
     def __init__(
         self,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("ScaleInvariantSignalNoiseRatio", "audio")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class _SignalDistortionRatio(SignalDistortionRatio):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> g = torch.manual_seed(1)
@@ -80,29 +82,30 @@
     >>> sdr = _SignalDistortionRatio()
     >>> sdr(preds, target)
     tensor(-12.0589)
     >>> # use with pit
     >>> from torchmetrics.functional import signal_distortion_ratio
     >>> preds = torch.randn(4, 2, 8000)  # [batch, spk, time]
     >>> target = torch.randn(4, 2, 8000)
-    >>> pit = _PermutationInvariantTraining(signal_distortion_ratio, 'max')
+    >>> pit = _PermutationInvariantTraining(signal_distortion_ratio,
+    ...     mode="speaker-wise", eval_func="max")
     >>> pit(preds, target)
     tensor(-11.6051)
     """
 
     def __init__(
         self,
         use_cg_iter: Optional[int] = None,
         filter_length: int = 512,
         zero_mean: bool = False,
         load_diag: Optional[float] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("SignalDistortionRatio", "audio")
-        return super().__init__(
+        super().__init__(
             use_cg_iter=use_cg_iter, filter_length=filter_length, zero_mean=zero_mean, load_diag=load_diag, **kwargs
         )
 
 
 class _SignalNoiseRatio(SignalNoiseRatio):
     """Wrapper for deprecated import.
 
@@ -116,8 +119,8 @@
 
     def __init__(
         self,
         zero_mean: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("SignalNoiseRatio", "audio")
-        return super().__init__(zero_mean=zero_mean, **kwargs)
+        super().__init__(zero_mean=zero_mean, **kwargs)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/pesq.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/pesq.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     """
 
     sum_pesq: Tensor
     total: Tensor
     full_state_update: bool = False
     is_differentiable: bool = False
     higher_is_better: bool = True
-    plot_lower_bound: float = 1.0
+    plot_lower_bound: float = -0.5
     plot_upper_bound: float = 4.5
 
     def __init__(
         self,
         fs: int,
         mode: str,
         n_processes: int = 1,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/pit.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/pit.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,64 +40,76 @@
 
     As output of `forward` and `compute` the metric returns the following output
 
     - ``pesq`` (:class:`~torch.Tensor`): float scalar tensor with average PESQ value over samples
 
     Args:
         metric_func:
-            a metric function accept a batch of target and estimate,
-            i.e. ``metric_func(preds[:, i, ...], target[:, j, ...])``, and returns a batch of metric
-            tensors ``(batch,)``
+            a metric function accept a batch of target and estimate.
+
+            if `mode`==`'speaker-wise'`, then ``metric_func(preds[:, i, ...], target[:, j, ...])`` is called
+            and expected to return a batch of metric tensors ``(batch,)``;
+
+            if `mode`==`'permutation-wise'`, then ``metric_func(preds[:, p, ...], target[:, :, ...])`` is called,
+            where `p` is one possible permutation, e.g. [0,1] or [1,0] for 2-speaker case, and expected to return
+            a batch of metric tensors ``(batch,)``;
+        mode:
+            can be `'speaker-wise'` or `'permutation-wise'`.
         eval_func:
             the function to find the best permutation, can be 'min' or 'max', i.e. the smaller the better
             or the larger the better.
         kwargs: Additional keyword arguments for either the ``metric_func`` or distributed communication,
             see :ref:`Metric kwargs` for more info.
 
     Example:
         >>> import torch
         >>> from torchmetrics.audio import PermutationInvariantTraining
         >>> from torchmetrics.functional.audio import scale_invariant_signal_noise_ratio
         >>> _ = torch.manual_seed(42)
         >>> preds = torch.randn(3, 2, 5) # [batch, spk, time]
         >>> target = torch.randn(3, 2, 5) # [batch, spk, time]
-        >>> pit = PermutationInvariantTraining(scale_invariant_signal_noise_ratio, 'max')
+        >>> pit = PermutationInvariantTraining(scale_invariant_signal_noise_ratio,
+        ...     mode="speaker-wise", eval_func="max")
         >>> pit(preds, target)
         tensor(-2.1065)
     """
 
     full_state_update: bool = False
     is_differentiable: bool = True
     sum_pit_metric: Tensor
     total: Tensor
-    plot_lower_bound: float = -10.0
-    plot_upper_bound: float = 1.0
+    plot_lower_bound: Optional[float] = None
+    plot_upper_bound: Optional[float] = None
 
     def __init__(
         self,
         metric_func: Callable,
+        mode: Literal["speaker-wise", "permutation-wise"] = "speaker-wise",
         eval_func: Literal["max", "min"] = "max",
         **kwargs: Any,
     ) -> None:
         base_kwargs: Dict[str, Any] = {
             "dist_sync_on_step": kwargs.pop("dist_sync_on_step", False),
             "process_group": kwargs.pop("process_group", None),
             "dist_sync_fn": kwargs.pop("dist_sync_fn", None),
         }
         super().__init__(**base_kwargs)
         self.metric_func = metric_func
+        self.mode = mode
         self.eval_func = eval_func
         self.kwargs = kwargs
 
         self.add_state("sum_pit_metric", default=tensor(0.0), dist_reduce_fx="sum")
         self.add_state("total", default=tensor(0), dist_reduce_fx="sum")
 
     def update(self, preds: Tensor, target: Tensor) -> None:
         """Update state with predictions and targets."""
-        pit_metric = permutation_invariant_training(preds, target, self.metric_func, self.eval_func, **self.kwargs)[0]
+        pit_metric = permutation_invariant_training(
+            preds, target, self.metric_func, self.mode, self.eval_func, **self.kwargs
+        )[0]
 
         self.sum_pit_metric += pit_metric.sum()
         self.total += pit_metric.numel()
 
     def compute(self) -> Tensor:
         """Compute metric."""
         return self.sum_pit_metric / self.total
@@ -122,27 +134,29 @@
 
             >>> # Example plotting a single value
             >>> import torch
             >>> from torchmetrics.audio import PermutationInvariantTraining
             >>> from torchmetrics.functional.audio import scale_invariant_signal_noise_ratio
             >>> preds = torch.randn(3, 2, 5) # [batch, spk, time]
             >>> target = torch.randn(3, 2, 5) # [batch, spk, time]
-            >>> metric = PermutationInvariantTraining(scale_invariant_signal_noise_ratio, 'max')
+            >>> metric = PermutationInvariantTraining(scale_invariant_signal_noise_ratio,
+            ...     mode="speaker-wise", eval_func="max")
             >>> metric.update(preds, target)
             >>> fig_, ax_ = metric.plot()
 
         .. plot::
             :scale: 75
 
             >>> # Example plotting multiple values
             >>> import torch
             >>> from torchmetrics.audio import PermutationInvariantTraining
             >>> from torchmetrics.functional.audio import scale_invariant_signal_noise_ratio
             >>> preds = torch.randn(3, 2, 5) # [batch, spk, time]
             >>> target = torch.randn(3, 2, 5) # [batch, spk, time]
-            >>> metric = PermutationInvariantTraining(scale_invariant_signal_noise_ratio, 'max')
+            >>> metric = PermutationInvariantTraining(scale_invariant_signal_noise_ratio,
+            ...     mode="speaker-wise", eval_func="max")
             >>> values = [ ]
             >>> for _ in range(10):
             ...     values.append(metric(preds, target))
             >>> fig_, ax_ = metric.plot(values)
         """
         return self._plot(val, ax)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/sdr.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/sdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,26 +71,27 @@
         >>> sdr(preds, target)
         tensor(-12.0589)
         >>> # use with pit
         >>> from torchmetrics.audio import PermutationInvariantTraining
         >>> from torchmetrics.functional.audio import signal_distortion_ratio
         >>> preds = torch.randn(4, 2, 8000)  # [batch, spk, time]
         >>> target = torch.randn(4, 2, 8000)
-        >>> pit = PermutationInvariantTraining(signal_distortion_ratio, 'max')
+        >>> pit = PermutationInvariantTraining(signal_distortion_ratio,
+        ...     mode="speaker-wise", eval_func="max")
         >>> pit(preds, target)
         tensor(-11.6051)
     """
 
     sum_sdr: Tensor
     total: Tensor
     full_state_update: bool = False
     is_differentiable: bool = True
     higher_is_better: bool = True
-    plot_lower_bound: float = -20.0
-    plot_upper_bound: float = 1.0
+    plot_lower_bound: Optional[float] = None
+    plot_upper_bound: Optional[float] = None
 
     def __init__(
         self,
         use_cg_iter: Optional[int] = None,
         filter_length: int = 512,
         zero_mean: bool = False,
         load_diag: Optional[float] = None,
@@ -191,16 +192,16 @@
         tensor(18.4030)
     """
 
     is_differentiable = True
     higher_is_better = True
     sum_si_sdr: Tensor
     total: Tensor
-    plot_lower_bound: float = -40.0
-    plot_upper_bound: float = 20.0
+    plot_lower_bound: Optional[float] = None
+    plot_upper_bound: Optional[float] = None
 
     def __init__(
         self,
         zero_mean: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/snr.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/snr.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,21 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Optional, Sequence, Union
 
 from torch import Tensor, tensor
 
-from torchmetrics.functional.audio.snr import scale_invariant_signal_noise_ratio, signal_noise_ratio
+from torchmetrics.functional.audio.snr import (
+    complex_scale_invariant_signal_noise_ratio,
+    scale_invariant_signal_noise_ratio,
+    signal_noise_ratio,
+)
 from torchmetrics.metric import Metric
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
 if not _MATPLOTLIB_AVAILABLE:
-    __doctest_skip__ = ["SignalNoiseRatio.plot", "ScaleInvariantSignalNoiseRatio.plot"]
+    __doctest_skip__ = [
+        "SignalNoiseRatio.plot",
+        "ScaleInvariantSignalNoiseRatio.plot",
+        "ComplexScaleInvariantSignalNoiseRatio.plot",
+    ]
 
 
 class SignalNoiseRatio(Metric):
     r"""Calculate `Signal-to-noise ratio`_ (SNR_) meric for evaluating quality of audio.
 
     .. math::
         \text{SNR} = \frac{P_{signal}}{P_{noise}}
@@ -60,16 +68,16 @@
         tensor(16.1805)
     """
     full_state_update: bool = False
     is_differentiable: bool = True
     higher_is_better: bool = True
     sum_snr: Tensor
     total: Tensor
-    plot_lower_bound: float = -20.0
-    plot_upper_bound: float = 5.0
+    plot_lower_bound: Optional[float] = None
+    plot_upper_bound: Optional[float] = None
 
     def __init__(
         self,
         zero_mean: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
@@ -147,29 +155,30 @@
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
     Raises:
         TypeError:
             if target and preds have a different shape
 
     Example:
+        >>> import torch
         >>> from torch import tensor
         >>> from torchmetrics.audio import ScaleInvariantSignalNoiseRatio
         >>> target = tensor([3.0, -0.5, 2.0, 7.0])
         >>> preds = tensor([2.5, 0.0, 2.0, 8.0])
         >>> si_snr = ScaleInvariantSignalNoiseRatio()
         >>> si_snr(preds, target)
         tensor(15.0918)
     """
 
     is_differentiable = True
     sum_si_snr: Tensor
     total: Tensor
     higher_is_better = True
-    plot_lower_bound: float = -20.0
-    plot_upper_bound: float = 10.0
+    plot_lower_bound: Optional[float] = None
+    plot_upper_bound: Optional[float] = None
 
     def __init__(
         self,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
 
@@ -221,7 +230,116 @@
             >>> metric = ScaleInvariantSignalNoiseRatio()
             >>> values = [ ]
             >>> for _ in range(10):
             ...     values.append(metric(torch.rand(4), torch.rand(4)))
             >>> fig_, ax_ = metric.plot(values)
         """
         return self._plot(val, ax)
+
+
+class ComplexScaleInvariantSignalNoiseRatio(Metric):
+    """Calculate `Complex scale-invariant signal-to-noise ratio`_ (C-SI-SNR) metric for evaluating quality of audio.
+
+    As input to `forward` and `update` the metric accepts the following input
+
+    - ``preds`` (:class:`~torch.Tensor`): real/complex float tensor with shape ``(..., frequency, time, 2)``\
+        / ``(..., frequency, time)``
+
+    - ``target`` (: :class:`~torch.Tensor`): real/complex float tensor with shape ``(..., frequency, time, 2)``\
+        / ``(..., frequency, time)``
+
+    As output of `forward` and `compute` the metric returns the following output
+
+    - ``c_si_snr`` (: :class:`~torch.Tensor`): float scalar tensor with average C-SI-SNR value over samples
+
+    Args:
+        zero_mean: if to zero mean target and preds or not
+        kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
+
+    Raises:
+        ValueError:
+            If ``zero_mean`` is not an bool
+        TypeError:
+            If ``preds`` is not the shape (..., frequency, time, 2) (after being converted to real if it is complex).
+            If ``preds`` and ``target`` does not have the same shape.
+
+    Example:
+        >>> import torch
+        >>> from torch import tensor
+        >>> from torchmetrics.audio import ComplexScaleInvariantSignalNoiseRatio
+        >>> g = torch.manual_seed(1)
+        >>> preds = torch.randn((1,257,100,2))
+        >>> target = torch.randn((1,257,100,2))
+        >>> c_si_snr = ComplexScaleInvariantSignalNoiseRatio()
+        >>> c_si_snr(preds, target)
+        tensor(-63.4849)
+    """
+
+    is_differentiable = True
+    ci_snr_sum: Tensor
+    num: Tensor
+    higher_is_better = True
+    plot_lower_bound: Optional[float] = None
+    plot_upper_bound: Optional[float] = None
+
+    def __init__(
+        self,
+        zero_mean: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        super().__init__(**kwargs)
+        if not isinstance(zero_mean, bool):
+            raise ValueError(f"Expected argument `zero_mean` to be an bool, but got {zero_mean}")
+        self.zero_mean = zero_mean
+
+        self.add_state("ci_snr_sum", default=tensor(0.0), dist_reduce_fx="sum")
+        self.add_state("num", default=tensor(0), dist_reduce_fx="sum")
+
+    def update(self, preds: Tensor, target: Tensor) -> None:
+        """Update state with predictions and targets."""
+        v = complex_scale_invariant_signal_noise_ratio(preds=preds, target=target, zero_mean=self.zero_mean)
+
+        self.ci_snr_sum += v.sum()
+        self.num += v.numel()
+
+    def compute(self) -> Tensor:
+        """Compute metric."""
+        return self.ci_snr_sum / self.num
+
+    def plot(self, val: Union[Tensor, Sequence[Tensor], None] = None, ax: Optional[_AX_TYPE] = None) -> _PLOT_OUT_TYPE:
+        """Plot a single or multiple values from the metric.
+
+        Args:
+            val: Either a single result from calling `metric.forward` or `metric.compute` or a list of these results.
+                If no value is provided, will automatically call `metric.compute` and plot that result.
+            ax: An matplotlib axis object. If provided will add plot to that axis
+
+        Returns:
+            Figure and Axes object
+
+        Raises:
+            ModuleNotFoundError:
+                If `matplotlib` is not installed
+
+        .. plot::
+            :scale: 75
+
+            >>> # Example plotting a single value
+            >>> import torch
+            >>> from torchmetrics.audio import ComplexScaleInvariantSignalNoiseRatio
+            >>> metric = ComplexScaleInvariantSignalNoiseRatio()
+            >>> metric.update(torch.rand(1,257,100,2), torch.rand(1,257,100,2))
+            >>> fig_, ax_ = metric.plot()
+
+        .. plot::
+            :scale: 75
+
+            >>> # Example plotting multiple values
+            >>> import torch
+            >>> from torchmetrics.audio import ComplexScaleInvariantSignalNoiseRatio
+            >>> metric = ComplexScaleInvariantSignalNoiseRatio()
+            >>> values = [ ]
+            >>> for _ in range(10):
+            ...     values.append(metric(torch.rand(1,257,100,2), torch.rand(1,257,100,2)))
+            >>> fig_, ax_ = metric.plot(values)
+        """
+        return self._plot(val, ax)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/audio/stoi.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/audio/stoi.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         tensor(-0.0100)
     """
     sum_stoi: Tensor
     total: Tensor
     full_state_update: bool = False
     is_differentiable: bool = False
     higher_is_better: bool = True
-    plot_lower_bound: float = -20.0
-    plot_upper_bound: float = 5.0
+    plot_lower_bound: float = 0.0
+    plot_upper_bound: float = 1.0
 
     def __init__(
         self,
         fs: int,
         extended: bool = False,
         **kwargs: Any,
     ) -> None:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/accuracy.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
     As output to ``forward`` and ``compute`` the metric returns the following output:
 
         - ``ba`` (:class:`~torch.Tensor`): If ``multidim_average`` is set to ``global``, metric returns a scalar value.
           If ``multidim_average`` is set to ``samplewise``, the metric returns ``(N,)`` vector consisting of a scalar
           value per sample.
 
+    Additional dimension ``...`` will be flattened into the batch dimension.
+
     Args:
         threshold: Threshold for transforming probability to binary {0,1} predictions
         multidim_average:
             Defines how additionally dimensions ``...`` should be handled. Should be one of the following:
 
             - ``global``: Additional dimensions are flatted along the batch dimension
             - ``samplewise``: Statistic will be calculated independently for each sample on the ``N`` axis.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/auroc.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/average_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/average_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             >>> fig_, ax_ = metric.plot(values)
 
         """
         return self._plot(val, ax)
 
 
 class MulticlassAveragePrecision(MulticlassPrecisionRecallCurve):
-    r"""Compute the average precision (AP) score for binary tasks.
+    r"""Compute the average precision (AP) score for multiclass tasks.
 
     The AP score summarizes a precision-recall curve as an weighted mean of precisions at each threshold, with the
     difference in recall from the previous threshold as weight:
 
     .. math::
         AP = \sum_{n} (R_n - R_{n-1}) P_n
 
@@ -303,15 +303,15 @@
             ...     values.append(metric(torch.randn(20, 3), torch.randint(3, (20,))))
             >>> fig_, ax_ = metric.plot(values)
         """
         return self._plot(val, ax)
 
 
 class MultilabelAveragePrecision(MultilabelPrecisionRecallCurve):
-    r"""Compute the average precision (AP) score for binary tasks.
+    r"""Compute the average precision (AP) score for multilabel tasks.
 
     The AP score summarizes a precision-recall curve as an weighted mean of precisions at each threshold, with the
     difference in recall from the previous threshold as weight:
 
     .. math::
         AP = \sum_{n} (R_n - R_{n-1}) P_n
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/calibration_error.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/calibration_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
     ``task`` argument to either ``'binary'`` or ``'multiclass'``. See the documentation of
     :mod:`BinaryCalibrationError` and :mod:`MulticlassCalibrationError` for the specific details of
     each argument influence and examples.
     """
 
     def __new__(
         cls,
-        task: Literal["binary", "multiclass"] = None,
+        task: Literal["binary", "multiclass"],
         n_bins: int = 15,
         norm: Literal["l1", "l2", "max"] = "l1",
         num_classes: Optional[int] = None,
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
@@ -369,8 +369,8 @@
         kwargs.update({"n_bins": n_bins, "norm": norm, "ignore_index": ignore_index, "validate_args": validate_args})
         if task == ClassificationTaskNoMultilabel.BINARY:
             return BinaryCalibrationError(**kwargs)
         if task == ClassificationTaskNoMultilabel.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             return MulticlassCalibrationError(num_classes, **kwargs)
-        return None
+        raise ValueError(f"Not handled value: {task}")  # this is for compliant of mypy
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/cohen_kappa.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/confusion_matrix.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/confusion_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,19 @@
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~torch.Tensor`): An int or float tensor of shape ``(N, ...)``. If preds is a floating point
       tensor with values outside [0,1] range we consider the input to be logits and will auto apply sigmoid per
       element. Addtionally, we convert to int tensor with thresholding using the value in ``threshold``.
     - ``target`` (:class:`~torch.Tensor`): An int tensor of shape ``(N, ...)``.
 
-    .. note::
-       Additional dimension ``...`` will be flattened into the batch dimension.
-
     As output to ``forward`` and ``compute`` the metric returns the following output:
 
-    - ``bcm`` (:class:`~torch.Tensor`): A tensor containing a ``(2, 2)`` matrix
+    - ``confusion_matrix`` (:class:`~torch.Tensor`): A tensor containing a ``(2, 2)`` matrix
+
+    Additional dimension ``...`` will be flattened into the batch dimension.
 
     Args:
         threshold: Threshold for transforming probability to binary (0,1) predictions
         ignore_index:
             Specifies a target value that is ignored and does not contribute to the metric calculation
         normalize: Normalization mode for confusion matrix. Choose from:
 
@@ -175,35 +174,17 @@
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~torch.Tensor`): An int or float tensor of shape ``(N, ...)``. If preds is a floating point
       tensor with values outside [0,1] range we consider the input to be logits and will auto apply sigmoid per
       element. Addtionally, we convert to int tensor with thresholding using the value in ``threshold``.
     - ``target`` (:class:`~torch.Tensor`): An int tensor of shape ``(N, ...)``.
 
-    .. note::
-       Additional dimension ``...`` will be flattened into the batch dimension.
-
     As output to ``forward`` and ``compute`` the metric returns the following output:
 
-    - ``bcm`` (:class:`~torch.Tensor`): A tensor containing a ``(2, 2)`` matrix
-
-    ---
-
-    As input to 'update' the metric accepts the following input:
-
-    - ``preds``: ``(N, ...)`` (int tensor) or ``(N, C, ..)`` (float tensor). If preds is a floating point
-      we apply ``torch.argmax`` along the ``C`` dimension to automatically convert probabilities/logits into
-      an int tensor.
-    - ``target`` (int tensor): ``(N, ...)``
-
-    Additional dimension ``...`` will be flattened into the batch dimension.
-
-    As output of 'compute' the metric returns the following output:
-
-    - ``confusion matrix``: [num_classes, num_classes] matrix
+    - ``confusion_matrix``: [num_classes, num_classes] matrix
 
     Args:
         num_classes: Integer specifing the number of classes
         ignore_index:
             Specifies a target value that is ignored and does not contribute to the metric calculation
         normalize: Normalization mode for confusion matrix. Choose from:
 
@@ -318,16 +299,14 @@
     As input to 'update' the metric accepts the following input:
 
     - ``preds`` (int or float tensor): ``(N, C, ...)``. If preds is a floating point tensor with values outside
       [0,1] range we consider the input to be logits and will auto apply sigmoid per element. Addtionally,
       we convert to int tensor with thresholding using the value in ``threshold``.
     - ``target`` (int tensor): ``(N, C, ...)``
 
-    Additional dimension ``...`` will be flattened into the batch dimension.
-
     As output of 'compute' the metric returns the following output:
 
     - ``confusion matrix``: [num_labels,2,2] matrix
 
     Args:
         num_classes: Integer specifing the number of labels
         threshold: Threshold for transforming probability to binary (0,1) predictions
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/dice.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/dice.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
         if average == "macro" and (not num_classes or num_classes < 1):
             raise ValueError("When you set `average` as 'macro', you have to provide the number of classes.")
 
         if num_classes and ignore_index is not None and (not ignore_index < num_classes or num_classes == 1):
             raise ValueError(f"The `ignore_index` {ignore_index} is not valid for inputs with {num_classes} classes")
 
-        default: Callable = lambda: []
+        default: Callable = list
         reduce_fn: Optional[str] = "cat"
         if mdmc_average != "samplewise" and average != "samples":
             if average == "micro":
                 zeros_shape = []
             elif average == "macro":
                 zeros_shape = [num_classes]
             else:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/exact_match.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/f_beta.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/f_beta.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,17 @@
             _multilabel_fbeta_score_arg_validation(beta, num_labels, threshold, average, multidim_average, ignore_index)
         self.validate_args = validate_args
         self.beta = beta
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
-        return _fbeta_reduce(tp, fp, tn, fn, self.beta, average=self.average, multidim_average=self.multidim_average)
+        return _fbeta_reduce(
+            tp, fp, tn, fn, self.beta, average=self.average, multidim_average=self.multidim_average, multilabel=True
+        )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/group_fairness.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/group_fairness.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/hamming.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/hinge.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/jaccard.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/matthews_corrcoef.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/matthews_corrcoef.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         >>> matthews_corrcoef = MatthewsCorrCoef(task='binary')
         >>> matthews_corrcoef(preds, target)
         tensor(0.5774)
     """
 
     def __new__(
         cls,
-        task: Literal["binary", "multiclass", "multilabel"] = None,
+        task: Literal["binary", "multiclass", "multilabel"],
         threshold: float = 0.5,
         num_classes: Optional[int] = None,
         num_labels: Optional[int] = None,
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
@@ -398,8 +398,8 @@
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             return MulticlassMatthewsCorrCoef(num_classes, **kwargs)
         if task == ClassificationTask.MULTILABEL:
             if not isinstance(num_labels, int):
                 raise ValueError(f"`num_labels` is expected to be `int` but `{type(num_labels)} was passed.`")
             return MultilabelMatthewsCorrCoef(num_labels, threshold, **kwargs)
-        return None
+        raise ValueError(f"Not handled value: {task}")  # this is for compliant of mypy
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/precision_fixed_recall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/precision_recall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/precision_recall.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
         return _precision_recall_reduce(
-            "precision", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average
+            "precision", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average, multilabel=True
         )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
@@ -815,15 +815,15 @@
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
         return _precision_recall_reduce(
-            "recall", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average
+            "recall", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average, multilabel=True
         )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/precision_recall_curve.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/ranking.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/recall_fixed_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/roc.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/specificity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/specificity.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,17 @@
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
-        return _specificity_reduce(tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average)
+        return _specificity_reduce(
+            tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average, multilabel=True
+        )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/specificity_sensitivity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/classification/stat_scores.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/classification/stat_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self,
         size: int,
         multidim_average: Literal["global", "samplewise"] = "global",
     ) -> None:
         """Initialize the states for the different statistics."""
         default: Union[Callable[[], list], Callable[[], Tensor]]
         if multidim_average == "samplewise":
-            default = lambda: []
+            default = list
             dist_reduce_fx = "cat"
         else:
             default = lambda: torch.zeros(size, dtype=torch.long)
             dist_reduce_fx = "sum"
 
         self.add_state("tp", default(), dist_reduce_fx=dist_reduce_fx)
         self.add_state("fp", default(), dist_reduce_fx=dist_reduce_fx)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/collections.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # this is just a bypass for this module name collision with build-in one
 from collections import OrderedDict
 from copy import deepcopy
-from typing import Any, Dict, Hashable, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Hashable, Iterable, Iterator, List, Optional, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module, ModuleDict
+from typing_extensions import Literal
 
 from torchmetrics.metric import Metric
 from torchmetrics.utilities import rank_zero_warn
-from torchmetrics.utilities.data import _flatten_dict, allclose
+from torchmetrics.utilities.data import allclose
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE, plot_single_or_multi_val
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["MetricCollection.plot", "MetricCollection.plot_all"]
 
 
@@ -172,36 +173,34 @@
     @torch.jit.unused
     def forward(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Call forward for each metric sequentially.
 
         Positional arguments (args) will be passed to every metric in the collection, while keyword arguments (kwargs)
         will be filtered based on the signature of the individual metric.
         """
-        res = {k: m(*args, **m._filter_kwargs(**kwargs)) for k, m in self.items(keep_base=True, copy_state=False)}
-        res = _flatten_dict(res)
-        return {self._set_name(k): v for k, v in res.items()}
+        return self._compute_and_reduce("forward", *args, **kwargs)
 
     def update(self, *args: Any, **kwargs: Any) -> None:
         """Call update for each metric sequentially.
 
         Positional arguments (args) will be passed to every metric in the collection, while keyword arguments (kwargs)
         will be filtered based on the signature of the individual metric.
         """
         # Use compute groups if already initialized and checked
         if self._groups_checked:
-            for _, cg in self._groups.items():
+            for cg in self._groups.values():
                 # only update the first member
                 m0 = getattr(self, cg[0])
                 m0.update(*args, **m0._filter_kwargs(**kwargs))
             if self._state_is_copy:
                 # If we have deep copied state inbetween updates, reestablish link
                 self._compute_groups_create_state_ref()
                 self._state_is_copy = False
         else:  # the first update always do per metric to form compute groups
-            for _, m in self.items(keep_base=True, copy_state=False):
+            for m in self.values(copy_state=False):
                 m_kwargs = m._filter_kwargs(**kwargs)
                 m.update(*args, **m_kwargs)
 
             if self._enable_compute_groups:
                 self._merge_compute_groups()
                 # create reference between states
                 self._compute_groups_create_state_ref()
@@ -271,34 +270,68 @@
         """Create reference between metrics in the same compute group.
 
         Args:
             copy: If `True` the metric state will between members will be copied instead
                 of just passed by reference
         """
         if not self._state_is_copy:
-            for _, cg in self._groups.items():
+            for cg in self._groups.values():
                 m0 = getattr(self, cg[0])
                 for i in range(1, len(cg)):
                     mi = getattr(self, cg[i])
                     for state in m0._defaults:
                         m0_state = getattr(m0, state)
                         # Determine if we just should set a reference or a full copy
                         setattr(mi, state, deepcopy(m0_state) if copy else m0_state)
-                    setattr(mi, "_update_count", deepcopy(m0._update_count) if copy else m0._update_count)
+                    mi._update_count = deepcopy(m0._update_count) if copy else m0._update_count
         self._state_is_copy = copy
 
     def compute(self) -> Dict[str, Any]:
         """Compute the result for each metric in the collection."""
-        res = {k: m.compute() for k, m in self.items(keep_base=True, copy_state=False)}
-        res = _flatten_dict(res)
-        return {self._set_name(k): v for k, v in res.items()}
+        return self._compute_and_reduce("compute")
+
+    def _compute_and_reduce(
+        self, method_name: Literal["compute", "forward"], *args: Any, **kwargs: Any
+    ) -> Dict[str, Any]:
+        """Compute result from collection and reduce into a single dictionary.
+
+        Args:
+            method_name: The method to call on each metric in the collection.
+                Should be either `compute` or `forward`.
+            args: Positional arguments to pass to each metric (if method_name is `forward`)
+            kwargs: Keyword arguments to pass to each metric (if method_name is `forward`)
+
+        Raises:
+            ValueError:
+                If method_name is not `compute` or `forward`.
+
+        """
+        result = {}
+        for k, m in self.items(keep_base=True, copy_state=False):
+            if method_name == "compute":
+                res = m.compute()
+            elif method_name == "forward":
+                res = m(*args, **m._filter_kwargs(**kwargs))
+            else:
+                raise ValueError("method_name should be either 'compute' or 'forward', but got {method_name}")
+
+            if isinstance(res, dict):
+                for key, v in res.items():
+                    if hasattr(m, "prefix") and m.prefix is not None:
+                        key = f"{m.prefix}{key}"
+                    if hasattr(m, "postfix") and m.postfix is not None:
+                        key = f"{key}{m.postfix}"
+                    result[key] = v
+            else:
+                result[k] = res
+        return {self._set_name(k): v for k, v in result.items()}
 
     def reset(self) -> None:
         """Call reset for each metric sequentially."""
-        for _, m in self.items(keep_base=True, copy_state=False):
+        for m in self.values(copy_state=False):
             m.reset()
         if self._enable_compute_groups and self._groups_checked:
             # reset state reference
             self._compute_groups_create_state_ref()
 
     def clone(self, prefix: Optional[str] = None, postfix: Optional[str] = None) -> "MetricCollection":
         """Make a copy of the metric collection.
@@ -313,15 +346,15 @@
             mc.prefix = self._check_arg(prefix, "prefix")
         if postfix:
             mc.postfix = self._check_arg(postfix, "postfix")
         return mc
 
     def persistent(self, mode: bool = True) -> None:
         """Change if metric states should be saved to its state_dict after initialization."""
-        for _, m in self.items(keep_base=True, copy_state=False):
+        for m in self.values(copy_state=False):
             m.persistent(mode)
 
     def add_metrics(
         self, metrics: Union[Metric, Sequence[Metric], Dict[str, Metric]], *additional_metrics: Metric
     ) -> None:
         """Add new metrics to Metric Collection."""
         if isinstance(metrics, Metric):
@@ -354,14 +387,16 @@
                         f"Value {metric} belonging to key {name} is not an instance of"
                         " `torchmetrics.Metric` or `torchmetrics.MetricCollection`"
                     )
                 if isinstance(metric, Metric):
                     self[name] = metric
                 else:
                     for k, v in metric.items(keep_base=False):
+                        v.postfix = metric.postfix
+                        v.prefix = metric.prefix
                         self[f"{name}_{k}"] = v
         elif isinstance(metrics, Sequence):
             for metric in metrics:
                 if not isinstance(metric, (Metric, MetricCollection)):
                     raise ValueError(
                         f"Input {metric} to `MetricCollection` is not a instance of"
                         " `torchmetrics.Metric` or `torchmetrics.MetricCollection`"
@@ -369,17 +404,22 @@
                 if isinstance(metric, Metric):
                     name = metric.__class__.__name__
                     if name in self:
                         raise ValueError(f"Encountered two metrics both named {name}")
                     self[name] = metric
                 else:
                     for k, v in metric.items(keep_base=False):
+                        v.postfix = metric.postfix
+                        v.prefix = metric.prefix
                         self[k] = v
         else:
-            raise ValueError("Unknown input to MetricCollection.")
+            raise ValueError(
+                "Unknown input to MetricCollection. Expected, `Metric`, `MetricCollection` or `dict`/`sequence` of the"
+                f" previous, but got {metrics}"
+            )
 
         self._groups_checked = False
         if self._enable_compute_groups:
             self._init_compute_groups()
         else:
             self._groups = {}
 
@@ -415,14 +455,18 @@
 
     def _to_renamed_ordered_dict(self) -> OrderedDict:
         od = OrderedDict()
         for k, v in self._modules.items():
             od[self._set_name(k)] = v
         return od
 
+    def __iter__(self) -> Iterator[str]:
+        """Return an iterator over the keys of the MetricDict."""
+        return iter(self.keys())
+
     # TODO: redefine this as native python dict
     def keys(self, keep_base: bool = False) -> Iterable[Hashable]:
         r"""Return an iterable of the ModuleDict key.
 
         Args:
             keep_base: Whether to add prefix/postfix on the items collection.
         """
@@ -481,15 +525,15 @@
 
     def set_dtype(self, dst_type: Union[str, torch.dtype]) -> "MetricCollection":
         """Transfer all metric state to specific dtype. Special version of standard `type` method.
 
         Arguments:
             dst_type (type or string): the desired type.
         """
-        for _, m in self.items(keep_base=True, copy_state=False):
+        for m in self.values(copy_state=False):
             m.set_dtype(dst_type)
         return self
 
     def plot(
         self,
         val: Optional[Union[Dict, Sequence[Dict]]] = None,
         ax: Optional[Union[_AX_TYPE, Sequence[_AX_TYPE]]] = None,
@@ -549,19 +593,16 @@
         if not isinstance(together, bool):
             raise ValueError(f"Expected argument `together` to be a boolean, but got {type(together)}")
         if ax is not None:
             if together and not isinstance(ax, _AX_TYPE):
                 raise ValueError(
                     f"Expected argument `ax` to be a matplotlib axis object, but got {type(ax)} when `together=True`"
                 )
-            if (
-                not together
-                and not isinstance(ax, Sequence)
-                and not all(isinstance(a, _AX_TYPE) for a in ax)
-                and len(ax) != len(self)
+            if not together and not (
+                isinstance(ax, Sequence) and all(isinstance(a, _AX_TYPE) for a in ax) and len(ax) == len(self)
             ):
                 raise ValueError(
                     f"Expected argument `ax` to be a sequence of matplotlib axis objects with the same length as the "
                     f"number of metrics in the collection, but got {type(ax)} with len {len(ax)} when `together=False`"
                 )
 
         val = val or self.compute()
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/_deprecated.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self,
         things: Collection[int],
         stuffs: Collection[int],
         allow_unknown_preds_category: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("ModifiedPanopticQuality", "detection")
-        return super().__init__(
+        super().__init__(
             things=things, stuffs=stuffs, allow_unknown_preds_category=allow_unknown_preds_category, **kwargs
         )
 
 
 class _PanopticQuality(PanopticQuality):
     """Wrapper for deprecated import.
 
@@ -51,10 +51,10 @@
         self,
         things: Collection[int],
         stuffs: Collection[int],
         allow_unknown_preds_category: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("PanopticQuality", "detection")
-        return super().__init__(
+        super().__init__(
             things=things, stuffs=stuffs, allow_unknown_preds_category=allow_unknown_preds_category, **kwargs
         )
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/ciou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/ciou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/diou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/diou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/giou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/giou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/helpers.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/iou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/mean_ap.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/mean_ap.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch
+import torch.distributed as dist
 from torch import IntTensor, Tensor
 
 from torchmetrics.detection.helpers import _fix_empty_tensors, _input_validator
 from torchmetrics.metric import Metric
 from torchmetrics.utilities.data import _cumsum
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE, _PYCOCOTOOLS_AVAILABLE, _TORCHVISION_GREATER_EQUAL_0_8
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
@@ -39,28 +40,27 @@
     mask_utils = None
     __doctest_skip__ = ["MeanAveragePrecision.plot", "MeanAveragePrecision"]
 
 
 log = logging.getLogger(__name__)
 
 
-def compute_area(input: List[Any], iou_type: str = "bbox") -> Tensor:
+def compute_area(inputs: List[Any], iou_type: str = "bbox") -> Tensor:
     """Compute area of input depending on the specified iou_type.
 
     Default output for empty input is :class:`~torch.Tensor`
     """
-    if len(input) == 0:
+    if len(inputs) == 0:
         return Tensor([])
 
     if iou_type == "bbox":
-        return box_area(torch.stack(input))
+        return box_area(torch.stack(inputs))
     if iou_type == "segm":
-        input = [{"size": i[0], "counts": i[1]} for i in input]
-        area = torch.tensor(mask_utils.area(input).astype("float"))
-        return area
+        inputs = [{"size": i[0], "counts": i[1]} for i in inputs]
+        return torch.tensor(mask_utils.area(inputs).astype("float"))
 
     raise Exception(f"IOU type {iou_type} is not supported")
 
 
 def compute_iou(
     det: List[Any],
     gt: List[Any],
@@ -240,15 +240,15 @@
             Option to enable per-class metrics for mAP and mAR_100. Has a performance impact.
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
     Raises:
         ModuleNotFoundError:
             If ``torchvision`` is not installed or version installed is lower than 0.8.0
         ModuleNotFoundError:
-            If ``iou_type`` is equal to ``seqm`` and ``pycocotools`` is not installed
+            If ``iou_type`` is equal to ``segm`` and ``pycocotools`` is not installed
         ValueError:
             If ``class_metrics`` is not a boolean
         ValueError:
             If ``preds`` is not of type (:class:`~List[Dict[str, Tensor]]`)
         ValueError:
             If ``target`` is not of type ``List[Dict[str, Tensor]]``
         ValueError:
@@ -866,14 +866,55 @@
         metrics.update(map_val)
         metrics.update(mar_val)
         metrics.map_per_class = map_per_class_values
         metrics[f"mar_{self.max_detection_thresholds[-1]}_per_class"] = mar_max_dets_per_class_values
         metrics.classes = torch.tensor(classes, dtype=torch.int)
         return metrics
 
+    def _apply(self, fn: Callable) -> torch.nn.Module:
+        """Custom apply function.
+
+        Excludes the detections and groundtruths from the casting when the iou_type is set to `segm` as the state is
+        no longer a tensor but a tuple.
+        """
+        if self.iou_type == "segm":
+            this = super()._apply(fn, exclude_state=("detections", "groundtruths"))
+        else:
+            this = super()._apply(fn)
+        return this
+
+    def _sync_dist(self, dist_sync_fn: Optional[Callable] = None, process_group: Optional[Any] = None) -> None:
+        """Custom sync function.
+
+        For the iou_type `segm` the detections and groundtruths are no longer tensors but tuples. Therefore, we need
+        to gather the list of tuples and then convert it back to a list of tuples.
+
+        """
+        super()._sync_dist(dist_sync_fn=dist_sync_fn, process_group=process_group)
+
+        if self.iou_type == "segm":
+            self.detections = self._gather_tuple_list(self.detections, process_group)
+            self.groundtruths = self._gather_tuple_list(self.groundtruths, process_group)
+
+    @staticmethod
+    def _gather_tuple_list(list_to_gather: List[Tuple], process_group: Optional[Any] = None) -> List[Any]:
+        """Gather a list of tuples over multiple devices."""
+        world_size = dist.get_world_size(group=process_group)
+        dist.barrier(group=process_group)
+
+        list_gathered = [None for _ in range(world_size)]
+        dist.all_gather_object(list_gathered, list_to_gather, group=process_group)
+
+        list_merged = []
+        for idx in range(len(list_gathered[0])):
+            for rank in range(world_size):
+                list_merged.append(list_gathered[rank][idx])
+
+        return list_merged
+
     def plot(
         self, val: Optional[Union[Dict[str, Tensor], Sequence[Dict[str, Tensor]]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
             val: Either a single result from calling `metric.forward` or `metric.compute` or a list of these results.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/detection/panoptic_qualities.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/detection/panoptic_qualities.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     _structural_similarity_index_measure as structural_similarity_index_measure,
 )
 from torchmetrics.functional.image._deprecated import _total_variation as total_variation
 from torchmetrics.functional.image._deprecated import _universal_image_quality_index as universal_image_quality_index
 from torchmetrics.functional.nominal import (
     cramers_v,
     cramers_v_matrix,
+    fleiss_kappa,
     pearsons_contingency_coefficient,
     pearsons_contingency_coefficient_matrix,
     theils_u,
     theils_u_matrix,
     tschuprows_t,
     tschuprows_t_matrix,
 )
@@ -96,14 +97,15 @@
     mean_absolute_error,
     mean_absolute_percentage_error,
     mean_squared_error,
     mean_squared_log_error,
     minkowski_distance,
     pearson_corrcoef,
     r2_score,
+    relative_squared_error,
     spearman_corrcoef,
     symmetric_mean_absolute_percentage_error,
     tweedie_deviance_score,
     weighted_mean_absolute_percentage_error,
 )
 from torchmetrics.functional.retrieval._deprecated import _retrieval_average_precision as retrieval_average_precision
 from torchmetrics.functional.retrieval._deprecated import _retrieval_fall_out as retrieval_fall_out
@@ -128,16 +130,16 @@
 from torchmetrics.functional.text._deprecated import _translation_edit_rate as translation_edit_rate
 from torchmetrics.functional.text._deprecated import _word_error_rate as word_error_rate
 from torchmetrics.functional.text._deprecated import _word_information_lost as word_information_lost
 from torchmetrics.functional.text._deprecated import _word_information_preserved as word_information_preserved
 from torchmetrics.utilities.imports import _TRANSFORMERS_AVAILABLE
 
 if _TRANSFORMERS_AVAILABLE:
-    from torchmetrics.functional.text._deprecated import _bert_score as bert_score  # noqa: F401
-    from torchmetrics.functional.text._deprecated import _infolm as infolm  # noqa: F401
+    from torchmetrics.functional.text._deprecated import _bert_score as bert_score
+    from torchmetrics.functional.text._deprecated import _infolm as infolm
 
 __all__ = [
     "accuracy",
     "auroc",
     "average_precision",
     "bleu_score",
     "calibration_error",
@@ -153,14 +155,15 @@
     "dice",
     "error_relative_global_dimensionless_synthesis",
     "exact_match",
     "explained_variance",
     "extended_edit_distance",
     "f1_score",
     "fbeta_score",
+    "fleiss_kappa",
     "hamming_distance",
     "hinge_loss",
     "image_gradients",
     "jaccard_index",
     "kendall_rank_corrcoef",
     "kl_divergence",
     "log_cosh_error",
@@ -186,14 +189,15 @@
     "pit_permutate",
     "precision",
     "precision_recall_curve",
     "peak_signal_noise_ratio",
     "r2_score",
     "recall",
     "relative_average_spectral_error",
+    "relative_squared_error",
     "retrieval_average_precision",
     "retrieval_fall_out",
     "retrieval_hit_rate",
     "retrieval_normalized_dcg",
     "retrieval_precision",
     "retrieval_r_precision",
     "retrieval_recall",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,35 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from torchmetrics.functional.audio.pit import permutation_invariant_training, pit_permutate  # noqa: F401
-from torchmetrics.functional.audio.sdr import (  # noqa: F401
-    scale_invariant_signal_distortion_ratio,
-    signal_distortion_ratio,
+from torchmetrics.functional.audio.pit import permutation_invariant_training, pit_permutate
+from torchmetrics.functional.audio.sdr import scale_invariant_signal_distortion_ratio, signal_distortion_ratio
+from torchmetrics.functional.audio.snr import (
+    complex_scale_invariant_signal_noise_ratio,
+    scale_invariant_signal_noise_ratio,
+    signal_noise_ratio,
 )
-from torchmetrics.functional.audio.snr import scale_invariant_signal_noise_ratio, signal_noise_ratio  # noqa: F401
 from torchmetrics.utilities.imports import _PESQ_AVAILABLE, _PYSTOI_AVAILABLE
 
-__all__ = []
+__all__ = [
+    "permutation_invariant_training",
+    "pit_permutate",
+    "scale_invariant_signal_distortion_ratio",
+    "signal_distortion_ratio",
+    "scale_invariant_signal_noise_ratio",
+    "signal_noise_ratio",
+    "complex_scale_invariant_signal_noise_ratio",
+]
 
 if _PESQ_AVAILABLE:
-    from torchmetrics.functional.audio.pesq import perceptual_evaluation_speech_quality  # noqa: F401
+    from torchmetrics.functional.audio.pesq import perceptual_evaluation_speech_quality
 
     __all__.append("perceptual_evaluation_speech_quality")
 
 if _PYSTOI_AVAILABLE:
-    from torchmetrics.functional.audio.stoi import short_time_objective_intelligibility  # noqa: F401
+    from torchmetrics.functional.audio.stoi import short_time_objective_intelligibility
 
     __all__.append("short_time_objective_intelligibility")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/_deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,34 +6,39 @@
 from torchmetrics.functional.audio.pit import permutation_invariant_training, pit_permutate
 from torchmetrics.functional.audio.sdr import scale_invariant_signal_distortion_ratio, signal_distortion_ratio
 from torchmetrics.functional.audio.snr import scale_invariant_signal_noise_ratio, signal_noise_ratio
 from torchmetrics.utilities.prints import _deprecated_root_import_func
 
 
 def _permutation_invariant_training(
-    preds: Tensor, target: Tensor, metric_func: Callable, eval_func: Literal["max", "min"] = "max", **kwargs: Any
+    preds: Tensor,
+    target: Tensor,
+    metric_func: Callable,
+    mode: Literal["speaker-wise", "permutation-wise"] = "speaker-wise",
+    eval_func: Literal["max", "min"] = "max",
+    **kwargs: Any
 ) -> Tuple[Tensor, Tensor]:
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> preds = tensor([[[-0.0579,  0.3560, -0.9604], [-0.1719,  0.3205,  0.2951]]])
     >>> target = tensor([[[ 1.0958, -0.1648,  0.5228], [-0.4100,  1.1942, -0.5103]]])
     >>> best_metric, best_perm = _permutation_invariant_training(
-    ...     preds, target, _scale_invariant_signal_distortion_ratio, 'max')
+    ...     preds, target, _scale_invariant_signal_distortion_ratio)
     >>> best_metric
     tensor([-5.1091])
     >>> best_perm
     tensor([[0, 1]])
     >>> pit_permutate(preds, best_perm)
     tensor([[[-0.0579,  0.3560, -0.9604],
              [-0.1719,  0.3205,  0.2951]]])
     """
     _deprecated_root_import_func("permutation_invariant_training", "audio")
     return permutation_invariant_training(
-        preds=preds, target=target, metric_func=metric_func, eval_func=eval_func, **kwargs
+        preds=preds, target=target, metric_func=metric_func, mode=mode, eval_func=eval_func, **kwargs
     )
 
 
 def _pit_permutate(preds: Tensor, perm: Tensor) -> Tensor:
     """Wrapper for deprecated import."""
     _deprecated_root_import_func("pit_permutate", "audio")
     return pit_permutate(preds=preds, perm=perm)
@@ -67,15 +72,15 @@
     >>> preds = torch.randn(8000)
     >>> target = torch.randn(8000)
     >>> _signal_distortion_ratio(preds, target)
     tensor(-12.0589)
     >>> # use with permutation_invariant_training
     >>> preds = torch.randn(4, 2, 8000)  # [batch, spk, time]
     >>> target = torch.randn(4, 2, 8000)
-    >>> best_metric, best_perm = _permutation_invariant_training(preds, target, _signal_distortion_ratio, 'max')
+    >>> best_metric, best_perm = _permutation_invariant_training(preds, target, _signal_distortion_ratio)
     >>> best_metric
     tensor([-11.6375, -11.4358, -11.7148, -11.6325])
     >>> best_perm
     tensor([[1, 0],
             [0, 1],
             [1, 0],
             [0, 1]])
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/pesq.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/pit.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/pit.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,25 +11,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from itertools import permutations
 from typing import Any, Callable, Tuple, Union
 from warnings import warn
 
+import numpy as np
 import torch
 from torch import Tensor
 from typing_extensions import Literal
 
+from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.imports import _SCIPY_AVAILABLE
 
 # _ps_dict: cache of permutations
 # it's necessary to cache it, otherwise it will consume a large amount of time
 _ps_dict: dict = {}  # _ps_dict[str(spk_num)+str(device)] = permutations
 
 
+def _gen_permutations(spk_num: int, device: torch.device) -> Tensor:
+    key = str(spk_num) + str(device)
+    if key not in _ps_dict:
+        # ps: all the permutations, shape [perm_num, spk_num]
+        # ps: In i-th permutation, the predcition corresponds to the j-th target is ps[j,i]
+        ps = torch.tensor(list(permutations(range(spk_num))), device=device)
+        _ps_dict[key] = ps
+    else:
+        ps = _ps_dict[key]  # all the permutations, shape [perm_num, spk_num]
+    return ps
+
+
 def _find_best_perm_by_linear_sum_assignment(
     metric_mtx: Tensor,
     eval_func: Union[torch.min, torch.max],
 ) -> Tuple[Tensor, Tensor]:
     """Solves the linear sum assignment problem.
 
     This implementation uses scipy and input is therefore transferred to cpu during calculations.
@@ -41,15 +55,15 @@
     Returns:
         best_metric: shape ``[batch]``
         best_perm: shape ``[batch, spk]``
     """
     from scipy.optimize import linear_sum_assignment
 
     mmtx = metric_mtx.detach().cpu()
-    best_perm = torch.tensor([linear_sum_assignment(pwm, eval_func == torch.max)[1] for pwm in mmtx])
+    best_perm = torch.tensor(np.array([linear_sum_assignment(pwm, eval_func == torch.max)[1] for pwm in mmtx]))
     best_perm = best_perm.to(metric_mtx.device)
     best_metric = torch.gather(metric_mtx, 2, best_perm[:, :, None]).mean([-1, -2])
     return best_metric, best_perm  # shape [batch], shape [batch, spk]
 
 
 def _find_best_perm_by_exhaustive_method(
     metric_mtx: Tensor,
@@ -67,108 +81,137 @@
     Returns:
         best_metric: shape ``[batch]``
         best_perm: shape ``[batch, spk]``
     """
     # create/read/cache the permutations and its indexes
     # reading from cache would be much faster than creating in CPU then moving to GPU
     batch_size, spk_num = metric_mtx.shape[:2]
-    key = str(spk_num) + str(metric_mtx.device)
-    if key not in _ps_dict:
-        # ps: all the permutations, shape [spk_num, perm_num]
-        # ps: In i-th permutation, the predcition corresponds to the j-th target is ps[j,i]
-        ps = torch.tensor(list(permutations(range(spk_num))), device=metric_mtx.device).T
-        _ps_dict[key] = ps
-    else:
-        ps = _ps_dict[key]  # all the permutations, shape [spk_num, perm_num]
+    ps = _gen_permutations(spk_num=spk_num, device=metric_mtx.device)  # [perm_num, spk_num]
 
     # find the metric of each permutation
-    perm_num = ps.shape[-1]
-    # shape [batch_size, spk_num, perm_num]
-    bps = ps[None, ...].expand(batch_size, spk_num, perm_num)
-    # shape [batch_size, spk_num, perm_num]
+    perm_num = ps.shape[0]
+    # shape of [batch_size, spk_num, perm_num]
+    bps = ps.T[None, ...].expand(batch_size, spk_num, perm_num)
+    # shape of [batch_size, spk_num, perm_num]
     metric_of_ps_details = torch.gather(metric_mtx, 2, bps)
-    # shape [batch_size, perm_num]
+    # shape of [batch_size, perm_num]
     metric_of_ps = metric_of_ps_details.mean(dim=1)
 
     # find the best metric and best permutation
     best_metric, best_indexes = eval_func(metric_of_ps, dim=1)
     best_indexes = best_indexes.detach()
-    best_perm = ps.T[best_indexes, :]
+    best_perm = ps[best_indexes, :]
     return best_metric, best_perm  # shape [batch], shape [batch, spk]
 
 
 def permutation_invariant_training(
-    preds: Tensor, target: Tensor, metric_func: Callable, eval_func: Literal["max", "min"] = "max", **kwargs: Any
+    preds: Tensor,
+    target: Tensor,
+    metric_func: Callable,
+    mode: Literal["speaker-wise", "permutation-wise"] = "speaker-wise",
+    eval_func: Literal["max", "min"] = "max",
+    **kwargs: Any,
 ) -> Tuple[Tensor, Tensor]:
     """Calculate `Permutation invariant training`_ (PIT).
 
     This metric can evaluate models for speaker independent multi-talker speech separation in a permutation
     invariant way.
 
     Args:
         preds: float tensor with shape ``(batch_size,num_speakers,...)``
         target: float tensor with shape ``(batch_size,num_speakers,...)``
-        metric_func: a metric function accept a batch of target and estimate,
-            i.e. ``metric_func(preds[:, i, ...], target[:, j, ...])``, and returns a batch of metric
-            tensors ``(batch,)``
+        metric_func: a metric function accept a batch of target and estimate.
+            if `mode`==`'speaker-wise'`, then ``metric_func(preds[:, i, ...], target[:, j, ...])`` is called
+            and expected to return a batch of metric tensors ``(batch,)``;
+
+            if `mode`==`'permutation-wise'`, then ``metric_func(preds[:, p, ...], target[:, :, ...])`` is called,
+            where `p` is one possible permutation, e.g. [0,1] or [1,0] for 2-speaker case, and expected to return
+            a batch of metric tensors ``(batch,)``;
+
+        mode: can be `'speaker-wise'` or `'permutation-wise'`.
         eval_func: the function to find the best permutation, can be ``'min'`` or ``'max'``,
             i.e. the smaller the better or the larger the better.
         kwargs: Additional args for metric_func
 
     Returns:
         Tuple of two float tensors. First tensor with shape ``(batch,)`` contains the best metric value for each sample
         and second tensor with shape ``(batch,)`` contains the best permutation.
 
     Example:
         >>> from torchmetrics.functional.audio import scale_invariant_signal_distortion_ratio
         >>> # [batch, spk, time]
         >>> preds = torch.tensor([[[-0.0579,  0.3560, -0.9604], [-0.1719,  0.3205,  0.2951]]])
         >>> target = torch.tensor([[[ 1.0958, -0.1648,  0.5228], [-0.4100,  1.1942, -0.5103]]])
         >>> best_metric, best_perm = permutation_invariant_training(
-        ...     preds, target, scale_invariant_signal_distortion_ratio, 'max')
+        ...     preds, target, scale_invariant_signal_distortion_ratio,
+        ...     mode="speaker-wise", eval_func="max")
         >>> best_metric
         tensor([-5.1091])
         >>> best_perm
         tensor([[0, 1]])
         >>> pit_permutate(preds, best_perm)
         tensor([[[-0.0579,  0.3560, -0.9604],
                  [-0.1719,  0.3205,  0.2951]]])
     """
     if preds.shape[0:2] != target.shape[0:2]:
         raise RuntimeError(
             "Predictions and targets are expected to have the same shape at the batch and speaker dimensions"
         )
     if eval_func not in ["max", "min"]:
         raise ValueError(f'eval_func can only be "max" or "min" but got {eval_func}')
+    if mode not in ["speaker-wise", "permutation-wise"]:
+        raise ValueError(f'mode can only be "speaker-wise" or "permutation-wise" but got {eval_func}')
     if target.ndim < 2:
         raise ValueError(f"Inputs must be of shape [batch, spk, ...], got {target.shape} and {preds.shape} instead")
 
+    eval_op = torch.max if eval_func == "max" else torch.min
+
     # calculate the metric matrix
     batch_size, spk_num = target.shape[0:2]
+
+    if mode == "permutation-wise":
+        perms = _gen_permutations(spk_num=spk_num, device=preds.device)  # [perm_num, spk_num]
+        perm_num = perms.shape[0]
+        # shape of ppreds and ptarget: [batch_size*perm_num, spk_num, ...]
+        ppreds = torch.index_select(preds, dim=1, index=perms.reshape(-1)).reshape(
+            batch_size * perm_num, *preds.shape[1:]
+        )
+        ptarget = target.repeat_interleave(repeats=perm_num, dim=0)
+        # shape of metric_of_ps [batch_size*perm_num] or [batch_size*perm_num, spk_num]
+        metric_of_ps = metric_func(ppreds, ptarget)
+        metric_of_ps = torch.mean(metric_of_ps.reshape(batch_size, len(perms), -1), dim=-1)
+        # find the best metric and best permutation
+        best_metric, best_indexes = eval_op(metric_of_ps, dim=1)
+        best_indexes = best_indexes.detach()
+        best_perm = perms[best_indexes, :]
+        return best_metric, best_perm
+
+    # speaker-wise
     metric_mtx = None
     for target_idx in range(spk_num):  # we have spk_num speeches in target in each sample
         for preds_idx in range(spk_num):  # we have spk_num speeches in preds in each sample
             if metric_mtx is not None:
                 metric_mtx[:, target_idx, preds_idx] = metric_func(
                     preds[:, preds_idx, ...], target[:, target_idx, ...], **kwargs
                 )
             else:
                 first_ele = metric_func(preds[:, preds_idx, ...], target[:, target_idx, ...], **kwargs)
                 metric_mtx = torch.empty((batch_size, spk_num, spk_num), dtype=first_ele.dtype, device=first_ele.device)
                 metric_mtx[:, target_idx, preds_idx] = first_ele
 
     # find best
-    op = torch.max if eval_func == "max" else torch.min
     if spk_num < 3 or not _SCIPY_AVAILABLE:
         if spk_num >= 3 and not _SCIPY_AVAILABLE:
-            warn(f"In pit metric for speaker-num {spk_num}>3, we recommend installing scipy for better performance")
+            rank_zero_warn(
+                f"In pit metric for speaker-num {spk_num}>3, we recommend installing scipy for better performance"
+            )
 
-        best_metric, best_perm = _find_best_perm_by_exhaustive_method(metric_mtx, op)
+        best_metric, best_perm = _find_best_perm_by_exhaustive_method(metric_mtx, eval_op)
     else:
-        best_metric, best_perm = _find_best_perm_by_linear_sum_assignment(metric_mtx, op)
+        best_metric, best_perm = _find_best_perm_by_linear_sum_assignment(metric_mtx, eval_op)
 
     return best_metric, best_perm
 
 
 def pit_permutate(preds: Tensor, perm: Tensor) -> Tensor:
     """Permutate estimate according to perm.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/sdr.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/sdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import torch
 from torch import Tensor
 
 # import or def the norm/solve function
 from torch.linalg import norm
 
+from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.checks import _check_same_shape
 from torchmetrics.utilities.imports import _FAST_BSS_EVAL_AVAILABLE
 
 solve = torch.linalg.solve
 
 if _FAST_BSS_EVAL_AVAILABLE:
     from fast_bss_eval.torch.cgd import toeplitz_conjugate_gradient
@@ -137,15 +138,15 @@
         >>> target = torch.randn(8000)
         >>> signal_distortion_ratio(preds, target)
         tensor(-12.0589)
         >>> # use with permutation_invariant_training
         >>> from torchmetrics.functional.audio import permutation_invariant_training
         >>> preds = torch.randn(4, 2, 8000)  # [batch, spk, time]
         >>> target = torch.randn(4, 2, 8000)
-        >>> best_metric, best_perm = permutation_invariant_training(preds, target, signal_distortion_ratio, 'max')
+        >>> best_metric, best_perm = permutation_invariant_training(preds, target, signal_distortion_ratio)
         >>> best_metric
         tensor([-11.6375, -11.4358, -11.7148, -11.6325])
         >>> best_perm
         tensor([[1, 0],
                 [0, 1],
                 [1, 0],
                 [0, 1]])
@@ -174,15 +175,15 @@
         r_0[..., 0] += load_diag
 
     if use_cg_iter is not None and _FAST_BSS_EVAL_AVAILABLE:
         # use preconditioned conjugate gradient
         sol = toeplitz_conjugate_gradient(r_0, b, n_iter=use_cg_iter)
     else:
         if use_cg_iter is not None and not _FAST_BSS_EVAL_AVAILABLE:
-            warnings.warn(
+            rank_zero_warn(
                 "The `use_cg_iter` parameter of `SDR` requires that `fast-bss-eval` is installed. "
                 "To make this this warning disappear, you could install `fast-bss-eval` using "
                 "`pip install fast-bss-eval` or set `use_cg_iter=None`. For this time, the solver "
                 "provided by Pytorch is used.",
                 UserWarning,
             )
         # regular matrix solver
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/snr.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/snr.py`

 * *Files 21% similar despite different names*

```diff
@@ -79,7 +79,49 @@
         >>> from torchmetrics.functional.audio import scale_invariant_signal_noise_ratio
         >>> target = torch.tensor([3.0, -0.5, 2.0, 7.0])
         >>> preds = torch.tensor([2.5, 0.0, 2.0, 8.0])
         >>> scale_invariant_signal_noise_ratio(preds, target)
         tensor(15.0918)
     """
     return scale_invariant_signal_distortion_ratio(preds=preds, target=target, zero_mean=True)
+
+
+def complex_scale_invariant_signal_noise_ratio(preds: Tensor, target: Tensor, zero_mean: bool = False) -> Tensor:
+    """`Complex scale-invariant signal-to-noise ratio`_ (C-SI-SNR).
+
+    Args:
+        preds: real/complex float tensor with shape ``(..., frequency, time, 2)``/``(..., frequency, time)``
+        target: real/complex float tensor with shape ``(..., frequency, time, 2)``/``(..., frequency, time)``
+        zero_mean: When set to True, the mean of all signals is subtracted prior to computation of the metrics
+
+    Returns:
+         Float tensor with shape ``(...,)`` of C-SI-SNR values per sample
+
+    Raises:
+        RuntimeError:
+            If ``preds`` is not the shape (..., frequency, time, 2) (after being converted to real if it is complex).
+            If ``preds`` and ``target`` does not have the same shape.
+
+    Example:
+        >>> import torch
+        >>> from torchmetrics.functional.audio import complex_scale_invariant_signal_noise_ratio
+        >>> g = torch.manual_seed(1)
+        >>> preds = torch.randn((1,257,100,2))
+        >>> target = torch.randn((1,257,100,2))
+        >>> complex_scale_invariant_signal_noise_ratio(preds, target)
+        tensor([-63.4849])
+    """
+    if preds.is_complex():
+        preds = torch.view_as_real(preds)
+    if target.is_complex():
+        target = torch.view_as_real(target)
+
+    if (preds.ndim < 3 or preds.shape[-1] != 2) or (target.ndim < 3 or target.shape[-1] != 2):
+        raise RuntimeError(
+            "Predictions and targets are expected to have the shape (..., frequency, time, 2),"
+            " but got {preds.shape} and {target.shape}."
+        )
+
+    preds = preds.reshape(*preds.shape[:-3], -1)
+    target = target.reshape(*target.shape[:-3], -1)
+
+    return scale_invariant_signal_distortion_ratio(preds=preds, target=target, zero_mean=zero_mean)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/audio/stoi.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/accuracy.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     _multiclass_stat_scores_tensor_validation,
     _multiclass_stat_scores_update,
     _multilabel_stat_scores_arg_validation,
     _multilabel_stat_scores_format,
     _multilabel_stat_scores_tensor_validation,
     _multilabel_stat_scores_update,
 )
-from torchmetrics.utilities.compute import _safe_divide
+from torchmetrics.utilities.compute import _adjust_weights_safe_divide, _safe_divide
 from torchmetrics.utilities.enums import ClassificationTask
 
 
 def _accuracy_reduce(
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
@@ -79,18 +79,15 @@
         if multilabel:
             fp = fp.sum(dim=0 if multidim_average == "global" else 1)
             tn = tn.sum(dim=0 if multidim_average == "global" else 1)
             return _safe_divide(tp + tn, tp + tn + fp + fn)
         return _safe_divide(tp, tp + fn)
 
     score = _safe_divide(tp + tn, tp + tn + fp + fn) if multilabel else _safe_divide(tp, tp + fn)
-    if average is None or average == "none":
-        return score
-    weights = tp + fn if average == "weighted" else torch.ones_like(score)
-    return _safe_divide(weights * score, weights.sum(-1, keepdim=True)).sum(-1)
+    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn)
 
 
 def binary_accuracy(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/auroc.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/average_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/calibration_error.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/calibration_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
     confidences, accuracies = _multiclass_calibration_error_update(preds, target)
     return _ce_compute(confidences, accuracies, n_bins, norm)
 
 
 def calibration_error(
     preds: Tensor,
     target: Tensor,
-    task: Literal["binary", "multiclass"] = None,
+    task: Literal["binary", "multiclass"],
     n_bins: int = 15,
     norm: Literal["l1", "l2", "max"] = "l1",
     num_classes: Optional[int] = None,
     ignore_index: Optional[int] = None,
     validate_args: bool = True,
 ) -> Tensor:
     r"""`Top-label Calibration Error`_.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/cohen_kappa.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/cohen_kappa.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         w_mat = w_mat.reshape(n_classes, n_classes)
     elif weights in ("linear", "quadratic"):
         w_mat = torch.zeros_like(confmat)
         w_mat += torch.arange(n_classes, dtype=w_mat.dtype, device=w_mat.device)
         w_mat = torch.abs(w_mat - w_mat.T) if weights == "linear" else torch.pow(w_mat - w_mat.T, 2.0)
     else:
         raise ValueError(
-            f"Received {weights} for argument ``weights`` but should be either" " None, 'linear' or 'quadratic'"
+            f"Received {weights} for argument ``weights`` but should be either None, 'linear' or 'quadratic'"
         )
     k = torch.sum(w_mat * confmat) / torch.sum(w_mat * expected)
     return 1 - k
 
 
 def _binary_cohen_kappa_arg_validation(
     threshold: float = 0.5,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/confusion_matrix.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/confusion_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     if ignore_index is None:
         check = torch.any((unique_values != 0) & (unique_values != 1))
     else:
         check = torch.any((unique_values != 0) & (unique_values != 1) & (unique_values != ignore_index))
     if check:
         raise RuntimeError(
             f"Detected the following values in `target`: {unique_values} but expected only"
-            f" the following values {[0,1] + [] if ignore_index is None else [ignore_index]}."
+            f" the following values {[0, 1] if ignore_index is None else [ignore_index]}."
         )
 
     # If preds is label tensor, also check that it only contains {0,1} values
     if not preds.is_floating_point():
         unique_values = torch.unique(preds)
         if torch.any((unique_values != 0) & (unique_values != 1)):
             raise RuntimeError(
@@ -453,15 +453,15 @@
     if ignore_index is None:
         check = torch.any((unique_values != 0) & (unique_values != 1))
     else:
         check = torch.any((unique_values != 0) & (unique_values != 1) & (unique_values != ignore_index))
     if check:
         raise RuntimeError(
             f"Detected the following values in `target`: {unique_values} but expected only"
-            f" the following values {[0,1] + [] if ignore_index is None else [ignore_index]}."
+            f" the following values {[0, 1] if ignore_index is None else [ignore_index]}."
         )
 
     # If preds is label tensor, also check that it only contains [0,1] values
     if not preds.is_floating_point():
         unique_values = torch.unique(preds)
         if torch.any((unique_values != 0) & (unique_values != 1)):
             raise RuntimeError(
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/dice.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/exact_match.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/f_beta.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/f_beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,41 +27,39 @@
     _multiclass_stat_scores_tensor_validation,
     _multiclass_stat_scores_update,
     _multilabel_stat_scores_arg_validation,
     _multilabel_stat_scores_format,
     _multilabel_stat_scores_tensor_validation,
     _multilabel_stat_scores_update,
 )
-from torchmetrics.utilities.compute import _safe_divide
+from torchmetrics.utilities.compute import _adjust_weights_safe_divide, _safe_divide
 from torchmetrics.utilities.enums import ClassificationTask
 
 
 def _fbeta_reduce(
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
     fn: Tensor,
     beta: float,
     average: Optional[Literal["binary", "micro", "macro", "weighted", "none"]],
     multidim_average: Literal["global", "samplewise"] = "global",
+    multilabel: bool = False,
 ) -> Tensor:
     beta2 = beta**2
     if average == "binary":
         return _safe_divide((1 + beta2) * tp, (1 + beta2) * tp + beta2 * fn + fp)
     if average == "micro":
         tp = tp.sum(dim=0 if multidim_average == "global" else 1)
         fn = fn.sum(dim=0 if multidim_average == "global" else 1)
         fp = fp.sum(dim=0 if multidim_average == "global" else 1)
         return _safe_divide((1 + beta2) * tp, (1 + beta2) * tp + beta2 * fn + fp)
 
     fbeta_score = _safe_divide((1 + beta2) * tp, (1 + beta2) * tp + beta2 * fn + fp)
-    if average is None or average == "none":
-        return fbeta_score
-    weights = tp + fn if average == "weighted" else torch.ones_like(fbeta_score)
-    return _safe_divide(weights * fbeta_score, weights.sum(-1, keepdim=True)).sum(-1)
+    return _adjust_weights_safe_divide(fbeta_score, average, multilabel, tp, fp, fn)
 
 
 def _binary_fbeta_score_arg_validation(
     beta: float,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
     ignore_index: Optional[int] = None,
@@ -371,15 +369,15 @@
                 [0.0000, 0.0000, 0.0000]])
     """
     if validate_args:
         _multilabel_fbeta_score_arg_validation(beta, num_labels, threshold, average, multidim_average, ignore_index)
         _multilabel_stat_scores_tensor_validation(preds, target, num_labels, multidim_average, ignore_index)
     preds, target = _multilabel_stat_scores_format(preds, target, num_labels, threshold, ignore_index)
     tp, fp, tn, fn = _multilabel_stat_scores_update(preds, target, multidim_average)
-    return _fbeta_reduce(tp, fp, tn, fn, beta, average=average, multidim_average=multidim_average)
+    return _fbeta_reduce(tp, fp, tn, fn, beta, average=average, multidim_average=multidim_average, multilabel=True)
 
 
 def binary_f1_score(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/group_fairness.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/group_fairness.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/hamming.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/hamming.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     _multiclass_stat_scores_tensor_validation,
     _multiclass_stat_scores_update,
     _multilabel_stat_scores_arg_validation,
     _multilabel_stat_scores_format,
     _multilabel_stat_scores_tensor_validation,
     _multilabel_stat_scores_update,
 )
-from torchmetrics.utilities.compute import _safe_divide
+from torchmetrics.utilities.compute import _adjust_weights_safe_divide, _safe_divide
 from torchmetrics.utilities.enums import ClassificationTask
 
 
 def _hamming_distance_reduce(
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
@@ -76,18 +76,15 @@
         if multilabel:
             fp = fp.sum(dim=0 if multidim_average == "global" else 1)
             tn = tn.sum(dim=0 if multidim_average == "global" else 1)
             return 1 - _safe_divide(tp + tn, tp + tn + fp + fn)
         return 1 - _safe_divide(tp, tp + fn)
 
     score = 1 - _safe_divide(tp + tn, tp + tn + fp + fn) if multilabel else 1 - _safe_divide(tp, tp + fn)
-    if average is None or average == "none":
-        return score
-    weights = tp + fn if average == "weighted" else torch.ones_like(score)
-    return _safe_divide(weights * score, weights.sum(-1, keepdim=True)).sum(-1)
+    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn)
 
 
 def binary_hamming_distance(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/hinge.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/jaccard.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/jaccard.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,17 @@
     allowed_average = ["binary", "micro", "macro", "weighted", "none", None]
     if average not in allowed_average:
         raise ValueError(f"The `average` has to be one of {allowed_average}, got {average}.")
     confmat = confmat.float()
     if average == "binary":
         return confmat[1, 1] / (confmat[0, 1] + confmat[1, 0] + confmat[1, 1])
 
-    ignore_index_cond = ignore_index is not None and 0 <= ignore_index <= confmat.shape[0]
-    if confmat.ndim == 3:  # multilabel
+    ignore_index_cond = ignore_index is not None and 0 <= ignore_index < confmat.shape[0]
+    multilabel = confmat.ndim == 3
+    if multilabel:
         num = confmat[:, 1, 1]
         denom = confmat[:, 1, 1] + confmat[:, 0, 1] + confmat[:, 1, 0]
     else:  # multiclass
         num = torch.diag(confmat)
         denom = confmat.sum(0) + confmat.sum(1) - num
 
     if average == "micro":
@@ -83,14 +84,16 @@
         return jaccard
     if average == "weighted":
         weights = confmat[:, 1, 1] + confmat[:, 1, 0] if confmat.ndim == 3 else confmat.sum(1)
     else:
         weights = torch.ones_like(jaccard)
         if ignore_index_cond:
             weights[ignore_index] = 0.0
+        if not multilabel:
+            weights[confmat.sum(1) + confmat.sum(0) == 0] = 0.0
     return ((weights * jaccard) / weights.sum()).sum()
 
 
 def binary_jaccard_index(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/matthews_corrcoef.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/matthews_corrcoef.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,31 +31,54 @@
     _multilabel_confusion_matrix_tensor_validation,
     _multilabel_confusion_matrix_update,
 )
 from torchmetrics.utilities.enums import ClassificationTask
 
 
 def _matthews_corrcoef_reduce(confmat: Tensor) -> Tensor:
-    """Reduce an un-normalized confusion matrix of shape (n_classes, n_classes) into the matthews corrcoef score."""
+    """Reduce an un-normalized confusion matrix of shape (n_classes, n_classes) into the matthews corrcoef score.
+
+    See: https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-019-6413-7 for more info.
+    """
     # convert multilabel into binary
     confmat = confmat.sum(0) if confmat.ndim == 3 else confmat
 
+    if confmat.numel() == 4:  # binary case
+        tn, fp, fn, tp = confmat.reshape(-1)
+        if tp != 0 and tn == 0 and fp == 0 and fn == 0:
+            return torch.tensor(1.0, dtype=confmat.dtype, device=confmat.device)
+
+        if tp == 0 and tn != 0 and fp == 0 and fn == 0:
+            return torch.tensor(-1.0, dtype=confmat.dtype, device=confmat.device)
+
     tk = confmat.sum(dim=-1).float()
     pk = confmat.sum(dim=-2).float()
     c = torch.trace(confmat).float()
     s = confmat.sum().float()
 
     cov_ytyp = c * s - sum(tk * pk)
     cov_ypyp = s**2 - sum(pk * pk)
     cov_ytyt = s**2 - sum(tk * tk)
 
+    numerator = cov_ytyp
     denom = cov_ypyp * cov_ytyt
-    if denom == 0:
+
+    if denom == 0 and confmat.numel() == 4:
+        if tp == 0 or tn == 0:
+            a = tp + tn
+
+        if fp == 0 or fn == 0:
+            b = fp + fn
+
+        eps = torch.tensor(torch.finfo(torch.float32).eps, dtype=torch.float32, device=confmat.device)
+        numerator = torch.sqrt(eps) * (a - b)
+        denom = torch.sqrt(2 * (a + b) * (a + eps) * (b + eps))
+    elif denom == 0:
         return torch.tensor(0, dtype=confmat.dtype, device=confmat.device)
-    return cov_ytyp / torch.sqrt(denom)
+    return numerator / torch.sqrt(denom)
 
 
 def binary_matthews_corrcoef(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     ignore_index: Optional[int] = None,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/precision_fixed_recall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/precision_recall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/precision_recall.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,41 +27,39 @@
     _multiclass_stat_scores_tensor_validation,
     _multiclass_stat_scores_update,
     _multilabel_stat_scores_arg_validation,
     _multilabel_stat_scores_format,
     _multilabel_stat_scores_tensor_validation,
     _multilabel_stat_scores_update,
 )
-from torchmetrics.utilities.compute import _safe_divide
+from torchmetrics.utilities.compute import _adjust_weights_safe_divide, _safe_divide
 from torchmetrics.utilities.enums import ClassificationTask
 
 
 def _precision_recall_reduce(
     stat: Literal["precision", "recall"],
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
     fn: Tensor,
     average: Optional[Literal["binary", "micro", "macro", "weighted", "none"]],
     multidim_average: Literal["global", "samplewise"] = "global",
+    multilabel: bool = False,
 ) -> Tensor:
     different_stat = fp if stat == "precision" else fn  # this is what differs between the two scores
     if average == "binary":
         return _safe_divide(tp, tp + different_stat)
     if average == "micro":
         tp = tp.sum(dim=0 if multidim_average == "global" else 1)
         fn = fn.sum(dim=0 if multidim_average == "global" else 1)
         different_stat = different_stat.sum(dim=0 if multidim_average == "global" else 1)
         return _safe_divide(tp, tp + different_stat)
 
     score = _safe_divide(tp, tp + different_stat)
-    if average is None or average == "none":
-        return score
-    weights = tp + fn if average == "weighted" else torch.ones_like(score)
-    return _safe_divide(weights * score, weights.sum(-1, keepdim=True)).sum(-1)
+    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn)
 
 
 def binary_precision(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
@@ -332,15 +330,17 @@
                 [0.0000, 0.0000, 0.0000]])
     """
     if validate_args:
         _multilabel_stat_scores_arg_validation(num_labels, threshold, average, multidim_average, ignore_index)
         _multilabel_stat_scores_tensor_validation(preds, target, num_labels, multidim_average, ignore_index)
     preds, target = _multilabel_stat_scores_format(preds, target, num_labels, threshold, ignore_index)
     tp, fp, tn, fn = _multilabel_stat_scores_update(preds, target, multidim_average)
-    return _precision_recall_reduce("precision", tp, fp, tn, fn, average=average, multidim_average=multidim_average)
+    return _precision_recall_reduce(
+        "precision", tp, fp, tn, fn, average=average, multidim_average=multidim_average, multilabel=True
+    )
 
 
 def binary_recall(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
@@ -611,15 +611,17 @@
                 [0., 0., 0.]])
     """
     if validate_args:
         _multilabel_stat_scores_arg_validation(num_labels, threshold, average, multidim_average, ignore_index)
         _multilabel_stat_scores_tensor_validation(preds, target, num_labels, multidim_average, ignore_index)
     preds, target = _multilabel_stat_scores_format(preds, target, num_labels, threshold, ignore_index)
     tp, fp, tn, fn = _multilabel_stat_scores_update(preds, target, multidim_average)
-    return _precision_recall_reduce("recall", tp, fp, tn, fn, average=average, multidim_average=multidim_average)
+    return _precision_recall_reduce(
+        "recall", tp, fp, tn, fn, average=average, multidim_average=multidim_average, multilabel=True
+    )
 
 
 def precision(
     preds: Tensor,
     target: Tensor,
     task: Literal["binary", "multiclass", "multilabel"],
     threshold: float = 0.5,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/precision_recall_curve.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/precision_recall_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     if ignore_index is None:
         check = torch.any((unique_values != 0) & (unique_values != 1))
     else:
         check = torch.any((unique_values != 0) & (unique_values != 1) & (unique_values != ignore_index))
     if check:
         raise RuntimeError(
             f"Detected the following values in `target`: {unique_values} but expected only"
-            f" the following values {[0,1] + [] if ignore_index is None else [ignore_index]}."
+            f" the following values {[0, 1] if ignore_index is None else [ignore_index]}."
         )
 
 
 def _binary_precision_recall_curve_format(
     preds: Tensor,
     target: Tensor,
     thresholds: Optional[Union[int, List[float], Tensor]] = None,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/ranking.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/recall_fixed_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/roc.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/specificity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/specificity.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,38 +27,36 @@
     _multiclass_stat_scores_tensor_validation,
     _multiclass_stat_scores_update,
     _multilabel_stat_scores_arg_validation,
     _multilabel_stat_scores_format,
     _multilabel_stat_scores_tensor_validation,
     _multilabel_stat_scores_update,
 )
-from torchmetrics.utilities.compute import _safe_divide
+from torchmetrics.utilities.compute import _adjust_weights_safe_divide, _safe_divide
 from torchmetrics.utilities.enums import ClassificationTask
 
 
 def _specificity_reduce(
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
     fn: Tensor,
     average: Optional[Literal["binary", "micro", "macro", "weighted", "none"]],
     multidim_average: Literal["global", "samplewise"] = "global",
+    multilabel: bool = False,
 ) -> Tensor:
     if average == "binary":
         return _safe_divide(tn, tn + fp)
     if average == "micro":
         tn = tn.sum(dim=0 if multidim_average == "global" else 1)
         fp = fp.sum(dim=0 if multidim_average == "global" else 1)
         return _safe_divide(tn, tn + fp)
 
     specificity_score = _safe_divide(tn, tn + fp)
-    if average is None or average == "none":
-        return specificity_score
-    weights = tp + fn if average == "weighted" else torch.ones_like(specificity_score)
-    return _safe_divide(weights * specificity_score, weights.sum(-1, keepdim=True)).sum(-1)
+    return _adjust_weights_safe_divide(specificity_score, average, multilabel, tp, fp, fn)
 
 
 def binary_specificity(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
@@ -329,15 +327,15 @@
                 [0., 0., 1.]])
     """
     if validate_args:
         _multilabel_stat_scores_arg_validation(num_labels, threshold, average, multidim_average, ignore_index)
         _multilabel_stat_scores_tensor_validation(preds, target, num_labels, multidim_average, ignore_index)
     preds, target = _multilabel_stat_scores_format(preds, target, num_labels, threshold, ignore_index)
     tp, fp, tn, fn = _multilabel_stat_scores_update(preds, target, multidim_average)
-    return _specificity_reduce(tp, fp, tn, fn, average=average, multidim_average=multidim_average)
+    return _specificity_reduce(tp, fp, tn, fn, average=average, multidim_average=multidim_average, multilabel=True)
 
 
 def specificity(
     preds: Tensor,
     target: Tensor,
     task: Literal["binary", "multiclass", "multilabel"],
     threshold: float = 0.5,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/specificity_sensitivity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/classification/stat_scores.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/classification/stat_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if ignore_index is None:
         check = torch.any((unique_values != 0) & (unique_values != 1))
     else:
         check = torch.any((unique_values != 0) & (unique_values != 1) & (unique_values != ignore_index))
     if check:
         raise RuntimeError(
             f"Detected the following values in `target`: {unique_values} but expected only"
-            f" the following values {[0,1] + [] if ignore_index is None else [ignore_index]}."
+            f" the following values {[0, 1] if ignore_index is None else [ignore_index]}."
         )
 
     # If preds is label tensor, also check that it only contains [0,1] values
     if not preds.is_floating_point():
         unique_values = torch.unique(preds)
         if torch.any((unique_values != 0) & (unique_values != 1)):
             raise RuntimeError(
@@ -250,15 +250,15 @@
     target: Tensor,
     num_classes: int,
     multidim_average: Literal["global", "samplewise"] = "global",
     ignore_index: Optional[int] = None,
 ) -> None:
     """Validate tensor input.
 
-    - if target has one more dimension than preds, then all dimensions except for preds.shape[1] should match
+    - if preds has one more dimension than target, then all dimensions except for preds.shape[1] should match
     exactly. preds.shape[1] should have size equal to number of classes
     - if preds and target have same number of dims, then all dimensions should match
     - if ``multidim_average`` is set to ``samplewise`` preds tensor needs to be atleast 2 dimensional in the
     int case and 3 dimensional in the float case
     - all values in target tensor that are not ignored have to be {0, ..., num_classes - 1}
     - if pred tensor is not floating point, then all values also have to be in {0, ..., num_classes - 1}
     """
@@ -612,15 +612,15 @@
     if ignore_index is None:
         check = torch.any((unique_values != 0) & (unique_values != 1))
     else:
         check = torch.any((unique_values != 0) & (unique_values != 1) & (unique_values != ignore_index))
     if check:
         raise RuntimeError(
             f"Detected the following values in `target`: {unique_values} but expected only"
-            f" the following values {[0,1] + [] if ignore_index is None else [ignore_index]}."
+            f" the following values {[0, 1] if ignore_index is None else [ignore_index]}."
         )
 
     # If preds is label tensor, also check that it only contains [0,1] values
     if not preds.is_floating_point():
         unique_values = torch.unique(preds)
         if torch.any((unique_values != 0) & (unique_values != 1)):
             raise RuntimeError(
@@ -895,15 +895,15 @@
     reduce: Optional[str] = "micro",
     mdmc_reduce: Optional[str] = None,
     num_classes: Optional[int] = None,
     top_k: Optional[int] = 1,
     threshold: float = 0.5,
     multiclass: Optional[bool] = None,
     ignore_index: Optional[int] = None,
-    mode: DataType = None,
+    mode: Optional[DataType] = None,
 ) -> Tuple[Tensor, Tensor, Tensor, Tensor]:
     """Calculate true positives, false positives, true negatives, false negatives.
 
     Raises:
         ValueError:
             The `ignore_index` is not valid
         ValueError:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     _TORCHVISION_GREATER_EQUAL_0_8,
     _TORCHVISION_GREATER_EQUAL_0_13,
 )
 
 __all__ = ["modified_panoptic_quality", "panoptic_quality"]
 
 if _TORCHVISION_AVAILABLE and _TORCHVISION_GREATER_EQUAL_0_8:
-    from torchmetrics.functional.detection.giou import generalized_intersection_over_union  # noqa: F401
-    from torchmetrics.functional.detection.iou import intersection_over_union  # noqa: F401
+    from torchmetrics.functional.detection.giou import generalized_intersection_over_union
+    from torchmetrics.functional.detection.iou import intersection_over_union
 
     __all__.append("generalized_intersection_over_union")
     __all__.append("intersection_over_union")
 
 if _TORCHVISION_AVAILABLE and _TORCHVISION_GREATER_EQUAL_0_13:
-    from torchmetrics.functional.detection.ciou import complete_intersection_over_union  # noqa: F401
-    from torchmetrics.functional.detection.diou import distance_intersection_over_union  # noqa: F401
+    from torchmetrics.functional.detection.ciou import complete_intersection_over_union
+    from torchmetrics.functional.detection.diou import distance_intersection_over_union
 
     __all__.append("complete_intersection_over_union")
     __all__.append("distance_intersection_over_union")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/_panoptic_quality_common.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/_panoptic_quality_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     Args:
         things: The set of category IDs for things.
         stuffs: The set of category IDs for stuffs.
 
     Returns:
         A new color ID that does not belong to things nor stuffs.
     """
-    unused_category_id = 1 + max([0] + list(things) + list(stuffs))
+    unused_category_id = 1 + max([0, *list(things), *list(stuffs)])
     return unused_category_id, 0
 
 
 def _get_category_id_to_continuous_id(things: Set[int], stuffs: Set[int]) -> Dict[int, int]:
     """Convert original IDs to continuous IDs.
 
     Args:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/ciou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/ciou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/diou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/diou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/giou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/giou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/iou.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/detection/panoptic_qualities.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/detection/panoptic_qualities.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/d_lambda.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/d_lambda.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,34 +15,37 @@
 from typing import Tuple
 
 import torch
 from torch import Tensor
 from typing_extensions import Literal
 
 from torchmetrics.functional.image.uqi import universal_image_quality_index
-from torchmetrics.utilities.checks import _check_same_shape
 from torchmetrics.utilities.distributed import reduce
 
 
 def _spectral_distortion_index_update(preds: Tensor, target: Tensor) -> Tuple[Tensor, Tensor]:
     """Update and returns variables required to compute Spectral Distortion Index.
 
     Args:
         preds: Low resolution multispectral image
         target: High resolution fused image
     """
     if preds.dtype != target.dtype:
         raise TypeError(
             f"Expected `ms` and `fused` to have the same data type. Got ms: {preds.dtype} and fused: {target.dtype}."
         )
-    _check_same_shape(preds, target)
     if len(preds.shape) != 4:
         raise ValueError(
             f"Expected `preds` and `target` to have BxCxHxW shape. Got preds: {preds.shape} and target: {target.shape}."
         )
+    if preds.shape[:2] != target.shape[:2]:
+        raise ValueError(
+            "Expected `preds` and `target` to have same batch and channel sizes."
+            f"Got preds: {preds.shape} and target: {target.shape}."
+        )
     return preds, target
 
 
 def _spectral_distortion_index_compute(
     preds: Tensor,
     target: Tensor,
     p: int = 1,
@@ -65,21 +68,37 @@
         >>> preds = torch.rand([16, 3, 16, 16])
         >>> target = torch.rand([16, 3, 16, 16])
         >>> preds, target = _spectral_distortion_index_update(preds, target)
         >>> _spectral_distortion_index_compute(preds, target)
         tensor(0.0234)
     """
     length = preds.shape[1]
-    m1 = torch.zeros((length, length))
-    m2 = torch.zeros((length, length))
+
+    m1 = torch.zeros((length, length), device=preds.device)
+    m2 = torch.zeros((length, length), device=preds.device)
 
     for k in range(length):
-        for r in range(k, length):
-            m1[k, r] = m1[r, k] = universal_image_quality_index(target[:, k : k + 1, :, :], target[:, r : r + 1, :, :])
-            m2[k, r] = m2[r, k] = universal_image_quality_index(preds[:, k : k + 1, :, :], preds[:, r : r + 1, :, :])
+        num = length - (k + 1)
+        if num == 0:
+            continue
+        stack1 = target[:, k : k + 1, :, :].repeat(num, 1, 1, 1)
+        stack2 = torch.cat([target[:, r : r + 1, :, :] for r in range(k + 1, length)], dim=0)
+        score = [
+            s.mean() for s in universal_image_quality_index(stack1, stack2, reduction="none").split(preds.shape[0])
+        ]
+        m1[k, k + 1 :] = torch.stack(score, 0)
+
+        stack1 = preds[:, k : k + 1, :, :].repeat(num, 1, 1, 1)
+        stack2 = torch.cat([preds[:, r : r + 1, :, :] for r in range(k + 1, length)], dim=0)
+        score = [
+            s.mean() for s in universal_image_quality_index(stack1, stack2, reduction="none").split(preds.shape[0])
+        ]
+        m2[k, k + 1 :] = torch.stack(score, 0)
+    m1 = m1 + m1.T
+    m2 = m2 + m2.T
 
     diff = torch.pow(torch.abs(m1 - m2), p)
     # Special case: when number of channels (L) is 1, there will be only one element in M1 and M2. Hence no need to sum.
     if length == 1:
         output = torch.pow(diff, (1.0 / p))
     else:
         output = torch.pow(1.0 / (length * (length - 1)) * torch.sum(diff), (1.0 / p))
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/ergas.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/gradients.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/gradients.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/helper.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,22 +116,21 @@
 
     Return:
         Image transformed with the uniform input
     """
     inputs = _reflection_pad_2d(inputs, window_size // 2, window_size % 2)
     kernel_weight, kernel_bias = _uniform_weight_bias_conv2d(inputs, window_size)
     # Iterate over channels
-    inputs = torch.cat(
+    return torch.cat(
         [
             F.conv2d(inputs[:, channel].unsqueeze(1), kernel_weight, kernel_bias, padding=0)
             for channel in range(inputs.shape[1])
         ],
         dim=1,
     )
-    return inputs
 
 
 def _gaussian_kernel_3d(
     channel: int, kernel_size: Sequence[int], sigma: Sequence[float], dtype: torch.dtype, device: torch.device
 ) -> Tensor:
     """Compute 3D gaussian kernel.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,31 +63,31 @@
         super().__init__()
         pretrained_features = _get_net("squeezenet1_1", pretrained)
 
         self.N_slices = 7
         slices = []
         feature_ranges = [range(2), range(2, 5), range(5, 8), range(8, 10), range(10, 11), range(11, 12), range(12, 13)]
         for feature_range in feature_ranges:
-            slice = torch.nn.Sequential()
+            seq = torch.nn.Sequential()
             for i in feature_range:
-                slice.add_module(str(i), pretrained_features[i])
-            slices.append(slice)
+                seq.add_module(str(i), pretrained_features[i])
+            slices.append(seq)
 
         self.slices = nn.ModuleList(slices)
         if not requires_grad:
             for param in self.parameters():
                 param.requires_grad = False
 
     def forward(self, x: Tensor) -> NamedTuple:
         """Process input."""
         squeeze_output = namedtuple("squeeze_output", ["relu1", "relu2", "relu3", "relu4", "relu5", "relu6", "relu7"])
 
         relus = []
-        for slice in self.slices:
-            x = slice(x)
+        for slice_ in self.slices:
+            x = slice_(x)
             relus.append(x)
         return squeeze_output(*relus)
 
 
 class Alexnet(torch.nn.Module):
     """Alexnet implementation."""
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/alex.pth` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/alex.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/squeeze.pth` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/squeeze.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/lpips_models/vgg.pth` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/lpips_models/vgg.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/psnr.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/psnrb.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/rase.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/rase.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/rmse_sw.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/sam.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/ssim.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/tv.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/image/uqi.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/image/uqi.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     mu_pred_target = output_list[0] * output_list[1]
 
     sigma_pred_sq = output_list[2] - mu_pred_sq
     sigma_target_sq = output_list[3] - mu_target_sq
     sigma_pred_target = output_list[4] - mu_pred_target
 
     upper = 2 * sigma_pred_target
-    lower = sigma_pred_sq + sigma_target_sq
+    lower = sigma_pred_sq + sigma_target_sq + torch.finfo(sigma_pred_sq.dtype).eps
 
     uqi_idx = ((2 * mu_pred_target) * upper) / ((mu_pred_sq + mu_target_sq) * lower)
     uqi_idx = uqi_idx[..., pad_h:-pad_h, pad_w:-pad_w]
 
     return reduce(uqi_idx, reduction)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/multimodal/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/multimodal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.utilities.imports import _TRANSFORMERS_AVAILABLE
 
 __all__ = []
 
 if _TRANSFORMERS_AVAILABLE:
-    from torchmetrics.functional.multimodal.clip_score import clip_score  # noqa: F401
+    from torchmetrics.functional.multimodal.clip_score import clip_score
 
     __all__.append("clip_score")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/multimodal/clip_score.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.functional.nominal.cramers import cramers_v, cramers_v_matrix
+from torchmetrics.functional.nominal.fleiss_kappa import fleiss_kappa
 from torchmetrics.functional.nominal.pearson import (
     pearsons_contingency_coefficient,
     pearsons_contingency_coefficient_matrix,
 )
 from torchmetrics.functional.nominal.theils_u import theils_u, theils_u_matrix
 from torchmetrics.functional.nominal.tschuprows import tschuprows_t, tschuprows_t_matrix
 
 __all__ = [
     "cramers_v",
     "cramers_v_matrix",
+    "fleiss_kappa",
     "pearsons_contingency_coefficient",
     "pearsons_contingency_coefficient_matrix",
     "theils_u",
     "theils_u_matrix",
     "tschuprows_t",
     "tschuprows_t_matrix",
 ]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/cramers.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/pearson.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/theils_u.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/tschuprows.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/nominal/utils.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/nominal/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/cosine.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/cosine.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/euclidean.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/euclidean.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/helpers.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/linear.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/linear.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/manhattan.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/manhattan.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/pairwise/minkowski.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/pairwise/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from torchmetrics.functional.regression.log_mse import mean_squared_log_error
 from torchmetrics.functional.regression.mae import mean_absolute_error
 from torchmetrics.functional.regression.mape import mean_absolute_percentage_error
 from torchmetrics.functional.regression.minkowski import minkowski_distance
 from torchmetrics.functional.regression.mse import mean_squared_error
 from torchmetrics.functional.regression.pearson import pearson_corrcoef
 from torchmetrics.functional.regression.r2 import r2_score
+from torchmetrics.functional.regression.rse import relative_squared_error
 from torchmetrics.functional.regression.spearman import spearman_corrcoef
 from torchmetrics.functional.regression.symmetric_mape import symmetric_mean_absolute_percentage_error
 from torchmetrics.functional.regression.tweedie_deviance import tweedie_deviance_score
 from torchmetrics.functional.regression.wmape import weighted_mean_absolute_percentage_error
 
 __all__ = [
     "concordance_corrcoef",
@@ -41,12 +42,13 @@
     "mean_absolute_error",
     "mean_squared_error",
     "pearson_corrcoef",
     "mean_absolute_percentage_error",
     "mean_absolute_percentage_error",
     "minkowski_distance",
     "r2_score",
+    "relative_squared_error",
     "spearman_corrcoef",
     "symmetric_mean_absolute_percentage_error",
     "tweedie_deviance_score",
     "weighted_mean_absolute_percentage_error",
 ]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/concordance.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/cosine_similarity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/explained_variance.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/kendall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/kendall.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,30 +220,32 @@
         p_value *= 2
     return p_value
 
 
 def _kendall_corrcoef_update(
     preds: Tensor,
     target: Tensor,
-    concat_preds: List[Tensor] = [],
-    concat_target: List[Tensor] = [],
+    concat_preds: Optional[List[Tensor]] = None,
+    concat_target: Optional[List[Tensor]] = None,
     num_outputs: int = 1,
 ) -> Tuple[List[Tensor], List[Tensor]]:
     """Update variables required to compute Kendall rank correlation coefficient.
 
     Args:
         preds: Sequence of data
         target: Sequence of data
         concat_preds: List of batches of preds sequence to be concatenated
         concat_target: List of batches of target sequence to be concatenated
         num_outputs: Number of outputs in multioutput setting
 
     Raises:
         RuntimeError: If ``preds`` and ``target`` do not have the same shape
     """
+    concat_preds = concat_preds or []
+    concat_target = concat_target or []
     # Data checking
     _check_same_shape(preds, target)
     _check_data_shape_to_num_outputs(preds, target, num_outputs)
 
     if num_outputs == 1:
         preds = preds.unsqueeze(1)
         target = target.unsqueeze(1)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/kl_divergence.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/log_cosh.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/log_mse.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/mae.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/mape.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/minkowski.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/mse.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/pearson.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/pearson.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,20 @@
         var_y: variance estimate of y tensor
         corr_xy: covariance estimate between x and y tensor
         nb: number of observations
     """
     var_x /= nb - 1
     var_y /= nb - 1
     corr_xy /= nb - 1
+    # if var_x, var_y is float16 and on cpu, make it bfloat16 as sqrt is not supported for float16
+    # on cpu, remove this after https://github.com/pytorch/pytorch/issues/54774 is fixed
+    if var_x.dtype == torch.float16 and var_x.device == torch.device("cpu"):
+        var_x = var_x.bfloat16()
+        var_y = var_y.bfloat16()
+
     corrcoef = (corr_xy / (var_x * var_y).sqrt()).squeeze()
     return torch.clamp(corrcoef, -1.0, 1.0)
 
 
 def pearson_corrcoef(preds: Tensor, target: Tensor) -> Tensor:
     """Compute pearson correlation coefficient.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/r2.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/r2.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,25 +98,25 @@
     else:
         raise ValueError(
             "Argument `multioutput` must be either `raw_values`,"
             f" `uniform_average` or `variance_weighted`. Received {multioutput}."
         )
 
     if adjusted < 0 or not isinstance(adjusted, int):
-        raise ValueError("`adjusted` parameter should be an integer larger or" " equal to 0.")
+        raise ValueError("`adjusted` parameter should be an integer larger or equal to 0.")
 
     if adjusted != 0:
         if adjusted > n_obs - 1:
             rank_zero_warn(
                 "More independent regressions than data points in"
                 " adjusted r2 score. Falls back to standard r2 score.",
                 UserWarning,
             )
         elif adjusted == n_obs - 1:
-            rank_zero_warn("Division by zero in adjusted r2 score. Falls back to" " standard r2 score.", UserWarning)
+            rank_zero_warn("Division by zero in adjusted r2 score. Falls back to standard r2 score.", UserWarning)
         else:
             return 1 - (1 - r2) * (n_obs - 1) / (n_obs - adjusted - 1)
     return r2
 
 
 def r2_score(
     preds: Tensor,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/spearman.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/symmetric_mape.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/tweedie_deviance.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/utils.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/regression/wmape.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/average_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/fall_out.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/hit_rate.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/ndcg.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/precision_recall_curve.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/r_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/recall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/retrieval/reciprocal_rank.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from torchmetrics.functional.text.ter import translation_edit_rate
 from torchmetrics.functional.text.wer import word_error_rate
 from torchmetrics.functional.text.wil import word_information_lost
 from torchmetrics.functional.text.wip import word_information_preserved
 from torchmetrics.utilities.imports import _TRANSFORMERS_AVAILABLE
 
 if _TRANSFORMERS_AVAILABLE:
-    from torchmetrics.functional.text.bert import bert_score  # noqa: F401
-    from torchmetrics.functional.text.infolm import infolm  # noqa: F401
+    from torchmetrics.functional.text.bert import bert_score
+    from torchmetrics.functional.text.infolm import infolm
 
 
 __all__ = [
     "bleu_score",
     "char_error_rate",
     "chrf_score",
     "extended_edit_distance",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/bert.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     TokenizedDataset,
     _check_shape_of_model_output,
     _get_progress_bar,
     _input_data_collator,
     _output_data_collator,
     _process_attention_mask_for_special_tokens,
 )
+from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.checks import _SKIP_SLOW_DOCTEST, _try_proceed_with_timeout
 from torchmetrics.utilities.imports import _TQDM_AVAILABLE, _TRANSFORMERS_AVAILABLE
 
 # Default model recommended in the original implementation.
 _DEFAULT_MODEL = "roberta-large"
 
 if _TRANSFORMERS_AVAILABLE:
@@ -209,16 +210,16 @@
         baseline = _read_csv_from_url(baseline_url)
     # Read default baseline from the original `bert-score` package https://github.com/Tiiiger/bert_score
     elif lang and model_name_or_path:
         url_base = "https://raw.githubusercontent.com/Tiiiger/bert_score/master/bert_score/rescale_baseline"
         baseline_url = f"{url_base}/{lang}/{model_name_or_path}.tsv"
         baseline = _read_csv_from_url(baseline_url)
     else:
-        baseline = None
-        warn("Baseline was not successfully loaded. No baseline is going to be used.")
+        rank_zero_warn("Baseline was not successfully loaded. No baseline is going to be used.")
+        return None
 
     return baseline
 
 
 def _rescale_metrics_with_baseline(
     precision: Tensor,
     recall: Tensor,
@@ -343,15 +344,15 @@
     if model is None:
         if not _TRANSFORMERS_AVAILABLE:
             raise ModuleNotFoundError(
                 "`bert_score` metric with default models requires `transformers` package be installed."
                 " Either install with `pip install transformers>=4.0` or `pip install torchmetrics[text]`."
             )
         if model_name_or_path is None:
-            warn(
+            rank_zero_warn(
                 "The argument `model_name_or_path` was not specified while it is required when default"
                 " `transformers` model are used."
                 f"It is, therefore, used the default recommended model - {_DEFAULT_MODEL}."
             )
         tokenizer = AutoTokenizer.from_pretrained(model_name_or_path or _DEFAULT_MODEL)
         model = AutoModel.from_pretrained(model_name_or_path or _DEFAULT_MODEL)
     else:
@@ -362,25 +363,25 @@
     try:
         if num_layers and num_layers > model.config.num_hidden_layers:  # type: ignore
             raise ValueError(
                 f"num_layers={num_layers} is forbidden for {model_name_or_path}."  # type: ignore
                 f" Please use num_layers <= {model.config.num_hidden_layers}"
             )
     except AttributeError:
-        warn("It was not possible to retrieve the parameter `num_layers` from the model specification.")
+        rank_zero_warn("It was not possible to retrieve the parameter `num_layers` from the model specification.")
 
     _are_empty_lists = all(isinstance(text, list) and len(text) == 0 for text in (preds, target))
     _are_valid_lists = all(
         isinstance(text, list) and len(text) > 0 and isinstance(text[0], str) for text in (preds, target)
     )
     _are_valid_tensors = all(
         isinstance(text, dict) and isinstance(text["input_ids"], Tensor) for text in (preds, target)
     )
     if _are_empty_lists:
-        warn("Predictions and references are empty.")
+        rank_zero_warn("Predictions and references are empty.")
         output_dict: Dict[str, Union[Tensor, List[float], str]] = {
             "precision": [0.0],
             "recall": [0.0],
             "f1": [0.0],
         }
         if return_hash:
             output_dict.update({"hash": _get_hash(model_name_or_path, num_layers, idf)})
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/bleu.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/bleu.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 ) -> Tensor:
     """Calculate `BLEU score`_ of machine translated text with one or more references.
 
     Args:
         preds: An iterable of machine translated corpus
         target: An iterable of iterables of reference corpus
         n_gram: Gram value ranged from 1 to 4
-        smooth: Whether to apply smoothing – see [2]
+        smooth: Whether to apply smoothing - see [2]
         weights:
             Weights used for unigrams, bigrams, etc. to calculate BLEU score.
             If not provided, uniform weights are used.
 
     Return:
         Tensor with BLEU Score
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/cer.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/chrf.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/eed.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/eed.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,15 @@
         ("i . e .", "i.e."),
         ("U . S .", "U.S."),
     ]
     for pattern, replacement in rules_interpunction:
         sentence = sentence.replace(pattern, replacement)
 
     # add space to beginning and end of string
-    sentence = " " + sentence + " "
-
-    return sentence
+    return " " + sentence + " "
 
 
 def _preprocess_ja(sentence: str) -> str:
     """Preprocess japanese sentences.
 
     Copy from https://github.com/rwth-i6/ExtendedEditDistance/blob/master/util.py.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/helper.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         """
         trace: Tuple[_EditOperations, ...] = ()
         i = prediction_len
         j = self.reference_len
 
         while i > 0 or j > 0:
             operation = edit_distance[i][j][1]
-            trace = (operation,) + trace
+            trace = (operation, *trace)
             if operation in (_EditOperations.OP_SUBSTITUTE, _EditOperations.OP_NOTHING):
                 i -= 1
                 j -= 1
             elif operation == _EditOperations.OP_INSERT:
                 j -= 1
             elif operation == _EditOperations.OP_DELETE:
                 i -= 1
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/helper_embedding_metric.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/helper_embedding_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,16 @@
     if not own_tokenizer:
         tokenized_data = tokenizer(
             text, padding="max_length", max_length=max_length, truncation=truncation, return_tensors="pt"
         )
     else:
         try:
             tokenized_data = tokenizer(text, max_length)
-        except BaseException as e:
-            raise BaseException(f"Tokenization was not successful: {e}")
+        except BaseException as ex:
+            raise RuntimeError(f"Tokenization was not successful: {ex}") from ex
 
     if sort_according_length:
         input_ids, attention_mask, sorting_indices = _sort_data_according_length(
             tokenized_data["input_ids"], tokenized_data["attention_mask"]
         )
         input_dict = {"input_ids": input_ids, "attention_mask": attention_mask}
     else:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/infolm.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/mer.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/perplexity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/rouge.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/rouge.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,23 +45,23 @@
     """Check whether `nltk` `punkt` is downloaded.
 
     If not, try to download if a machine is connected to the internet.
     """
     import nltk
 
     try:
-        nltk.data.find("tokenizers/punkt.zip")
+        nltk.data.find("tokenizers/punkt")
     except LookupError:
         try:
             nltk.download("punkt", quiet=True, force=False, halt_on_error=False, raise_on_error=True)
-        except ValueError:
+        except ValueError as err:
             raise OSError(
                 "`nltk` resource `punkt` is not available on a disk and cannot be downloaded as a machine is not "
                 "connected to the internet."
-            )
+            ) from err
 
 
 def _split_sentence(x: str) -> Sequence[str]:
     """Split sentence to get rougeLsum scores matching published rougeL scores for BART and PEGASUS."""
     if not _NLTK_AVAILABLE:
         raise ModuleNotFoundError("ROUGE-Lsum calculation requires that `nltk` is installed. Use `pip install nltk`.")
     import nltk
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/sacre_bleu.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/sacre_bleu.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ##############
 
 # MIT License
 # Copyright (c) 2017 - Shujian Huang <huangsj@nju.edu.cn>
 
 import re
 from functools import partial
-from typing import Optional, Sequence
+from typing import ClassVar, Optional, Sequence
 
 import torch
 from torch import Tensor, tensor
 from typing_extensions import Literal
 
 from torchmetrics.functional.text.bleu import _bleu_score_compute, _bleu_score_update
 from torchmetrics.utilities.imports import _REGEX_AVAILABLE
@@ -105,15 +105,15 @@
             (regex.compile(r"(\P{N})(\p{P})"), r"\1 \2 "),
             # Separate out punctuations followed by a non-digit
             (regex.compile(r"(\p{P})(\P{N})"), r" \1 \2"),
             # Separate out symbols
             (regex.compile(r"(\p{S})"), r" \1 "),
         )
 
-    _TOKENIZE_FN = {
+    _TOKENIZE_FN: ClassVar[dict] = {
         "none": "_tokenize_base",
         "13a": "_tokenize_13a",
         "zh": "_tokenize_zh",
         "intl": "_tokenize_international",
         "char": "_tokenize_char",
     }
 
@@ -170,15 +170,15 @@
         Return:
             the tokenized line
         """
         return line
 
     @classmethod
     def _tokenize_13a(cls, line: str) -> str:
-        """Tokenizes an line using a relatively minimal tokenization that is equivalent to mteval-v13a, used by WMT.
+        """Tokenizes a line using a relatively minimal tokenization that is equivalent to mteval-v13a, used by WMT.
 
         Args:
             line: input sentence
 
         Return:
             tokenized sentence
         """
@@ -189,15 +189,15 @@
 
         if "&" in line:
             line = line.replace("&quot;", '"')
             line = line.replace("&amp;", "&")
             line = line.replace("&lt;", "<")
             line = line.replace("&gt;", ">")
 
-        return cls._tokenize_regex(line)
+        return cls._tokenize_regex(f" {line} ")
 
     @classmethod
     def _tokenize_zh(cls, line: str) -> str:
         """Tokenization of Chinese text.
 
         This is done in two steps: separate each Chinese characters (by utf-8 encoding) and afterwards tokenize the
         Chinese part (following the `13a` i.e. mteval tokenizer).
@@ -286,15 +286,15 @@
 
     This implementation follows the behaviour of SacreBLEU [2] implementation from https://github.com/mjpost/sacrebleu.
 
     Args:
         preds: An iterable of machine translated corpus
         target: An iterable of iterables of reference corpus
         n_gram: Gram value ranged from 1 to 4
-        smooth: Whether to apply smoothing – see [2]
+        smooth: Whether to apply smoothing - see [2]
         tokenize: Tokenization technique to be used.
             Supported tokenization: ['none', '13a', 'zh', 'intl', 'char']
         lowercase: If ``True``, BLEU score over lowercased text is calculated.
         weights:
             Weights used for unigrams, bigrams, etc. to calculate BLEU score.
             If not provided, uniform weights are used.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/squad.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/ter.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/ter.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             asian_support: An indication whether asian characters to be processed.
         """
         self.normalize = normalize
         self.no_punctuation = no_punctuation
         self.lowercase = lowercase
         self.asian_support = asian_support
 
-    @lru_cache(maxsize=2**16)
+    @lru_cache(maxsize=2**16)  # noqa: B019
     def __call__(self, sentence: str) -> str:
         """Apply a different tokenization techniques according.
 
         Args:
             sentence: An input sentence to pre-process and tokenize.
 
         Return:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/wer.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/wil.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/functional/text/wip.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/functional/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     __all__ += [
         "FrechetInceptionDistance",
         "InceptionScore",
         "KernelInceptionDistance",
     ]
 
 if _LPIPS_AVAILABLE:
-    from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity  # noqa: F401
+    from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
     __all__.append("LearnedPerceptualImagePatchSimilarity")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/_deprecated.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(
         self,
         ratio: Union[int, float] = 4,
         reduction: Literal["elementwise_mean", "sum", "none", None] = "elementwise_mean",
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("ErrorRelativeGlobalDimensionlessSynthesis", "image")
-        return super().__init__(ratio=ratio, reduction=reduction, **kwargs)
+        super().__init__(ratio=ratio, reduction=reduction, **kwargs)
 
 
 class _MultiScaleStructuralSimilarityIndexMeasure(MultiScaleStructuralSimilarityIndexMeasure):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> preds = torch.rand([3, 3, 256, 256], generator=torch.manual_seed(42))
@@ -56,15 +56,15 @@
         k1: float = 0.01,
         k2: float = 0.03,
         betas: Tuple[float, ...] = (0.0448, 0.2856, 0.3001, 0.2363, 0.1333),
         normalize: Literal["relu", "simple", None] = "relu",
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("MultiScaleStructuralSimilarityIndexMeasure", "image")
-        return super().__init__(
+        super().__init__(
             gaussian_kernel=gaussian_kernel,
             kernel_size=kernel_size,
             sigma=sigma,
             reduction=reduction,
             data_range=data_range,
             k1=k1,
             k2=k2,
@@ -90,15 +90,15 @@
         data_range: Optional[Union[float, Tuple[float, float]]] = None,
         base: float = 10.0,
         reduction: Literal["elementwise_mean", "sum", "none", None] = "elementwise_mean",
         dim: Optional[Union[int, Tuple[int, ...]]] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("PeakSignalNoiseRatio", "image")
-        return super().__init__(data_range=data_range, base=base, reduction=reduction, dim=dim, **kwargs)
+        super().__init__(data_range=data_range, base=base, reduction=reduction, dim=dim, **kwargs)
 
 
 class _RelativeAverageSpectralError(RelativeAverageSpectralError):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> g = torch.manual_seed(22)
@@ -111,15 +111,15 @@
 
     def __init__(
         self,
         window_size: int = 8,
         **kwargs: Dict[str, Any],
     ) -> None:
         _deprecated_root_import_class("RelativeAverageSpectralError", "image")
-        return super().__init__(window_size=window_size, **kwargs)
+        super().__init__(window_size=window_size, **kwargs)
 
 
 class _RootMeanSquaredErrorUsingSlidingWindow(RootMeanSquaredErrorUsingSlidingWindow):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> g = torch.manual_seed(22)
@@ -132,15 +132,15 @@
 
     def __init__(
         self,
         window_size: int = 8,
         **kwargs: Dict[str, Any],
     ) -> None:
         _deprecated_root_import_class("RootMeanSquaredErrorUsingSlidingWindow", "image")
-        return super().__init__(window_size=window_size, **kwargs)
+        super().__init__(window_size=window_size, **kwargs)
 
 
 class _SpectralAngleMapper(SpectralAngleMapper):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> preds = torch.rand([16, 3, 16, 16], generator=torch.manual_seed(42))
@@ -152,15 +152,15 @@
 
     def __init__(
         self,
         reduction: Literal["elementwise_mean", "sum", "none"] = "elementwise_mean",
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("SpectralAngleMapper", "image")
-        return super().__init__(reduction=reduction, **kwargs)
+        super().__init__(reduction=reduction, **kwargs)
 
 
 class _SpectralDistortionIndex(SpectralDistortionIndex):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> _ = torch.manual_seed(42)
@@ -171,15 +171,15 @@
     tensor(0.0234)
     """
 
     def __init__(
         self, p: int = 1, reduction: Literal["elementwise_mean", "sum", "none"] = "elementwise_mean", **kwargs: Any
     ) -> None:
         _deprecated_root_import_class("SpectralDistortionIndex", "image")
-        return super().__init__(p=p, reduction=reduction, **kwargs)
+        super().__init__(p=p, reduction=reduction, **kwargs)
 
 
 class _StructuralSimilarityIndexMeasure(StructuralSimilarityIndexMeasure):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> preds = torch.rand([3, 3, 256, 256])
@@ -199,15 +199,15 @@
         k1: float = 0.01,
         k2: float = 0.03,
         return_full_image: bool = False,
         return_contrast_sensitivity: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("StructuralSimilarityIndexMeasure", "image")
-        return super().__init__(
+        super().__init__(
             gaussian_kernel=gaussian_kernel,
             sigma=sigma,
             kernel_size=kernel_size,
             reduction=reduction,
             data_range=data_range,
             k1=k1,
             k2=k2,
@@ -226,15 +226,15 @@
     >>> img = torch.rand(5, 3, 28, 28)
     >>> tv(img)
     tensor(7546.8018)
     """
 
     def __init__(self, reduction: Literal["mean", "sum", "none", None] = "sum", **kwargs: Any) -> None:
         _deprecated_root_import_class("TotalVariation", "image")
-        return super().__init__(reduction=reduction, **kwargs)
+        super().__init__(reduction=reduction, **kwargs)
 
 
 class _UniversalImageQualityIndex(UniversalImageQualityIndex):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> preds = torch.rand([16, 1, 16, 16])
@@ -249,10 +249,8 @@
         kernel_size: Sequence[int] = (11, 11),
         sigma: Sequence[float] = (1.5, 1.5),
         reduction: Literal["elementwise_mean", "sum", "none", None] = "elementwise_mean",
         data_range: Optional[float] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("UniversalImageQualityIndex", "image")
-        return super().__init__(
-            kernel_size=kernel_size, sigma=sigma, reduction=reduction, data_range=data_range, **kwargs
-        )
+        super().__init__(kernel_size=kernel_size, sigma=sigma, reduction=reduction, data_range=data_range, **kwargs)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/d_lambda.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/ergas.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/fid.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/fid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/inception.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/inception.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 raise ModuleNotFoundError(
                     "InceptionScore metric requires that `Torch-fidelity` is installed."
                     " Either install as `pip install torchmetrics[image]` or `pip install torch-fidelity`."
                 )
             valid_int_input = ("logits_unbiased", 64, 192, 768, 2048)
             if feature not in valid_int_input:
                 raise ValueError(
-                    f"Integer input to argument `feature` must be one of {valid_int_input}," f" but got {feature}."
+                    f"Integer input to argument `feature` must be one of {valid_int_input}, but got {feature}."
                 )
 
             self.inception = NoTrainInceptionV3(name="inception-v3-compat", features_list=[str(feature)])
         elif isinstance(feature, Module):
             self.inception = feature
         else:
             raise TypeError("Got unknown input to argument `feature`")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/kid.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/kid.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 raise ModuleNotFoundError(
                     "Kernel Inception Distance metric requires that `Torch-fidelity` is installed."
                     " Either install as `pip install torchmetrics[image]` or `pip install torch-fidelity`."
                 )
             valid_int_input = ("logits_unbiased", 64, 192, 768, 2048)
             if feature not in valid_int_input:
                 raise ValueError(
-                    f"Integer input to argument `feature` must be one of {valid_int_input}," f" but got {feature}."
+                    f"Integer input to argument `feature` must be one of {valid_int_input}, but got {feature}."
                 )
 
             self.inception: Module = NoTrainInceptionV3(name="inception-v3-compat", features_list=[str(feature)])
         elif isinstance(feature, Module):
             self.inception = feature
         else:
             raise TypeError("Got unknown input to argument `feature`")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/lpip.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/lpip.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-from typing import Any, List, Optional, Sequence, Union
+from typing import Any, ClassVar, List, Optional, Sequence, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 from typing_extensions import Literal
 
 from torchmetrics.functional.image.lpips import _LPIPS, _lpips_compute, _lpips_update, _NoTrainLpips
@@ -97,15 +97,15 @@
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     real_features: List[Tensor]
     fake_features: List[Tensor]
 
     # due to the use of named tuple in the backbone the net variable cannot be scripted
-    __jit_ignored_attributes__ = ["net"]
+    __jit_ignored_attributes__: ClassVar[List[str]] = ["net"]
 
     def __init__(
         self,
         net_type: Literal["alex", "alex", "squeeze"] = "alex",
         reduction: Literal["sum", "mean"] = "mean",
         normalize: bool = False,
         **kwargs: Any,
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/psnr.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/psnrb.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/rase.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/rase.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/rmse_sw.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/sam.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/ssim.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/tv.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/image/uqi.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/metric.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+# It is needed to distinguish between native float and Metric's' function called float.
+# later, this function was used instead of the built-in float type...
+import builtins
 import functools
 import inspect
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from copy import deepcopy
-from typing import Any, Callable, Dict, Generator, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, ClassVar, Dict, Generator, List, Optional, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 
 from torchmetrics.utilities.data import (
     _flatten,
@@ -69,19 +73,20 @@
                 for list states.
             - dist_sync_on_step: If metric state should synchronize on ``forward()``. Default is ``False``
             - process_group: The process group on which the synchronization is called. Default is the world.
             - dist_sync_fn: function that performs the allgather option on the metric state. Default is an
                 custom implementation that calls ``torch.distributed.all_gather`` internally.
             - distributed_available_fn: function that checks if the distributed backend is available.
                 Defaults to a check of ``torch.distributed.is_available()`` and ``torch.distributed.is_initialized()``.
-            - sync_on_compute: If metric state should synchronize when ``compute`` is called. Default is ``True``-
+            - sync_on_compute: If metric state should synchronize when ``compute`` is called. Default is ``True``
+            - compute_with_cache: If results from ``compute`` should be cached. Default is ``False``
     """
 
-    __jit_ignored_attributes__ = ["device"]
-    __jit_unused_properties__ = [
+    __jit_ignored_attributes__: ClassVar[List[str]] = ["device"]
+    __jit_unused_properties__: ClassVar[List[str]] = [
         "is_differentiable",
         "higher_is_better",
         "plot_lower_bound",
         "plot_upper_bound",
         "plot_legend_name",
     ]
     is_differentiable: Optional[bool] = None
@@ -127,14 +132,19 @@
         self.distributed_available_fn = kwargs.pop("distributed_available_fn", None) or jit_distributed_available
 
         self.sync_on_compute = kwargs.pop("sync_on_compute", True)
         if not isinstance(self.sync_on_compute, bool):
             raise ValueError(
                 f"Expected keyword argument `sync_on_compute` to be a `bool` but got {self.sync_on_compute}"
             )
+        self.compute_with_cache = kwargs.pop("compute_with_cache", True)
+        if not isinstance(self.compute_with_cache, bool):
+            raise ValueError(
+                f"Expected keyword argument `compute_with_cache` to be a `bool` but got {self.compute_with_cache}"
+            )
 
         if kwargs:
             kwargs_ = [f"`{a}`" for a in sorted(kwargs)]
             raise ValueError(f"Unexpected keyword arguments: {', '.join(kwargs_)}")
 
         # initialize
         self._update_signature = inspect.signature(self.update)
@@ -555,18 +565,20 @@
             # if synchronization happened, the current rank accumulated states will be restored to keep
             # accumulation going if ``should_unsync=True``,
             with self.sync_context(
                 dist_sync_fn=self.dist_sync_fn,
                 should_sync=self._to_sync,
                 should_unsync=self._should_unsync,
             ):
-                value = compute(*args, **kwargs)
-                self._computed = _squeeze_if_scalar(value)
+                value = _squeeze_if_scalar(compute(*args, **kwargs))
 
-            return self._computed
+            if self.compute_with_cache:
+                self._computed = value
+
+            return value
 
         return wrapped_func
 
     @abstractmethod
     def update(self, *_: Any, **__: Any) -> None:
         """Override this method to update the state variables of your metric class."""
 
@@ -660,22 +672,22 @@
         super().__setattr__(name, value)
 
     @property
     def device(self) -> "torch.device":
         """Return the device of the metric."""
         return self._device
 
-    def type(self, dst_type: Union[str, torch.dtype]) -> "Metric":
+    def type(self, dst_type: Union[str, torch.dtype]) -> "Metric":  # noqa: A003
         """Override default and prevent dtype casting.
 
         Please use `metric.set_dtype(dtype)` instead.
         """
         return self
 
-    def float(self) -> "Metric":
+    def float(self) -> "Metric":  # noqa: A003
         """Override default and prevent dtype casting.
 
         Please use `metric.set_dtype(dtype)` instead.
         """
         return self
 
     def double(self) -> "Metric":
@@ -699,41 +711,49 @@
             dst_type (type or string): the desired type.
         """
         self._dtype_convert = True
         out = super().type(dst_type)
         out._dtype_convert = False
         return out
 
-    def _apply(self, fn: Callable) -> Module:
+    def _apply(self, fn: Callable, exclude_state: Sequence[str] = "") -> Module:
         """Overwrite _apply function such that we can also move metric states to the correct device.
 
         This method is called by the base ``nn.Module`` class whenever `.to`, `.cuda`, `.float`, `.half` etc. methods
         are called. Dtype conversion is garded and will only happen through the special `set_dtype` method.
+
+        Args:
+            fn: the function to apply
+            exclude_state: list of state variables to exclude from applying the function, that then needs to be handled
+                by the metric class itself.
         """
         this = super()._apply(fn)
         fs = str(fn)
         cond = any(f in fs for f in ["Module.type", "Module.half", "Module.float", "Module.double", "Module.bfloat16"])
         if not self._dtype_convert and cond:
             return this
 
         # Also apply fn to metric states and defaults
         for key, value in this._defaults.items():
+            if key in exclude_state:
+                continue
+
             if isinstance(value, Tensor):
                 this._defaults[key] = fn(value)
             elif isinstance(value, Sequence):
                 this._defaults[key] = [fn(v) for v in value]
 
             current_val = getattr(this, key)
             if isinstance(current_val, Tensor):
                 setattr(this, key, fn(current_val))
             elif isinstance(current_val, Sequence):
                 setattr(this, key, [fn(cur_v) for cur_v in current_val])
             else:
                 raise TypeError(
-                    "Expected metric state to be either a Tensor" f"or a list of Tensor, but encountered {current_val}"
+                    f"Expected metric state to be either a Tensor or a list of Tensor, but encountered {current_val}"
                 )
 
         # make sure to update the device attribute
         # if the dummy tensor moves device by fn function we should also update the attribute
         self._device = fn(torch.zeros(1, device=self.device)).device
 
         # Additional apply to forward cache and computed attributes (may be nested)
@@ -840,125 +860,146 @@
             if hasattr(val, "__iter__") and not isinstance(val, Tensor):
                 hash_vals.extend(val)
             else:
                 hash_vals.append(val)
 
         return hash(tuple(hash_vals))
 
-    def __add__(self, other: "Metric") -> "CompositionalMetric":
+    def __add__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the addition operator."""
         return CompositionalMetric(torch.add, self, other)
 
-    def __and__(self, other: "Metric") -> "CompositionalMetric":
+    def __and__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the logical and operator."""
         return CompositionalMetric(torch.bitwise_and, self, other)
 
-    def __eq__(self, other: "Metric") -> "CompositionalMetric":  # type: ignore[override]
+    def __eq__(  # type: ignore[override]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the equal operator."""
         return CompositionalMetric(torch.eq, self, other)
 
-    def __floordiv__(self, other: "Metric") -> "CompositionalMetric":
+    def __floordiv__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the floor division operator."""
         return CompositionalMetric(torch.floor_divide, self, other)
 
-    def __ge__(self, other: "Metric") -> "CompositionalMetric":
+    def __ge__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the greater than or equal operator."""
         return CompositionalMetric(torch.ge, self, other)
 
-    def __gt__(self, other: "Metric") -> "CompositionalMetric":
+    def __gt__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the greater than operator."""
         return CompositionalMetric(torch.gt, self, other)
 
-    def __le__(self, other: "Metric") -> "CompositionalMetric":
+    def __le__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the less than or equal operator."""
         return CompositionalMetric(torch.le, self, other)
 
-    def __lt__(self, other: "Metric") -> "CompositionalMetric":
+    def __lt__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the less than operator."""
         return CompositionalMetric(torch.lt, self, other)
 
-    def __matmul__(self, other: "Metric") -> "CompositionalMetric":
+    def __matmul__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the matrix multiplication operator."""
         return CompositionalMetric(torch.matmul, self, other)
 
-    def __mod__(self, other: "Metric") -> "CompositionalMetric":
+    def __mod__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the remainder operator."""
         return CompositionalMetric(torch.fmod, self, other)
 
-    def __mul__(self, other: "Metric") -> "CompositionalMetric":
+    def __mul__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the multiplication operator."""
         return CompositionalMetric(torch.mul, self, other)
 
-    # Fixme: this shall return bool instead of Metric
-    def __ne__(self, other: "Metric") -> "CompositionalMetric":  # type: ignore[override]
+    def __ne__(  # type: ignore[override]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the not equal operator."""
         return CompositionalMetric(torch.ne, self, other)
 
-    def __or__(self, other: "Metric") -> "CompositionalMetric":
+    def __or__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the logical or operator."""
         return CompositionalMetric(torch.bitwise_or, self, other)
 
-    def __pow__(self, other: "Metric") -> "CompositionalMetric":
+    def __pow__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the exponential/power operator."""
         return CompositionalMetric(torch.pow, self, other)
 
-    def __radd__(self, other: "Metric") -> "CompositionalMetric":
+    def __radd__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the addition operator."""
         return CompositionalMetric(torch.add, other, self)
 
-    def __rand__(self, other: "Metric") -> "CompositionalMetric":
+    def __rand__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the logical and operator."""
         # swap them since bitwise_and only supports that way and it's commutative
         return CompositionalMetric(torch.bitwise_and, self, other)
 
     def __rfloordiv__(self, other: "CompositionalMetric") -> "Metric":
         """Construct compositional metric using the floor division operator."""
         return CompositionalMetric(torch.floor_divide, other, self)
 
-    def __rmatmul__(self, other: "Metric") -> "CompositionalMetric":
+    def __rmatmul__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the matrix multiplication operator."""
         return CompositionalMetric(torch.matmul, other, self)
 
-    def __rmod__(self, other: "Metric") -> "CompositionalMetric":
+    def __rmod__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the remainder operator."""
         return CompositionalMetric(torch.fmod, other, self)
 
-    def __rmul__(self, other: "Metric") -> "CompositionalMetric":
+    def __rmul__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the multiplication operator."""
         return CompositionalMetric(torch.mul, other, self)
 
-    def __ror__(self, other: "Metric") -> "CompositionalMetric":
+    def __ror__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the logical or operator."""
         return CompositionalMetric(torch.bitwise_or, other, self)
 
-    def __rpow__(self, other: "Metric") -> "CompositionalMetric":
+    def __rpow__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the exponential/power operator."""
         return CompositionalMetric(torch.pow, other, self)
 
-    def __rsub__(self, other: "Metric") -> "CompositionalMetric":
+    def __rsub__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the subtraction operator."""
         return CompositionalMetric(torch.sub, other, self)
 
-    def __rtruediv__(self, other: "Metric") -> "CompositionalMetric":
+    def __rtruediv__(  # type: ignore[misc]
+        self, other: Union["Metric", int, builtins.float, Tensor]
+    ) -> "CompositionalMetric":
         """Construct compositional metric using the true divide operator."""
         return CompositionalMetric(torch.true_divide, other, self)
 
-    def __rxor__(self, other: "Metric") -> "CompositionalMetric":
+    def __rxor__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the logical xor operator."""
         return CompositionalMetric(torch.bitwise_xor, other, self)
 
-    def __sub__(self, other: "Metric") -> "CompositionalMetric":
+    def __sub__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the subtraction operator."""
         return CompositionalMetric(torch.sub, self, other)
 
-    def __truediv__(self, other: "Metric") -> "CompositionalMetric":
+    def __truediv__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the true divide operator."""
         return CompositionalMetric(torch.true_divide, self, other)
 
-    def __xor__(self, other: "Metric") -> "CompositionalMetric":
+    def __xor__(self, other: Union["Metric", int, builtins.float, Tensor]) -> "CompositionalMetric":
         """Construct compositional metric using the logical xor operator."""
         return CompositionalMetric(torch.bitwise_xor, self, other)
 
     def __abs__(self) -> "CompositionalMetric":
         """Construct compositional metric using the absolute operator."""
         return CompositionalMetric(torch.abs, self, None)
 
@@ -1031,15 +1072,14 @@
         if isinstance(metric_b, Tensor):
             self.register_buffer("metric_b", metric_b, persistent=False)
         else:
             self.metric_b = metric_b
 
     def _sync_dist(self, dist_sync_fn: Optional[Callable] = None, process_group: Optional[Any] = None) -> None:
         """No syncing required here. syncing will be done in metric_a and metric_b."""
-        pass
 
     def update(self, *args: Any, **kwargs: Any) -> None:
         """Redirect the call to the input which the conposition was formed from."""
         if isinstance(self.metric_a, Metric):
             self.metric_a.update(*args, **self.metric_a._filter_kwargs(**kwargs))
 
         if isinstance(self.metric_b, Metric):
@@ -1067,25 +1107,29 @@
         val_b = (
             self.metric_b(*args, **self.metric_b._filter_kwargs(**kwargs))
             if isinstance(self.metric_b, Metric)
             else self.metric_b
         )
 
         if val_a is None:
-            return None
+            self._forward_cache = None
+            return self._forward_cache
 
         if val_b is None:
             if isinstance(self.metric_b, Metric):
-                return None
+                self._forward_cache = None
+                return self._forward_cache
 
             # Unary op
-            return self.op(val_a)
+            self._forward_cache = self.op(val_a)
+            return self._forward_cache
 
         # Binary op
-        return self.op(val_a, val_b)
+        self._forward_cache = self.op(val_a, val_b)
+        return self._forward_cache
 
     def reset(self) -> None:
         """Redirect the call to the input which the conposition was formed from."""
         if isinstance(self.metric_a, Metric):
             self.metric_a.reset()
 
         if isinstance(self.metric_b, Metric):
@@ -1101,13 +1145,13 @@
         if isinstance(self.metric_a, Metric):
             self.metric_a.persistent(mode=mode)
         if isinstance(self.metric_b, Metric):
             self.metric_b.persistent(mode=mode)
 
     def __repr__(self) -> str:
         """Return a representation of the compositional metric, including the two inputs it was formed from."""
-        _op_metrics = f"(\n  {self.op.__name__}(\n    {repr(self.metric_a)},\n    {repr(self.metric_b)}\n  )\n)"
+        _op_metrics = f"(\n  {self.op.__name__}(\n    {self.metric_a!r},\n    {self.metric_b!r}\n  )\n)"
         return self.__class__.__name__ + _op_metrics
 
     def _wrap_compute(self, compute: Callable) -> Callable:
         """No wrapping nessesary for compositional metrics."""
         return compute
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/multimodal/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/multimodal/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.utilities.imports import _TRANSFORMERS_AVAILABLE
 
 __all__ = []
 
 if _TRANSFORMERS_AVAILABLE:
-    from torchmetrics.multimodal.clip_score import CLIPScore  # noqa: F401
+    from torchmetrics.multimodal.clip_score import CLIPScore
 
     __all__.append("CLIPScore")
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/multimodal/clip_score.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/multimodal/clip_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = True
     plot_lower_bound: float = 0.0
 
     score: Tensor
     n_samples: Tensor
-    plot_lower_bound = 0.0
     plot_upper_bound = 100.0
 
     def __init__(
         self,
         model_name_or_path: Literal[
             "openai/clip-vit-base-patch16",
             "openai/clip-vit-base-patch32",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/nominal/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/nominal/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.nominal.cramers import CramersV
+from torchmetrics.nominal.fleiss_kappa import FleissKappa
 from torchmetrics.nominal.pearson import PearsonsContingencyCoefficient
 from torchmetrics.nominal.theils_u import TheilsU
 from torchmetrics.nominal.tschuprows import TschuprowsT
 
 __all__ = [
     "CramersV",
+    "FleissKappa",
     "PearsonsContingencyCoefficient",
     "TheilsU",
     "TschuprowsT",
 ]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/nominal/cramers.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/nominal/pearson.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/nominal/theils_u.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/nominal/tschuprows.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from torchmetrics.regression.log_mse import MeanSquaredLogError
 from torchmetrics.regression.mae import MeanAbsoluteError
 from torchmetrics.regression.mape import MeanAbsolutePercentageError
 from torchmetrics.regression.minkowski import MinkowskiDistance
 from torchmetrics.regression.mse import MeanSquaredError
 from torchmetrics.regression.pearson import PearsonCorrCoef
 from torchmetrics.regression.r2 import R2Score
+from torchmetrics.regression.rse import RelativeSquaredError
 from torchmetrics.regression.spearman import SpearmanCorrCoef
 from torchmetrics.regression.symmetric_mape import SymmetricMeanAbsolutePercentageError
 from torchmetrics.regression.tweedie_deviance import TweedieDevianceScore
 from torchmetrics.regression.wmape import WeightedMeanAbsolutePercentageError
 
 __all__ = [
     "ConcordanceCorrCoef",
@@ -39,12 +40,13 @@
     "MeanSquaredLogError",
     "MeanAbsoluteError",
     "MeanAbsolutePercentageError",
     "MinkowskiDistance",
     "MeanSquaredError",
     "PearsonCorrCoef",
     "R2Score",
+    "RelativeSquaredError",
     "SpearmanCorrCoef",
     "SymmetricMeanAbsolutePercentageError",
     "TweedieDevianceScore",
     "WeightedMeanAbsolutePercentageError",
 ]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/concordance.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/cosine_similarity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/explained_variance.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/kendall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/kendall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/kl_divergence.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/log_cosh.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/log_mse.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/mae.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/mape.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/minkowski.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/mse.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/pearson.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/r2.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/spearman.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/symmetric_mape.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/tweedie_deviance.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/regression/wmape.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.retrieval.average_precision import RetrievalMAP
-from torchmetrics.retrieval.base import RetrievalMetric  # noqa: F401
+from torchmetrics.retrieval.base import RetrievalMetric
 from torchmetrics.retrieval.fall_out import RetrievalFallOut
 from torchmetrics.retrieval.hit_rate import RetrievalHitRate
 from torchmetrics.retrieval.ndcg import RetrievalNormalizedDCG
 from torchmetrics.retrieval.precision import RetrievalPrecision
 from torchmetrics.retrieval.precision_recall_curve import RetrievalPrecisionRecallCurve, RetrievalRecallAtFixedPrecision
 from torchmetrics.retrieval.r_precision import RetrievalRPrecision
 from torchmetrics.retrieval.recall import RetrievalRecall
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/_deprecated.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,15 @@
         self,
         empty_target_action: str = "pos",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalFallOut", "retrieval")
-        return super().__init__(
-            empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs
-        )
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs)
 
 
 class _RetrievalHitRate(RetrievalHitRate):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> indexes = tensor([0, 0, 0, 1, 1, 1, 1])
@@ -53,17 +51,15 @@
         self,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalHitRate", "retrieval")
-        return super().__init__(
-            empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs
-        )
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs)
 
 
 class _RetrievalMAP(RetrievalMAP):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> indexes = tensor([0, 0, 0, 1, 1, 1, 1])
@@ -78,17 +74,15 @@
         self,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalMAP", "retrieval")
-        return super().__init__(
-            empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs
-        )
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs)
 
 
 class _RetrievalRecall(RetrievalRecall):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> indexes = tensor([0, 0, 0, 1, 1, 1, 1])
@@ -103,17 +97,15 @@
         self,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalRecall", "retrieval")
-        return super().__init__(
-            empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs
-        )
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs)
 
 
 class _RetrievalRPrecision(RetrievalRPrecision):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> indexes = tensor([0, 0, 0, 1, 1, 1, 1])
@@ -127,15 +119,15 @@
     def __init__(
         self,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalRPrecision", "retrieval")
-        return super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, **kwargs)
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, **kwargs)
 
 
 class _RetrievalNormalizedDCG(RetrievalNormalizedDCG):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> indexes = tensor([0, 0, 0, 1, 1, 1, 1])
@@ -150,17 +142,15 @@
         self,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalNormalizedDCG", "retrieval")
-        return super().__init__(
-            empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs
-        )
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, top_k=top_k, **kwargs)
 
 
 class _RetrievalPrecision(RetrievalPrecision):
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> indexes = tensor([0, 0, 0, 1, 1, 1, 1])
@@ -176,15 +166,15 @@
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         adaptive_k: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("", "retrieval")
-        return super().__init__(
+        super().__init__(
             empty_target_action=empty_target_action,
             ignore_index=ignore_index,
             top_k=top_k,
             adaptive_k=adaptive_k,
             **kwargs,
         )
 
@@ -211,15 +201,15 @@
         max_k: Optional[int] = None,
         adaptive_k: bool = False,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("", "retrieval")
-        return super().__init__(
+        super().__init__(
             max_k=max_k,
             adaptive_k=adaptive_k,
             empty_target_action=empty_target_action,
             ignore_index=ignore_index,
             **kwargs,
         )
 
@@ -242,15 +232,15 @@
         max_k: Optional[int] = None,
         adaptive_k: bool = False,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("RetrievalRecallAtFixedPrecision", "retrieval")
-        return super().__init__(
+        super().__init__(
             min_precision=min_precision,
             max_k=max_k,
             adaptive_k=adaptive_k,
             empty_target_action=empty_target_action,
             ignore_index=ignore_index,
             **kwargs,
         )
@@ -271,8 +261,8 @@
     def __init__(
         self,
         empty_target_action: str = "neg",
         ignore_index: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("", "retrieval")
-        return super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, **kwargs)
+        super().__init__(empty_target_action=empty_target_action, ignore_index=ignore_index, **kwargs)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/average_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/base.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/fall_out.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/hit_rate.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/ndcg.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/precision_recall_curve.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/r_precision.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/recall.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/retrieval/reciprocal_rank.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from torchmetrics.text.ter import TranslationEditRate
 from torchmetrics.text.wer import WordErrorRate
 from torchmetrics.text.wil import WordInfoLost
 from torchmetrics.text.wip import WordInfoPreserved
 from torchmetrics.utilities.imports import _TRANSFORMERS_AVAILABLE
 
 if _TRANSFORMERS_AVAILABLE:
-    from torchmetrics.text.bert import BERTScore  # noqa: F401
-    from torchmetrics.text.infolm import InfoLM  # noqa: F401
+    from torchmetrics.text.bert import BERTScore
+    from torchmetrics.text.infolm import InfoLM
 
 
 __all__ = [
     "BLEUScore",
     "CharErrorRate",
     "CHRFScore",
     "ExtendedEditDistance",
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/_deprecated.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/_deprecated.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self,
         n_gram: int = 4,
         smooth: bool = False,
         weights: Optional[Sequence[float]] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("BLEUScore", "text")
-        return super().__init__(n_gram=n_gram, smooth=smooth, weights=weights, **kwargs)
+        super().__init__(n_gram=n_gram, smooth=smooth, weights=weights, **kwargs)
 
 
 class _CharErrorRate(CharErrorRate):
     """Wrapper for deprecated import.
 
     >>> preds = ["this is the prediction", "there is an other sample"]
     >>> target = ["this is the reference", "there is another one"]
@@ -47,15 +47,15 @@
     """
 
     def __init__(
         self,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("CharErrorRate", "text")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class _CHRFScore(CHRFScore):
     """Wrapper for deprecated import.
 
     >>> preds = ['the cat is on the mat']
     >>> target = [['there is a cat on the mat', 'a cat is on the mat']]
@@ -71,15 +71,15 @@
         beta: float = 2.0,
         lowercase: bool = False,
         whitespace: bool = False,
         return_sentence_level_score: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("CHRFScore", "text")
-        return super().__init__(
+        super().__init__(
             n_char_order=n_char_order,
             n_word_order=n_word_order,
             beta=beta,
             lowercase=lowercase,
             whitespace=whitespace,
             return_sentence_level_score=return_sentence_level_score,
             **kwargs,
@@ -103,15 +103,15 @@
         alpha: float = 2.0,
         rho: float = 0.3,
         deletion: float = 0.2,
         insertion: float = 1.0,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("ExtendedEditDistance", "text")
-        return super().__init__(
+        super().__init__(
             language=language,
             return_sentence_level_score=return_sentence_level_score,
             alpha=alpha,
             rho=rho,
             deletion=deletion,
             insertion=insertion,
             **kwargs,
@@ -129,15 +129,15 @@
     """
 
     def __init__(
         self,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("MatchErrorRate", "text")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class _Perplexity(Perplexity):
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> preds = torch.rand(2, 8, 5, generator=torch.manual_seed(22))
@@ -150,15 +150,15 @@
 
     def __init__(
         self,
         ignore_index: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("Perplexity", "text")
-        return super().__init__(ignore_index=ignore_index, **kwargs)
+        super().__init__(ignore_index=ignore_index, **kwargs)
 
 
 class _SacreBLEUScore(SacreBLEUScore):
     """Wrapper for deprecated import.
 
     >>> preds = ['the cat is on the mat']
     >>> target = [['there is a cat on the mat', 'a cat is on the mat']]
@@ -173,15 +173,15 @@
         smooth: bool = False,
         tokenize: Literal["none", "13a", "zh", "intl", "char"] = "13a",
         lowercase: bool = False,
         weights: Optional[Sequence[float]] = None,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("SacreBLEUScore", "text")
-        return super().__init__(
+        super().__init__(
             n_gram=n_gram, smooth=smooth, tokenize=tokenize, lowercase=lowercase, weights=weights, **kwargs
         )
 
 
 class _SQuAD(SQuAD):
     """Wrapper for deprecated import.
 
@@ -190,15 +190,15 @@
     >>> squad = _SQuAD()
     >>> squad(preds, target)
     {'exact_match': tensor(100.), 'f1': tensor(100.)}
     """
 
     def __init__(self, **kwargs: Any) -> None:
         _deprecated_root_import_class("SQuAD", "text")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class _TranslationEditRate(TranslationEditRate):
     """Wrapper for deprecated import.
 
     >>> preds = ['the cat is on the mat']
     >>> target = [['there is a cat on the mat', 'a cat is on the mat']]
@@ -213,15 +213,15 @@
         no_punctuation: bool = False,
         lowercase: bool = True,
         asian_support: bool = False,
         return_sentence_level_score: bool = False,
         **kwargs: Any,
     ) -> None:
         _deprecated_root_import_class("TranslationEditRate", "text")
-        return super().__init__(
+        super().__init__(
             normalize=normalize,
             no_punctuation=no_punctuation,
             lowercase=lowercase,
             asian_support=asian_support,
             return_sentence_level_score=return_sentence_level_score,
             **kwargs,
         )
@@ -235,38 +235,38 @@
     >>> wer = _WordErrorRate()
     >>> wer(preds, target)
     tensor(0.5000)
     """
 
     def __init__(self, **kwargs: Any) -> None:
         _deprecated_root_import_class("WordErrorRate", "text")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class _WordInfoLost(WordInfoLost):
     """Wrapper for deprecated import.
 
     >>> preds = ["this is the prediction", "there is an other sample"]
     >>> target = ["this is the reference", "there is another one"]
     >>> wil = _WordInfoLost()
     >>> wil(preds, target)
     tensor(0.6528)
     """
 
     def __init__(self, **kwargs: Any) -> None:
         _deprecated_root_import_class("WordInfoLost", "text")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class _WordInfoPreserved(WordInfoPreserved):
     """Wrapper for deprecated import.
 
     >>> preds = ["this is the prediction", "there is an other sample"]
     >>> target = ["this is the reference", "there is another one"]
     >>> wip = WordInfoPreserved()
     >>> wip(preds, target)
     tensor(0.3472)
     """
 
     def __init__(self, **kwargs: Any) -> None:
         _deprecated_root_import_class("WordInfoPreserved", "text")
-        return super().__init__(**kwargs)
+        super().__init__(**kwargs)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/bert.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import torch
 from torch import Tensor
 from torch.nn import Module
 
 from torchmetrics.functional.text.bert import bert_score
 from torchmetrics.functional.text.helper_embedding_metric import _preprocess_text
 from torchmetrics.metric import Metric
+from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.checks import _SKIP_SLOW_DOCTEST, _try_proceed_with_timeout
 from torchmetrics.utilities.data import dim_zero_cat
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE, _TRANSFORMERS_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["BERTScore.plot"]
@@ -176,15 +177,15 @@
         else:
             if not _TRANSFORMERS_AVAILABLE:
                 raise ModuleNotFoundError(
                     "`BERTScore` metric with default tokenizers requires `transformers` package be installed."
                     " Either install with `pip install transformers>=4.0` or `pip install torchmetrics[text]`."
                 )
             if model_name_or_path is None:
-                warn(
+                rank_zero_warn(
                     "The argument `model_name_or_path` was not specified while it is required when the default"
                     " `transformers` model is used."
                     f" It will use the default recommended model - {_DEFAULT_MODEL!r}."
                 )
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_name_or_path)
             self.user_tokenizer = False
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/bleu.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/cer.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/chrf.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/eed.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/infolm.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/mer.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/perplexity.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/rouge.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/sacre_bleu.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/squad.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/ter.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/wer.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/wil.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/text/wip.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/checks.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/checks.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/compute.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/compute.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Tuple
+from typing import Optional, Tuple
 
 import torch
 from torch import Tensor
 
 from torchmetrics.utilities.imports import _TORCH_GREATER_EQUAL_1_9
 
 
@@ -51,14 +51,28 @@
     """
     denom[denom == 0.0] = 1
     num = num if num.is_floating_point() else num.float()
     denom = denom if denom.is_floating_point() else denom.float()
     return num / denom
 
 
+def _adjust_weights_safe_divide(
+    score: Tensor, average: Optional[str], multilabel: bool, tp: Tensor, fp: Tensor, fn: Tensor
+) -> Tensor:
+    if average is None or average == "none":
+        return score
+    if average == "weighted":
+        weights = tp + fn
+    else:
+        weights = torch.ones_like(score)
+        if not multilabel:
+            weights[tp + fp + fn == 0] = 0.0
+    return _safe_divide(weights * score, weights.sum(-1, keepdim=True)).sum(-1)
+
+
 def _auc_format_inputs(x: Tensor, y: Tensor) -> Tuple[Tensor, Tensor]:
     """Check that auc input is correct."""
     x = x.squeeze() if x.ndim > 1 else x
     y = y.squeeze() if y.ndim > 1 else y
 
     if x.ndim > 1 or y.ndim > 1:
         raise ValueError(
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/data.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/data.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/distributed.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,15 @@
     if class_reduction == "macro":
         return torch.mean(fraction)
     if class_reduction == "weighted":
         return torch.sum(fraction * (weights.float() / torch.sum(weights)))
     if class_reduction == "none" or class_reduction is None:
         return fraction
 
-    raise ValueError(
-        f"Reduction parameter {class_reduction} unknown." f" Choose between one of these: {valid_reduction}"
-    )
+    raise ValueError(f"Reduction parameter {class_reduction} unknown. Choose between one of these: {valid_reduction}")
 
 
 def _simple_gather_all_tensors(result: Tensor, group: Any, world_size: int) -> List[Tensor]:
     gathered_result = [torch.zeros_like(result) for _ in range(world_size)]
     torch.distributed.all_gather(gathered_result, result, group)
     return gathered_result
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/enums.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,19 @@
         >>> MyEnum.from_str("c")
         Traceback (most recent call last):
           ...
         ValueError: Invalid Task: expected one of ['a', 'b'], but got c.
         """
         try:
             me = super().from_str(value.replace("-", "_"), source=source)
-        except ValueError:
+        except ValueError as err:
             _allowed_im = [m.lower() for m in cls._member_names_]
-            raise ValueError(f"Invalid {cls._name()}: expected one of {cls._allowed_matches(source)}, but got {value}.")
+            raise ValueError(
+                f"Invalid {cls._name()}: expected one of {cls._allowed_matches(source)}, but got {value}."
+            ) from err
         return cls(me)
 
 
 class DataType(EnumStr):
     """Enum to represent data type.
 
     >>> "Binary" in list(DataType)
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/exceptions.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/imports.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/plot.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     @contextmanager
     def style_change(*args: Any, **kwargs: Any) -> Generator:
         """No-ops decorator if matplotlib is not installed."""
         yield
 
 
 if _SCIENCEPLOT_AVAILABLE:
-    import scienceplots  # noqa: F401
+    import scienceplots
 
     _style = ["science", "no-latex"]
 
 _style = ["science"] if _SCIENCEPLOT_AVAILABLE and _LATEX_AVAILABLE else ["default"]
 
 
 def _error_on_missing_matplotlib() -> None:
@@ -143,15 +143,15 @@
 
     ax.grid(True)
     ax.set_ylabel(name if name is not None else None)
 
     xlim = ax.get_xlim()
     factor = 0.1 * (xlim[1] - xlim[0])
 
-    y_ = [lower_bound, upper_bound] if lower_bound or upper_bound else []
+    y_ = [lower_bound, upper_bound] if lower_bound and upper_bound else []
     ax.hlines(y_, xlim[0], xlim[1], linestyles="dashed", colors="k")
     if higher_is_better is not None:
         if lower_bound is not None and not higher_is_better:
             ax.set_xlim(xlim[0] - factor, xlim[1])
             ax.text(
                 xlim[0], lower_bound, s="Optimal \n value", horizontalalignment="center", verticalalignment="center"
             )
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/utilities/prints.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/utilities/prints.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 # add the attribute to the function but don't overwrite in case Trainer has already set it
 rank_zero_only.rank = getattr(rank_zero_only, "rank", int(os.environ.get("LOCAL_RANK", 0)))
 
 
 def _warn(*args: Any, **kwargs: Any) -> None:
-    warnings.warn(*args, **kwargs)
+    warnings.warn(*args, **kwargs)  # noqa: B028
 
 
 def _info(*args: Any, **kwargs: Any) -> None:
     log.info(*args, **kwargs)
 
 
 def _debug(*args: Any, **kwargs: Any) -> None:
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/__init__.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from torchmetrics.wrappers.bootstrapping import BootStrapper
 from torchmetrics.wrappers.classwise import ClasswiseWrapper
 from torchmetrics.wrappers.minmax import MinMaxMetric
 from torchmetrics.wrappers.multioutput import MultioutputWrapper
+from torchmetrics.wrappers.multitask import MultitaskWrapper
+from torchmetrics.wrappers.running import Running
 from torchmetrics.wrappers.tracker import MetricTracker
 
 __all__ = [
     "BootStrapper",
     "ClasswiseWrapper",
     "MinMaxMetric",
     "MultioutputWrapper",
+    "MultitaskWrapper",
     "MetricTracker",
+    "Running",
 ]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/bootstrapping.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/bootstrapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
         resampled tensor
     """
     if sampling_strategy == "poisson":
         p = torch.distributions.Poisson(1)
         n = p.sample((size,))
         return torch.arange(size).repeat_interleave(n.long(), dim=0)
     if sampling_strategy == "multinomial":
-        idx = torch.multinomial(torch.ones(size), num_samples=size, replacement=True)
-        return idx
+        return torch.multinomial(torch.ones(size), num_samples=size, replacement=True)
     raise ValueError("Unknown sampling strategy")
 
 
 class BootStrapper(Metric):
     r"""Using `Turn a Metric into a Bootstrapped`_.
 
     That can automate the process of getting confidence intervals for metric values. This wrapper
@@ -96,15 +95,15 @@
         raw: bool = False,
         sampling_strategy: str = "poisson",
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         if not isinstance(base_metric, Metric):
             raise ValueError(
-                "Expected base metric to be an instance of torchmetrics.Metric" f" but received {base_metric}"
+                f"Expected base metric to be an instance of torchmetrics.Metric but received {base_metric}"
             )
 
         self.metrics = ModuleList([deepcopy(base_metric) for _ in range(num_bootstraps)])
         self.num_bootstraps = num_bootstraps
 
         self.mean = mean
         self.std = std
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/classwise.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/classwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 from torch import Tensor
 
-from torchmetrics import Metric
+from torchmetrics.metric import Metric
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["ClasswiseWrapper.plot"]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/minmax.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/minmax.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/multioutput.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/multioutput.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from copy import deepcopy
 from typing import Any, Callable, List, Optional, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor
 from torch.nn import ModuleList
 
-from torchmetrics import Metric
+from torchmetrics.metric import Metric
 from torchmetrics.utilities import apply_to_collection
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["MultioutputWrapper.plot"]
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics/wrappers/tracker.py` & `torchmetrics-1.0.0rc1/src/torchmetrics/wrappers/tracker.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/PKG-INFO` & `torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -37,41 +37,41 @@
 Provides-Extra: visual
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc0/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc1/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
   <a href="#implementing-your-own-module-metric">Implementing a metric</a> •
   <a href="#build-in-metrics">Built-in metrics</a> •
-  <a href="https://torchmetrics.readthedocs.io/en/v1.0.0.rc0">Docs</a> •
+  <a href="https://torchmetrics.readthedocs.io/en/v1.0.0.rc1">Docs</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 ______________________________________________________________________
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchmetrics)](https://pypi.org/project/torchmetrics/)
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI Status](https://pepy.tech/badge/torchmetrics)](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing - complete](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.0.rc0)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.0.rc0)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.0.rc0/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.0.rc1)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.0.rc1)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.0.rc1/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -306,15 +306,15 @@
 acc = torchmetrics.functional.classification.multiclass_accuracy(
     preds, target, num_classes=5
 )
 ```
 
 ### Covered domains and example metrics
 
-In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.0.rc0all-metrics.html), which
+In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.0.rc1all-metrics.html), which
 convers the following domains:
 
 - Audio
 - Classification
 - Detection
 - Information Retrieval
 - Image
@@ -360,15 +360,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc0/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.0.rc1/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/SOURCES.txt` & `torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 src/torchmetrics/functional/image/lpips_models/alex.pth
 src/torchmetrics/functional/image/lpips_models/squeeze.pth
 src/torchmetrics/functional/image/lpips_models/vgg.pth
 src/torchmetrics/functional/multimodal/__init__.py
 src/torchmetrics/functional/multimodal/clip_score.py
 src/torchmetrics/functional/nominal/__init__.py
 src/torchmetrics/functional/nominal/cramers.py
+src/torchmetrics/functional/nominal/fleiss_kappa.py
 src/torchmetrics/functional/nominal/pearson.py
 src/torchmetrics/functional/nominal/theils_u.py
 src/torchmetrics/functional/nominal/tschuprows.py
 src/torchmetrics/functional/nominal/utils.py
 src/torchmetrics/functional/pairwise/__init__.py
 src/torchmetrics/functional/pairwise/cosine.py
 src/torchmetrics/functional/pairwise/euclidean.py
@@ -158,14 +159,15 @@
 src/torchmetrics/functional/regression/log_mse.py
 src/torchmetrics/functional/regression/mae.py
 src/torchmetrics/functional/regression/mape.py
 src/torchmetrics/functional/regression/minkowski.py
 src/torchmetrics/functional/regression/mse.py
 src/torchmetrics/functional/regression/pearson.py
 src/torchmetrics/functional/regression/r2.py
+src/torchmetrics/functional/regression/rse.py
 src/torchmetrics/functional/regression/spearman.py
 src/torchmetrics/functional/regression/symmetric_mape.py
 src/torchmetrics/functional/regression/tweedie_deviance.py
 src/torchmetrics/functional/regression/utils.py
 src/torchmetrics/functional/regression/wmape.py
 src/torchmetrics/functional/retrieval/__init__.py
 src/torchmetrics/functional/retrieval/_deprecated.py
@@ -213,14 +215,15 @@
 src/torchmetrics/image/ssim.py
 src/torchmetrics/image/tv.py
 src/torchmetrics/image/uqi.py
 src/torchmetrics/multimodal/__init__.py
 src/torchmetrics/multimodal/clip_score.py
 src/torchmetrics/nominal/__init__.py
 src/torchmetrics/nominal/cramers.py
+src/torchmetrics/nominal/fleiss_kappa.py
 src/torchmetrics/nominal/pearson.py
 src/torchmetrics/nominal/theils_u.py
 src/torchmetrics/nominal/tschuprows.py
 src/torchmetrics/regression/__init__.py
 src/torchmetrics/regression/concordance.py
 src/torchmetrics/regression/cosine_similarity.py
 src/torchmetrics/regression/explained_variance.py
@@ -230,14 +233,15 @@
 src/torchmetrics/regression/log_mse.py
 src/torchmetrics/regression/mae.py
 src/torchmetrics/regression/mape.py
 src/torchmetrics/regression/minkowski.py
 src/torchmetrics/regression/mse.py
 src/torchmetrics/regression/pearson.py
 src/torchmetrics/regression/r2.py
+src/torchmetrics/regression/rse.py
 src/torchmetrics/regression/spearman.py
 src/torchmetrics/regression/symmetric_mape.py
 src/torchmetrics/regression/tweedie_deviance.py
 src/torchmetrics/regression/wmape.py
 src/torchmetrics/retrieval/__init__.py
 src/torchmetrics/retrieval/_deprecated.py
 src/torchmetrics/retrieval/average_precision.py
@@ -278,8 +282,10 @@
 src/torchmetrics/utilities/plot.py
 src/torchmetrics/utilities/prints.py
 src/torchmetrics/wrappers/__init__.py
 src/torchmetrics/wrappers/bootstrapping.py
 src/torchmetrics/wrappers/classwise.py
 src/torchmetrics/wrappers/minmax.py
 src/torchmetrics/wrappers/multioutput.py
+src/torchmetrics/wrappers/multitask.py
+src/torchmetrics/wrappers/running.py
 src/torchmetrics/wrappers/tracker.py
```

### Comparing `torchmetrics-1.0.0rc0/src/torchmetrics.egg-info/requires.txt` & `torchmetrics-1.0.0rc1/src/torchmetrics.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,144 +6,148 @@
 [:python_version < "3.9"]
 typing-extensions
 
 [all]
 pystoi<=0.3.3
 pycocotools>2.0.0
 torchvision>=0.8
-lpips<=0.1.4
 torch-fidelity<=0.3.0
 scipy>1.0.0
+lpips<=0.1.4
 transformers>=4.10.0
-tqdm>=4.41.0
 nltk>=3.6
+tqdm>=4.41.0
 regex>=2021.9.24
-types-emoji
-types-tabulate
+mypy==1.4.1
 types-six
-types-PyYAML
+types-emoji
+types-requests
 types-setuptools
 types-protobuf
-types-requests
-mypy==1.2.0
-SciencePlots>=2.0.0
+types-tabulate
+types-PyYAML
 matplotlib>=3.2.0
+SciencePlots>=2.0.0
 
 [audio]
 pystoi<=0.3.3
 
 [detection]
 pycocotools>2.0.0
 torchvision>=0.8
 
 [dev]
 pystoi<=0.3.3
 pycocotools>2.0.0
 torchvision>=0.8
-lpips<=0.1.4
 torch-fidelity<=0.3.0
 scipy>1.0.0
+lpips<=0.1.4
 transformers>=4.10.0
-tqdm>=4.41.0
 nltk>=3.6
+tqdm>=4.41.0
 regex>=2021.9.24
-types-emoji
-types-tabulate
+mypy==1.4.1
 types-six
-types-PyYAML
+types-emoji
+types-requests
 types-setuptools
 types-protobuf
-types-requests
-mypy==1.2.0
-SciencePlots>=2.0.0
+types-tabulate
+types-PyYAML
 matplotlib>=3.2.0
+SciencePlots>=2.0.0
+huggingface-hub<0.16
+coverage==7.2.7
+scikit-learn>=1.1.1
+pytest-timeout==2.1.0
+scikit-image>=0.19.0
+requests<=2.31.0
+cloudpickle>1.3
+dython<=0.7.4
+sacrebleu>=2.0.0
+pytest-cov==4.1.0
+pandas>=1.4.0
+pytorch-msssim==1.0.0
+bert_score==0.3.13
+kornia>=0.6.7
 mir-eval>=0.6
+sewar>=0.4.4
 rouge-score>0.1.0
-pytest-timeout==2.1.0
 psutil<=5.9.5
-cloudpickle>1.3
-pytest-rerunfailures==11.1.2
-transformers>4.4.0
+statsmodels>0.13.5
+torch_complex<=0.4.3
+pytest-doctestplus==0.13.0
+pandas>1.0.0
 fire<=0.5.0
-huggingface-hub<0.15
-kornia>=0.6.7
-netcal>1.0.0
-pytest-doctestplus==0.12.1
-phmdoctest==1.4.0
 fast-bss-eval>=0.1.0
-scikit-image>=0.19.0
-pandas>=1.4.0
-requests<=2.29.0
-dython<=0.7.3
-pytest==7.3.1
-coverage==7.2.5
-scikit-learn>=1.1.1
-pandas>1.0.0
-jiwer>=2.3.0
-torch_complex<=0.4.3
-sacrebleu>=2.0.0
-pytorch-msssim==0.2.1
-bert_score==0.3.13
+transformers>4.4.0
+phmdoctest==1.4.0
 fairlearn
-sewar>=0.4.4
-pytest-cov==4.0.0,>2.10
+pytest==7.4.0
+netcal>1.0.0
+jiwer>=2.3.0
+pytest-rerunfailures==11.1.2
+numpy<1.25.0
 
 [image]
-lpips<=0.1.4
+torchvision>=0.8
 torch-fidelity<=0.3.0
 scipy>1.0.0
-torchvision>=0.8
+lpips<=0.1.4
 
 [multimodal]
 transformers>=4.10.0
 
 [test]
+huggingface-hub<0.16
+coverage==7.2.7
+scikit-learn>=1.1.1
+pytest-timeout==2.1.0
+scikit-image>=0.19.0
+requests<=2.31.0
+cloudpickle>1.3
+dython<=0.7.4
+sacrebleu>=2.0.0
+pytest-cov==4.1.0
+pandas>=1.4.0
+pytorch-msssim==1.0.0
+scipy>1.0.0
+bert_score==0.3.13
+kornia>=0.6.7
 mir-eval>=0.6
+sewar>=0.4.4
 rouge-score>0.1.0
-pytest-timeout==2.1.0
 psutil<=5.9.5
-cloudpickle>1.3
-pytest-rerunfailures==11.1.2
-transformers>4.4.0
+statsmodels>0.13.5
+torch_complex<=0.4.3
+pytest-doctestplus==0.13.0
+pandas>1.0.0
 fire<=0.5.0
-huggingface-hub<0.15
-kornia>=0.6.7
-netcal>1.0.0
-scipy>1.0.0
-pytest-doctestplus==0.12.1
-phmdoctest==1.4.0
 fast-bss-eval>=0.1.0
-scikit-image>=0.19.0
-pandas>=1.4.0
-requests<=2.29.0
-dython<=0.7.3
-pytest==7.3.1
-coverage==7.2.5
-scikit-learn>=1.1.1
-pandas>1.0.0
-jiwer>=2.3.0
-torch_complex<=0.4.3
-sacrebleu>=2.0.0
-pytorch-msssim==0.2.1
-bert_score==0.3.13
+transformers>4.4.0
+phmdoctest==1.4.0
 fairlearn
-sewar>=0.4.4
-pytest-cov==4.0.0,>2.10
+pytest==7.4.0
+netcal>1.0.0
+jiwer>=2.3.0
+pytest-rerunfailures==11.1.2
+numpy<1.25.0
 
 [text]
-tqdm>=4.41.0
 nltk>=3.6
+tqdm>=4.41.0
 regex>=2021.9.24
 
 [typing]
-types-emoji
-types-tabulate
+mypy==1.4.1
 types-six
-types-PyYAML
+types-emoji
+types-requests
 types-setuptools
 types-protobuf
-types-requests
-mypy==1.2.0
+types-tabulate
+types-PyYAML
 
 [visual]
-SciencePlots>=2.0.0
 matplotlib>=3.2.0
+SciencePlots>=2.0.0
```

