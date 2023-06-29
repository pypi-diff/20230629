# Comparing `tmp/zhousf-lib-0.7.9.tar.gz` & `tmp/zhousf-lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.7.9.tar", last modified: Thu Jun 29 06:07:33 2023, max compression
+gzip compressed data, was "zhousf-lib-0.8.0.tar", last modified: Thu Jun 29 06:32:35 2023, max compression
```

## Comparing `zhousf-lib-0.7.9.tar` & `zhousf-lib-0.8.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.309444 zhousf-lib-0.7.9/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.7.9/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-06-29 06:07:33.308445 zhousf-lib-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.7.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 06:07:33.309444 zhousf-lib-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-06-29 06:07:17.000000 zhousf-lib-0.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.696876 zhousf-lib-0.7.9/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-06-29 06:07:32.000000 zhousf-lib-0.7.9/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2257 2023-06-29 06:07:32.000000 zhousf-lib-0.7.9/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:07:32.000000 zhousf-lib-0.7.9/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 06:07:32.000000 zhousf-lib-0.7.9/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.697876 zhousf-lib-0.7.9/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.9/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.698906 zhousf-lib-0.7.9/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.7.9/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.700905 zhousf-lib-0.7.9/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.7.9/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.769077 zhousf-lib-0.7.9/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.833496 zhousf-lib-0.7.9/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.842528 zhousf-lib-0.7.9/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.7.9/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.855493 zhousf-lib-0.7.9/zhousflib/db/
--rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.7.9/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.7.9/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.868492 zhousf-lib-0.7.9/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.9/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:32.884514 zhousf-lib-0.7.9/zhousflib/download/
--rw-rw-rw-   0        0        0       60 2023-06-16 08:05:46.000000 zhousf-lib-0.7.9/zhousflib/download/__init__.py
--rw-rw-rw-   0        0        0     4646 2023-06-16 08:07:58.000000 zhousf-lib-0.7.9/zhousflib/download/download_util.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.005020 zhousf-lib-0.7.9/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.7.9/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.7.9/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.7.9/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.017455 zhousf-lib-0.7.9/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.7.9/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.041664 zhousf-lib-0.7.9/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.9/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4761 2023-06-19 03:04:32.000000 zhousf-lib-0.7.9/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     5872 2023-06-19 03:04:56.000000 zhousf-lib-0.7.9/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.097334 zhousf-lib-0.7.9/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.7.9/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.127718 zhousf-lib-0.7.9/zhousflib/so/
--rw-rw-rw-   0        0        0       87 2023-06-27 03:01:19.000000 zhousf-lib-0.7.9/zhousflib/so/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-06-27 03:01:19.000000 zhousf-lib-0.7.9/zhousflib/so/project_to_so.py
--rw-rw-rw-   0        0        0      273 2023-06-27 03:01:19.000000 zhousf-lib-0.7.9/zhousflib/so/py_to_so.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.278450 zhousf-lib-0.7.9/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     2821 2023-06-29 06:07:00.000000 zhousf-lib-0.7.9/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0     2067 2023-06-27 02:49:36.000000 zhousf-lib-0.7.9/zhousflib/util/char_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2609 2023-06-16 08:07:58.000000 zhousf-lib-0.7.9/zhousflib/util/dict_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.7.9/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0     1592 2023-06-14 06:14:27.000000 zhousf-lib-0.7.9/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0     1564 2023-06-26 06:05:28.000000 zhousf-lib-0.7.9/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1432 2023-06-16 08:43:33.000000 zhousf-lib-0.7.9/zhousflib/util/math_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.7.9/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      502 2023-06-16 08:10:19.000000 zhousf-lib-0.7.9/zhousflib/util/random_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.7.9/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     2209 2023-06-16 08:11:27.000000 zhousf-lib-0.7.9/zhousflib/util/thread_util.py
--rw-rw-rw-   0        0        0      794 2023-06-16 08:11:54.000000 zhousf-lib-0.7.9/zhousflib/util/threadpool_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.7.9/zhousflib/util/time_util.py
--rw-rw-rw-   0        0        0     3122 2023-06-16 08:43:33.000000 zhousf-lib-0.7.9/zhousflib/util/zip_util.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:07:33.292446 zhousf-lib-0.7.9/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.7.9/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.7.9/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.7.9/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.102902 zhousf-lib-0.8.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2073 2023-06-29 06:32:35.101901 zhousf-lib-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 06:32:35.102902 zhousf-lib-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-06-29 06:32:27.000000 zhousf-lib-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.029884 zhousf-lib-0.8.0/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-06-29 06:32:34.000000 zhousf-lib-0.8.0/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2257 2023-06-29 06:32:34.000000 zhousf-lib-0.8.0/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:32:34.000000 zhousf-lib-0.8.0/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-29 06:32:34.000000 zhousf-lib-0.8.0/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.030885 zhousf-lib-0.8.0/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.8.0/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.031885 zhousf-lib-0.8.0/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.8.0/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.033885 zhousf-lib-0.8.0/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.8.0/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.039886 zhousf-lib-0.8.0/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.044888 zhousf-lib-0.8.0/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.046887 zhousf-lib-0.8.0/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.8.0/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.047888 zhousf-lib-0.8.0/zhousflib/db/
+-rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.8.0/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.8.0/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.050889 zhousf-lib-0.8.0/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.0/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.052888 zhousf-lib-0.8.0/zhousflib/download/
+-rw-rw-rw-   0        0        0       60 2023-06-16 08:05:46.000000 zhousf-lib-0.8.0/zhousflib/download/__init__.py
+-rw-rw-rw-   0        0        0     4646 2023-06-16 08:07:58.000000 zhousf-lib-0.8.0/zhousflib/download/download_util.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.067893 zhousf-lib-0.8.0/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.8.0/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.8.0/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.8.0/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.068919 zhousf-lib-0.8.0/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.8.0/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.071893 zhousf-lib-0.8.0/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.8.0/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4761 2023-06-19 03:04:32.000000 zhousf-lib-0.8.0/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     5872 2023-06-19 03:04:56.000000 zhousf-lib-0.8.0/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.075894 zhousf-lib-0.8.0/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.8.0/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.077895 zhousf-lib-0.8.0/zhousflib/so/
+-rw-rw-rw-   0        0        0       85 2023-06-29 06:08:24.000000 zhousf-lib-0.8.0/zhousflib/so/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-06-27 03:01:19.000000 zhousf-lib-0.8.0/zhousflib/so/project_to_so.py
+-rw-rw-rw-   0        0        0      273 2023-06-27 03:01:19.000000 zhousf-lib-0.8.0/zhousflib/so/py_to_so.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.097898 zhousf-lib-0.8.0/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-29 06:09:10.000000 zhousf-lib-0.8.0/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0     2067 2023-06-27 02:49:36.000000 zhousf-lib-0.8.0/zhousflib/util/char_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2609 2023-06-16 08:07:58.000000 zhousf-lib-0.8.0/zhousflib/util/dict_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.8.0/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0     1593 2023-06-29 06:32:27.000000 zhousf-lib-0.8.0/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0     1564 2023-06-26 06:05:28.000000 zhousf-lib-0.8.0/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1432 2023-06-16 08:43:33.000000 zhousf-lib-0.8.0/zhousflib/util/math_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.8.0/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      502 2023-06-16 08:10:19.000000 zhousf-lib-0.8.0/zhousflib/util/random_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.8.0/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     2209 2023-06-16 08:11:27.000000 zhousf-lib-0.8.0/zhousflib/util/thread_util.py
+-rw-rw-rw-   0        0        0      794 2023-06-16 08:11:54.000000 zhousf-lib-0.8.0/zhousflib/util/threadpool_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.8.0/zhousflib/util/time_util.py
+-rw-rw-rw-   0        0        0     3122 2023-06-16 08:43:33.000000 zhousf-lib-0.8.0/zhousflib/util/zip_util.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:32:35.100900 zhousf-lib-0.8.0/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.8.0/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.8.0/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.8.0/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.7.9/LICENSE` & `zhousf-lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/PKG-INFO` & `zhousf-lib-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.7.9
+Version: 0.8.0
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.7.9/README.md` & `zhousf-lib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/setup.py` & `zhousf-lib-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.7.9'
+VERSION = '0.8.0'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.7.9/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.8.0/zhousf_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.7.9
+Version: 0.8.0
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.7.9/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.8.0/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-0.8.0/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.8.0/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.8.0/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.8.0/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.8.0/zhousflib/db/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.8.0/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/download/download_util.py` & `zhousf-lib-0.8.0/zhousflib/download/download_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.8.0/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.8.0/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/font/__init__.py` & `zhousf-lib-0.8.0/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.8.0/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-0.8.0/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.8.0/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/pdf/export_image.py` & `zhousf-lib-0.8.0/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.8.0/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/so/project_to_so.py` & `zhousf-lib-0.8.0/zhousflib/so/project_to_so.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/calculater_util.py` & `zhousf-lib-0.8.0/zhousflib/util/calculater_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 # @Author  : zhousf
 # @Function: 计算器
 import re
