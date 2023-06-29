# Comparing `tmp/anatools-3.2.0.tar.gz` & `tmp/anatools-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatools-3.2.0.tar", last modified: Thu Jun 15 17:52:45 2023, max compression
+gzip compressed data, was "anatools-3.2.1.tar", last modified: Thu Jun 29 21:21:34 2023, max compression
```

## Comparing `anatools-3.2.0.tar` & `anatools-3.2.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.500299 anatools-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-15 17:52:22.000000 anatools-3.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-15 17:52:22.000000 anatools-3.2.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-06-15 17:52:45.500299 anatools-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6585 2023-06-15 17:52:22.000000 anatools-3.2.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.484298 anatools-3.2.0/anatools/
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-15 17:52:27.000000 anatools-3.2.0/anatools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.488298 anatools-3.2.0/anatools/anaclient/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11167 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/anaclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)    11005 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/annotations.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.488298 anatools-3.2.0/anatools/anaclient/api/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)     9403 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10389 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)    10116 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     4206 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     5334 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/limits.py
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/members.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/umap.py
--rw-rw-rw-   0 root         (0) root         (0)     8958 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)    18408 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     9203 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     9386 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/umap.py
--rw-rw-rw-   0 root         (0) root         (0)    17897 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/workspaces.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.492298 anatools-3.2.0/anatools/annotations/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_coco.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_kitti.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_pascal.py
--rw-rw-rw-   0 root         (0) root         (0)     4468 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_sagemaker.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/draw.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.492298 anatools-3.2.0/anatools/bin/
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/ana
--rw-rw-rw-   0 root         (0) root         (0)     9659 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/anadeploy
--rw-rw-rw-   0 root         (0) root         (0)     7692 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/anamount
--rw-rw-rw-   0 root         (0) root         (0)     4559 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/anautils
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.496299 anatools-3.2.0/anatools/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6974 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/ana_object.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/bbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/blender_main.py
--rw-rw-rw-   0 root         (0) root         (0)     4923 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/camera_checks.py
--rw-rw-rw-   0 root         (0) root         (0)    14524 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/directory_object.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/download.py
--rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/file_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/file_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/file_object.py
--rw-rw-rw-   0 root         (0) root         (0)     9556 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/interp.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/load.py
--rw-rw-rw-   0 root         (0) root         (0)    10556 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/object_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/package_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/print.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/python_main.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/rigged_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8111 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/search_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.500299 anatools-3.2.0/anatools/nodes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/constants.yml
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/generators.yml
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/logic.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/logic.yml
--rw-rw-rw-   0 root         (0) root         (0)     5381 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/random_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/random_generator.yml
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_arange.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_arange.yml
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_linspace.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_linspace.yml
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/vectors.yml
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_directory.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_directory.yml
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_file.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_file.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.484298 anatools-3.2.0/anatools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2717 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-15 17:52:22.000000 anatools-3.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-15 17:52:22.000000 anatools-3.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-15 17:52:45.500299 anatools-3.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-15 17:52:22.000000 anatools-3.2.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.500299 anatools-3.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-15 17:52:23.000000 anatools-3.2.0/tests/test_bbox.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.145289 anatools-3.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-29 21:21:16.000000 anatools-3.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-29 21:21:16.000000 anatools-3.2.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6975 2023-06-29 21:21:34.145289 anatools-3.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6585 2023-06-29 21:21:16.000000 anatools-3.2.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.129289 anatools-3.2.1/anatools/
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-29 21:21:19.000000 anatools-3.2.1/anatools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.133289 anatools-3.2.1/anatools/anaclient/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11517 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/anaclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)    11005 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/annotations.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.137289 anatools-3.2.1/anatools/anaclient/api/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)     9403 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4510 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10389 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10116 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5334 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/limits.py
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/members.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8958 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/api/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    18408 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     9203 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9386 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)    17897 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/anaclient/workspaces.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.141289 anatools-3.2.1/anatools/annotations/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/convert_coco.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/convert_kitti.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/convert_pascal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4468 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/convert_sagemaker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/convert_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/annotations/draw.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.141289 anatools-3.2.1/anatools/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/bin/ana
+-rw-rw-rw-   0 root         (0) root         (0)     9659 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/bin/anadeploy
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/bin/anamount
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/bin/anautils
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.141289 anatools-3.2.1/anatools/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6974 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/ana_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/bbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/blender_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4923 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/camera_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14524 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/directory_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/file_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/file_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/file_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     9556 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/interp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/load.py
+-rw-rw-rw-   0 root         (0) root         (0)    10556 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/object_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/package_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/print.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/python_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/rigged_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8111 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/lib/search_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.145289 anatools-3.2.1/anatools/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/constants.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/generators.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/logic.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/random_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/random_generator.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/sweep_arange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/sweep_arange.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/sweep_linspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/sweep_linspace.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/vectors.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/volume_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/volume_directory.yml
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/volume_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-29 21:21:16.000000 anatools-3.2.1/anatools/nodes/volume_file.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.129289 anatools-3.2.1/anatools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6975 2023-06-29 21:21:34.000000 anatools-3.2.1/anatools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2023-06-29 21:21:34.000000 anatools-3.2.1/anatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 21:21:34.000000 anatools-3.2.1/anatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-29 21:21:34.000000 anatools-3.2.1/anatools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-29 21:21:34.000000 anatools-3.2.1/anatools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-29 21:21:16.000000 anatools-3.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-29 21:21:16.000000 anatools-3.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-29 21:21:34.145289 anatools-3.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-29 21:21:16.000000 anatools-3.2.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 21:21:34.145289 anatools-3.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-29 21:21:16.000000 anatools-3.2.1/tests/test_bbox.py
```

### Comparing `anatools-3.2.0/LICENSE` & `anatools-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/PKG-INFO` & `anatools-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.2.0
+Version: 3.2.1
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.2.0/README.md` & `anatools-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/__init__.py` & `anatools-3.2.1/anatools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         https://support.rendered.ai/gc/Introduction-to-Rendered.ai.1577812005.html
 
 """
 
 from .anaclient.anaclient import client
 from .annotations.annotations import annotations
 
-__version__ = '3.2.0'
+__version__ = '3.2.1'
```

### Comparing `anatools-3.2.0/anatools/anaclient/anaclient.py` & `anatools-3.2.1/anatools/anaclient/anaclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """The client module is used for connecting to Rendered.ai's Platform API."""
 
 envs = {
     'prod': {
         'name': 'Rendered.ai Platform',
         'url':  'https://deckard.rendered.ai',
+        'statusAPI': 'https://api.rendered.ai/system',
         'api':  'https://api.rendered.ai/graphql' },
     'test': {
         'name': 'Rendered.ai Test Platform',
         'url':  'https://deckard-test.web.app',
+        'statusAPI': 'https://api.test.rendered.ai/system',
         'api':  'https://api.test.rendered.ai/graphql' },
     'dev': {
         'name': 'Rendered.ai Development Platform',
         'url':  'https://deckard-dev-8eaa5.web.app',
+        'statusAPI': 'https://api.dev.rendered.ai/system',
         'api':  'https://api.dev.rendered.ai/graphql' },
     'infra': {
         'name': 'Rendered.ai Infrastructure Platform',
         'url':  'https://deckard-infra.web.app',
+        'statusAPI': 'https://api.infra.rendered.ai/system',
         'api':  'https://api.infra.rendered.ai/graphql' }
 }
 
