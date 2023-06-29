# Comparing `tmp/yeastvision-0.1.5.tar.gz` & `tmp/yeastvision-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeastvision-0.1.5.tar", last modified: Mon Jun 26 13:35:08 2023, max compression
+gzip compressed data, was "yeastvision-0.1.6.tar", last modified: Thu Jun 29 18:29:07 2023, max compression
```

## Comparing `yeastvision-0.1.5.tar` & `yeastvision-0.1.6.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.174233 yeastvision-0.1.5/
--rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.5/LICENSE
--rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-26 13:35:08.173531 yeastvision-0.1.5/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     3290 2023-06-21 06:06:54.000000 yeastvision-0.1.5/README.md
--rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-26 13:35:08.174427 yeastvision-0.1.5/setup.cfg
--rw-r--r--   0 berk       (502) staff       (20)     1750 2023-06-26 13:34:56.000000 yeastvision-0.1.5/setup.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.125526 yeastvision-0.1.5/yeastvision/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.5/yeastvision/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)    80239 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/__main__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.131049 yeastvision-0.1.5/yeastvision/disk/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.5/yeastvision/disk/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/disk/io.py
--rw-rw-r--   0 berk       (502) staff       (20)    10386 2023-06-13 10:01:09.000000 yeastvision-0.1.5/yeastvision/disk/reader.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.133063 yeastvision-0.1.5/yeastvision/flou/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.5/yeastvision/flou/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.5/yeastvision/flou/blob_detect.py
--rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.5/yeastvision/flou/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     2688 2023-06-20 19:25:38.000000 yeastvision-0.1.5/yeastvision/ims.py
--rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.5/yeastvision/install_weights.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.139287 yeastvision-0.1.5/yeastvision/models/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.142429 yeastvision-0.1.5/yeastvision/models/YeaZ/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/segment.py
--rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.5/yeastvision/models/YeaZ/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.5/yeastvision/models/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.144177 yeastvision-0.1.5/yeastvision/models/artilife/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.5/yeastvision/models/artilife/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.145580 yeastvision-0.1.5/yeastvision/models/artilife/budSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.5/yeastvision/models/artilife/budSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.5/yeastvision/models/artilife/budSeg/model.py
--rw-r--r--   0 berk       (502) staff       (20)     9440 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/models/artilife/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.146804 yeastvision-0.1.5/yeastvision/models/budNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.5/yeastvision/models/budNET/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.5/yeastvision/models/budNET/model.py
--rw-r--r--   0 berk       (502) staff       (20)     3774 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/models/cp.py
--rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.5/yeastvision/models/eval.py
--rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.5/yeastvision/models/loss.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.148098 yeastvision-0.1.5/yeastvision/models/matSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.5/yeastvision/models/matSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.5/yeastvision/models/matSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.5/yeastvision/models/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.149815 yeastvision-0.1.5/yeastvision/models/tetradSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.5/yeastvision/models/tetradSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.5/yeastvision/models/tetradSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.5/yeastvision/models/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.5/yeastvision/models/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.151610 yeastvision-0.1.5/yeastvision/models/vacNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.5/yeastvision/models/vacNET/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.5/yeastvision/models/vacNET/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.161736 yeastvision-0.1.5/yeastvision/parts/
--rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/parts/canvas.py
--rw-r--r--   0 berk       (502) staff       (20)    30883 2023-06-13 09:57:15.000000 yeastvision-0.1.5/yeastvision/parts/dialogs.py
--rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.5/yeastvision/parts/guiparts.py
--rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/parts/menu.py
--rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.5/yeastvision/parts/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     2737 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/parts/workers.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.165173 yeastvision-0.1.5/yeastvision/plot/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.5/yeastvision/plot/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3442 2023-06-14 19:37:54.000000 yeastvision-0.1.5/yeastvision/plot/cell_table.py
--rw-r--r--   0 berk       (502) staff       (20)    11676 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/plot/plot.py
--rw-r--r--   0 berk       (502) staff       (20)     1149 2023-04-05 22:48:46.000000 yeastvision-0.1.5/yeastvision/plot/types.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.171985 yeastvision-0.1.5/yeastvision/track/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.5/yeastvision/track/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     5908 2023-06-13 09:55:42.000000 yeastvision-0.1.5/yeastvision/track/cell.py
--rw-r--r--   0 berk       (502) staff       (20)      265 2023-06-07 05:33:05.000000 yeastvision-0.1.5/yeastvision/track/data.py
--rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.5/yeastvision/track/hungarian_track.py
--rw-r--r--   0 berk       (502) staff       (20)     5510 2023-06-22 04:39:33.000000 yeastvision-0.1.5/yeastvision/track/lineage.py
--rw-r--r--   0 berk       (502) staff       (20)    18190 2023-06-22 04:45:43.000000 yeastvision-0.1.5/yeastvision/track/mat.py
--rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.5/yeastvision/track/track.py
--rw-r--r--   0 berk       (502) staff       (20)     5270 2023-06-20 19:16:44.000000 yeastvision-0.1.5/yeastvision/track/utils.py
--rw-rw-r--   0 berk       (502) staff       (20)     5491 2023-06-20 19:25:28.000000 yeastvision-0.1.5/yeastvision/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-26 13:35:08.129259 yeastvision-0.1.5/yeastvision.egg-info/
--rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     1825 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/SOURCES.txt
--rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/dependency_links.txt
--rw-r--r--   0 berk       (502) staff       (20)      116 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/entry_points.txt
--rw-r--r--   0 berk       (502) staff       (20)      273 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/requires.txt
--rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-26 13:35:08.000000 yeastvision-0.1.5/yeastvision.egg-info/top_level.txt
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.426939 yeastvision-0.1.6/
+-rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.6/LICENSE
+-rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-29 18:29:07.426659 yeastvision-0.1.6/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     3290 2023-06-21 06:06:54.000000 yeastvision-0.1.6/README.md
+-rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-29 18:29:07.427034 yeastvision-0.1.6/setup.cfg
+-rw-r--r--   0 berk       (502) staff       (20)     1750 2023-06-29 18:28:24.000000 yeastvision-0.1.6/setup.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.406439 yeastvision-0.1.6/yeastvision/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.6/yeastvision/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)    80318 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/__main__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.409163 yeastvision-0.1.6/yeastvision/disk/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.6/yeastvision/disk/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1212 2023-06-22 04:39:33.000000 yeastvision-0.1.6/yeastvision/disk/io.py
+-rw-r--r--   0 berk       (502) staff       (20)    10218 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/disk/reader.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.410106 yeastvision-0.1.6/yeastvision/flou/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.6/yeastvision/flou/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.6/yeastvision/flou/blob_detect.py
+-rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.6/yeastvision/flou/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     2688 2023-06-20 19:25:38.000000 yeastvision-0.1.6/yeastvision/ims.py
+-rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.6/yeastvision/install_weights.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.412016 yeastvision-0.1.6/yeastvision/models/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.413180 yeastvision-0.1.6/yeastvision/models/YeaZ/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/segment.py
+-rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.6/yeastvision/models/YeaZ/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.6/yeastvision/models/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.413820 yeastvision-0.1.6/yeastvision/models/artilife/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.6/yeastvision/models/artilife/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.414472 yeastvision-0.1.6/yeastvision/models/artilife/budSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.6/yeastvision/models/artilife/budSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      590 2023-06-21 06:06:54.000000 yeastvision-0.1.6/yeastvision/models/artilife/budSeg/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     9519 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/models/artilife/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.415076 yeastvision-0.1.6/yeastvision/models/budNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.6/yeastvision/models/budNET/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.6/yeastvision/models/budNET/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     3833 2023-06-27 20:12:02.000000 yeastvision-0.1.6/yeastvision/models/cp.py
+-rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.6/yeastvision/models/eval.py
+-rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.6/yeastvision/models/loss.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.415952 yeastvision-0.1.6/yeastvision/models/matSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.6/yeastvision/models/matSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.6/yeastvision/models/matSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.6/yeastvision/models/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.416449 yeastvision-0.1.6/yeastvision/models/tetradSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.6/yeastvision/models/tetradSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.6/yeastvision/models/tetradSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.6/yeastvision/models/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.6/yeastvision/models/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.417075 yeastvision-0.1.6/yeastvision/models/vacNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.6/yeastvision/models/vacNET/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.6/yeastvision/models/vacNET/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.419845 yeastvision-0.1.6/yeastvision/parts/
+-rw-r--r--   0 berk       (502) staff       (20)    13220 2023-06-22 04:39:33.000000 yeastvision-0.1.6/yeastvision/parts/canvas.py
+-rw-r--r--   0 berk       (502) staff       (20)    31747 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/parts/dialogs.py
+-rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.6/yeastvision/parts/guiparts.py
+-rw-r--r--   0 berk       (502) staff       (20)     3724 2023-06-22 04:39:33.000000 yeastvision-0.1.6/yeastvision/parts/menu.py
+-rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.6/yeastvision/parts/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     2734 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/parts/workers.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.421779 yeastvision-0.1.6/yeastvision/plot/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.6/yeastvision/plot/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3461 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/cell_table.py
+-rw-r--r--   0 berk       (502) staff       (20)    12653 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/plot.py
+-rw-r--r--   0 berk       (502) staff       (20)     5056 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/types.py
+-rw-r--r--   0 berk       (502) staff       (20)      391 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/plot/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.426042 yeastvision-0.1.6/yeastvision/track/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.6/yeastvision/track/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     6286 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/cell.py
+-rw-r--r--   0 berk       (502) staff       (20)     8241 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/data.py
+-rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.6/yeastvision/track/hungarian_track.py
+-rw-r--r--   0 berk       (502) staff       (20)        4 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/lc.py
+-rw-r--r--   0 berk       (502) staff       (20)     8413 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/lineage.py
+-rw-r--r--   0 berk       (502) staff       (20)    18443 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/mat.py
+-rw-rw-r--   0 berk       (502) staff       (20)     5357 2023-06-20 19:14:02.000000 yeastvision-0.1.6/yeastvision/track/track.py
+-rw-r--r--   0 berk       (502) staff       (20)     4574 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/track/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     5523 2023-06-29 18:12:58.000000 yeastvision-0.1.6/yeastvision/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-29 18:29:07.408427 yeastvision-0.1.6/yeastvision.egg-info/
+-rw-r--r--   0 berk       (502) staff       (20)     3638 2023-06-29 18:29:06.000000 yeastvision-0.1.6/yeastvision.egg-info/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     1875 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/SOURCES.txt
+-rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-29 18:29:06.000000 yeastvision-0.1.6/yeastvision.egg-info/dependency_links.txt
+-rw-r--r--   0 berk       (502) staff       (20)      115 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/entry_points.txt
+-rw-r--r--   0 berk       (502) staff       (20)      287 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/requires.txt
+-rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-29 18:29:07.000000 yeastvision-0.1.6/yeastvision.egg-info/top_level.txt
```

### Comparing `yeastvision-0.1.5/LICENSE` & `yeastvision-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/PKG-INFO` & `yeastvision-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.5
+Version: 0.1.6
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `yeastvision-0.1.5/README.md` & `yeastvision-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/setup.py` & `yeastvision-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             "yeastvision.models.vacNET", "yeastvision.models.YeaZ"]
 
 
 
 
 setup(
     name = "yeastvision",
-    version = "0.1.5",
+    version = "0.1.6",
     description = "Deep learning-enabled image analysis of the yeast full life cycle",
     author = "Berk Yalcinkaya",
     url = "https://github.com/berkyalcinkaya/yeastvision",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email="berkyalcinkaya55@gmail.com",
     license = "BSD",
```

