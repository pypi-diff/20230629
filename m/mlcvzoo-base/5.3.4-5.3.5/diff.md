# Comparing `tmp/mlcvzoo_base-5.3.4.tar.gz` & `tmp/mlcvzoo_base-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_base-5.3.4.tar", max compression
+gzip compressed data, was "mlcvzoo_base-5.3.5.tar", max compression
```

## Comparing `mlcvzoo_base-5.3.4.tar` & `mlcvzoo_base-5.3.5.tar`

### file list

```diff
@@ -1,102 +1,101 @@
--rw-r--r--   0        0        0    11412 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/LICENSE
--rw-r--r--   0        0        0      546 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/README.md
--rw-r--r--   0        0        0      244 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/__init__.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/configuration.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/__init__.py
--rw-r--r--   0        0        0    11270 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation.py
--rw-r--r--   0        0        0      816 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_attributes.py
--rw-r--r--   0        0        0     2429 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_builder.py
--rw-r--r--   0        0        0    26777 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_class_mapper.py
--rw-r--r--   0        0        0     1130 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_parser.py
--rw-r--r--   0        0        0      975 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_writer.py
--rw-r--r--   0        0        0     6146 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/bounding_box.py
--rw-r--r--   0        0        0    13021 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/box.py
--rw-r--r--   0        0        0     2734 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/class_identifier.py
--rw-r--r--   0        0        0     5253 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/classification.py
--rw-r--r--   0        0        0     3941 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/dataset_info.py
--rw-r--r--   0        0        0     3268 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/ocr_perception.py
--rw-r--r--   0        0        0    11655 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/segmentation.py
--rw-r--r--   0        0        0      362 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/types.py
--rw-r--r--   0        0        0      906 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/exceptions.py
--rw-r--r--   0        0        0     5029 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/interfaces.py
--rw-r--r--   0        0        0    12243 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/model.py
--rw-r--r--   0        0        0     2333 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/api/registry.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/__init__.py
--rw-r--r--   0        0        0     8184 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/annotation_handler_config.py
--rw-r--r--   0        0        0     3942 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/class_mapping_config.py
--rw-r--r--   0        0        0      656 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/config_registry.py
--rw-r--r--   0        0        0      772 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/device_query.py
--rw-r--r--   0        0        0     1692 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/mlfow_config.py
--rw-r--r--   0        0        0     3093 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/model_config.py
--rw-r--r--   0        0        0     2589 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/reduction_mapping_config.py
--rw-r--r--   0        0        0     3889 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/replacement_config.py
--rw-r--r--   0        0        0     3939 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/structs.py
--rw-r--r--   0        0        0     7286 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/utils.py
--rw-r--r--   0        0        0      628 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/visualization_config.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/__init__.py
--rw-r--r--   0        0        0      256 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
--rw-r--r--   0        0        0     8663 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
--rw-r--r--   0        0        0     7121 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
--rw-r--r--   0        0        0     2458 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
--rw-r--r--   0        0        0     8862 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
--rw-r--r--   0        0        0     6066 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
--rw-r--r--   0        0        0    14648 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_handler.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
--rw-r--r--   0        0        0     3289 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
--rw-r--r--   0        0        0     8168 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
--rw-r--r--   0        0        0    11628 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
--rw-r--r--   0        0        0     7841 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
--rw-r--r--   0        0        0    10617 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
--rw-r--r--   0        0        0     9205 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
--rw-r--r--   0        0        0    14717 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
--rw-r--r--   0        0        0     8684 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
--rw-r--r--   0        0        0     4097 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
--rw-r--r--   0        0        0      501 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/structs.py
--rw-r--r--   0        0        0    11234 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/utils.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.185691 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/__init__.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/__init__.py
--rw-r--r--   0        0        0     2227 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/configuration.py
--rw-r--r--   0        0        0     6836 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/data_classes.py
--rw-r--r--   0        0        0    54097 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
--rw-r--r--   0        0        0    12295 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
--rw-r--r--   0        0        0     4134 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
--rw-r--r--   0        0        0      633 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/structs.py
--rw-r--r--   0        0        0    15646 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/utils.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/__init__.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/__init__.py
--rw-r--r--   0        0        0     7255 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
--rw-r--r--   0        0        0     1676 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/utils.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/__init__.py
--rw-r--r--   0        0        0      257 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/constants.py
--rw-r--r--   0        0        0    10705 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/model_registry.py
--rw-r--r--   0        0        0      196 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/__init__.py
--rw-r--r--   0        0        0     1540 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/configuration.py
--rw-r--r--   0        0        0    10713 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/model.py
--rw-r--r--   0        0        0        0 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/py.typed
--rw-r--r--   0        0        0        0 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/__init__.py
--rw-r--r--   0        0        0     1078 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
--rw-r--r--   0        0        0      138 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
--rw-r--r--   0        0        0      249 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
--rw-r--r--   0        0        0     1774 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
--rw-r--r--   0        0        0     1117 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/LICENSE.txt
--rw-r--r--   0        0        0      108 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/README.md
--rw-r--r--   0        0        0      296 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/__init__.py
--rw-r--r--   0        0        0     2794 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/perspective.py
--rw-r--r--   0        0        0     3744 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
--rw-r--r--   0        0        0      127 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/README.md
--rw-r--r--   0        0        0      249 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
--rw-r--r--   0        0        0      488 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/__init__.py
--rw-r--r--   0        0        0     4725 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/annotation_utils.py
--rw-r--r--   0        0        0     2353 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/common_utils.py
--rw-r--r--   0        0        0    11836 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/draw_utils.py
--rw-r--r--   0        0        0     5992 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/file_utils.py
--rw-r--r--   0        0        0     5852 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/gpu_util.py
--rw-r--r--   0        0        0     3009 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/implicit_path_replacements.py
--rw-r--r--   0        0        0     2435 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/versioning_utils.py
--rw-r--r--   0        0        0     3811 2023-05-24 07:49:45.189692 mlcvzoo_base-5.3.4/mlcvzoo_base/utils/xml_utils.py
--rw-r--r--   0        0        0     4007 2023-05-24 07:50:46.943977 mlcvzoo_base-5.3.4/pyproject.toml
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.4/setup.py
--rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/LICENSE
+-rw-r--r--   0        0        0      546 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/README.md
+-rw-r--r--   0        0        0      244 2023-06-28 12:38:21.251374 mlcvzoo_base-5.3.5/mlcvzoo_base/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/configuration.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/__init__.py
+-rw-r--r--   0        0        0    11270 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation.py
+-rw-r--r--   0        0        0      816 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_attributes.py
+-rw-r--r--   0        0        0     2429 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_builder.py
+-rw-r--r--   0        0        0    26718 2023-06-26 18:45:14.775134 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_class_mapper.py
+-rw-r--r--   0        0        0     1130 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_parser.py
+-rw-r--r--   0        0        0      975 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_writer.py
+-rw-r--r--   0        0        0     6146 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/bounding_box.py
+-rw-r--r--   0        0        0    12867 2023-06-26 18:45:14.779134 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/box.py
+-rw-r--r--   0        0        0     2734 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/class_identifier.py
+-rw-r--r--   0        0        0     5253 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/classification.py
+-rw-r--r--   0        0        0     3941 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/dataset_info.py
+-rw-r--r--   0        0        0     3268 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/ocr_perception.py
+-rw-r--r--   0        0        0    11655 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/segmentation.py
+-rw-r--r--   0        0        0      362 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/types.py
+-rw-r--r--   0        0        0      906 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/exceptions.py
+-rw-r--r--   0        0        0     5029 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/interfaces.py
+-rw-r--r--   0        0        0    12243 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/model.py
+-rw-r--r--   0        0        0     2333 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/api/registry.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/__init__.py
+-rw-r--r--   0        0        0     8184 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/annotation_handler_config.py
+-rw-r--r--   0        0        0     3942 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/class_mapping_config.py
+-rw-r--r--   0        0        0      656 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/config_registry.py
+-rw-r--r--   0        0        0      772 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/device_query.py
+-rw-r--r--   0        0        0     1692 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/mlfow_config.py
+-rw-r--r--   0        0        0     3093 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/model_config.py
+-rw-r--r--   0        0        0     2589 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/reduction_mapping_config.py
+-rw-r--r--   0        0        0     3889 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/replacement_config.py
+-rw-r--r--   0        0        0     3939 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/structs.py
+-rw-r--r--   0        0        0     7286 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/utils.py
+-rw-r--r--   0        0        0      628 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/visualization_config.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
+-rw-r--r--   0        0        0     8679 2023-06-26 19:02:09.012193 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
+-rw-r--r--   0        0        0     7137 2023-06-26 19:02:09.012193 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
+-rw-r--r--   0        0        0     2458 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
+-rw-r--r--   0        0        0     8862 2023-06-26 18:45:14.779134 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
+-rw-r--r--   0        0        0     6011 2023-06-26 19:02:09.012193 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
+-rw-r--r--   0        0        0    14648 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_handler.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
+-rw-r--r--   0        0        0     3289 2023-06-26 09:55:34.504681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
+-rw-r--r--   0        0        0     8168 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
+-rw-r--r--   0        0        0    11589 2023-06-26 19:02:09.012193 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
+-rw-r--r--   0        0        0     7839 2023-06-26 18:45:14.779134 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
+-rw-r--r--   0        0        0    10617 2023-06-26 18:45:14.779134 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
+-rw-r--r--   0        0        0     9205 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
+-rw-r--r--   0        0        0    14717 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
+-rw-r--r--   0        0        0     8684 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
+-rw-r--r--   0        0        0     4097 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
+-rw-r--r--   0        0        0      501 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/structs.py
+-rw-r--r--   0        0        0    11234 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/utils.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/__init__.py
+-rw-r--r--   0        0        0     2227 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/configuration.py
+-rw-r--r--   0        0        0     6836 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/data_classes.py
+-rw-r--r--   0        0        0    54097 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
+-rw-r--r--   0        0        0    12295 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
+-rw-r--r--   0        0        0     4134 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
+-rw-r--r--   0        0        0      633 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/structs.py
+-rw-r--r--   0        0        0    15646 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/utils.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/metrics/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/metrics/mlflow/__init__.py
+-rw-r--r--   0        0        0     7255 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
+-rw-r--r--   0        0        0     1676 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/metrics/mlflow/utils.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/models/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/models/constants.py
+-rw-r--r--   0        0        0    10705 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/models/model_registry.py
+-rw-r--r--   0        0        0      196 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/models/read_from_file/__init__.py
+-rw-r--r--   0        0        0     1540 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/models/read_from_file/configuration.py
+-rw-r--r--   0        0        0    10713 2023-06-26 09:55:34.508681 mlcvzoo_base-5.3.5/mlcvzoo_base/models/read_from_file/model.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:05:46.619706 mlcvzoo_base-5.3.5/mlcvzoo_base/py.typed
+-rw-r--r--   0        0        0        0 2023-06-29 06:05:46.619706 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
+-rw-r--r--   0        0        0      138 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
+-rw-r--r--   0        0        0      249 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
+-rw-r--r--   0        0        0     1774 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
+-rw-r--r--   0        0        0     1117 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/imutils/LICENSE.txt
+-rw-r--r--   0        0        0      108 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/imutils/README.md
+-rw-r--r--   0        0        0      296 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/imutils/__init__.py
+-rw-r--r--   0        0        0     2794 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/imutils/perspective.py
+-rw-r--r--   0        0        0     3744 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
+-rw-r--r--   0        0        0      127 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/py_faster_rcnn/README.md
+-rw-r--r--   0        0        0      249 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
+-rw-r--r--   0        0        0     1649 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
+-rw-r--r--   0        0        0      488 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/__init__.py
+-rw-r--r--   0        0        0     4725 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/annotation_utils.py
+-rw-r--r--   0        0        0     2353 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/common_utils.py
+-rw-r--r--   0        0        0    11836 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/draw_utils.py
+-rw-r--r--   0        0        0     5992 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/file_utils.py
+-rw-r--r--   0        0        0     5852 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/gpu_util.py
+-rw-r--r--   0        0        0     3009 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/implicit_path_replacements.py
+-rw-r--r--   0        0        0     2435 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/versioning_utils.py
+-rw-r--r--   0        0        0     3811 2023-06-26 09:55:34.512681 mlcvzoo_base-5.3.5/mlcvzoo_base/utils/xml_utils.py
+-rw-r--r--   0        0        0     4024 2023-06-28 12:38:21.251374 mlcvzoo_base-5.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.5/PKG-INFO
```

### Comparing `mlcvzoo_base-5.3.4/LICENSE` & `mlcvzoo_base-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/README.md` & `mlcvzoo_base-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/configuration.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_attributes.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_attributes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_builder.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_class_mapper.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_class_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,14 @@
         self.__model_class_name_to_class_identifier_map: Dict[
             str, List[ClassIdentifier]
         ] = self.__create_model_class_name_to_class_identifier_map(
             annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map,
             model_class_id_to_class_identifier_map=self.__model_class_id_to_class_identifier_map,
         )
 