-from decimal import Decimal
 
 
 def cal(calc_formula: str) -> str:
     """
     公式计算，保持原有格式计算数值的项
     :param calc_formula:
     :return:
```

### Comparing `zhousf-lib-0.7.9/zhousflib/util/char_util.py` & `zhousf-lib-0.8.0/zhousflib/util/char_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/cv_util.py` & `zhousf-lib-0.8.0/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/dict_util.py` & `zhousf-lib-0.8.0/zhousflib/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.8.0/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/img_util.py` & `zhousf-lib-0.8.0/zhousflib/util/img_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Description:
 import imghdr
 import base64
 import hashlib
 from pathlib import Path
 
 
-def get_file_base64(file_path: Path, contain_file_name=True, split_char=","):
+def get_file_base64(file_path: Path, contain_file_name=False, split_char=","):
     """
     图片转base64
     :param file_path: 图片路径
     :param contain_file_name: 是否包含文件名称
     :param split_char: 分隔符
     :return: 'a.jpg,iVBORw0KGgoAAAANSUhEUgAABNcAAANtCAYAAACzHZ25AAA.....'
     """
```

### Comparing `zhousf-lib-0.7.9/zhousflib/util/iou_util.py` & `zhousf-lib-0.8.0/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/json_util.py` & `zhousf-lib-0.8.0/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/list_util.py` & `zhousf-lib-0.8.0/zhousflib/util/list_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/math_util.py` & `zhousf-lib-0.8.0/zhousflib/util/math_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/permission_util.py` & `zhousf-lib-0.8.0/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/poly_util.py` & `zhousf-lib-0.8.0/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/re_util.py` & `zhousf-lib-0.8.0/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/singleton.py` & `zhousf-lib-0.8.0/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/string_util.py` & `zhousf-lib-0.8.0/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/thread_util.py` & `zhousf-lib-0.8.0/zhousflib/util/thread_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/threadpool_util.py` & `zhousf-lib-0.8.0/zhousflib/util/threadpool_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/time_util.py` & `zhousf-lib-0.8.0/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/util/zip_util.py` & `zhousf-lib-0.8.0/zhousflib/util/zip_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/web/log_util.py` & `zhousf-lib-0.8.0/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/web/logger.py` & `zhousf-lib-0.8.0/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.9/zhousflib/web/response.py` & `zhousf-lib-0.8.0/zhousflib/web/response.py`

 * *Files identical despite different names*