### Comparing `yeastvision-0.1.5/yeastvision/__main__.py` & `yeastvision-0.1.6/yeastvision/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 tic = process_time()
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2' 
 from PyQt5 import QtWidgets, QtGui, QtCore
 from PyQt5.QtWidgets import (QApplication, QStyle, QMainWindow, QGroupBox, QPushButton, QDialog,
                             QDialogButtonBox, QLineEdit, QFormLayout, QMessageBox,QErrorMessage, QStatusBar, 
                              QFileDialog, QVBoxLayout, QCheckBox, QFrame, QSpinBox, QLabel, QWidget, QComboBox, QSizePolicy, QGridLayout)
-from PyQt5.QtCore import Qt
+from PyQt5.QtCore import Qt, QThread
 import pyqtgraph as pg
 import numpy as np
 import matplotlib.pyplot as plt
 from yeastvision.parts.canvas import ImageDraw, ViewBoxNoRightDrag
 from yeastvision.parts.guiparts import *
-from yeastvision.parts.workers import SegmentWorker
+from yeastvision.parts.workers import SegmentWorker, TrackWorker
 from yeastvision.parts.dialogs import *
 from yeastvision.track.track import track_to_cell, trackYeasts
-from yeastvision.track.data import LineageData
+from yeastvision.track.data import LineageData, TimeSeriesData
 from yeastvision.track.lineage import LineageConstruction
 from yeastvision.track.cell import LABEL_PROPS, IM_PROPS, EXTRA_IM_PROPS, getCellData, exportCellData, getHeatMaps, getDaughterMatrix
 import cv2
 from yeastvision.disk.reader import loadPkl, ImageData, MaskData
 import importlib
 import yeastvision.parts.menu as menu
 from yeastvision.models.utils import MODEL_DIR
@@ -219,17 +219,16 @@
                 self.imChanged, self.maskChanged, self.tChanged = True, True, True
                 self._tIndex = num
         except AttributeError:
             self._tIndex = num
     
 
     def handleFinished(self, error = False):
-        if self.workers[-1].button:
-            self.activateButton(self.workers[-1].button)
         self.closeThread(self.threads[-1])
+        self.updateThreadDisplay()
     
     def setEmptyDisplay(self, initial = False):
         self.tIndex = 0
         self.bigTStep = 3
         self.maxT = 0
         self.tChanged = False
 
@@ -278,16 +277,19 @@
         self.prevMaskOn = True
         self.maskOn = True
         self.contourOn = False
         self.probOn = False
         self.maskZ = -1
         self.currMask = np.zeros((512,512), dtype = np.uint8)
         self.pg_mask.setImage(self.currMask, autolevels  =False, levels =[0,0], lut = self.maskColors)
+
+        
+
+
         self.cellData = [] 
-        self.lineageData = []
         self.mother_daughters = []
 
         if not initial:
             self.labelSelect.clear()
             self.maskTypeSelect.uncheckAll()
             self.contourButton.setChecked(False)
             self.cellNumButton.setChecked(False)
@@ -332,16 +334,14 @@
         if name:
             self.labelSelect.addItem(self.getNewLabelName(name))
         else:
             self.labelSelect.addItem("Label " + str(self.maskData.maxZ))
         
         self.maskTypeSelect.checkMaskRemote()
 
-        self.lineageData.append(None)
-        self.mother_daughters.append(None)
         self.cellData.append(None)
         self.newData()
     
     def handleDummyMasks(self, add = True):
         if add:
             self.maskData.addZ(self.maskData.channels[self.maskZ][0,:,:,:])
         self.maskData.removeDummys()
@@ -780,90 +780,91 @@
         self.drawMask()
     
     def trackObjButtonClick(self):
         labelsToTrack =  self.labelSelect.currentText()
         dlg  = GeneralParamDialog({}, [], f"Track {labelsToTrack}", self, labelSelects=["Cytoplasm Label"])
 
         if dlg.exec():
-            self.trackObjButton.setEnabled(False)
-            self.trackObjButton.setStyleSheet(self.stylePressed)
+            self.deactivateButton(self.trackObjButton)
             data = dlg.getData()
 
             cellIdx = self.labelSelect.findText(data["Cytoplasm Label"])
-            cells = self.maskData.channels[cellIdx][0, :, :,:]
+            cells = self.maskData.channels[cellIdx][0, :, :,:].copy()
+            obj = self.maskData.channels[self.maskZ][0, :, :,:].copy()
 
-            worker = Worker(self, lambda: self.trackObj(self.maskZ, cells), self.trackObjButton)
-            worker.finished.connect(self.handleFinished)
+            task = lambda: track_to_cell(obj, cells)
+            worker = TrackWorker(self, task, cellIdx)            
+            self.runLongTask(worker, worker.run, self.trackObjFinished, self.trackObjButton)
 
-            try:
-                self.beginThread(worker)
-            except MemoryError:
-                error_dialog  = QErrorMessage()
-                error_dialog.showMessage(f"Cannot Track Until Other Processes are Finished")
-                self.activateButton(self.trackObjButton)
-                return
         else:
             return
     
-    def trackObj(self, z, cells):
-        tracked = track_to_cell(self.maskData.channels[z][0, :, :,:], cells)
+    def trackObjFinished(self, tracked, z):
+        self.activateButton(self.trackObjButton)
         self.maskData.channels[z][0,:,:,:] = tracked
+        contours = self.getCurrContourSet()
+        newContours = tracked.copy()
+        newContours[np.logical_not(contours>0)] = 0
+        self.maskData.contours[z] = newContours
         self.updateCellData(idx = z)
-
+        self.handleFinished()
+        self.maskZ = z
+        self.drawMask()
+    
+    def trackFinished(self, z, tracked):
+        self.activateButton(self.trackButton)
+        self.handleFinished()
+
+        print(type(tracked))
+        if isinstance(tracked, np.ndarray):
+            self.maskData.channels[z][0,:,:,:] = tracked
+            contours = self.getCurrContourSet()
+            newContours = tracked.copy()
+            newContours[np.logical_not(contours>0)] = 0
+            self.maskData.contours[z] = newContours
+            self.updateCellData(idx = z)
+            self.maskZ = z
+            self.drawMask()
+        
 
     def trackButtonClick(self):
         self.deactivateButton(self.trackButton)
 
         idxToTrack = self.maskZ
-        worker  = Worker(self, trackYeasts, idxToTrack)
-        worker.finished.connect(self.handleFinished)
-        
-        try:
-            self.beginThread(worker)
-        except MemoryError:
-            error_dialog  = QErrorMessage()
-            error_dialog.showMessage(f"Cannot Track Until Other Processes are Finished")
-            self.activateButton(self.trackButton)
-            return
-        self.maskZ = idxToTrack
-        self.drawMask()
-    
-    def track(self,z):
-        currMasks = self.getCurrMaskSet()
-        newMasks = trackYeasts(currMasks)
-        self.maskData.channels[z][0,:,:,:] = newMasks
-        self.cellData[z] = None
-        self.updateCellData(idx = z)
+        cells = self.getCurrMaskSet().copy()
+        task = lambda: trackYeasts(cells)
+        worker = TrackWorker(self, task, idxToTrack)            
+        self.runLongTask(worker, worker.run, self.trackFinished, self.trackButton)
+
         
     def updateCellData(self, idx = None):
         if not self.maskLoaded:
             return
-        self.toStatusBar("Updating Cell Data...")
+  
         if idx:
             masks  = self.maskData.channels[idx][0,:,:,:]
         else:
             masks = self.getCurrMaskSet()
             idx = self.maskZ
+
     
         viableIms = []
         viableImNames = []
         for i, imChannel in enumerate(self.imData.channels):
             if imChannel[0].shape == masks[0].shape and imChannel.shape[0] >= masks.shape[0]:
                 viableIms.append(imChannel)
                 viableImNames.append(self.channelSelect.itemText(i))
-        #try:
-        cellData = getCellData(masks, viableIms, viableImNames)    
-        # except:
-        #     self.showError("Error Getting Cell Data: Ensure Labels Have Been Tracked")    
-        #     return      
-                                                             
-        self.cellData[idx] = cellData
+
+        if self.cellData[idx] is not None:
+            self.cellData[idx].update_cell_data(masks, channels = viableIms, channel_names = viableImNames)
+        else:
+            self.cellData[idx] = TimeSeriesData(idx, masks, channels = viableIms, channel_names=viableImNames)
+
         self.statusBar.clearMessage()
         self.saveData()
-
         self.checkDataAvailibility()  
 
         if self.pWindow:
             self.pWindow.setData()
             self.pWindow.updatePlots()
     
     def updateCellTable(self):
@@ -872,68 +873,65 @@
         # self.pWindow.table.model.setData(self.getCellDataAbbrev())
         # self.pWindow.
     
 
     def hasCellData(self, i = None):
         if type(i) is not int:
             i = self.maskZ
-        return (type(self.cellData[i]) is pd.core.frame.DataFrame)
+        return (isinstance(self.cellData[i], TimeSeriesData))
     
     def hasLineageData(self, i = None):
         if not i:
             i = self.maskZ