-        logger.debug("AnnotationClassMapper initialized")
-
     @property
     def num_classes(self) -> int:
         """
         Returns the number of classes the AnnotationMapper 'knows'.
 
         Returns:
             The number of classes the AnnotationMapper 'knows'.
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/annotation_writer.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/bounding_box.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/bounding_box.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/box.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/box.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,20 +122,18 @@
 
         Returns:
             A Box object
         """
 
         xmin = box_list[0]
         if xmin < 0:
-            logger.warning("xmin=%d coordinate < 0, clamp xmin to 0" % xmin)
             xmin = max(0, xmin)
 
         ymin = box_list[1]
         if ymin < 0:
-            logger.warning("ymin=%d coordinate < 0, clamp ymin to 0" % ymin)
             ymin = max(0, ymin)
 
         if box_format == ObjectDetectionBBoxFormats.XYWH:
             width = box_list[2]
             if width < 0:
                 raise ValueError("Can not build a box with negative width")
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/class_identifier.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/class_identifier.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/classification.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/classification.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/dataset_info.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/dataset_info.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/ocr_perception.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/ocr_perception.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/data/segmentation.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/exceptions.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/interfaces.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/model.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/api/registry.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/api/registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/annotation_handler_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/annotation_handler_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/class_mapping_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/class_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/config_registry.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/config_registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/device_query.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/device_query.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/mlfow_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/mlfow_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/model_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/model_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/reduction_mapping_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/reduction_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/replacement_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/replacement_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/structs.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/configuration/visualization_config.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/configuration/visualization_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,18 +173,19 @@
                     class_name=coco_class_name
                 )
 
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=coco_class_name
                 )
             except ClassMappingNotFoundError:
-                logger.warning(
+                logger.debug(
                     "Could not find a valid class-mapping for class-name '%s'. "
-                    "BndBox will be skipped, coco-annotation= '%s'"
-                    % (coco_class_name, _coco_annotation)
+                    "BndBox will be skipped, coco-annotation= '%s'",
+                    coco_class_name,
+                    _coco_annotation,
                 )
                 continue
 
             (
                 difficult,
                 occluded,
                 content,
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,19 @@
                     class_name=annotation_class_name
                 )
 
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=annotation_class_name
                 )
             except ClassMappingNotFoundError:
-                logger.warning(
+                logger.debug(
                     "Could not find a valid class-mapping for class-name '%s'. "
-                    "BndBox will be skipped, csv-line-split = '%s'"
-                    % (annotation_class_name, line_split)
+                    "BndBox will be skipped, csv-line-split = '%s'",
+                    annotation_class_name,
+                    line_split,
                 )
                 continue
 
             bounding_boxes.append(
                 BoundingBox(
                     box=Box(
                         xmin=int(annotation_split[0]),
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,19 @@
                     class_name=annotation_class_name
                 )
 
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=annotation_class_name
                 )
             except ClassMappingNotFoundError:
-                logger.warning(
+                logger.debug(
                     "Could not find a valid class-mapping for class-name '%s'. "
-                    "BndBox will be skipped, file = '%s'"
-                    % (
-                        annotation_class_name,
-                        xml_file_path,
-                    )
+                    "BndBox will be skipped, file = '%s'",
+                    annotation_class_name,
+                    xml_file_path,
                 )
                 continue
 
             # TODO: Handle other properties, like 'occluded', 'truncated'
             # TODO: make it configurable? => add to ClassMapping
             difficult = False
             difficult_tag = member.find("difficult")
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_handler.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_handler.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,18 @@
                 class_name = self.mapper.map_annotation_class_name_to_model_class_name(
                     class_name=xml_class_name
                 )
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=xml_class_name
                 )
             except ClassMappingNotFoundError:
-                logger.warning(
+                logger.debug(
                     "Could not find a valid class-mapping for class-name '%s'. "
-                    "Classification will be skipped" % xml_class_name
+                    "Classification will be skipped",
+                    xml_class_name,
                 )
                 continue
 
             classification = Classification(
                 class_identifier=ClassIdentifier(
                     class_id=class_id,
                     class_name=class_name,
@@ -153,21 +154,19 @@
                     class_name=xml_class_name
                 )
 
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=xml_class_name
                 )
             except ClassMappingNotFoundError:
-                logger.warning(
+                logger.debug(
                     "Could not find a valid class-mapping for class-name '%s'. "
-                    "BndBox will be skipped, cvat-box= '%s'"
-                    % (
-                        xml_class_name,
-                        cvat_bbox,
-                    )
+                    "BndBox will be skipped, cvat-box= '%s'",
+                    xml_class_name,
+                    cvat_bbox,
                 )
                 continue
 
             occluded, difficult, content = CVATAnnotationParser.__read_attributes(
                 cvat_bbox.findall("attribute")
             )
 
@@ -214,15 +213,15 @@
                     class_name=xml_class_name
                 )
 
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=xml_class_name
                 )
             except ClassMappingNotFoundError:
-                logger.warning(
+                logger.debug(
                     "Could not find a valid class-mapping for class-name '%s'. "
                     "Segmentation will be skipped, cvat-segmentation= '%s'",
                     xml_class_name,
                     cvat_polygon,
                 )
                 continue
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,13 +175,13 @@
                         int(image_shape[0] * label_studio_value["height"] / 100),
                     ),
                     box_format=ObjectDetectionBBoxFormats.XYWH,
                 ),
             )
 
         except ClassMappingNotFoundError:
-            logger.warning(
+            logger.debug(
                 "Could not find a valid class-mapping for class-name '%s'. "
                 "BoundingBox will be skipped",
                 label_studio_class_name,
             )
             return None
```

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/data_preparation/utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/data_preparation/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/configuration.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/data_classes.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_computation.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/metrics_computation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/metrics_logging.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/metrics_logging.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/model_evaluation.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/structs.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/evaluation/object_detection/utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/evaluation/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/mlflow_runner.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/metrics/mlflow/mlflow_runner.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/metrics/mlflow/utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/metrics/mlflow/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/models/model_registry.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/models/model_registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/configuration.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/models/read_from_file/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/models/read_from_file/model.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/models/read_from_file/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE` & `mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/LICENSE.txt` & `mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/imutils/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/imutils/perspective.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/imutils/perspective.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE` & `mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/annotation_utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/common_utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/draw_utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/file_utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/gpu_util.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/gpu_util.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/implicit_path_replacements.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/implicit_path_replacements.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/versioning_utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/versioning_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/mlcvzoo_base/utils/xml_utils.py` & `mlcvzoo_base-5.3.5/mlcvzoo_base/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.4/pyproject.toml` & `mlcvzoo_base-5.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mlcvzoo_base"
 description = "MLCVZoo Base Package"
-version = "5.3.4"
+version = "5.3.5"
 license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -79,15 +79,15 @@
 extension-pkg-whitelist = ["numpy", "cv2"]
 ignore=["third_party"]
 jobs = 0
 
 [tool.pytest.ini_options]
 log_cli = 1
 log_cli_level = "DEBUG"
-log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s | %(filename)s:%(funcName)s:%(lineno)s"
+log_cli_format = "%(asctime)s [%(name)-30.80s] [%(levelname)8s] %(message)s | %(filename)s:%(funcName)s:%(lineno)s"
 log_cli_date_format= "%Y-%m-%d %H:%M:%S"
 
 [tool.mypy]
 python_version = 3.8
 exclude = ['mlcvzoo_base/tests', 'mlcvzoo_base/third_party']
 
 junit_xml = "xunit-reports/xunit-result-mypy.xml"
```

### Comparing `mlcvzoo_base-5.3.4/PKG-INFO` & `mlcvzoo_base-5.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-base
-Version: 5.3.4
+Version: 5.3.5
 Summary: MLCVZoo Base Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base
 License: Open Logistics Foundation License v1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