-
 class client:
 
     def __init__(self, workspaceId=None, environment='prod', email=None, password=None, local=False, interactive=True, verbose=None):
         import getpass
         import time
         import os
         from anatools.anaclient.api import api
@@ -32,26 +35,27 @@
         self.interactive = interactive
         if environment not in ['dev','test','prod','infra']:  print("Invalid environment argument, must be 'infra', 'dev', 'test' or 'prod'."); return
         if local:
             os.environ['NO_PROXY'] = '127.0.0.1'
             self.__url = 'http://127.0.0.1:3000'
             if interactive: print("Local is set to",self.__url)
         else: self.__url = envs[environment]['api']
+        self.__status_url = envs[environment]['statusAPI']
         self.__password = password
         self.__logout = True
         self.__notificationId = None
         self.email = email
         self.user = None
         self.organizations = {}
         self.workspaces ={}
         self.channels = {}
         self.volumes = {}
         self.organization = None
 
-        self.ana_api = api(self.__url, None, self.verbose)
+        self.ana_api = api(self.__url, self.__status_url, None, self.verbose)
 
         # fetch system notification
         notification = self.ana_api.getSystemNotifications()
         if notification:
             self.__notificationId = notification['notificationId']
             print_color(notification['message'], 'ffff00')
 
@@ -65,15 +69,15 @@
                 self.user = self.ana_api.login(self.email, self.__password)
         if self.user is None:
             try: self.user = self.ana_api.login(self.email, self.__password)
             except: print(f'Failed to login to {envs[environment]["name"]} with email {self.email}.'); return
         if self.user is False: print(f'Failed to login to {envs[environment]["name"]} with email {self.email}.'); return
         if self.verbose == 'debug': print(f'{self.user["uid"]}\n{self.user["idtoken"]}')
         self.__logout = False