-        return ((type(self.lineageData[self.maskZ]) is pd.core.frame.DataFrame) 
-                and type(self.mother_daughters[self.maskZ]) is np.ndarray)
+        return isinstance(self.cellData[i], LineageData) and self.cellData[i].hasLineages()
     
     def getLabelsWithPopulationData(self):
-        return [population for i,population in enumerate(self.labelSelect.items()) if self.hasCellData(i = i)]
+        return [population for i,population in enumerate(self.cellData) if self.hasCellData(i = i)]
     
-
     def getCellData(self):
         if not self.maskLoaded or not self.hasCellData():
             return None
         else:
             return self.cellData
+    
+    def getTimeSeriesDataName(self, tsObj):
+        index = tsObj.i
+        return self.labelSelect.items()[index]
 
     def getCellDataAbbrev(self):
         if not self.maskLoaded:
             return pd.DataFrame.from_dict(self.cellDataFormat)
-        
         if not self.hasCellData():
-            if self.hasLineageData():
-                return self.lineageData[self.maskZ]
-            else:
-                return pd.DataFrame.from_dict(self.cellDataFormat)
-
+            return pd.DataFrame.from_dict(self.cellDataFormat)
         elif self.maskLoaded and self.hasCellData():
-            data = self.cellData[self.maskZ].copy()[0:-1]
-            columnsToKeep = ["labels", "birth", "death"]
-            for columnName in data.columns:
-                if columnName not in columnsToKeep:
-                    data = data.drop(columns = columnName)
-
-            if self.hasLineageData():
-                lD = self.lineageData[self.maskZ]
-                data["mother"], data["confidence"] = lD["mother"], lD["confidence"]
-            return data
-    
+            return self.cellData[self.maskZ].get_cell_info()
+        
     def getLineages(self):
         dlg = GeneralParamDialog({}, [], "Lineage Construction", self, labelSelects=["bud necks", "cells"])
         if dlg.exec_():
             data = dlg.getData()
             neckI = self.labelSelect.findText(data["bud necks"])
             cellI = self.labelSelect.findText(data["cells"])
             necks = self.maskData.channels[neckI][0,:,:,:]
             cells = self.maskData.channels[cellI][0,:,:,:]
         else:
             return 
-        lng = LineageConstruction(cells, necks, backskip=0, forwardskip=5)
-        daughters, motherDF = lng.computeLineages()
-        self.mother_daughters[cellI] = daughters
-        self.lineageData[cellI] = motherDF
+        
+        
+        if isinstance(self.cellData[cellI], LineageData):
+            self.cellData[cellI].add_lineages(cells, necks)
+        else:
+            if isinstance(self.cellData[cellI], TimeSeriesData):
+                life = self.cellData[cellI].life_data
+                cell_data = self.cellData[cellI].cell_data
+            else:
+                life, cell_data = None, None
+
+            self.cellData[cellI] = LineageData(cellI, cells, necks, cell_data=cell_data, life_data=life)
+
         self.saveData()
         self.checkDataAvailibility()
     
     def getCellDataLabelProps(self):
         label_props = LABEL_PROPS.copy()
         label_props.remove("label")
         return sorted(label_props)
@@ -956,26 +954,14 @@
 
     def showError(self, message = ""):
         self.errorDialog = QtWidgets.QErrorMessage()
         self.errorDialog.setSizePolicy(QSizePolicy.Expanding,QSizePolicy.Expanding)
         self.errorDialog.setFixedWidth(500)
         self.errorDialog.showMessage(message)
 
-    def beginThread(self, worker):
-        if len(self.threads)+1>self.idealThreadCount:
-            self.showError("Too Many Threads Running At This Time")
-            return
-        thread = QtCore.QThread(self) 
-        self.threads.append(thread)
-        self.workers.append(worker)
-        self.workers[-1].thread = thread
-        self.workers[-1].moveToThread(thread)
-        thread.started.connect(self.workers[-1].run)
-        self.threads[-1].start()
-        self.updateThreadDisplay()
 
     def closeThread(self, thread):
         index = self.threads.index(thread)
         thread = self.threads[index]
         thread.quit()
         thread.wait()
         del self.threads[index]
@@ -1008,45 +994,35 @@
         vals, xtemp, ytemp = self.getCellCenters(self.currMask)
         image = self.pg_mask.image
         for i in range(0,len(xtemp)):
             image = cv2.putText(image, str(vals[i]), (xtemp[i], ytemp[i]), cv2.FONT_HERSHEY_SIMPLEX, 0.30, (255,255,255,255), 1)
         self.pg_mask.image = image
         self.pg_mask.updateImage()
     
-
-    
-    def parseProperties(self):
-            if not self.toPlot:
-                return {}
-            else:
-                toPlotDict = {}
-                for plot in self.plotTypes:
-                    toPlotDict[plot] = ["-".join((prop.split("-")[1:])) for prop in self.toPlot if plot in prop.split("-")[0]]
-                return toPlotDict
         
         
     def buildPlotWindow(self):
         win = PlotWindowCustomize(self)
 
         if win.exec_():
             self.toPlot = win.getData()
         else:
             self.plotButton.setCheckState(False)
             return
         
-        self.pWindow = plot.PlotWindow(self, self.parseProperties())
+        self.pWindow = plot.PlotWindow(self, self.toPlot)
         self.pWindow.show()
     
         
     def togglePlotWindow(self):
         self.plotWindowOn = self.plotButton.isChecked()
 
         if self.plotWindowOn:
             self.buildPlotWindow()   
-        else:
+        elif self.pWindow is not None:
             self.pWindow.close()
             self.pWindow = None
 
     def brushSizeChoose(self):
         self.brush_size = self.brushSelect.value()
         self.pg_mask.setDrawKernel(kernel_size=self.brush_size)
     
@@ -1357,22 +1333,24 @@
         self.contourOn = False
         self.drawMask()
 
         contour = self.getCurrContours().copy()
         self.addSpecificContours(contour, [mother, daughter], [[255,0,0,255], [0,255,0,255]])
     
     def getDaughters(self, cellNum):
-        potentialDaughters = self.mother_daughters[self.maskZ][cellNum-1]
+        potentialDaughters = self.cellData[self.maskZ].daughters[cellNum-1]
         daughters = list(np.where(potentialDaughters)[0]+1)
         return daughters
         
     def drawContours(self):
         contour = self.getCurrContours().copy()
         color = np.array(self.goldColor)
         if self.selectedCells:
+            print(self.selectedCells)
+            print(self.selectedCellContourColors)
             for i, cell in enumerate(self.selectedCells):
                 color = self.selectedCellContourColors[i]
                 self.addSpecificContours(contour, [cell], [color])
         else:
             self.pg_mask.addMask(contour, color)
     
     def addSpecificContours(self, contour, nums, colors):
@@ -1407,14 +1385,17 @@
         else:
             return np.zeros_like(self.currMask)
 
     def getCurrContours(self):
         maskData = self.maskData.contours
         return maskData[self.maskZ][self.tIndex,:,:]
 
+    def getCurrContourSet(self):
+        return self.maskData.contours[self.maskZ]
+
     def getCurrFrames(self):
         return (self.getCurrIm(), self.getCurrMask())
     
     def bootUp(self):
         self.pg_im.setImage(self.currIm, autoLevels=False, levels = [0,0])
         self.pg_mask.setImage(self.currMask, autolevels  =False, levels =[0,0], lut = self.maskColors)
 
@@ -1467,38 +1448,44 @@
             self.deselectAllCells()
             for num in self.getDaughters(cellNum)+[cellNum]:
                 print(num)
                 self.selectedCells.append(num)
                 self.selectedCellContourColors.append([255,0,0,255])
                 self.maskColors[num,:] = np.array(self.goldColor, dtype = np.uint8)
 
+        elif self.showMotherDaughters and self.hasLineageData:
+            self.deselectAllCells()
+            self.selectedCells.append(cellNum)
+            self.selectedCellContourColors.append([255,0,0,255])
+            self.maskColors[cellNum,:] = np.array(self.goldColor, dtype = np.uint8)
+            motherNum = self.getMotherFromLineageData(cellNum)
+            if motherNum:
+                print("selecting mother", motherNum, "for cell", cellNum)
+                if motherNum not in self.selectedCells:
+                    self.selectedCells.append(motherNum)
+                    self.selectedCellContourColors.append([0,255,0,255])
+                    self.maskColors[motherNum,:] = np.array(self.goldColor, dtype = np.uint8)
+                else:
+                    motherIdx = self.selectedCells.index(motherNum)
+                    self.selectedCellContourColors[motherIdx] = [0,255,0,255]
+        
         elif cellNum in self.selectedCells:
             self.deselectCell(cellNum)
+    
         else:
             self.selectedCells.append(cellNum)
             self.selectedCellContourColors.append([255,0,0,255])
             self.maskColors[cellNum,:] = np.array(self.goldColor, dtype = np.uint8)
-
-            if self.showMotherDaughters and self.hasLineageData:
-                motherNum = self.getMotherFromLineageData(cellNum)
-                if motherNum:
-                    print("selecting mother", motherNum, "for cell", cellNum)
-                    if motherNum not in self.selectedCells:
-                        self.selectedCells.append(motherNum)
-                        self.selectedCellContourColors.append([0,255,0,255])
-                        self.maskColors[motherNum,:] = np.array(self.goldColor, dtype = np.uint8)
-                    else:
-                        motherIdx = self.selectedCells.index(motherNum)
-                        self.selectedCellContourColors[motherIdx] = [0,255,0,255]
+        self.drawIm()
         self.drawMask() 
-        if self.pWindow and self.pWindow.hasPlots and self.labelSelect.currentText() in self.pWindow.singleCellPopulations:
+        if self.pWindow and self.pWindow.hasSingleCellPlots():
             self.pWindow.updateSingleCellPlots()
     
     def getMotherFromLineageData(self,cell):
-        ld = self.lineageData[self.maskZ]
+        ld = self.cellData[self.maskZ].mothers
         mother = ld["mother"].iloc[cell-1]
         if pd.notna(mother):
             return (int(mother))
         else:
             return None
 
     def deselectCell(self, num):
@@ -1704,27 +1691,35 @@
         imName = params["Channel"]
 
         if modelType == "artilife":
             counter = 0
             for labelName, outputTup in output.items():
                 if type(outputTup[0]) == np.ndarray:
                     counter += 1
-                    ims, prob = outputTup
+                    templates = []
                     for i in [0,1]:
-                        outputTup[i][tStart:tStop+1]
+                        template = np.zeros_like(ims, dtype = outputTup[i].dtype)
+                        template[tStart:tStop+1] = outputTup[i]
+                        templates.append(template)
+                    outputTup = (templates[0], templates[1])
                     self.loadMasks(outputTup, name = f"{imName}_{labelName}")
             if params["Time Series"]:
                 idx = self.maskZ - counter
                 self.updateCellData(idx = idx)
         else:
+            templates = []
             for i in [0,1]:
-                output[i][tStart:tStop+1]
-            self.loadMasks(output, name = f"{imName}_{modelType}")
+                template = np.zeros_like(ims, dtype = output[i].dtype)
+                template[tStart:tStop+1] = output[i]
+                templates.append(template)
+            outputTup = (templates[0], templates[1])
+            self.loadMasks(outputTup, name = f"{imName}_{modelType}_{tStart}-{tStop}")
         
         self.activateButton(self.modelButton)
+        self.handleFinished()
         
     def evaluate(self):
         if not self.maskLoaded:
             return
         params = {label: False for label in self.labelSelect.items()}
         paramtypes = [bool] * len(params)
         labelSelects = ["validation"]
@@ -1779,14 +1774,30 @@
         if not allNames:
             return potentialName
         n = (np.char.find(np.array(allNames), potentialName)+1).sum()
         if n>0:
             return f"{potentialName}-n"
         else:
             return potentialName
+    
+    def runLongTask(self, worker, task, finished, button):
+        if len(self.threads)+1>self.idealThreadCount:
+            self.showError("Too Many Threads Running At This Time")
+            self.activateButton(button)
+            return
+        
+        thread = QThread()
+        self.threads.append(thread)
+        thread.started.connect(task)
+        self.workers.append(worker)
+        worker.moveToThread(thread)
+        worker.finished.connect(finished)
+        thread.start()
+        self.updateThreadDisplay()
+
 
     def computeModels(self):
         weightName = self.modelChoose.currentText() 
         if weightName == '':
             return
         modelType = self.modelTypes[self.modelNames.index(weightName)]
         weightPath = join(MODEL_DIR, modelType, weightName)
@@ -1802,17 +1813,18 @@
         if dlg.exec():
             params = dlg.getData()
             channel = params["Channel"]
             channelIndex = self.channelSelect.findText(channel)
             ims = self.imData.channels[channelIndex]
 
             worker = SegmentWorker(self)
-            self.workers.append(worker)
-            worker.finished.connect(self.segment)
-            worker.run(modelClass,ims, params, weightPath, modelType)
+            self.runLongTask(worker, 
+                             lambda: worker.run(modelClass,ims, params, weightPath, modelType),
+                             self.segment,
+                             self.modelButton)
         else:
             self.activateButton(self.modelButton)
             return
 
     def doAdaptHist(self):
         files = self.imData.files[self.imZ]
         currName = self.channelSelect.currentText()
@@ -1962,16 +1974,16 @@
     def saveLineageData(self):
         if not self.maskLoaded:
             self.showError("No Label Data Loaded")
             return
         
         labelName = self.labelSelect.items()[self.maskZ]
         labelFileName = labelName.replace(" ", "")
-        motherdata, daughterdata = self.lineageData[self.maskZ], self.mother_daughters[self.maskZ]
         if self.hasLineageData():
+            motherdata, daughterdata = self.cellData[self.maskZ].mothers, self.cellData[self.maskZ].daughters
             fname1= join(self.imData.dirs[self.imZ], labelFileName + "_mother_daughters.csv")
             fname2 = join(self.imData.dirs[self.imZ], labelFileName + "_daughter_array.csv.csv")
             path, _ = QFileDialog.getSaveFileName(self, 
                             "save data as csv", 
                             fname1)
             if path:
                 np.savetxt(fname2, daughterdata, delimiter=",")
@@ -1982,15 +1994,15 @@
     def saveHeatMaps(self):
         if not self.maskLoaded:
             self.showError("No Label Data Loaded")
             return
         
         labelName = self.labelSelect.items()[self.maskZ]
         labelFileName = labelName.replace(" ", "")
-        if type(self.cellData[self.maskZ]) is pd.core.frame.DataFrame:
+        if self.hasCellData():
             data = getHeatMaps(self.cellData[self.maskZ])
             defaultFileName = join(self.imData.dirs[self.imZ], labelFileName + "_heatmaps.tif")
             path, _ = QFileDialog.getSaveFileName(self, 
                             "save heatmaps as stack tif", 
                             defaultFileName)
             imsave(path, data) 
         else:
@@ -2067,22 +2079,20 @@
                         "Files": self.imData.files}
             maskdata = {"Masks": self.maskData.channels,
                         "Contours":self.maskData.contours}
             if self.maskData.isDummy:
                 maskdata["Masks"] = ["Blank"]
             otherdata = {"Channels": self.channelSelect.items(),
                         "Labels": self.labelSelect.items()}
-            celldata = {"Cells": self.cellData,
-                        "Lineages": self.lineageData,
-                        "Daughters": self.mother_daughters}
+            celldata = {"Cells": self.cellData}
             i = 0
             for item in self.cellData:
-                if type(item) is pd.core.frame.DataFrame or type(item) is np.ndarray:
+                if isinstance(item, TimeSeriesData):
                     i+=1
-            print("Saving ", i, "valid dataframes")
+            print("Saving ", i, "valid cell data objects")
             data =  imdata | maskdata | otherdata | celldata
 
             try:
                 with open(path, "wb") as f:
                     pickle.dump(data, f)
             except:
                 print("ERROR: cannot sive archive to", path)
```

### Comparing `yeastvision-0.1.5/yeastvision/disk/io.py` & `yeastvision-0.1.6/yeastvision/disk/io.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/disk/reader.py` & `yeastvision-0.1.6/yeastvision/disk/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,25 @@
     dirs, files = data["Dirs"], data["Files"]
     for i in range(len(ims)):
         parent.imData.dirs.append(dirs[i])
         parent.imData.files.append(files[i])
         parent.loadImages(ims[i], name = names[i])
 
     masks, contours,labels = data["Masks"], data["Contours"], data["Labels"]
-    cellData, lineageData, daughterData = data['Cells'], data["Lineages"], data["Daughters"]
+    cellData = data['Cells']
     for i in range(len(masks)):
         maskStack = masks[i]
         hasFloats = maskStack.shape[0]>1
         if hasFloats:
             currMask = (maskStack[0,:,:,:], maskStack[1,:,:,:])
         else:
             currMask = maskStack[0,:,:,:]
         parent.loadMasks(currMask, name = labels[i], contours = contours[i])
 
         parent.cellData[-1] = (cellData[i])
-        parent.lineageData[-1] = (lineageData[i])
-        parent.mother_daughters[-1] = daughterData[i]
     parent.checkDataAvailibility()
     parent.saveData()
 
 class ImageData():
     fileEndings = ['.tif','.tiff',
                             '.jpg','.jpeg','.png','.bmp',
                             '.pbm','.pgm','.ppm','.pxm','.pnm','.jp2',
```

### Comparing `yeastvision-0.1.5/yeastvision/flou/blob_detect.py` & `yeastvision-0.1.6/yeastvision/flou/blob_detect.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/flou/utils.py` & `yeastvision-0.1.6/yeastvision/flou/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/ims.py` & `yeastvision-0.1.6/yeastvision/ims.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/install_weights.py` & `yeastvision-0.1.6/yeastvision/install_weights.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/YeaZ/model.py` & `yeastvision-0.1.6/yeastvision/models/YeaZ/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/YeaZ/segment.py` & `yeastvision-0.1.6/yeastvision/models/YeaZ/segment.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/YeaZ/unet.py` & `yeastvision-0.1.6/yeastvision/models/YeaZ/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/artilife/budSeg/model.py` & `yeastvision-0.1.6/yeastvision/models/artilife/budSeg/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/artilife/model.py` & `yeastvision-0.1.6/yeastvision/models/artilife/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from yeastvision.models.cp import CustomCPWrapper
 from skimage.measure import label
 from yeastvision.models.utils import addMasks
 from yeastvision.models.artilife.budSeg.model import BudSeg
 from skimage.measure import label
 from skimage.morphology import remove_small_objects
 from yeastvision.track.track import trackYeasts
+from yeastvision.track.mat import get_mating_data
 from yeastvision.track.cell import Cell, getBirthFrame, getCellData, getDeathFrame, getLifeData
 from yeastvision.models.utils import normalizeIm, produce_weight_path
 
 class Artilife(CustomCPWrapper):
     hyperparams  = { 
     "Mean Diameter":30, 
     "Flow Threshold":0.4, 
@@ -85,16 +86,16 @@
                                                                 cellprob_threshold = self.params["Flow Threshold"],
                                                                 do_3D = False)
         print("got mating cells")
         self.matprobs = [flow[2] for flow in matFlows]
         self.matprobs = np.array(self.processProbability(self.matprobs), dtype = np.uint8)
         
         if self.params["Time Series"]:
-            newMatMasks, newMasks = track_obj([im[:,:,0] for im in ims[matSlice]], self.masks[matSlice], self.matMasks[matSlice], True)
             matSlice = slice(int(self.params["matStart"]), int(self.params["matStop"])-1)
+            newMatMasks, newMasks = get_mating_data(self.matMasks[matSlice], self.masks[matSlice])
         else:
             newMasks = []
             for matMask, cellMask in zip(self.matMasks, self.masks):
                 if np.any(matMask>=1):
                     newMask = addMasks(matMask, cellMask)
                     newMasks.append(newMask)
                 else:
@@ -135,15 +136,15 @@
             return np.zeros_like(mask)
 
     def addSmallCells(self, ims, cellData):      
         newMasks = self.masks.copy()
         imsPadded = np.array([np.pad(im, 25, mode = "symmetric") for im in ims], dtype = np.uint16)
         masksPadded = np.array([np.pad(mask, 25) for mask in newMasks], dtype = np.uint16)
         
-        for val in cellData.index:
+        for val in range(len(cellData["birth"])):
             cellVal = int(val)+1
             if cellVal>0:
                 birthFrame = cellData["birth"][cellVal-1]
                 
                 if birthFrame > 0:
                     cell = Cell(masksPadded[birthFrame,:,:], cellVal)
                     r,c = cell.centroid
@@ -186,14 +187,15 @@
         print("formatting return")
         model.masks = np.array(model.masks, dtype = np.uint16)
 
         if model.params["Time Series"]:
             model.masks = trackYeasts(model.masks)
             cellData = getLifeData(model.masks)
             model.addSmallCells(ims, cellData)
+            model.masks = trackYeasts(model.masks)
 
         if model.matSeg:
             print('add mating cell')
             model.addMatingCells(ims3D)
         if model.tetradSeg:
             model.addTetrads(ims3D)
```

### Comparing `yeastvision-0.1.5/yeastvision/models/budNET/model.py` & `yeastvision-0.1.6/yeastvision/models/budNET/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/cp.py` & `yeastvision-0.1.6/yeastvision/models/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     def __init__(self, params, weights):
         super().__init__(params, weights)
         if self.params["Mean Diameter"] == 0:
             self.params["Mean Diameter"] = None
         
         self.model = CustomCellpose(pretrained_model=self.weights)
         self.cpAlone = self.model.cp
+        
     
     def processProbability(self, rawProb):
         return (np.clip(normalize99(rawProb.copy()), 0, 1) * 255).astype(np.uint8)
 
     
     def train(self, ims, labels, params):
         # ims must be 3D for cellpose
@@ -84,11 +85,11 @@
         assert len(ims[0].shape)==3
 
         model.masks, flows, _, model.diams = model.model.eval(ims, 
                                                 diameter = model.params["Mean Diameter"], 
                                                 channels = [0, 0],
                                                 cellprob_threshold = model.params["Flow Threshold"], 
                                                 do_3D=False)
-        probs = model.processProbability(flows)
-        model.cellprobs = [flow[2] for flow in probs]
+        model.cellprobs = [flow[2] for flow in flows]
+        model.cellprobs = np.array((model.processProbability(model.cellprobs)), dtype = np.uint8)
 
         return np.array(model.masks, dtype = np.uint16), np.array(model.cellprobs, dtype = np.float32)
```

### Comparing `yeastvision-0.1.5/yeastvision/models/model.py` & `yeastvision-0.1.6/yeastvision/models/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/unet.py` & `yeastvision-0.1.6/yeastvision/models/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/models/utils.py` & `yeastvision-0.1.6/yeastvision/models/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/parts/canvas.py` & `yeastvision-0.1.6/yeastvision/parts/canvas.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/parts/dialogs.py` & `yeastvision-0.1.6/yeastvision/parts/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
                             QWidget, QComboBox, QGridLayout, QHBoxLayout, QSizePolicy, QHeaderView, QVBoxLayout,
                             QScrollArea, QTreeWidget)
 from PyQt5.QtCore import Qt
 import numpy as np
 import os
 import datetime
 from yeastvision.parts.guiparts import *
+from yeastvision.plot.plot import PlotProperty
 
 class DirReaderDialog(QDialog):
     def __init__(self, dir, fnames):
         super().__init__()
 
         QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
         self.buttonBox = QDialogButtonBox(QBtn)
@@ -669,89 +670,104 @@
 
 
 
 class PlotWindowCustomize(QDialog):
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
-        self.setGeometry(100,100,850,400)
+        self.setGeometry(100,100,1000,450)
         self.setWindowTitle("Customize Plot Display")
         self.win = QWidget(self)
         self.l = QGridLayout()
         self.win.setLayout(self.l)
 
         self.morphProps = self.parent.getCellDataLabelProps()
         self.trees = []
         self.boxes = {}
-        #self.produceParamTreeSingleCell()
+        self.produceParamTreeSingleCell()
         self.produceParamTreeIncludePopulations()
 
         QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
 
         self.l.addWidget(self.buttonBox, 3, 0, 1, 2)
 
         self.win.show()
     
-    def getProps(self, populationName, propType):
+    def getProps(self, populationObj, propType):
         if propType == "morphology":
             return self.morphProps
         else:
-            i = self.parent.labelSelect.items().index(populationName)
-            return self.parent.getCellDataImProperties(i = i)
+            return [prop for prop in populationObj.properties if prop not in self.morphProps]
+
+    def produceParamTreeSingleCell(self):
+        populations = self.parent.getLabelsWithPopulationData()      
+        tree = self.produceTree()
+        self.trees.append(tree)
+        level1 = "single"
+        item = QTreeWidgetItem(tree, [level1])
+        item.setExpanded(True)
+
+        for level2 in populations:
+            setName = self.parent.getTimeSeriesDataName(level2)
+            item2 = QTreeWidgetItem(item, [setName])
+            item2.setExpanded(True)
+
+            for level3 in ["morphology", "pixel"]:
+                item3 = QTreeWidgetItem(item2, [level3])
+
+                for level4 in self.getProps(level2, level3):
+                    item4 = QTreeWidgetItem(item3, [level4])
+                    box = QCheckBox()
+                    tree.setItemWidget(item4, 1, box)
+                    self.boxes[PlotProperty(self.parent, "single", setName, level4)] = box
+        self.l.addWidget(tree, 0,0,2,1)
 
     def produceParamTreeIncludePopulations(self):
         populations = self.parent.getLabelsWithPopulationData()      
-        for i,level1 in enumerate(self.parent.plotTypes):
+        for i,level1 in enumerate(self.parent.populationPlotTypes):
             tree = self.produceTree()
             self.trees.append(tree)
             item = QTreeWidgetItem(tree, [level1])
             item.setExpanded(True)
 
             for level2 in populations:
-                item2 = QTreeWidgetItem(item, [level2])
+                setName = self.parent.getTimeSeriesDataName(level2)
+                item2 = QTreeWidgetItem(item, [setName])
                 item2.setExpanded(True)
 
-                for level3 in ["morphology", "pixel"]:
-                    item3 = QTreeWidgetItem(item2, [level3])
+                for level2a in level2.population_names:
+                    item2a = QTreeWidgetItem(item2, [level2a])
 
-                    for level4 in self.getProps(level2, level3):
-                        item4 = QTreeWidgetItem(item3, [level4])
-                        box = QCheckBox()
-                        tree.setItemWidget(item4, 1, box)
-                        self.boxes[f"{level1}-{level2}-{level4}"] = box
-            self.l.addWidget(tree, 0,i,2,1)
-    
-    def produceParamTreeSingleCell(self):
-        tree = self.produceTree()
-        self.trees.append(tree)
+                    for level3 in ["morphology", "pixel"]:
+                        item3 = QTreeWidgetItem(item2a, [level3])
 
-        item = QTreeWidgetItem(tree, ["single"])
+                        for level4 in self.getProps(level2, level3):
+                            item4 = QTreeWidgetItem(item3, [level4])
+                            box = QCheckBox()
+                            tree.setItemWidget(item4, 1, box)
+                            self.boxes[PlotProperty(self.parent, level1, setName, level4, populationName=level2a)] = box
+            self.l.addWidget(tree, 0,i+1,2,1)
 
-        for level2 in ["morphology", "pixel"]:
-            item2 = QTreeWidgetItem(item, [level2])
-
-            for level3 in self.props[level2]:
-                item3 = QTreeWidgetItem(item2, [level3])
-                box = QCheckBox()
-                tree.setItemWidget(item3, 1, box)
-                self.boxes[f"single-{level3}"] = box
-        tree.expandAll()
-        self.l.addWidget(tree,0,0,2,1)
-    
     def getData(self):
-        return [name for name, box in self.boxes.items() if box.isChecked()]
+        checked = [name for name, box in self.boxes.items() if box.isChecked()]
+        toPlotDict = {}
+        for plot in self.parent.plotTypes:
+            toPlotDict[plot] = [prop_obj for prop_obj in checked if plot in prop_obj.plotType]
+        return toPlotDict
+
     
     def produceTree(self):
         tree = QTreeWidget()
         tree.setColumnCount(2)
         tree.setHeaderHidden(True)
         tree.setMinimumHeight(300)
+        tree.setMinimumWidth(300)
         tree.header().setSectionResizeMode(QHeaderView.ResizeToContents)
         return tree
```

### Comparing `yeastvision-0.1.5/yeastvision/parts/guiparts.py` & `yeastvision-0.1.6/yeastvision/parts/guiparts.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/parts/menu.py` & `yeastvision-0.1.6/yeastvision/parts/menu.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/parts/workers.py` & `yeastvision-0.1.6/yeastvision/parts/workers.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,29 +45,29 @@
     def __init__(self, parent):
         super(SegmentWorker,self).__init__()
         self.parent = parent
     
     def run(self, modelClass,ims, params, weightPath, modelType):
         row, col = ims[0].shape
         newImTemplate = np.zeros((len(ims), row, col))
-        outputTup  = (newImTemplate, newImTemplate.copy())
         tStart, tStop = int(params["T Start"]), int(params["T Stop"])
 
         output = modelClass.run(ims[tStart:tStop+1],params, weightPath)
-        self.finished.emit(output, modelClass,ims, params, weightPath, modelType)
+        self.finished.emit(output, modelClass,newImTemplate, params, weightPath, modelType)
 
 class TrackWorker(QtCore.QObject):
     finished = QtCore.pyqtSignal(object, object)
 
     def __init__(self, parent, func, z):
+        super(TrackWorker,self).__init__()
         self.parent = parent
         self.trackfunc = func
-        self.z
+        self.z = z
     
-    def run(self, labels):
-        self.finished.emit(self.func(labels))
+    def run(self):
+        self.finished.emit(self.z, self.trackfunc())
 
 # class ImageWorker(QtCore.QObject):
 
 #     finished = QtCore.pyqtSignal(object, object)
 
 #     def __init__(self, parent, func, z):
```

### Comparing `yeastvision-0.1.5/yeastvision/plot/cell_table.py` & `yeastvision-0.1.6/yeastvision/plot/cell_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,20 +68,27 @@
         result = groups.filter(lambda x: len(x) > 1)
         idxs = result.index.tolist()
         self.turnRed = list(zip(idxs, [self.columns["mother"]]*len(idxs)))
     
     def handleselect(self, new, previous):
         if previous.column() == -1:
             return
-        if (new.column() == self.columns["cell"] or new.column() == self.columns["mother"]) and self.hasLineages:
-            value = int(self._data.iloc[new.row(), new.column()])
-            mother = self._data.iloc[value-1, self.columns["mother"]]
+        
+
+
+        if (new.column() == self.columns["cell"] or new.column() == self.columns["mother"]):
+            value = self._data.iloc[new.row(), new.column()]
+            if value == np.NaN:
+                return
             birth = int(self._data.iloc[value-1, self.columns["birth"]])