-        self.ana_api = api(self.__url, {'uid':self.user['uid'], 'idtoken':self.user['idtoken']}, self.verbose)
+        self.ana_api = api(self.__url, self.__status_url, {'uid':self.user['uid'], 'idtoken':self.user['idtoken']}, self.verbose)
         self.get_organizations()
         if len(self.organizations) == 0: print("No organizations available. Contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact."); return
         found_valid_org = False
         for organization in self.organizations:
             if organization['expired']:
                 print("Warning!!!")
                 print(f"    The subscription has expired for {organization['name']} organization (organizationId {organization['organizationId']}).") 
@@ -117,15 +121,15 @@
 
     def refresh_token(self):
         import time
         from anatools.anaclient.api import api
         from anatools.lib.print import print_color
         if int(time.time()) > int(self.user['expires']):
             self.user = self.ana_api.login(self.email, self.__password)
-            self.ana_api = api(self.__url, {'uid': self.user['uid'], 'idtoken': self.user['idtoken']}, self.verbose)
+            self.ana_api = api(self.__url, self.__status_url, {'uid': self.user['uid'], 'idtoken': self.user['idtoken']}, self.verbose)
             notification = self.ana_api.getSystemNotifications()
             if notification and notification['notificationId'] != self.__notificationId:
                 self.__notificationId = notification['notificationId']
                 print_color(notification['message'], 'ffff00')
 
 
     def check_logout(self):
```

### Comparing `anatools-3.2.0/anatools/anaclient/analytics.py` & `anatools-3.2.1/anatools/anaclient/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/annotations.py` & `anatools-3.2.1/anatools/anaclient/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/analytics.py` & `anatools-3.2.1/anatools/anaclient/api/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/annotations.py` & `anatools-3.2.1/anatools/anaclient/api/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/api.py` & `anatools-3.2.1/anatools/anaclient/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """API Module"""
 
 class api:
     
-    def __init__(self, url, headers, verbose=False):
+    def __init__(self, url, status_url, headers, verbose=False):
         import requests
         self.url = url