-            self.main.showMotherDaughter(mother, value, birth)
+            self.main.tIndex = birth
+            self.main.selectCellFromNum(value)
+
         
         if (new.column() in [self.columns["birth"], self.columns["death"]]):
-            self.parent.tIndex = int(self._data.iloc[new.row(), new.column()])
-            self.parent.drawMask()
+            self.main.tIndex = int(self._data.iloc[new.row(), new.column()])
+            self.main.drawIm()
+            self.main.drawMask()
```

### Comparing `yeastvision-0.1.5/yeastvision/plot/plot.py` & `yeastvision-0.1.6/yeastvision/plot/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,70 @@
 from PyQt5.QtWidgets import (QApplication, QRadioButton, QButtonGroup, QSlider, QStyle, QStyleOptionSlider, QMainWindow, QPushButton, QDialog,
                             QDialogButtonBox, QLineEdit, QFormLayout, QMessageBox,
                              QFileDialog, QVBoxLayout, QCheckBox, QFrame, QSpinBox, QLabel, QWidget, QComboBox, QTableWidget, QSizePolicy, QGridLayout, QHBoxLayout)
 import pyqtgraph as pg
 from pyqtgraph.dockarea.Dock import Dock
 from pyqtgraph.dockarea.DockArea import DockArea
 from yeastvision.plot.cell_table import TableModel