+        self.status_url = status_url
         self.headers = headers
         self.verbose = verbose
         self.session = requests.Session()
 
     def login(self, email, password):
         response = self.session.post(
             url = self.url, 
@@ -43,15 +44,15 @@
                         }
                     }"""})
         if 'errors' in response.json(): return False
         return self.errorhandler(response, "getSystemNotifications")
 
     def getSystemStatus(self, serviceId=None):
         response = self.session.post(
-            url = self.url, 
+            url = self.status_url, 
             json = {
                 "operationName": "getSystemStatus",
                 "variables": {
                     "serviceId": serviceId
                 },
                 "query": """query 
                     getSystemStatus($serviceId: String) {
```

### Comparing `anatools-3.2.0/anatools/anaclient/api/channels.py` & `anatools-3.2.1/anatools/anaclient/api/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/datasets.py` & `anatools-3.2.1/anatools/anaclient/api/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/gan.py` & `anatools-3.2.1/anatools/anaclient/api/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/graphs.py` & `anatools-3.2.1/anatools/anaclient/api/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/handlers.py` & `anatools-3.2.1/anatools/anaclient/api/handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/limits.py` & `anatools-3.2.1/anatools/anaclient/api/limits.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/members.py` & `anatools-3.2.1/anatools/anaclient/api/members.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/organizations.py` & `anatools-3.2.1/anatools/anaclient/api/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/umap.py` & `anatools-3.2.1/anatools/anaclient/api/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/volumes.py` & `anatools-3.2.1/anatools/anaclient/api/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/api/workspaces.py` & `anatools-3.2.1/anatools/anaclient/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/channels.py` & `anatools-3.2.1/anatools/anaclient/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/datasets.py` & `anatools-3.2.1/anatools/anaclient/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/gan.py` & `anatools-3.2.1/anatools/anaclient/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/graphs.py` & `anatools-3.2.1/anatools/anaclient/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/organizations.py` & `anatools-3.2.1/anatools/anaclient/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/umap.py` & `anatools-3.2.1/anatools/anaclient/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/volumes.py` & `anatools-3.2.1/anatools/anaclient/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/anaclient/workspaces.py` & `anatools-3.2.1/anatools/anaclient/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/annotations.py` & `anatools-3.2.1/anatools/annotations/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/convert_coco.py` & `anatools-3.2.1/anatools/annotations/convert_coco.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/convert_kitti.py` & `anatools-3.2.1/anatools/annotations/convert_kitti.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/convert_pascal.py` & `anatools-3.2.1/anatools/annotations/convert_pascal.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/convert_sagemaker.py` & `anatools-3.2.1/anatools/annotations/convert_sagemaker.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/convert_yolo.py` & `anatools-3.2.1/anatools/annotations/convert_yolo.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/annotations/draw.py` & `anatools-3.2.1/anatools/annotations/draw.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/bin/ana` & `anatools-3.2.1/anatools/bin/ana`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/bin/anadeploy` & `anatools-3.2.1/anatools/bin/anadeploy`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/bin/anamount` & `anatools-3.2.1/anatools/bin/anamount`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/bin/anautils` & `anatools-3.2.1/anatools/bin/anautils`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/ana_object.py` & `anatools-3.2.1/anatools/lib/ana_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/bbox.py` & `anatools-3.2.1/anatools/lib/bbox.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/blender_main.py` & `anatools-3.2.1/anatools/lib/blender_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/camera_checks.py` & `anatools-3.2.1/anatools/lib/camera_checks.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/channel.py` & `anatools-3.2.1/anatools/lib/channel.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/context.py` & `anatools-3.2.1/anatools/lib/context.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/directory_object.py` & `anatools-3.2.1/anatools/lib/directory_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/file_handlers.py` & `anatools-3.2.1/anatools/lib/file_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,31 @@
     """
 
     if self.loaded:
         # only load the object once
         return
 
     blender_file = kwargs.pop("blender_file")
-    # load the collections containing the object
+
+    # load the collection containing the object
     with bpy.data.libraries.load(filepath="//" + blender_file, link=False) as (df, dt):
         dt.collections = df.collections
     
-    # find the topmost object and set the ana collection to that object's collection
-    self.root = find_root(dt.collections[0])
-    self.collection = self.root.users_collection[0]
+    if len(dt.collections) > 0:
+        # the object was in a collection
+        self.root = find_root(dt.collections[0])
+        self.collection = self.root.users_collection[0]
+    else:
+        # there was no collection found. load the first object found.
+        with bpy.data.libraries.load(filepath="//" + blender_file, link=False) as (df, dt):
+            dt.objects = df.objects
+        name = dt.objects[0].name
+        self.collection = bpy.data.collections.new(name)
+        bpy.data.collections[name].objects.link(dt.objects[0])
+        self.root = dt.objects[0]
     
     # link the collection to the scene
     bpy.context.scene.collection.children.link(self.collection)
 
     # deprecated parameter
     self.loaded = True
```

### Comparing `anatools-3.2.0/anatools/lib/file_metadata.py` & `anatools-3.2.1/anatools/lib/file_metadata.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/file_object.py` & `anatools-3.2.1/anatools/lib/file_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/generator.py` & `anatools-3.2.1/anatools/lib/generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/interp.py` & `anatools-3.2.1/anatools/lib/interp.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/load.py` & `anatools-3.2.1/anatools/lib/load.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/node.py` & `anatools-3.2.1/anatools/lib/node.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/object_utils.py` & `anatools-3.2.1/anatools/lib/object_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/package_utils.py` & `anatools-3.2.1/anatools/lib/package_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/python_main.py` & `anatools-3.2.1/anatools/lib/python_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/rigged_object.py` & `anatools-3.2.1/anatools/lib/rigged_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/scene.py` & `anatools-3.2.1/anatools/lib/scene.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/lib/search_utils.py` & `anatools-3.2.1/anatools/lib/search_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/constants.py` & `anatools-3.2.1/anatools/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/constants.yml` & `anatools-3.2.1/anatools/nodes/constants.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/generators.py` & `anatools-3.2.1/anatools/nodes/generators.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/generators.yml` & `anatools-3.2.1/anatools/nodes/generators.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/logic.py` & `anatools-3.2.1/anatools/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/logic.yml` & `anatools-3.2.1/anatools/nodes/logic.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/random_generator.py` & `anatools-3.2.1/anatools/nodes/random_generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/random_generator.yml` & `anatools-3.2.1/anatools/nodes/random_generator.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/sweep_arange.py` & `anatools-3.2.1/anatools/nodes/sweep_arange.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/sweep_arange.yml` & `anatools-3.2.1/anatools/nodes/sweep_arange.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/sweep_linspace.py` & `anatools-3.2.1/anatools/nodes/sweep_linspace.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/sweep_linspace.yml` & `anatools-3.2.1/anatools/nodes/sweep_linspace.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/vectors.py` & `anatools-3.2.1/anatools/nodes/vectors.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/vectors.yml` & `anatools-3.2.1/anatools/nodes/vectors.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/volume_directory.py` & `anatools-3.2.1/anatools/nodes/volume_directory.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/volume_directory.yml` & `anatools-3.2.1/anatools/nodes/volume_directory.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/volume_file.py` & `anatools-3.2.1/anatools/nodes/volume_file.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools/nodes/volume_file.yml` & `anatools-3.2.1/anatools/nodes/volume_file.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/anatools.egg-info/PKG-INFO` & `anatools-3.2.1/anatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.2.0
+Version: 3.2.1
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.2.0/anatools.egg-info/SOURCES.txt` & `anatools-3.2.1/anatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/setup.py` & `anatools-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.0/tests/test_bbox.py` & `anatools-3.2.1/tests/test_bbox.py`

 * *Files identical despite different names*