+from yeastvision.plot.types import SingleCellUpdatePlot, HeatMap, PopulationPlot
+from yeastvision.track.data import PopulationReplicate, Population
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
-class CustomizePlot(QWidget):
-    def __init__(self):
-        pass
+
+class PlotProperty():
+    def __init__(self, parent, plotType, setName, property, populationName = None):
+        self.parent = parent
+        self.plotType = plotType
+        self.labelIdx = self.getLabelIdx(setName)
+        self.prop = property
+        self.population = populationName
+    
+    def getPlotName(self):
+        labelName = self.getLabelName()
+        if self.populationName:
+            return "f{labelName}-{self.population}-{self.prop}"
+        else:
+            return "f{labelName}-{self.prop}"
+    
+    def getLabelIdx(self, setName):
+        return self.parent.labelSelect.items().index(setName)
+    
+    def getLabelName(self):
+        return self.labelSelect.items()[self.labelIdx]
+    
+    def get_timeseries_obj(self):
+        return self.parent.cellData[self.labelIdx]
+    
+    @staticmethod
+    def cluster_property(plot_property_list):
+        by_property = {}
+        for plot_property_obj in plot_property_list:
+            prop = plot_property_obj.prop
+            if prop not in by_property:
+                by_property[prop] = [plot_property_obj]
+            else:
+                by_property[prop].append(plot_property_obj)
+        return by_property
+
+    @staticmethod
+    def cluster_population(plot_property_list):
+        by_population = {}
+        for plot_property_obj in plot_property_list:
+            pop = plot_property_obj.population
+            if pop not in by_population:
+                by_population[pop] = [plot_property_obj]
+            else:
+                by_population[pop].append(plot_property_obj)
+        return by_population
+
+    
 
 class EvalWindow(QWidget):
     def __init__(self, parent, data_dict, IOUs):
         '''
         params
         data_dict - key: name of the plot (precision, recall, F1, accuracy), values - list of tuple for each set of labels being 
         evaluated where tup1 is the name and tup2 is data vs IOU score
@@ -97,176 +144,180 @@
     def __init__(self, parent, propDict):
         super().__init__()
         self.parent = parent
         pg.setConfigOption('imageAxisOrder', 'row-major')
         self.hLayout = QHBoxLayout()
         self.setLayout(self.hLayout)
         self.createTable()
-        self.propDict = propDict
         pg.setConfigOption('imageAxisOrder', 'row-major')
         self.cmap = pg.colormap.get("jet", source = 'matplotlib')
-
-        # print(propDict)
-        # print(propDict["single"])
-        self.singleCellPopulations = self.getSingleCellPopulations(propDict["single"]) if "single" in propDict else []
-        print(self.singleCellPopulations)
         self.setData()
+        
+        self.propDict = propDict
 
-        self.hasPlots = bool(propDict)
 
-        self.propDict = propDict
-        if self.propDict:
+        if self.hasPlots():
             self.area = DockArea()
             self.hLayout.addWidget(self.area, 7)
             self.docks = {} # key = name of dock, value = (dock object, widget contained in dock)
-            
-            for plotType, props in self.propDict.items():
-                if props:
-
-                    # dock
-                    dockName = f"{plotType} plots"
-                    newDock = Dock(dockName, closable = True)
-                    dockLayout = DockArea()
-                    newDock.addWidget(dockLayout)
-                    self.docks[plotType] = (newDock, dockLayout)
-                    self.area.addDock(newDock, "bottom")
-
-                    for i, prop in enumerate(props):
-                        if i == 0:
-                            position = "bottom"
-                            relativeTo = None
-                        else:
-                            position = "above"
-                            plotRelativeTo = props[i-1]
-                            relativeTo = self.docks[f"{plotType} {plotRelativeTo}"][0]
-
-                        if "heatmap" in plotType:
-                            name = f'{prop}'
-                            imDock = Dock(name, closable = True)
-                            imData = self.getHeatMap(prop)
-                            view  = pg.PlotWidget(title = name)
-                            im = pg.ImageItem(colorMap = self.cmap)
-                            im.setImage(imData, autoLevels = True)
-                            view.addItem(im)
-                            imDock.addWidget(view)
-                            self.docks[f"{plotType} {prop}"] = (imDock,im)
-                            dockLayout.addDock(imDock, position, relativeTo)
-                        else:
-                            name = f"{prop}"
-                            plotDock = Dock(name, closable = True)
-                            newPlot = pg.PlotWidget(title=name)
-                            
-                            data = self.getData(plotType, prop)
-                            if type(data) is dict:
-                                newPlot.addLegend()
-                                i = 0
-                                for cellnum, dataset in data.items():
-                                    color = parent.cmaps[0][i][0:-1]
-                                    newPlot.plot(dataset, name = str(cellnum), pen = tuple(color))
-                                    i+=1
-                            else:
-                                newPlot.plot(data)
-
-                            self.docks[f"{plotType} {prop}"] = (plotDock,newPlot)
-
-                            plotDock.addWidget(newPlot)    
-                            dockLayout.addDock(plotDock, position, relativeTo)
-        if self.hasPlots:
+            if self.hasSingleCellPlots():
+                self.addSingleCellPlots()
+            if self.hasHeatmaps():
+                self.addHeatmaps()
+            if self.hasPopulationPlots():
+                self.addPopulationsPlots()
             self.setGeometry(500, 100, 1500, 1500)
     
-    def getSingleCellPopulations(self, singleCelProps):
-        return [prop.split("-")[0] for prop in singleCelProps]
+    def hasPlots(self):
+        return self.hasSingleCellPlots() or self.hasHeatmaps() or self.hasPopulationPlots()
+
+    def hasSingleCellPlots(self):
+        return "single" in self.propDict and self.propDict["single"]
+    
+    def hasMplPlots(self):
+        return self.hasPopulationPlots()
+    
+    def hasHeatmaps(self):
+        return "heatmap" in self.propDict and self.propDict["heatmap"]
+    
+    def hasPopulationPlots(self):
+        return "population" in self.propDict and self.propDict["population"]
+
+    def updateAll(self):
+        if self.hasSingleCellPlots():
+            self.updateSingleCellPlots()
+        if self.hasHeatmaps():
+            self.updateHeatMaps()
+        if self.hasPopulationPlots():
+            self.updatePopulationPlots
+
+    
+    def addSingleCellPlots(self):
+        self.singleCellPlots = []
+        single_cell_prop_obj = self.propDict["single"]
+        clustered_by_property = PlotProperty.cluster_property(single_cell_prop_obj)
+        for property in clustered_by_property:
+            timeseries = [prop.get_timeseries_obj() for prop in clustered_by_property[property]]
+            self.singleCellPlots.append(SingleCellUpdatePlot(self.parent, property, timeseries, self.parent.selectedCells))
+        
+ 
+        dockName = f"single plots"
+        newDock = Dock(dockName, closable = True)
+        dockLayout = DockArea()
+        newDock.addWidget(dockLayout)
+        self.area.addDock(newDock, "bottom")
+        
+
+        for i, plot in enumerate(self.singleCellPlots):
+            if i == 0:
+                position = "bottom"
+                relativeTo = None
+            else:
+                position = "above"
+                plotRelativeTo = self.singleCellPlots[i-1]
+                relativeTo = self.docks[plotRelativeTo]
+
+            name = f"{plot.property}"
+            plotDock = Dock(name, closable = True)
+            plotDock.addWidget(plot.getPlotWidget())
+            self.docks[plot] = (plotDock)
+  
+            dockLayout.addDock(plotDock, position, relativeTo)
+    
+    def addHeatmaps(self):
+        self.heatMaps = []
+        heatmap_prop_obj = self.propDict["heatmap"]
+        clustered_by_property = PlotProperty.cluster_property(heatmap_prop_obj)
+        for property, properties in clustered_by_property.items():
+            timeseries = [prop.get_timeseries_obj() for prop in properties]
+            populations = [prop.population for prop in properties]
+            for ts, population in zip(timeseries, populations):
+                self.heatMaps.append(HeatMap(self, property, population, ts))
+    
+        dockName = f"heatmaps"
+        newDock = Dock(dockName, closable = True)
+        dockLayout = DockArea()
+        newDock.addWidget(dockLayout)
+        self.area.addDock(newDock, "bottom")
+
+        for i, plot in enumerate(self.heatMaps):
+            if i == 0:
+                position = "bottom"
+                relativeTo = None
+            else:
+                position = "above"
+                plotRelativeTo = self.heatMaps[i-1]
+                relativeTo = self.docks[plotRelativeTo]
+
+            name = f"{plot.property}"
+            plotDock = Dock(name, closable = True)
+            plotDock.addWidget(plot.getPlotWidget())
+            self.docks[plot] = (plotDock)
+
+            dockLayout.addDock(plotDock, position, relativeTo)
+    
+    def addPopulationsPlots(self):
+        self.populationPlots = []
+        population_prop_obj = self.propDict["population"]
+        clustered_by_property = PlotProperty.cluster_property(population_prop_obj)
+        for property, properties in clustered_by_property.items():
+            timeseries = [prop.get_timeseries_obj() for prop in properties]
+            populations = [prop.population for prop in properties]
+            for ts, population in zip(timeseries, populations):
+                self.populationPlots.append(PopulationPlot(self, property, ts, population))
+    
+        dockName = f"population plots"
+        newDock = Dock(dockName, closable = True)
+        dockLayout = DockArea()
+        newDock.addWidget(dockLayout)
+        self.area.addDock(newDock, "bottom")
+
+        for i, plot in enumerate(self.populationPlots):
+            if i == 0:
+                position = "bottom"
+                relativeTo = None
+            else:
+                position = "above"
+                plotRelativeTo = self.populationPlots[i-1]
+                relativeTo = self.docks[plotRelativeTo]
+
+            name = f"{plot.property}"
+            plotDock = Dock(name, closable = True)
+            plotDock.addWidget(plot.getPlotWidget())
+            self.docks[plot] = (plotDock)
+
+            dockLayout.addDock(plotDock, position, relativeTo)
+    
+    def addMplPlots():
+        pass
 
     def updateSingleCellPlots(self):
-        for plotName, widgets in self.docks.items():
-            if " " in plotName:
-                s = plotName.split(" ")
-                plotType, prop = s[0], s[1]
-                if "single" in plotType:
-                    _, newPlot = widgets
-                    newPlot.clear()
-                    data = self.getData(plotType, prop) 
-
-                    if type(data) is dict:     
-                        newPlot.addLegend()
-                        i = 0
-                        for cellnum, dataset in data.items():
-                            color = self.parent.cmaps[0][i][0:-1]
-                            newPlot.plot(dataset, name = str(cellnum), pen = tuple(color))
-                            i+=1
-                    else:
-                        newPlot.plot(data)
+        for plot in self.singleCellPlots:
+            plot.update()
+        
 
     def updatePopulationPlots(self):
-        for plotName, widgets in self.docks.items():
-            if " " in plotName:
-                s = plotName.split(" ")
-                plotType, prop = s[0], s[1]
-                if "population" in plotType:
-                    _, im = widgets
-                    imData = self.getHeatMap(prop)
-                    im.setImage(imData, autoLevels = True)
+        for plot in self.populationPlots:
+            plot.update()
     
     def updateHeatMaps(self):
-        for plotName, widgets in self.docks.items():
-            if " " in plotName:
-                s = plotName.split(" ")
-                plotType, prop = s[0], s[1]
-                if "heatmap" in plotType:
-                    _, newPlot = widgets
-                    newPlot.clear()
-                    data = self.getData(plotType, prop)        
-                    newPlot.plot(data)
+        for plot in self.heatMaps:
+            plot.update()
 
     def setData(self):
         self.data = self.parent.getCellData()
 
     def getDataIdx(self, population):
         try:
             idx = self.parent.labelSelect.items().index(population)
             print(idx)
             return idx
         except ValueError:
             return None
 
-    def getDataToUse(self, prop):
-        if self.data:
-            idx = self.getDataIdx(prop)
-            if idx is not None:
-                return self.data[idx]
-            else:
-                return None
-        else:
-            return None
-
-    def getData(self, cellType, property):
-        s = property.split("-")
-        population, property = s[0],"-".join(s[1:])
-        dataToUse = self.getDataToUse(population)
-        if type(dataToUse) is pd.core.frame.DataFrame:
-            if cellType == "population":
-                cellNum = "population"
-                data = (dataToUse.loc[dataToUse["labels"] == cellNum][property]).tolist()[0]
-            elif cellType == "single" and self.parent.selectedCells:
-                data = {}
-                for cellNum in self.parent.selectedCells:
-                    data[cellNum] = (dataToUse.loc[dataToUse["labels"] == cellNum][property]).tolist()[0]
-            elif cellType == "single" and not (self.parent.selectedCells):
-                data =  [0]*10
-            return data
-        else:
-            return [0]*10
-    
-    def getHeatMap(self, property):
-        dataToUse = self.getDataToUse("heatmap")
-        if type(dataToUse) is pd.core.frame.DataFrame:
-            return np.array(dataToUse[property][0:-1].to_list())
-        else:
-            return np.zeros((10,10))
-
     def updatePlots(self):
         self.updateSingleCellPlots()
         self.updatePopulationPlots()
         self.updateHeatMaps()
 
     def createTable(self):
         # create table with dummy data
```

### Comparing `yeastvision-0.1.5/yeastvision/track/cell.py` & `yeastvision-0.1.6/yeastvision/track/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from skimage.measure import regionprops, regionprops_table
 from skimage.measure import shannon_entropy as shentr
 import numpy as np
 import pandas as pd
-from yeastvision.track.utils import normalize_im
+from yeastvision.utils import normalize_im
 from tqdm import tqdm
 
 class Cell():
     def __init__(self, mask, num):
         self.cell = (mask == num)
         self.centroid = self.getCentroid()
 
@@ -31,20 +31,20 @@
 def intensity_total(label, intensity_im):
     return np.sum(intensity_im)
 
 def concentration(label, intensity_im):
     return intensity_total(label, intensity_im)/np.sum(label)
 
 LABEL_PROPS = ["area", "eccentricity", "label", ]
-IM_PROPS = ["intensity_max", "intensity_min", "intensity_mean", ]
-EXTRA_IM_PROPS = [median, var, intensity_total, concentration, entropy]
+IM_PROPS = ["intensity_mean"]
+EXTRA_IM_PROPS = [ var, intensity_total, concentration]
 
 def getLifeData(labels):
     lifeData = {"birth":[], "death":[]}
-    for val in np.unique(labels)[1:]:
+    for val in tqdm(np.unique(labels)[1:]):
         lifeData["birth"].append(getBirthFrame(labels, val))
         lifeData["death"].append(getDeathFrame(labels, val))
     return lifeData
 
 def getPropDf(data):
     #newData = data.drop[data[data["labels"] == "population"].index]
     return data.drop(columns = ["labels", "birth", "death"])
@@ -83,15 +83,15 @@
 
 def getCellData(labels, intensity_ims = None, intensity_im_names = None):
     total_labels = np.unique(labels) # all indeces of cells present in the movie
     total_labels = total_labels[total_labels!=0]
     total_data = {"labels": total_labels} # dictionary storing cell data, to be converted to pd.df
     
     # add birth and death data
-    total_data = total_data | getLifeData(labels)
+    total_data = total_data #| getLifeData(labels)
 
     # determine whether or not to include image properties in call to regionprops_table
     if intensity_ims:
         intensity_ims = [normalize_im(im) for im in intensity_ims]
         props = LABEL_PROPS + IM_PROPS
         extra_properties = EXTRA_IM_PROPS
     else:
@@ -112,48 +112,64 @@
         
         im_data = regionprops_table(label, intensity_im, properties = props, extra_properties = extra_properties)
         
         # add zeros for cells not present in im data
         for label in total_labels:
             if label not in im_data["label"]:
                 for property in im_data:
-                    vals = [round(val, 3) for val in list(im_data[property])]
+                    vals = [round(val, 3) if val is not None else None for val in list(im_data[property])]
                     im_data[property] = vals
 
                     if property != "label":
                         # prevent index out of bound error
                         if label-1 < len(im_data[property]):
-                            im_data[property][label-1] = 0
+                            im_data[property][label-1] = None
                         else:
-                            im_data[property].append(0)
+                            im_data[property].append(None)
         
         for property in im_data:
             if property != "label":
                 if property not in total_data:
                     total_data[property] = [[prop] for prop in im_data[property]]
                 else:
                     for label in total_labels:
                         total_data[property][label-1].append(im_data[property][label-1])
         
     if intensity_im_names:
         for property in im_data:
-            if "-" in property:
-                parts = property.split("-")
-                name, index = parts[0], int(parts[1])
-                newPropertyName = "-".join([name, intensity_im_names[index]])
+            isImProp = False
+            for prop in IM_PROPS+EXTRA_IM_PROPS:
+                try:
+                    prop = prop.__name__
+                except AttributeError:
+                    prop = str(prop)
+
+                if prop in property:
+                    isImProp = True
+                    break
+            if isImProp:
+                if "-" in property:
+                    idx = int(property.split("-")[-1])-1
+                else:
+                    idx = 0
+                newPropertyName = "-".join([intensity_im_names[idx], prop])
                 total_data[newPropertyName] = total_data[property]
                 del total_data[property]
+
+
+                
+
     
-    # get population average for each property
-    for property in total_data:
-        if property not in ["labels", "birth", "death"]:
-            property_array = np.array(total_data[property], dtype = np.float32) # rows are cells (axis 0), columns are time (axis 1)
-            property_array[property_array == 0.0] = np.nan
-            total_data[property].append(list(np.nanmean(property_array, axis = 0)))
-        elif property == "labels":
-            total_data["labels"] = list(total_data["labels"])
-            total_data["labels"].append("population")
-        else:
-            total_data[property].append(0)
+    # # get population average for each property
+    # for property in total_data:
+    #     if property not in ["labels", "birth", "death"]:
+    #         property_array = np.array(total_data[property], dtype = np.float32) # rows are cells (axis 0), columns are time (axis 1)
+    #         property_array[property_array == 0.0] = np.nan
+    #         total_data[property].append(list(np.nanmean(property_array, axis = 0)))
+    #     elif property == "labels":
+    #         total_data["labels"] = list(total_data["labels"])
+    #         total_data["labels"].append("population")
+    #     else:
+    #         total_data[property].append(0)
 
     df = pd.DataFrame.from_dict(total_data)
     return df
```

### Comparing `yeastvision-0.1.5/yeastvision/track/hungarian_track.py` & `yeastvision-0.1.6/yeastvision/track/hungarian_track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/track/lineage.py` & `yeastvision-0.1.6/yeastvision/track/lineage.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,110 @@
 from skimage.morphology import binary_dilation, binary_erosion, dilation, erosion, disk
 from skimage.measure import label, regionprops
 from yeastvision.models.unet import unet
 from yeastvision.track.cell import getBirthFrame, getLifeData
 import matplotlib.pyplot as plt 
 from yeastvision.track.utils import normalize_dict_by_sum
 from tqdm import tqdm
+from skimage.morphology import skeletonize
 
 def count_objects(labeledMask):
     return np.count_nonzero(np.unique(labeledMask))
 
+def get_daughters(tree, cell):
+    potentialDaughters = tree[cell-1]
+    daughters = list(np.where(potentialDaughters)[0]+1)
+    return daughters
+
+def has_daughters(tree, cell):
+    return np.any(tree[cell-1,:])   
+
+    
+def get_generations(tree, initial_generation):
+    generations = [[]]
+    for val in initial_generation:
+        generations[0].append(val)
+        get_generations_recur(tree, 1, generations, 0, val)
+    print(generations)
+    return generations
+
+def get_generations_recur(tree, generation, generations, max_generation, cell):
+    if not has_daughters(tree, cell):
+        return 
+    
+    daughters = get_daughters(tree, cell)
+    if generation>=len(generations):
+        generations.append([])
+        max_generation = generation
+    for daughter in daughters:
+        generations[generation].append(daughter)
+        get_generations_recur(tree, generation+1, generations, max_generation, daughter)
+
+def get_gametes(skeleton, cyto, idx):
+    found_gametes = False
+    overlap = []
+    previous_overlaps = []
+    while (not found_gametes) and idx>=0:
+        mask = cyto[idx]
+        overlap = np.unique(mask[skeleton>0])
+        overlap = overlap[overlap!=0]
+
+        previous_overlaps.append(overlap)
+        found_gametes = len(overlap)==2
+        idx -=1
+    
+    if len(overlap)==0:
+        for previous_overlap in previous_overlaps:
+            if len(previous_overlap)>0:
+                overlap = previous_overlap
+                break
+
+    if len(overlap)>2:
+        overlap = overlap[0:2]
+    else:
+        overlap = np.append(overlap, [None, None])
+    return found_gametes, overlap
+
+def is_mating_cell(mat, cyto, cell):
+    return np.all(mat[cyto==cell]==cell)
+
+def compute_mating_lineage(tracked, cyto):
+
+    cellVals = np.unique(cyto)
+    cellVals = cellVals[cellVals!=0]
+
+    matingCells = np.unique(tracked)
+    matingCells = matingCells[matingCells!=0]
+
+    numCells = np.count_nonzero(matingCells)
+    
+    print("computing lineages for", numCells, "cells")
+    gamete_dict = {
+                  "gamete1":[],
+                    "gamete2":[],
+                    "isMating":[],
+                    "foundGametes":[]}
+
+    for label in tqdm(cellVals):
+        isMating = label in matingCells
+        if isMating:
+            birth = getBirthFrame(tracked, label)
+            mat_birth_mask = (tracked[birth] == label).astype(np.uint8)
+            found_gametes, gametes = get_gametes(skeletonize(mat_birth_mask),
+                                                 cyto, birth-1)
+        else:
+            found_gametes = False
+            gametes = [None, None]
+        
+        gamete_dict["gamete1"].append(gametes[0])
+        gamete_dict["gamete2"].append(gametes[1])
+        gamete_dict["isMating"].append(isMating)
+        gamete_dict["foundGametes"].append(found_gametes)
+    
+    return pd.DataFrame.from_dict(gamete_dict)
 
 class LineageConstruction():
     def __init__(self, segMasks, budMasks = None, backskip = 0, forwardskip = 0):
         self.cellMasks = segMasks 
         self.neckMasks = budMasks
         self.backskip = backskip
         self.forskip = forwardskip
@@ -95,15 +187,15 @@
                 daughterArray[mother-1, cellId-1] = True
             motherDict["mother"].append(mother)
             motherDict["confidence"].append(confidence)
         
         motherDF = pd.DataFrame.from_dict(motherDict)
         #daughterDF = pd.DataFrame(data = daughterArray, index = cellVals, columns=cellVals)
         #motherDF = motherDF.set_index("cell")
-        return daughterArray, motherDF[["cell", "birth", "death", "mother", "confidence"]]
+        return daughterArray, motherDF[["birth", "death", "mother", "confidence"]]
     
     def getMother(self, cellNum):
         '''
         1) get bud that overlaps with daughter the most
         2) '''
         birth = getBirthFrame(self.cellMasks, cellNum)
         birthFrame = self.cellMasks[birth]
```

### Comparing `yeastvision-0.1.5/yeastvision/track/mat.py` & `yeastvision-0.1.6/yeastvision/track/mat.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import statistics as stats
 import matplotlib.pyplot as plt
 from skimage.morphology import thin, skeletonize, opening, dilation, erosion, square
 from skimage.measure import regionprops, label
 from tqdm import tqdm
 
 def get_mating_data(mating, cells):
-    pass
+    mating_tracks = correct_mat_tracks(track_mating(mating))
+    return merge(cells, mating_tracks)
 
 
 def track_mating(mating_masks, visualize = False):
     cell_margin = 20
     numbM = len(mating_masks)
     MATC = [[[] for _ in range(numbM)] for _ in range(2)]
     
@@ -367,15 +368,15 @@
     return np.array(MATrack, dtype = np.uint16)
 
 def merge(full_masks, Matmasks, visualize = False):
     #Corrected MATracking masks
     numbM = Matmasks[0].shape[0]
     no_obj = np.max(Matmasks[0, numbM-1, :, :])
     MATC = [[[] for _ in range(numbM)] for _ in range(1)]
-    new_tracks = np.zeros_like(Matmasks[0])
+    new_tracks = np.zeros_like(Matmasks)
     print("Merging mating cells into cell mask")
     print("\t Loop 1/1")
     for cxell in tqdm(range(1,no_obj.astype(int)+1)):
         for im_no, mask in enumerate(full_masks[0:numbM]):
             if cxell == 1:
                 I2 = mask.copy()
             else:
@@ -460,9 +461,12 @@
                 MATC[0][im_no] = I2
                 new_tracks[im_no][pix] = new_num
                 
                 if visualize:
                     plt.imshow(I2==np.max(I2))
                     plt.title('cxell: ' + str(cxell) + ', im_no: ' + str(im_no))
                     plt.show()
-    return MATC, new_tracks
+    MATC[0].append(MATC[0][-1])
+    new_tracks = list(new_tracks)
+    new_tracks.append(new_tracks[-1])
+    return np.array(MATC[0], dtype = np.uint16), np.array(new_tracks, dtype = np.uint16)
```

### Comparing `yeastvision-0.1.5/yeastvision/track/track.py` & `yeastvision-0.1.6/yeastvision/track/track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.5/yeastvision/track/utils.py` & `yeastvision-0.1.6/yeastvision/track/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,39 +52,14 @@
     centroid = regionprops(bool_im.astype(np.uint8))[0].centroid
     r_size, c_size = bool_im.shape
     r,c = centroid
     r,c = round(r), round(c)
     bbox = slice(max([0, r-cell_margin]), min([r_size, r+cell_margin])), slice(max([0, c-cell_margin]), min([c_size, c+cell_margin]))
     return bbox
 
-def normalize_im(im, clip = True):
-    """
-    Normalizes a given image such that the values range between 0 and 1.     
-    
-    Parameters
-    ---------- 
-    im : 2d-array
-        Image to be normalized.
-    clip: boolean
-        Whether or not to set im values <0 to 0
-        
-    Returns
-    -------
-    im_norm: 2d-array
-        Normalized image ranging from 0.0 to 1.0. Note that this is now
-        a floating point image and not an unsigned integer array. 
-    """ 
-    assert not np.any(np.isnan(im))
-    if clip:
-        im[im<0] = 0
-    if im.max()==0:
-        return im.astype(np.float32)
-    im_norm = (im - im.min()) / (im.max() - im.min())
-    return im_norm.astype(np.float32)
-
 def avg_cell_size(Matmasks,nu,no_obj):
     avg = [[[] for _ in range(nu)] for _ in range(no_obj.astype(int)+1)]
     avg_cell = [0]*no_obj.astype(int)
 
     for iv in range(1,no_obj.astype(int)+1):
         for its in range(nu):
             avg[iv-1][its] = np.average(Matmasks[0][its]==iv)
```

### Comparing `yeastvision-0.1.5/yeastvision/utils.py` & `yeastvision-0.1.6/yeastvision/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 
 def enlarge_bud(bud_mask, footprint = None, kernel_size = 4):
     if not footprint:
         footprint = disk(kernel_size)
     return binary_dilation(bud_mask, footprint)
 
-def normalize_im(im, clip = True):
+def normalize_im(im_o, clip = True):
     """
     Normalizes a given image such that the values range between 0 and 1.     
     
     Parameters
     ---------- 
     im : 2d-array
         Image to be normalized.
@@ -115,20 +115,21 @@
         
     Returns
     -------
     im_norm: 2d-array
         Normalized image ranging from 0.0 to 1.0. Note that this is now
         a floating point image and not an unsigned integer array. 
     """ 
-    assert not np.any(np.isnan(im))
+    im = np.nan_to_num(im_o)
     if clip:
         im[im<0] = 0
     if im.max()==0:
         return im.astype(np.float32)
     im_norm = (im - im.min()) / (im.max() - im.min())
+    im_norm[np.isnan(im_o)] = np.nan
     return im_norm.astype(np.float32)
 
 def convertGreyToRGBA(im):
     image = skimage.util.img_as_ubyte(normalize_im(im))
     image_3D = cv2.merge((image,image,image))
     return image_3D
     # rgba = cv2.cvtColor(rgb, cv2.COLOR_RGB2RGBA)
```

### Comparing `yeastvision-0.1.5/yeastvision.egg-info/PKG-INFO` & `yeastvision-0.1.6/yeastvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastvision
-Version: 0.1.5
+Version: 0.1.6
 Summary: Deep learning-enabled image analysis of the yeast full life cycle
 Home-page: https://github.com/berkyalcinkaya/yeastvision
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `yeastvision-0.1.5/yeastvision.egg-info/SOURCES.txt` & `yeastvision-0.1.6/yeastvision.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 yeastvision/parts/menu.py
 yeastvision/parts/utils.py
 yeastvision/parts/workers.py
 yeastvision/plot/__init__.py
 yeastvision/plot/cell_table.py
 yeastvision/plot/plot.py
 yeastvision/plot/types.py
+yeastvision/plot/utils.py
 yeastvision/track/__init__.py
 yeastvision/track/cell.py
 yeastvision/track/data.py
 yeastvision/track/hungarian_track.py
+yeastvision/track/lc.py
 yeastvision/track/lineage.py
 yeastvision/track/mat.py
 yeastvision/track/track.py
 yeastvision/track/utils.py
```

