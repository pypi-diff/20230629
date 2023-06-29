# Comparing `tmp/mmcv-lite-2.0.0rc4.tar.gz` & `tmp/mmcv-lite-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmcv-lite-2.0.0rc4.tar", last modified: Sun Jan 29 09:35:44 2023, max compression
+gzip compressed data, was "mmcv-lite-2.0.1.tar", last modified: Thu Jun 29 08:39:45 2023, max compression
```

## Comparing `mmcv-lite-2.0.0rc4.tar` & `mmcv-lite-2.0.1.tar`

### file list

```diff
@@ -1,540 +1,565 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (116)    11413 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1007 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/LICENSES.md
--rw-r--r--   0 runner    (1001) docker     (116)      490 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      827 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8322 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/
--rw-r--r--   0 runner    (1001) docker     (116)      321 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (116)      133 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2114 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (116)     1412 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2075 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (116)     1510 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3101 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4818 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (116)     1751 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (116)     2733 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (116)     9222 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     6225 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (116)     4558 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     2286 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (116)    16056 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (116)     1664 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (116)    11401 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (116)     5597 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (116)     3038 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (116)      489 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (116)    37139 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3180 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (116)     7082 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (116)    10514 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      197 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    23248 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1940 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (116)     6393 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (116)     1755 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10341 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (116)    28007 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (116)    14461 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     2065 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)    21048 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/
--rwxr-xr-x   0 runner    (1001) docker     (116)     6190 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2230 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/active_rotated_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     4761 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (116)     3138 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     4555 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (116)     4825 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/bezier_align.py
--rw-r--r--   0 runner    (1001) docker     (116)     3908 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (116)     1709 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/box_iou_quadri.py
--rw-r--r--   0 runner    (1001) docker     (116)     5252 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (116)    10564 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (116)     3146 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (116)     3374 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (116)     1935 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (116)     1853 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/convex_iou.py
--rw-r--r--   0 runner    (1001) docker     (116)     2386 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     6874 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/
--rw-r--r--   0 runner    (1001) docker     (116)    12955 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/
--rw-r--r--   0 runner    (1001) docker     (116)     2227 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4594 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     5724 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     9898 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     6913 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2876 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2459 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    12440 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4363 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     3727 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     3329 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    23369 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     7694 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    15470 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     7888 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4428 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4212 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     1708 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2384 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    12932 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2462 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2409 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     7743 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    17255 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    33575 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4052 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     5469 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     5057 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     3424 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     3334 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    15141 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     6160 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    10994 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     8616 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     9045 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     3448 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    10602 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4905 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     4702 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     6284 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2241 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/spconv/
--rw-r--r--   0 runner    (1001) docker     (116)     9124 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/spconv/indice.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     5859 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2069 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     3826 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)    11437 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     1804 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     1728 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)     7740 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/
--rw-r--r--   0 runner    (1001) docker     (116)     2734 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/carafe_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    16143 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    34933 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/iou3d_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    24191 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/nms_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     1286 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/psamask_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      937 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mlu/roi_align_rotated_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/
--rw-r--r--   0 runner    (1001) docker     (116)     1446 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSDevice.h
--rw-r--r--   0 runner    (1001) docker     (116)     1683 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSLibrary.h
--rw-r--r--   0 runner    (1001) docker     (116)     3728 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSLibrary.mm
--rw-r--r--   0 runner    (1001) docker     (116)     3486 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSStream.h
--rw-r--r--   0 runner    (1001) docker     (116)     1833 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSUtils.h
--rw-r--r--   0 runner    (1001) docker     (116)     1881 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/parrots_cpp_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4353 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/parrots_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      763 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      418 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     5047 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_device_registry.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2244 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     1337 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_npu_helper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/
--rw-r--r--   0 runner    (1001) docker     (116)     2125 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
--rw-r--r--   0 runner    (1001) docker     (116)    16039 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/prettyprint.h
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/
--rw-r--r--   0 runner    (1001) docker     (116)    10145 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h
--rw-r--r--   0 runner    (1001) docker     (116)     3743 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h
--rw-r--r--   0 runner    (1001) docker     (116)     1469 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h
--rw-r--r--   0 runner    (1001) docker     (116)    14014 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h
--rw-r--r--   0 runner    (1001) docker     (116)     1382 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/tensorview/
--rw-r--r--   0 runner    (1001) docker     (116)     2418 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (116)      464 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_launch.h
--rw-r--r--   0 runner    (1001) docker     (116)    37579 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/
--rw-r--r--   0 runner    (1001) docker     (116)     1137 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      485 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/active_rotated_filter_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/assign_score_withk.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2752 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      944 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1201 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ball_query._parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      902 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      384 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ball_query_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      622 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/bbox_overlaps.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1154 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      358 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/bbox_overlaps_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1348 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/border_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1770 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/border_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      627 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/border_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      889 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1892 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      530 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2015 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_naive.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2641 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      652 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     3164 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      750 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1693 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/chamfer_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1912 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      694 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     3290 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/contour_expand.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1456 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      469 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/contour_expand_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/convex_iou.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1307 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      356 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/convex_iou_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2560 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/correlation.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5873 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/correlation_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      856 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/correlation_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)    87064 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/cudabind.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    21266 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     9465 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1482 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_conv_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2269 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3709 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      892 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      635 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      899 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      358 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/diff_iou_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2512 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3711 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      970 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/focal_loss_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1679 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/furthest_point_sample.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1773 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      650 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     5437 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1383 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1308 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/gather_points.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2032 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/gather_points_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      536 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/gather_points_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1556 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2124 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/group_points_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      581 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/group_points_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1585 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/info.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2439 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/iou3d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/iou3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      562 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/iou3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      704 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/knn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1093 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/knn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      318 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/knn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1610 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/masked_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2369 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      693 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      380 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/min_area_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      744 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      275 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/min_area_polygons_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)    10725 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     7468 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1047 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     3087 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ms_deform_attn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3101 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1337 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4436 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1279 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1862 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      384 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/pixel_group_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2248 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2101 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      622 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      615 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      813 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      293 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_polygons_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2278 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/prroi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3275 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      779 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2136 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4546 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/psamask_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1534 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/psamask_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2344 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2764 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      842 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2230 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5354 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1515 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     2212 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5278 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1517 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1474 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2229 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      619 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     3707 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2040 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      572 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1663 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1036 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      361 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roipoint_pool3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1909 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3184 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      733 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     3202 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/sync_bn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4181 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1212 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/sync_bn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2210 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      631 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      729 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_nn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1034 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_nn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      354 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_nn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)      724 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/tin_shift.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1359 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      370 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/tin_shift_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (116)     5389 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/upfirdn2d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1470 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3605 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/voxelization.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4114 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/voxelization_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      913 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/voxelization_pytorch.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/
--rw-r--r--   0 runner    (1001) docker     (116)     1137 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/assign_score_withk.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1834 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      622 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1897 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/bezier_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1348 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/border_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      747 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      889 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2015 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/carafe.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/carafe_naive.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1693 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/chamfer_distance.cpp
--rwxr-xr-x   0 runner    (1001) docker     (116)     3290 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/contour_expand.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/convex_iou.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2560 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/correlation.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/
--rw-r--r--   0 runner    (1001) docker     (116)     4965 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    17454 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1411 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1566 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    18378 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    20255 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     7278 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2203 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2347 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp
--rwxr-xr-x   0 runner    (1001) docker     (116)     4806 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2136 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     9213 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    18587 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    17468 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     9196 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3762 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3162 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2452 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     7155 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/
--rw-r--r--   0 runner    (1001) docker     (116)     2619 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2800 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1326 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1682 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2351 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2885 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)      978 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1124 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     8976 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2267 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2955 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1814 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4261 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)    98447 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5466 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2614 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1305 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     5057 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4983 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     3027 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4437 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2079 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2330 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4253 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1176 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2627 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)      964 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu
--rw-r--r--   0 runner    (1001) docker     (116)     5100 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)    18307 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2675 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1255 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2935 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2749 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2711 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2785 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2337 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2221 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     5033 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2340 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2700 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     5066 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     7280 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu
--rw-r--r--   0 runner    (1001) docker     (116)    19211 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4106 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     6631 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu
--rw-r--r--   0 runner    (1001) docker     (116)    22064 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1844 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2481 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4894 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2473 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     1177 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)     2268 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)    11894 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (116)    11432 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)    21266 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2269 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      635 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2512 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1679 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5437 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1308 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/gather_points.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3886 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1585 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/info.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2439 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/iou3d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      704 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/knn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1610 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/masked_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      380 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/min_area_polygons.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/
--rw-r--r--   0 runner    (1001) docker     (116)     4115 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    17624 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    15865 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    14183 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5821 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (116)    10375 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    20969 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     6455 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    13458 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     9132 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (116)    10904 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    11780 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    21446 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     8221 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4469 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     8825 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    10725 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mps/
--rw-r--r--   0 runner    (1001) docker     (116)     3648 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
--rw-r--r--   0 runner    (1001) docker     (116)     3087 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1337 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/nms_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1279 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/nms_rotated.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/
--rw-r--r--   0 runner    (1001) docker     (116)     2643 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     6080 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1637 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1948 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2855 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1186 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (116)     1110 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2248 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      615 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/points_in_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2278 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/prroi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2136 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    53472 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2344 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2230 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2214 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1474 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3707 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1663 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1909 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2325 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/scatter_points.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2290 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     8280 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/spconv_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2420 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/spconv_utils.h
--rw-r--r--   0 runner    (1001) docker     (116)     3202 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/sync_bn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/three_interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      729 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/three_nn.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      724 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/tin_shift.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5389 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/upfirdn2d.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3605 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/voxelization.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    17377 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (116)     7888 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (116)    11369 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/diff_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (116)     6633 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (116)     2588 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (116)    10686 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (116)     1682 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (116)    10890 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (116)      600 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/info.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8143 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     2653 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (116)     4851 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (116)     6227 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (116)      599 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/min_area_polygons.py
--rw-r--r--   0 runner    (1001) docker     (116)    14273 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (116)    16140 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (116)    18431 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (116)     3378 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (116)    11857 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (116)     5470 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1520 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/points_in_polygons.py
--rw-r--r--   0 runner    (1001) docker     (116)     6330 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (116)     5361 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/prroi_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     2992 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (116)     5082 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/riroi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (116)     8324 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (116)     7062 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (116)     2867 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     4633 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3332 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (116)     3406 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/rotated_feature_align.py
--rw-r--r--   0 runner    (1001) docker     (116)     5908 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (116)     5886 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (116)    14049 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sparse_conv.py
--rw-r--r--   0 runner    (1001) docker     (116)     6394 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sparse_functional.py
--rw-r--r--   0 runner    (1001) docker     (116)     7243 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sparse_modules.py
--rw-r--r--   0 runner    (1001) docker     (116)     6830 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sparse_ops.py
--rw-r--r--   0 runner    (1001) docker     (116)     3274 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sparse_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     2228 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sparse_structure.py
--rw-r--r--   0 runner    (1001) docker     (116)    11519 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (116)     2240 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1558 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/three_nn.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2426 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (116)    12411 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (116)     8039 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/
--rw-r--r--   0 runner    (1001) docker     (116)     1382 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      986 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      103 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/builder.py
--rw-r--r--   0 runner    (1001) docker     (116)     3732 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (116)    12952 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (116)    57971 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/processing.py
--rw-r--r--   0 runner    (1001) docker     (116)     9372 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    24679 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/transforms/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      388 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      334 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/utils/device_type.py
--rw-r--r--   0 runner    (1001) docker     (116)     3311 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (116)     2079 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (116)      922 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (116)     1183 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (116)      570 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10254 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (116)    10221 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (116)     5643 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)      338 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1457 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (116)     5674 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     3557 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      827 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    20630 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      453 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)       86 2023-01-29 09:35:41.000000 mmcv-lite-2.0.0rc4/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (116)      633 2023-01-29 09:35:44.000000 mmcv-lite-2.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)    14452 2023-01-29 09:35:43.000000 mmcv-lite-2.0.0rc4/setup.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.974753 mmcv-lite-2.0.1/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11413 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/LICENSE
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1592 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/LICENSES.md
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      490 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/MANIFEST.in
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      824 2023-06-29 08:39:45.974753 mmcv-lite-2.0.1/PKG-INFO
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11600 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/README.md
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.909753 mmcv-lite-2.0.1/mmcv/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      321 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/__init__.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.909753 mmcv-lite-2.0.1/mmcv/arraymisc/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      133 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/arraymisc/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2114 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/arraymisc/quantization.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.909753 mmcv-lite-2.0.1/mmcv/cnn/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1501 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2075 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/alexnet.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.912753 mmcv-lite-2.0.1/mmcv/cnn/bricks/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1510 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3101 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/activation.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4818 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/context_block.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1868 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/conv.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2733 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14429 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/conv_module.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6225 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/conv_ws.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4558 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2286 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/drop.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    16056 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/generalized_attention.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1664 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/hsigmoid.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1071 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/hswish.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11401 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/non_local.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5719 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/norm.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1500 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/padding.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3155 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/plugin.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1962 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/scale.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      489 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/swish.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    37139 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/transformer.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3299 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/upsample.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7082 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/bricks/wrappers.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10514 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/resnet.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.912753 mmcv-lite-2.0.1/mmcv/cnn/rfsearch/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      210 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/rfsearch/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6787 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/rfsearch/operator.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10167 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/rfsearch/search.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2000 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/rfsearch/utils.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.913753 mmcv-lite-2.0.1/mmcv/cnn/utils/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      197 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/utils/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    23248 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/utils/flops_counter.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1940 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6393 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/cnn/vgg.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.913753 mmcv-lite-2.0.1/mmcv/image/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1755 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/image/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10341 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/image/colorspace.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    28189 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/image/geometric.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14461 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/image/io.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2065 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/image/misc.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    21048 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/image/photometric.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.922753 mmcv-lite-2.0.1/mmcv/ops/
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)     6429 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2230 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/active_rotated_filter.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4761 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/assign_score_withk.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3138 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/ball_query.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4423 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/bbox.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4825 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/bezier_align.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14058 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/bias_act.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3908 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/border_align.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1709 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/box_iou_quadri.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5362 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/box_iou_rotated.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10564 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/carafe.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3146 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/cc_attention.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3374 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/chamfer_distance.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1935 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/contour_expand.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    13463 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/conv2d_gradfix.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1853 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/convex_iou.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2475 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/corner_pool.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6874 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/correlation.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.907753 mmcv-lite-2.0.1/mmcv/ops/csrc/
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.923753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    12955 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.929753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2227 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4594 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1746 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5724 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9898 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6913 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2876 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2459 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    12437 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4363 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3727 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3329 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    23369 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7694 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    15470 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7888 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4428 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4212 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1708 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2384 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    12932 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2462 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2409 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7743 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    17255 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    33575 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4052 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5469 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5057 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3424 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3334 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1994 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    15141 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6160 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10994 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8616 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9045 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3448 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10602 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4905 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4702 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6284 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2241 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2111 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.929753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/spconv/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9124 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/spconv/indice.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5859 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2069 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3826 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11437 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1804 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1728 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2161 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7740 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.929753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mlu/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10647 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.930753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1446 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSDevice.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1683 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3728 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.mm
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3486 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSStream.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1833 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSUtils.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1881 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/parrots_cpp_helper.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4353 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/parrots_cuda_helper.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      763 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      418 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5047 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_device_registry.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2244 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1337 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_npu_helper.hpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.907753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.930753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2125 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    16039 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/prettyprint.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1956 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.931753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10145 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3743 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1469 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1190 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14014 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1382 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.931753 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2418 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      464 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_launch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    37579 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.948753 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1137 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2188 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      485 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2296 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2752 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      944 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1201 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ball_query._parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      902 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ball_query.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      384 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ball_query_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      622 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1154 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      358 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1348 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/border_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1770 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/border_align_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      627 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/border_align_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      889 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1892 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      530 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2015 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1559 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_naive.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2641 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      652 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3164 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      750 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1693 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1912 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      694 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3290 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/contour_expand.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1456 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      469 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/contour_expand_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      838 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/convex_iou.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1307 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      356 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/convex_iou_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2560 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/correlation.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5873 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/correlation_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      856 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/correlation_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    84444 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/cudabind.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    21266 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_conv.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9465 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1482 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_conv_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2269 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3709 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      892 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      635 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      899 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      358 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2512 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/focal_loss.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3711 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      970 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/focal_loss_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1679 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1773 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      650 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5437 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1383 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1308 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/gather_points.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2032 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/gather_points_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      536 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/gather_points_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1556 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/group_points.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2124 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/group_points_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      581 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/group_points_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1585 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/info.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2439 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/iou3d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2259 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/iou3d_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      562 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/iou3d_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      704 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/knn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1093 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/knn_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      318 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/knn_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1610 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2369 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      693 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      380 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      744 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      275 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10725 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7468 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1047 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3087 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3101 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1337 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4436 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      740 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1279 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1110 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/pixel_group.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1862 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      384 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/pixel_group_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2248 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2101 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      622 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      615 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      813 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      293 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2278 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/prroi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3275 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      779 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2136 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/psamask.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4546 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/psamask_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1534 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/psamask_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2344 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2764 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      842 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2230 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5354 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1515 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2212 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5278 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1517 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1474 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2229 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      619 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_pool_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3707 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2040 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      572 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1663 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1036 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      361 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1909 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3184 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      733 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3202 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/sync_bn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4181 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1212 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/sync_bn_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1575 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_interpolate.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2210 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      631 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      729 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_nn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1034 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_nn_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      354 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_nn_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      724 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/tin_shift.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1359 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      370 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/tin_shift_pytorch.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5389 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1470 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3605 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/voxelization.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4114 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/voxelization_parrots.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      913 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/voxelization_pytorch.h
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.955753 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1137 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2296 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/assign_score_withk.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1834 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/ball_query.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2137 2023-06-29 08:38:24.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1897 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/bezier_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1023 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/bias_act.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1348 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/border_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      747 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      889 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2015 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/carafe.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1559 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/carafe_naive.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1693 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/chamfer_distance.cpp
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)     3290 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/contour_expand.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      838 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/convex_iou.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2560 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/correlation.cpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.957753 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4965 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3043 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    17454 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1411 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1566 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    18378 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    20255 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7278 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2203 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2347 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)     4806 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2136 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9213 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/psamask.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    18587 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    17468 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9196 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3762 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3162 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2452 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7155 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.965753 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2619 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2800 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1326 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1682 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2351 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9833 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2885 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      978 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1124 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8976 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2267 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2955 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1814 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4261 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    99744 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5466 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2614 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1305 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    83983 2023-06-29 08:38:24.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5057 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4983 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3027 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4437 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2079 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2330 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4253 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1176 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2627 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      964 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5100 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    18325 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1559 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2163 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2303 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2675 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1255 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2935 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2749 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2711 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2785 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2337 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2221 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5033 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2340 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2700 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5066 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7280 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    19211 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4106 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6631 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    22064 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1844 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2481 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4894 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2473 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1177 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2268 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    30436 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11432 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    21266 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/deform_conv.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2269 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      635 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1871 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5820 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/focal_loss.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1679 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5437 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1579 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1308 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/gather_points.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3886 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/group_points.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1585 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/info.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2439 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/iou3d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      704 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/knn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1610 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/masked_conv2d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      380 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/min_area_polygons.cpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.968753 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2273 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4115 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2504 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9415 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7836 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14183 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3406 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)    10375 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5695 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3695 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7020 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3797 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2514 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5127 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9090 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5881 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11780 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8234 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8221 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5840 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    19423 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3044 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8825 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5106 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    18472 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.968753 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mps/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3648 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3087 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2713 2023-06-29 08:38:24.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/nms.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1140 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/nms_quadri.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1975 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/nms_rotated.cpp
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.969753 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1144 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1817 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2643 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6080 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1637 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      968 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1921 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1178 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2855 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2794 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2936 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2262 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)     1110 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/pixel_group.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2248 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/points_in_boxes.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      615 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/points_in_polygons.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2278 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/prroi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2136 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/psamask.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    55203 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/pybind.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2344 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6733 2023-06-29 08:38:24.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roi_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2214 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1474 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roi_pool.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3707 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1663 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1909 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2325 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/scatter_points.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2290 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9567 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/spconv_ops.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2420 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/spconv_utils.h
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3202 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/sync_bn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1575 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/three_interpolate.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      729 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/three_nn.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      724 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/tin_shift.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5399 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/upfirdn2d.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9617 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/voxelization.cpp
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    17467 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/deform_conv.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7888 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/deform_roi_pool.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1583 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/deprecated_wrappers.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11369 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/diff_iou_rotated.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    17614 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/filtered_lrelu.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6633 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/focal_loss.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2588 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/furthest_point_sample.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10686 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/fused_bias_leakyrelu.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1682 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/gather_points.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10890 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/group_points.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      600 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/info.py
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)     8143 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/iou3d.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2653 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/knn.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4851 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/masked_conv.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6227 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/merge_cells.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      599 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/min_area_polygons.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14424 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/modulated_deform_conv.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    16768 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/multi_scale_deform_attn.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    19306 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/nms.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3378 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/pixel_group.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11857 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/point_sample.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5470 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/points_in_boxes.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1520 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/points_in_polygons.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6330 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/points_sampler.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5361 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/prroi_pool.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2992 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/psa_mask.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5082 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/riroi_align_rotated.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8324 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/roi_align.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7062 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/roi_align_rotated.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2867 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/roi_pool.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     4633 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/roiaware_pool3d.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3332 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/roipoint_pool3d.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3406 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/rotated_feature_align.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5908 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/saconv.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5886 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/scatter_points.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    14049 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sparse_conv.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6394 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sparse_functional.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     7243 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sparse_modules.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     6830 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sparse_ops.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3274 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sparse_pool.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2228 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sparse_structure.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    11519 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/sync_bn.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2240 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/three_interpolate.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1558 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/three_nn.py
+-rwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)     2426 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/tin_shift.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    17765 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/upfirdn2d.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     8039 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/ops/voxelize.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.970753 mmcv-lite-2.0.1/mmcv/transforms/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1382 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      986 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/base.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      103 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/builder.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3732 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/formatting.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    13176 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/loading.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    57971 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/processing.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     9372 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/utils.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    24709 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/transforms/wrappers.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.971753 mmcv-lite-2.0.1/mmcv/utils/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      388 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/utils/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      334 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/utils/device_type.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3311 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/utils/env.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2079 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/utils/ext_loader.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      922 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/utils/parrots_jit.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1208 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/version.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.971753 mmcv-lite-2.0.1/mmcv/video/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      570 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/video/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10254 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/video/io.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    10221 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/video/optflow.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5643 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/video/processing.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.972753 mmcv-lite-2.0.1/mmcv/visualization/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      338 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/visualization/__init__.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     1457 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/visualization/color.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     5674 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/visualization/image.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     3557 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/mmcv/visualization/optflow.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.974753 mmcv-lite-2.0.1/mmcv_lite.egg-info/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      824 2023-06-29 08:39:45.000000 mmcv-lite-2.0.1/mmcv_lite.egg-info/PKG-INFO
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    21536 2023-06-29 08:39:45.000000 mmcv-lite-2.0.1/mmcv_lite.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)        1 2023-06-29 08:39:45.000000 mmcv-lite-2.0.1/mmcv_lite.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)        1 2023-06-29 08:39:45.000000 mmcv-lite-2.0.1/mmcv_lite.egg-info/not-zip-safe
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      436 2023-06-29 08:39:45.000000 mmcv-lite-2.0.1/mmcv_lite.egg-info/requires.txt
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)        5 2023-06-29 08:39:45.000000 mmcv-lite-2.0.1/mmcv_lite.egg-info/top_level.txt
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.974753 mmcv-lite-2.0.1/requirements/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)       86 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/requirements/runtime.txt
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      633 2023-06-29 08:39:45.974753 mmcv-lite-2.0.1/setup.cfg
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)    20584 2023-06-29 08:39:02.000000 mmcv-lite-2.0.1/setup.py
+drwxrwxr-x   0 zhouzaida (900020515) zhouzaida (900020515)        0 2023-06-29 08:39:45.974753 mmcv-lite-2.0.1/tests/
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)     2199 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/tests/test_arraymisc.py
+-rw-rw-r--   0 zhouzaida (900020515) zhouzaida (900020515)      599 2023-06-29 08:37:35.000000 mmcv-lite-2.0.1/tests/test_visualization.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mmcv-lite-2.0.0rc4/LICENSE` & `mmcv-lite-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/PKG-INFO` & `mmcv-lite-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcv-lite
-Version: 2.0.0rc4
+Version: 2.0.1
 Summary: OpenMMLab Computer Vision Foundation
 Home-page: https://github.com/open-mmlab/mmcv
 Author: MMCV Contributors
 Author-email: openmmlab@gmail.com
 Keywords: computer vision
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/arraymisc/quantization.py` & `mmcv-lite-2.0.1/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/__init__.py` & `mmcv-lite-2.0.1/mmcv/cnn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,22 @@
                      HSigmoid, HSwish, Linear, MaxPool2d, MaxPool3d,
                      NonLocal1d, NonLocal2d, NonLocal3d, Scale, Swish,
                      build_activation_layer, build_conv_layer,
                      build_norm_layer, build_padding_layer, build_plugin_layer,
                      build_upsample_layer, conv_ws_2d, is_norm)
 # yapf: enable
 from .resnet import ResNet, make_res_layer
+from .rfsearch import Conv2dRFSearchOp, RFSearchHook
 from .utils import fuse_conv_bn, get_model_complexity_info
 from .vgg import VGG, make_vgg_layer
 
 __all__ = [
     'AlexNet', 'VGG', 'make_vgg_layer', 'ResNet', 'make_res_layer',
     'ConvModule', 'build_activation_layer', 'build_conv_layer',
     'build_norm_layer', 'build_padding_layer', 'build_upsample_layer',
     'build_plugin_layer', 'is_norm', 'NonLocal1d', 'NonLocal2d', 'NonLocal3d',
     'ContextBlock', 'HSigmoid', 'Swish', 'HSwish', 'GeneralizedAttention',
     'Scale', 'conv_ws_2d', 'ConvAWS2d', 'ConvWS2d',
     'DepthwiseSeparableConvModule', 'Linear', 'Conv2d', 'ConvTranspose2d',
     'MaxPool2d', 'ConvTranspose3d', 'MaxPool3d', 'Conv3d', 'fuse_conv_bn',
-    'get_model_complexity_info'
+    'get_model_complexity_info', 'Conv2dRFSearchOp', 'RFSearchHook'
 ]
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/alexnet.py` & `mmcv-lite-2.0.1/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/__init__.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/activation.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/context_block.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import inspect
 from typing import Dict, Optional
 
 from mmengine.registry import MODELS
 from torch import nn
 
 MODELS.register_module('Conv1d', module=nn.Conv1d)
 MODELS.register_module('Conv2d', module=nn.Conv2d)
@@ -31,15 +32,16 @@
         if not isinstance(cfg, dict):
             raise TypeError('cfg must be a dict')
         if 'type' not in cfg:
             raise KeyError('the cfg dict must contain the key "type"')
         cfg_ = cfg.copy()
 
     layer_type = cfg_.pop('type')
-
+    if inspect.isclass(layer_type):
+        return layer_type(*args, **kwargs, **cfg_)  # type: ignore
     # Switch registry to the target scope. If `conv_layer` cannot be found
     # in the registry, fallback to search `conv_layer` in the
     # mmengine.MODELS.
     with MODELS.switch_scope_and_registry(None) as registry:
         conv_layer = registry.get(layer_type)
     if conv_layer is None:
         raise KeyError(f'Cannot find {conv_layer} in registry under scope '
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv_module.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/conv_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,73 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import warnings
+from functools import partial
 from typing import Dict, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from mmengine.model import constant_init, kaiming_init
 from mmengine.registry import MODELS
 from mmengine.utils.dl_utils.parrots_wrapper import _BatchNorm, _InstanceNorm
 
 from .activation import build_activation_layer
 from .conv import build_conv_layer
 from .norm import build_norm_layer
 from .padding import build_padding_layer
 
 
+def fast_conv_bn_eval_forward(bn: _BatchNorm, conv: nn.modules.conv._ConvNd,
+                              x: torch.Tensor):
+    """
+    Implementation based on https://arxiv.org/abs/2305.11624
+    "Tune-Mode ConvBN Blocks For Efficient Transfer Learning"
+    It leverages the associative law between convolution and affine transform,
+    i.e., normalize (weight conv feature) = (normalize weight) conv feature.
+    It works for Eval mode of ConvBN blocks during validation, and can be used
+    for training as well. It reduces memory and computation cost.
+
+    Args:
+        bn (_BatchNorm): a BatchNorm module.
+        conv (nn._ConvNd): a conv module
+        x (torch.Tensor): Input feature map.
+    """
+    # These lines of code are designed to deal with various cases
+    # like bn without affine transform, and conv without bias
+    weight_on_the_fly = conv.weight
+    if conv.bias is not None:
+        bias_on_the_fly = conv.bias
+    else:
+        bias_on_the_fly = torch.zeros_like(bn.running_var)
+
+    if bn.weight is not None:
+        bn_weight = bn.weight
+    else:
+        bn_weight = torch.ones_like(bn.running_var)
+
+    if bn.bias is not None:
+        bn_bias = bn.bias
+    else:
+        bn_bias = torch.zeros_like(bn.running_var)
+
+    # shape of [C_out, 1, 1, 1] in Conv2d
+    weight_coeff = torch.rsqrt(bn.running_var +
+                               bn.eps).reshape([-1] + [1] *
+                                               (len(conv.weight.shape) - 1))
+    # shape of [C_out, 1, 1, 1] in Conv2d
+    coefff_on_the_fly = bn_weight.view_as(weight_coeff) * weight_coeff
+
+    # shape of [C_out, C_in, k, k] in Conv2d
+    weight_on_the_fly = weight_on_the_fly * coefff_on_the_fly
+    # shape of [C_out] in Conv2d
+    bias_on_the_fly = bn_bias + coefff_on_the_fly.flatten() *\
+        (bias_on_the_fly - bn.running_mean)
+
+    return conv._conv_forward(x, weight_on_the_fly, bias_on_the_fly)
+
+
 @MODELS.register_module()
 class ConvModule(nn.Module):
     """A conv block that bundles conv/norm/activation layers.
 
     This block simplifies the usage of convolution layers, which are commonly
     used with a norm layer (e.g., BatchNorm) and activation layer (e.g., ReLU).
     It is based upon three build methods: `build_conv_layer()`,
@@ -61,14 +111,17 @@
             instead. Currently, we support ['zeros', 'circular'] with official
             implementation and ['reflect'] with our own implementation.
             Default: 'zeros'.
         order (tuple[str]): The order of conv/norm/activation layers. It is a
             sequence of "conv", "norm" and "act". Common examples are
             ("conv", "norm", "act") and ("act", "conv", "norm").
             Default: ('conv', 'norm', 'act').
+        fast_conv_bn_eval (bool): Whether use fast conv when the consecutive
+            bn is in eval mode (either training or testing), as proposed in
+            https://arxiv.org/abs/2305.11624 . Default: False.
     """
 
     _abbr_ = 'conv_block'
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
@@ -80,15 +133,16 @@
                  bias: Union[bool, str] = 'auto',
                  conv_cfg: Optional[Dict] = None,
                  norm_cfg: Optional[Dict] = None,
                  act_cfg: Optional[Dict] = dict(type='ReLU'),
                  inplace: bool = True,
                  with_spectral_norm: bool = False,
                  padding_mode: str = 'zeros',
-                 order: tuple = ('conv', 'norm', 'act')):
+                 order: tuple = ('conv', 'norm', 'act'),
+                 fast_conv_bn_eval: bool = False):
         super().__init__()
         assert conv_cfg is None or isinstance(conv_cfg, dict)
         assert norm_cfg is None or isinstance(norm_cfg, dict)
         assert act_cfg is None or isinstance(act_cfg, dict)
         official_padding_mode = ['zeros', 'circular']
         self.conv_cfg = conv_cfg
         self.norm_cfg = norm_cfg
@@ -151,14 +205,16 @@
             if self.with_bias:
                 if isinstance(norm, (_BatchNorm, _InstanceNorm)):
                     warnings.warn(
                         'Unnecessary conv bias before batch/instance norm')
         else:
             self.norm_name = None  # type: ignore
 
+        self.turn_on_fast_conv_bn_eval(fast_conv_bn_eval)
+
         # build activation layer
         if self.with_activation:
             act_cfg_ = act_cfg.copy()  # type: ignore
             # nn.Tanh has no 'inplace' argument
             if act_cfg_['type'] not in [
                     'Tanh', 'PReLU', 'Sigmoid', 'HSigmoid', 'Swish', 'GELU'
             ]:
@@ -196,17 +252,85 @@
         if self.with_norm:
             constant_init(self.norm, 1, bias=0)
 
     def forward(self,
                 x: torch.Tensor,
                 activate: bool = True,
                 norm: bool = True) -> torch.Tensor:
-        for layer in self.order:
+        layer_index = 0
+        while layer_index < len(self.order):
+            layer = self.order[layer_index]
             if layer == 'conv':
                 if self.with_explicit_padding:
                     x = self.padding_layer(x)
-                x = self.conv(x)
+                # if the next operation is norm and we have a norm layer in
+                # eval mode and we have enabled fast_conv_bn_eval for the conv
+                # operator, then activate the optimized forward and skip the
+                # next norm operator since it has been fused
+                if layer_index + 1 < len(self.order) and \
+                        self.order[layer_index + 1] == 'norm' and norm and \
+                        self.with_norm and not self.norm.training and \
+                        self.fast_conv_bn_eval_forward is not None:
+                    self.conv.forward = partial(self.fast_conv_bn_eval_forward,
+                                                self.norm, self.conv)
+                    layer_index += 1
+                    x = self.conv(x)
+                    del self.conv.forward
+                else:
+                    x = self.conv(x)
             elif layer == 'norm' and norm and self.with_norm:
                 x = self.norm(x)
             elif layer == 'act' and activate and self.with_activation:
                 x = self.activate(x)
+            layer_index += 1
         return x
+
+    def turn_on_fast_conv_bn_eval(self, fast_conv_bn_eval=True):
+        # fast_conv_bn_eval works for conv + bn
+        # with `track_running_stats` option
+        if fast_conv_bn_eval and self.norm \
+                            and isinstance(self.norm, _BatchNorm) \
+                            and self.norm.track_running_stats:
+            self.fast_conv_bn_eval_forward = fast_conv_bn_eval_forward
+        else:
+            self.fast_conv_bn_eval_forward = None  # type: ignore
+
+    @staticmethod
+    def create_from_conv_bn(conv: torch.nn.modules.conv._ConvNd,
+                            bn: torch.nn.modules.batchnorm._BatchNorm,
+                            fast_conv_bn_eval=True) -> 'ConvModule':
+        """Create a ConvModule from a conv and a bn module."""
+        self = ConvModule.__new__(ConvModule)
+        super(ConvModule, self).__init__()
+
+        self.conv_cfg = None
+        self.norm_cfg = None
+        self.act_cfg = None
+        self.inplace = False
+        self.with_spectral_norm = False
+        self.with_explicit_padding = False
+        self.order = ('conv', 'norm', 'act')
+
+        self.with_norm = True
+        self.with_activation = False
+        self.with_bias = conv.bias is not None
+
+        # build convolution layer
+        self.conv = conv
+        # export the attributes of self.conv to a higher level for convenience
+        self.in_channels = self.conv.in_channels
+        self.out_channels = self.conv.out_channels
+        self.kernel_size = self.conv.kernel_size
+        self.stride = self.conv.stride
+        self.padding = self.conv.padding
+        self.dilation = self.conv.dilation
+        self.transposed = self.conv.transposed
+        self.output_padding = self.conv.output_padding
+        self.groups = self.conv.groups
+
+        # build normalization layers
+        self.norm_name, norm = 'bn', bn
+        self.add_module(self.norm_name, norm)
+
+        self.turn_on_fast_conv_bn_eval(fast_conv_bn_eval)
+
+        return self
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/conv_ws.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/drop.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/generalized_attention.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/generalized_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 @MODELS.register_module()
 class GeneralizedAttention(nn.Module):
     """GeneralizedAttention module.
 
     See 'An Empirical Study of Spatial Attention Mechanisms in Deep Networks'
-    (https://arxiv.org/abs/1711.07971) for details.
+    (https://arxiv.org/abs/1904.05873) for details.
 
     Args:
         in_channels (int): Channels of the input feature map.
         spatial_range (int): The spatial range. -1 indicates no spatial range
             constraint. Default: -1.
         num_heads (int): The head number of empirical_attention module.
             Default: 9.
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/hsigmoid.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/hswish.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/non_local.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/norm.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/norm.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,30 +94,33 @@
         raise TypeError('cfg must be a dict')
     if 'type' not in cfg:
         raise KeyError('the cfg dict must contain the key "type"')
     cfg_ = cfg.copy()
 
     layer_type = cfg_.pop('type')
 
-    # Switch registry to the target scope. If `norm_layer` cannot be found
-    # in the registry, fallback to search `norm_layer` in the
-    # mmengine.MODELS.
-    with MODELS.switch_scope_and_registry(None) as registry:
-        norm_layer = registry.get(layer_type)
-    if norm_layer is None:
-        raise KeyError(f'Cannot find {norm_layer} in registry under scope '
-                       f'name {registry.scope}')
+    if inspect.isclass(layer_type):
+        norm_layer = layer_type
+    else:
+        # Switch registry to the target scope. If `norm_layer` cannot be found
+        # in the registry, fallback to search `norm_layer` in the
+        # mmengine.MODELS.
+        with MODELS.switch_scope_and_registry(None) as registry:
+            norm_layer = registry.get(layer_type)
+        if norm_layer is None:
+            raise KeyError(f'Cannot find {norm_layer} in registry under '
+                           f'scope name {registry.scope}')
     abbr = infer_abbr(norm_layer)
 
     assert isinstance(postfix, (int, str))
     name = abbr + str(postfix)
 
     requires_grad = cfg_.pop('requires_grad', True)
     cfg_.setdefault('eps', 1e-5)
-    if layer_type != 'GN':
+    if norm_layer is not nn.GroupNorm:
         layer = norm_layer(num_features, **cfg_)
         if layer_type == 'SyncBN' and hasattr(layer, '_specify_ddp_gpu_num'):
             layer._specify_ddp_gpu_num(1)
     else:
         assert 'num_groups' in cfg_
         layer = norm_layer(num_channels=num_features, **cfg_)
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/padding.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/padding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import inspect
 from typing import Dict
 
 import torch.nn as nn
 from mmengine.registry import MODELS
 
 MODELS.register_module('zero', module=nn.ZeroPad2d)
 MODELS.register_module('reflect', module=nn.ReflectionPad2d)
@@ -23,15 +24,16 @@
     if not isinstance(cfg, dict):
         raise TypeError('cfg must be a dict')
     if 'type' not in cfg:
         raise KeyError('the cfg dict must contain the key "type"')
 
     cfg_ = cfg.copy()
     padding_type = cfg_.pop('type')
-
+    if inspect.isclass(padding_type):
+        return padding_type(*args, **kwargs, **cfg_)
     # Switch registry to the target scope. If `padding_layer` cannot be found
     # in the registry, fallback to search `padding_layer` in the
     # mmengine.MODELS.
     with MODELS.switch_scope_and_registry(None) as registry:
         padding_layer = registry.get(padding_type)
     if padding_layer is None:
         raise KeyError(f'Cannot find {padding_layer} in registry under scope '
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/plugin.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,23 +75,26 @@
     if not isinstance(cfg, dict):
         raise TypeError('cfg must be a dict')
     if 'type' not in cfg:
         raise KeyError('the cfg dict must contain the key "type"')
     cfg_ = cfg.copy()
 
     layer_type = cfg_.pop('type')
-
-    # Switch registry to the target scope. If `plugin_layer` cannot be found
-    # in the registry, fallback to search `plugin_layer` in the
-    # mmengine.MODELS.
-    with MODELS.switch_scope_and_registry(None) as registry:
-        plugin_layer = registry.get(layer_type)
-    if plugin_layer is None:
-        raise KeyError(f'Cannot find {plugin_layer} in registry under scope '
-                       f'name {registry.scope}')
+    if inspect.isclass(layer_type):
+        plugin_layer = layer_type
+    else:
+        # Switch registry to the target scope. If `plugin_layer` cannot be
+        # found in the registry, fallback to search `plugin_layer` in the
+        # mmengine.MODELS.
+        with MODELS.switch_scope_and_registry(None) as registry:
+            plugin_layer = registry.get(layer_type)
+        if plugin_layer is None:
+            raise KeyError(
+                f'Cannot find {plugin_layer} in registry under scope '
+                f'name {registry.scope}')
     abbr = infer_abbr(plugin_layer)
 
     assert isinstance(postfix, (int, str))
     name = abbr + str(postfix)
 
     layer = plugin_layer(**kwargs, **cfg_)
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/scale.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/transformer.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/upsample.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/upsample.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import inspect
 from typing import Dict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from mmengine.model import xavier_init
 from mmengine.registry import MODELS
@@ -72,19 +73,22 @@
     if 'type' not in cfg:
         raise KeyError(
             f'the cfg dict must contain the key "type", but got {cfg}')
     cfg_ = cfg.copy()
 
     layer_type = cfg_.pop('type')
 
+    if inspect.isclass(layer_type):
+        upsample = layer_type
     # Switch registry to the target scope. If `upsample` cannot be found
     # in the registry, fallback to search `upsample` in the
     # mmengine.MODELS.
-    with MODELS.switch_scope_and_registry(None) as registry:
-        upsample = registry.get(layer_type)
-    if upsample is None:
-        raise KeyError(f'Cannot find {upsample} in registry under scope '
-                       f'name {registry.scope}')
-    if upsample is nn.Upsample:
-        cfg_['mode'] = layer_type
+    else:
+        with MODELS.switch_scope_and_registry(None) as registry:
+            upsample = registry.get(layer_type)
+        if upsample is None:
+            raise KeyError(f'Cannot find {upsample} in registry under scope '
+                           f'name {registry.scope}')
+        if upsample is nn.Upsample:
+            cfg_['mode'] = layer_type
     layer = upsample(*args, **kwargs, **cfg_)
     return layer
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/bricks/wrappers.py` & `mmcv-lite-2.0.1/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/resnet.py` & `mmcv-lite-2.0.1/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/utils/flops_counter.py` & `mmcv-lite-2.0.1/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/utils/fuse_conv_bn.py` & `mmcv-lite-2.0.1/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/cnn/vgg.py` & `mmcv-lite-2.0.1/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/image/__init__.py` & `mmcv-lite-2.0.1/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/image/colorspace.py` & `mmcv-lite-2.0.1/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/image/geometric.py` & `mmcv-lite-2.0.1/mmcv/image/geometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     from PIL import Image
 except ImportError:
     Image = None
 
 
 def _scale_size(
     size: Tuple[int, int],
-    scale: Union[float, int, tuple],
+    scale: Union[float, int, Tuple[float, float], Tuple[int, int]],
 ) -> Tuple[int, int]:
     """Rescale a size by a ratio.
 
     Args:
         size (tuple[int]): (w, h).
-        scale (float | tuple(float)): Scaling factor.
+        scale (float | int | tuple(float) | tuple(int)): Scaling factor.
 
     Returns:
         tuple[int]: scaled size.
     """
     if isinstance(scale, (float, int)):
         scale = (scale, scale)
     w, h = size
@@ -124,15 +124,16 @@
 
 
 @no_type_check
 def imresize_to_multiple(
     img: np.ndarray,
     divisor: Union[int, Tuple[int, int]],
     size: Union[int, Tuple[int, int], None] = None,
-    scale_factor: Union[float, Tuple[float, float], None] = None,
+    scale_factor: Union[float, int, Tuple[float, float], Tuple[int, int],
+                        None] = None,
     keep_ratio: bool = False,
     return_scale: bool = False,
     interpolation: str = 'bilinear',
     out: Optional[np.ndarray] = None,
     backend: Optional[str] = None
 ) -> Union[Tuple[np.ndarray, float, float], np.ndarray]:
     """Resize image according to a given size or scale factor and then rounds
@@ -141,17 +142,18 @@
 
     Args:
         img (ndarray): The input image.
         divisor (int | tuple): Resized image size will be a multiple of
             divisor. If divisor is a tuple, divisor should be
             (w_divisor, h_divisor).
         size (None | int | tuple[int]): Target size (w, h). Default: None.
-        scale_factor (None | float | tuple[float]): Multiplier for spatial
-            size. Should match input size if it is a tuple and the 2D style is
-            (w_scale_factor, h_scale_factor). Default: None.
+        scale_factor (None | float | int | tuple[float] | tuple[int]):
+            Multiplier for spatial size. Should match input size if it is a
+            tuple and the 2D style is (w_scale_factor, h_scale_factor).
+            Default: None.
         keep_ratio (bool): Whether to keep the aspect ratio when resizing the
             image. Default: False.
         return_scale (bool): Whether to return `w_scale` and `h_scale`.
         interpolation (str): Interpolation method, accepted values are
             "nearest", "bilinear", "bicubic", "area", "lanczos" for 'cv2'
             backend, "nearest", "bilinear" for 'pillow' backend.
         out (ndarray): The output destination.
@@ -211,24 +213,24 @@
         `resized_img`.
     """
     h, w = dst_img.shape[:2]
     return imresize(img, (w, h), return_scale, interpolation, backend=backend)
 
 
 def rescale_size(old_size: tuple,
-                 scale: Union[float, int, tuple],
+                 scale: Union[float, int, Tuple[int, int]],
                  return_scale: bool = False) -> tuple:
     """Calculate the new size to be rescaled to.
 
     Args:
         old_size (tuple[int]): The old size (w, h) of image.
-        scale (float | tuple[int]): The scaling factor or maximum size.
-            If it is a float number, then the image will be rescaled by this
-            factor, else if it is a tuple of 2 integers, then the image will
-            be rescaled as large as possible within the scale.
+        scale (float | int | tuple[int]): The scaling factor or maximum size.
+            If it is a float number or an integer, then the image will be
+            rescaled by this factor, else if it is a tuple of 2 integers, then
+            the image will be rescaled as large as possible within the scale.
         return_scale (bool): Whether to return the scaling factor besides the
             rescaled image size.
 
     Returns:
         tuple[int]: The new rescaled image size.
     """
     w, h = old_size
@@ -251,27 +253,27 @@
         return new_size, scale_factor
     else:
         return new_size
 
 
 def imrescale(
     img: np.ndarray,
-    scale: Union[float, Tuple[int, int]],
+    scale: Union[float, int, Tuple[int, int]],
     return_scale: bool = False,
     interpolation: str = 'bilinear',
     backend: Optional[str] = None
 ) -> Union[np.ndarray, Tuple[np.ndarray, float]]:
     """Resize image while keeping the aspect ratio.
 
     Args:
         img (ndarray): The input image.
-        scale (float | tuple[int]): The scaling factor or maximum size.
-            If it is a float number, then the image will be rescaled by this
-            factor, else if it is a tuple of 2 integers, then the image will
-            be rescaled as large as possible within the scale.
+        scale (float | int | tuple[int]): The scaling factor or maximum size.
+            If it is a float number or an integer, then the image will be
+            rescaled by this factor, else if it is a tuple of 2 integers, then
+            the image will be rescaled as large as possible within the scale.
         return_scale (bool): Whether to return the scaling factor besides the
             rescaled image.
         interpolation (str): Same as :func:`resize`.
         backend (str | None): Same as :func:`resize`.
 
     Returns:
         ndarray: The rescaled image.
@@ -436,15 +438,15 @@
 
     3 steps: scale the bboxes -> clip bboxes -> crop and pad.
 
     Args:
         img (ndarray): Image to be cropped.
         bboxes (ndarray): Shape (k, 4) or (4, ), location of cropped bboxes.
         scale (float, optional): Scale ratio of bboxes, the default value
-            1.0 means no padding.
+            1.0 means no scaling.
         pad_fill (Number | list[Number]): Value to be filled for padding.
             Default: None, which means no padding.
 
     Returns:
         list[ndarray] | ndarray: The cropped image patches.
     """
     chn = 1 if img.ndim == 2 else img.shape[2]
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/image/io.py` & `mmcv-lite-2.0.1/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/image/misc.py` & `mmcv-lite-2.0.1/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/image/photometric.py` & `mmcv-lite-2.0.1/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/__init__.py` & `mmcv-lite-2.0.1/mmcv/ops/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .active_rotated_filter import active_rotated_filter
 from .assign_score_withk import assign_score_withk
 from .ball_query import ball_query
 from .bbox import bbox_overlaps
 from .bezier_align import BezierAlign, bezier_align
+from .bias_act import bias_act
 from .border_align import BorderAlign, border_align
 from .box_iou_quadri import box_iou_quadri
 from .box_iou_rotated import box_iou_rotated
 from .carafe import CARAFE, CARAFENaive, CARAFEPack, carafe, carafe_naive
 from .cc_attention import CrissCrossAttention
 from .chamfer_distance import chamfer_distance
 from .contour_expand import contour_expand
+from .conv2d_gradfix import conv2d, conv_transpose2d
 from .convex_iou import convex_giou, convex_iou
 from .corner_pool import CornerPool
 from .correlation import Correlation
 from .deform_conv import DeformConv2d, DeformConv2dPack, deform_conv2d
 from .deform_roi_pool import (DeformRoIPool, DeformRoIPoolPack,
                               ModulatedDeformRoIPoolPack, deform_roi_pool)
 from .deprecated_wrappers import Conv2d_deprecated as Conv2d
 from .deprecated_wrappers import ConvTranspose2d_deprecated as ConvTranspose2d
 from .deprecated_wrappers import Linear_deprecated as Linear
 from .deprecated_wrappers import MaxPool2d_deprecated as MaxPool2d
 from .diff_iou_rotated import diff_iou_rotated_2d, diff_iou_rotated_3d
+from .filtered_lrelu import filtered_lrelu
 from .focal_loss import (SigmoidFocalLoss, SoftmaxFocalLoss,
                          sigmoid_focal_loss, softmax_focal_loss)
 from .furthest_point_sample import (furthest_point_sample,
                                     furthest_point_sample_with_dist)
 from .fused_bias_leakyrelu import FusedBiasLeakyReLU, fused_bias_leakyrelu
 from .gather_points import gather_points
 from .group_points import GroupAll, QueryAndGroup, grouping_operation
@@ -64,15 +67,15 @@
 from .sparse_modules import SparseModule, SparseSequential
 from .sparse_pool import SparseMaxPool2d, SparseMaxPool3d
 from .sparse_structure import SparseConvTensor, scatter_nd
 from .sync_bn import SyncBatchNorm
 from .three_interpolate import three_interpolate
 from .three_nn import three_nn
 from .tin_shift import TINShift, tin_shift
-from .upfirdn2d import upfirdn2d
+from .upfirdn2d import filter2d, upfirdn2d, upsample2d
 from .voxelize import Voxelization, voxelization
 
 __all__ = [
     'bbox_overlaps', 'CARAFE', 'CARAFENaive', 'CARAFEPack', 'carafe',
     'carafe_naive', 'CornerPool', 'DeformConv2d', 'DeformConv2dPack',
     'deform_conv2d', 'DeformRoIPool', 'DeformRoIPoolPack',
     'ModulatedDeformRoIPoolPack', 'deform_roi_pool', 'SigmoidFocalLoss',
@@ -99,9 +102,10 @@
     'SparseConv3d', 'SparseConvTranspose2d', 'SparseConvTranspose3d',
     'SparseInverseConv2d', 'SparseInverseConv3d', 'SubMConv2d', 'SubMConv3d',
     'SparseModule', 'SparseSequential', 'SparseMaxPool2d', 'SparseMaxPool3d',
     'SparseConvTensor', 'scatter_nd', 'points_in_boxes_part',
     'points_in_boxes_cpu', 'points_in_boxes_all', 'points_in_polygons',
     'min_area_polygons', 'active_rotated_filter', 'convex_iou', 'convex_giou',
     'diff_iou_rotated_2d', 'diff_iou_rotated_3d', 'chamfer_distance',
-    'PrRoIPool', 'prroi_pool', 'BezierAlign', 'bezier_align'
+    'PrRoIPool', 'prroi_pool', 'bias_act', 'filtered_lrelu', 'conv2d',
+    'conv_transpose2d', 'filter2d', 'upsample2d', 'BezierAlign', 'bezier_align'
 ]
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/active_rotated_filter.py` & `mmcv-lite-2.0.1/mmcv/ops/active_rotated_filter.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/assign_score_withk.py` & `mmcv-lite-2.0.1/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/ball_query.py` & `mmcv-lite-2.0.1/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/bbox.py` & `mmcv-lite-2.0.1/mmcv/ops/bbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,29 +102,25 @@
     # Either the boxes are empty or the length of boxes' last dimension is 4
     assert (bboxes1.size(-1) == 4 or bboxes1.size(0) == 0)
     assert (bboxes2.size(-1) == 4 or bboxes2.size(0) == 0)
     assert offset == 1 or offset == 0
 
     rows = bboxes1.size(0)
     cols = bboxes2.size(0)
+
     if aligned:
         assert rows == cols
+        ious = bboxes1.new_zeros(rows)
+    else:
+        ious = bboxes1.new_zeros((rows, cols))
 
     if rows * cols == 0:
-        return bboxes1.new(rows, 1) if aligned else bboxes1.new(rows, cols)
+        return ious
 
-    if bboxes1.device.type == 'cpu':
+    if bboxes1.device.type == 'cpu' and torch.__version__ == 'parrots':
         return _bbox_overlaps_cpu(
             bboxes1, bboxes2, mode=mode, aligned=aligned, offset=offset)
-    else:
-        if aligned:
-            ious = bboxes1.new_zeros(rows)
-        else:
-            ious = bboxes1.new_zeros((rows, cols))
-        ext_module.bbox_overlaps(
-            bboxes1,
-            bboxes2,
-            ious,
-            mode=mode_flag,
-            aligned=aligned,
-            offset=offset)
-        return ious
+
+    ext_module.bbox_overlaps(
+        bboxes1, bboxes2, ious, mode=mode_flag, aligned=aligned, offset=offset)
+
+    return ious
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/bezier_align.py` & `mmcv-lite-2.0.1/mmcv/ops/bezier_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/border_align.py` & `mmcv-lite-2.0.1/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/box_iou_quadri.py` & `mmcv-lite-2.0.1/mmcv/ops/box_iou_quadri.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/box_iou_rotated.py` & `mmcv-lite-2.0.1/mmcv/ops/box_iou_rotated.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,18 @@
     mode_dict = {'iou': 0, 'iof': 1}
     mode_flag = mode_dict[mode]
     rows = bboxes1.size(0)
     cols = bboxes2.size(0)
     if aligned:
         ious = bboxes1.new_zeros(rows)
     else:
-        ious = bboxes1.new_zeros(rows * cols)
+        if bboxes1.device.type == 'mlu':
+            ious = bboxes1.new_zeros([rows, cols])
+        else:
+            ious = bboxes1.new_zeros(rows * cols)
     if not clockwise:
         flip_mat = bboxes1.new_ones(bboxes1.shape[-1])
         flip_mat[-1] = -1
         bboxes1 = bboxes1 * flip_mat
         bboxes2 = bboxes2 * flip_mat
     bboxes1 = bboxes1.contiguous()
     bboxes2 = bboxes2.contiguous()
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/carafe.py` & `mmcv-lite-2.0.1/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/cc_attention.py` & `mmcv-lite-2.0.1/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/chamfer_distance.py` & `mmcv-lite-2.0.1/mmcv/ops/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/contour_expand.py` & `mmcv-lite-2.0.1/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/convex_iou.py` & `mmcv-lite-2.0.1/mmcv/ops/convex_iou.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/corner_pool.py` & `mmcv-lite-2.0.1/mmcv/ops/corner_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch
+from mmengine.utils import digit_version
 from torch import Tensor, nn
 
 _mode_dict = {'top': 0, 'bottom': 1, 'left': 2, 'right': 3}
 
 
 def _corner_pool(x: Tensor, dim: int, flip: bool) -> Tensor:
     size = x.size(dim)
@@ -66,15 +67,16 @@
 
     def __init__(self, mode: str):
         super().__init__()
         assert mode in self.cummax_dim_flip
         self.mode = mode
 
     def forward(self, x: Tensor) -> Tensor:
-        if torch.__version__ != 'parrots' and torch.__version__ >= '1.5.0':
+        if (torch.__version__ != 'parrots' and
+                digit_version(torch.__version__) >= digit_version('1.5.0')):
             dim, flip = self.cummax_dim_flip[self.mode]
             if flip:
                 x = x.flip(dim)
             pool_tensor, _ = torch.cummax(x, dim=dim)
             if flip:
                 pool_tensor = pool_tensor.flip(dim)
             return pool_tensor
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/correlation.py` & `mmcv-lite-2.0.1/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 template <>
 __device__ __forceinline__ phalf warpReduceSum(phalf val) {
   for (int offset = WARP_SIZE / 2; offset > 0; offset /= 2)
 #ifdef MMCV_WITH_HIP
     __PHALF(val) += __shfl_down(val, offset);
 #else
     __PHALF(val) +=
-        __shfl_down_sync(FULL_MASK, static_cast<__half>(__PHALF(val)), offset);
+        __shfl_down_sync(FULL_MASK, __PHALF(val).operator __half(), offset);
 #endif
   return val;
 }
 
 // Splits the original matrix into submatrices with size 32 * 32.
 // Each block transposes one submatrix by loading it into shared memory.
 // Reference https://devblogs.nvidia.com/efficient-matrix-transpose-cuda-cc/
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/spconv/indice.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/spconv/indice.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSDevice.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSDevice.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSLibrary.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSLibrary.mm` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.mm`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSStream.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSStream.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/mps/MPSUtils.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/mps/MPSUtils.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/parrots_cpp_helper.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/parrots_cpp_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/parrots_cuda_helper.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/parrots_cuda_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_device_registry.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_device_registry.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/pytorch_npu_helper.hpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/pytorch_npu_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/prettyprint.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/prettyprint.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/active_rotated_filter.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/assign_score_withk.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ball_query._parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ball_query._parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ball_query.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/bbox_overlaps.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/border_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/border_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/border_align_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/border_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/border_align_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/border_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/box_iou_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_naive.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_naive.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/carafe_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/carafe_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/chamfer_distance.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/contour_expand.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/contour_expand.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/convex_iou.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/convex_iou.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/correlation.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/correlation.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/correlation_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/correlation_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/correlation_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/correlation_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/cudabind.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/cudabind.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -560,65 +560,14 @@
                                 Tensor grad_points);
 
 REGISTER_DEVICE_IMPL(group_points_forward_impl, CUDA,
                      group_points_forward_cuda);
 REGISTER_DEVICE_IMPL(group_points_backward_impl, CUDA,
                      group_points_backward_cuda);
 
-void IoU3DBoxesOverlapBevForwardCUDAKernelLauncher(const int num_a,
-                                                   const Tensor boxes_a,
-                                                   const int num_b,
-                                                   const Tensor boxes_b,
-                                                   Tensor ans_overlap);
-
-void IoU3DNMS3DForwardCUDAKernelLauncher(const Tensor boxes, Tensor& keep,
-                                         Tensor& keep_num,
-                                         float nms_overlap_thresh);
-
-void IoU3DNMS3DNormalForwardCUDAKernelLauncher(const Tensor boxes, Tensor& keep,
-                                               Tensor& keep_num,
-                                               float nms_overlap_thresh);
-
-void iou3d_boxes_overlap_bev_forward_cuda(const int num_a, const Tensor boxes_a,
-                                          const int num_b, const Tensor boxes_b,
-                                          Tensor ans_overlap) {
-  IoU3DBoxesOverlapBevForwardCUDAKernelLauncher(num_a, boxes_a, num_b, boxes_b,
-                                                ans_overlap);
-};
-
-void iou3d_nms3d_forward_cuda(const Tensor boxes, Tensor& keep,
-                              Tensor& keep_num, float nms_overlap_thresh) {
-  IoU3DNMS3DForwardCUDAKernelLauncher(boxes, keep, keep_num,
-                                      nms_overlap_thresh);
-};
-
-void iou3d_nms3d_normal_forward_cuda(const Tensor boxes, Tensor& keep,
-                                     Tensor& keep_num,
-                                     float nms_overlap_thresh) {
-  IoU3DNMS3DNormalForwardCUDAKernelLauncher(boxes, keep, keep_num,
-                                            nms_overlap_thresh);
-};
-
-void iou3d_boxes_overlap_bev_forward_impl(const int num_a, const Tensor boxes_a,
-                                          const int num_b, const Tensor boxes_b,
-                                          Tensor ans_overlap);
-
-void iou3d_nms3d_forward_impl(const Tensor boxes, Tensor& keep,
-                              Tensor& keep_num, float nms_overlap_thresh);
-
-void iou3d_nms3d_normal_forward_impl(const Tensor boxes, Tensor& keep,
-                                     Tensor& keep_num,
-                                     float nms_overlap_thresh);
-
-REGISTER_DEVICE_IMPL(iou3d_boxes_overlap_bev_forward_impl, CUDA,
-                     iou3d_boxes_overlap_bev_forward_cuda);
-REGISTER_DEVICE_IMPL(iou3d_nms3d_forward_impl, CUDA, iou3d_nms3d_forward_cuda);
-REGISTER_DEVICE_IMPL(iou3d_nms3d_normal_forward_impl, CUDA,
-                     iou3d_nms3d_normal_forward_cuda);
-
 void KNNForwardCUDAKernelLauncher(int b, int n, int m, int nsample,
                                   const Tensor xyz, const Tensor new_xyz,
                                   Tensor idx, Tensor dist2);
 
 void knn_forward_cuda(int b, int n, int m, int nsample, const Tensor xyz,
                       const Tensor new_xyz, Tensor idx, Tensor dist2) {
   KNNForwardCUDAKernelLauncher(b, n, m, nsample, xyz, new_xyz, idx, dist2);
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_conv.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_conv_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_conv_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_roi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/focal_loss.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/focal_loss.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/focal_loss_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/focal_loss_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/furthest_point_sample.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/gather_points.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/gather_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/gather_points_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/gather_points_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/gather_points_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/gather_points_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/group_points.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/group_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/group_points_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/group_points_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/group_points_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/group_points_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/info.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/info.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/iou3d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/iou3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/iou3d_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/iou3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/iou3d_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/iou3d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/knn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/knn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/knn_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/knn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/masked_conv2d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ms_deform_attn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/nms_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/pixel_group.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_boxes.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_polygons.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/prroi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/prroi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/psamask.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/psamask_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/psamask_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/psamask_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/psamask_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roi_pool_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/rotated_feature_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/sync_bn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/sync_bn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/sync_bn_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/sync_bn_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_interpolate.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_nn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_nn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/three_nn_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/three_nn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/tin_shift.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/tin_shift.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/upfirdn2d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/voxelization.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/voxelization_parrots.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/voxelization_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/parrots/voxelization_pytorch.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/parrots/voxelization_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/assign_score_withk.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/assign_score_withk.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/ball_query.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/bezier_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/bezier_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/border_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/border_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/carafe.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/carafe.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/carafe_naive.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/carafe_naive.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/chamfer_distance.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/contour_expand.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/contour_expand.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/convex_iou.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/convex_iou.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/correlation.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/correlation.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/nms.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/psamask.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 
 void AssignScoreWithKForwardCUDAKernelLauncher(
     int B, int N0, int N1, int M, int K, int O, int aggregate,
-    const Tensor& points, const Tensor& centers, const Tensor& scores,
-    const Tensor& knn_idx, Tensor& output);
+    const Tensor &points, const Tensor &centers, const Tensor &scores,
+    const Tensor &knn_idx, Tensor &output);
 
 void AssignScoreWithKBackwardCUDAKernelLauncher(
     int B, int N0, int N1, int M, int K, int O, int aggregate,
-    const Tensor& grad_out, const Tensor& points, const Tensor& centers,
-    const Tensor& scores, const Tensor& knn_idx, Tensor& grad_points,
-    Tensor& grad_centers, Tensor& grad_scores);
+    const Tensor &grad_out, const Tensor &points, const Tensor &centers,
+    const Tensor &scores, const Tensor &knn_idx, Tensor &grad_points,
+    Tensor &grad_centers, Tensor &grad_scores);
 
 void assign_score_withk_forward_cuda(int B, int N0, int N1, int M, int K, int O,
-                                     int aggregate, const Tensor& points,
-                                     const Tensor& centers,
-                                     const Tensor& scores,
-                                     const Tensor& knn_idx, Tensor& output) {
+                                     int aggregate, const Tensor &points,
+                                     const Tensor &centers,
+                                     const Tensor &scores,
+                                     const Tensor &knn_idx, Tensor &output) {
   AssignScoreWithKForwardCUDAKernelLauncher(
       B, N0, N1, M, K, O, aggregate, points, centers, scores, knn_idx, output);
 };
 
 void assign_score_withk_backward_cuda(
     int B, int N0, int N1, int M, int K, int O, int aggregate,
-    const Tensor& grad_out, const Tensor& points, const Tensor& centers,
-    const Tensor& scores, const Tensor& knn_idx, Tensor& grad_points,
-    Tensor& grad_centers, Tensor& grad_scores) {
+    const Tensor &grad_out, const Tensor &points, const Tensor &centers,
+    const Tensor &scores, const Tensor &knn_idx, Tensor &grad_points,
+    Tensor &grad_centers, Tensor &grad_scores) {
   AssignScoreWithKBackwardCUDAKernelLauncher(
       B, N0, N1, M, K, O, aggregate, grad_out, points, centers, scores, knn_idx,
       grad_points, grad_centers, grad_scores);
 };
 
 void assign_score_withk_forward_impl(int B, int N0, int N1, int M, int K, int O,
-                                     int aggregate, const Tensor& points,
-                                     const Tensor& centers,
-                                     const Tensor& scores,
-                                     const Tensor& knn_idx, Tensor& output);
+                                     int aggregate, const Tensor &points,
+                                     const Tensor &centers,
+                                     const Tensor &scores,
+                                     const Tensor &knn_idx, Tensor &output);
 
 void assign_score_withk_backward_impl(
     int B, int N0, int N1, int M, int K, int O, int aggregate,
-    const Tensor& grad_out, const Tensor& points, const Tensor& centers,
-    const Tensor& scores, const Tensor& knn_idx, Tensor& grad_points,
-    Tensor& grad_centers, Tensor& grad_scores);
+    const Tensor &grad_out, const Tensor &points, const Tensor &centers,
+    const Tensor &scores, const Tensor &knn_idx, Tensor &grad_points,
+    Tensor &grad_centers, Tensor &grad_scores);
 
 REGISTER_DEVICE_IMPL(assign_score_withk_forward_impl, CUDA,
                      assign_score_withk_forward_cuda);
 REGISTER_DEVICE_IMPL(assign_score_withk_backward_impl, CUDA,
                      assign_score_withk_backward_cuda);
 
 void BallQueryForwardCUDAKernelLauncher(int b, int n, int m, float min_radius,
@@ -100,45 +100,45 @@
   BBoxOverlapsCUDAKernelLauncher(bboxes1, bboxes2, ious, mode, aligned, offset);
 }
 
 void bbox_overlaps_impl(const Tensor bboxes1, const Tensor bboxes2, Tensor ious,
                         const int mode, const bool aligned, const int offset);
 REGISTER_DEVICE_IMPL(bbox_overlaps_impl, CUDA, bbox_overlaps_cuda);
 
-void BorderAlignForwardCUDAKernelLauncher(const Tensor& input,
-                                          const Tensor& boxes, Tensor output,
+void BorderAlignForwardCUDAKernelLauncher(const Tensor &input,
+                                          const Tensor &boxes, Tensor output,
                                           Tensor argmax_idx,
                                           const int pool_size);
 
-void BorderAlignBackwardCUDAKernelLauncher(const Tensor& grad_output,
-                                           const Tensor& boxes,
-                                           const Tensor& argmax_idx,
+void BorderAlignBackwardCUDAKernelLauncher(const Tensor &grad_output,
+                                           const Tensor &boxes,
+                                           const Tensor &argmax_idx,
                                            Tensor grad_input,
                                            const int pool_size);
 
-void border_align_forward_cuda(const Tensor& input, const Tensor& boxes,
+void border_align_forward_cuda(const Tensor &input, const Tensor &boxes,
                                Tensor output, Tensor argmax_idx,
                                const int pool_size) {
   BorderAlignForwardCUDAKernelLauncher(input, boxes, output, argmax_idx,
                                        pool_size);
 }
 
-void border_align_backward_cuda(const Tensor& grad_output, const Tensor& boxes,
-                                const Tensor& argmax_idx, Tensor grad_input,
+void border_align_backward_cuda(const Tensor &grad_output, const Tensor &boxes,
+                                const Tensor &argmax_idx, Tensor grad_input,
                                 const int pool_size) {
   BorderAlignBackwardCUDAKernelLauncher(grad_output, boxes, argmax_idx,
                                         grad_input, pool_size);
 }
 
-void border_align_forward_impl(const Tensor& input, const Tensor& boxes,
+void border_align_forward_impl(const Tensor &input, const Tensor &boxes,
                                Tensor output, Tensor argmax_idx,
                                const int pool_size);
 
-void border_align_backward_impl(const Tensor& grad_output, const Tensor& boxes,
-                                const Tensor& argmax_idx, Tensor grad_input,
+void border_align_backward_impl(const Tensor &grad_output, const Tensor &boxes,
+                                const Tensor &argmax_idx, Tensor grad_input,
                                 const int pool_size);
 
 REGISTER_DEVICE_IMPL(border_align_forward_impl, CUDA,
                      border_align_forward_cuda);
 REGISTER_DEVICE_IMPL(border_align_backward_impl, CUDA,
                      border_align_backward_cuda);
 
@@ -468,36 +468,36 @@
                      sigmoid_focal_loss_backward_cuda);
 REGISTER_DEVICE_IMPL(softmax_focal_loss_forward_impl, CUDA,
                      softmax_focal_loss_forward_cuda);
 REGISTER_DEVICE_IMPL(softmax_focal_loss_backward_impl, CUDA,
                      softmax_focal_loss_backward_cuda);
 
 void FurthestPointSamplingForwardCUDAKernelLauncher(int b, int n, int m,
-                                                    const float* dataset,
-                                                    float* temp, int* idxs);
+                                                    const float *dataset,
+                                                    float *temp, int *idxs);
 
 void FurthestPointSamplingWithDistForwardCUDAKernelLauncher(
-    int b, int n, int m, const float* dataset, float* temp, int* idxs);
+    int b, int n, int m, const float *dataset, float *temp, int *idxs);
 
 void furthest_point_sampling_forward_cuda(Tensor points_tensor,
                                           Tensor temp_tensor, Tensor idx_tensor,
                                           int b, int n, int m) {
-  const float* dataset = points_tensor.data_ptr<float>();
-  float* temp = temp_tensor.data_ptr<float>();
-  int* idxs = idx_tensor.data_ptr<int>();
+  const float *dataset = points_tensor.data_ptr<float>();
+  float *temp = temp_tensor.data_ptr<float>();
+  int *idxs = idx_tensor.data_ptr<int>();
   FurthestPointSamplingForwardCUDAKernelLauncher(b, n, m, dataset, temp, idxs);
 }
 
 void furthest_point_sampling_with_dist_forward_cuda(Tensor points_tensor,
                                                     Tensor temp_tensor,
                                                     Tensor idx_tensor, int b,
                                                     int n, int m) {
-  const float* dataset = points_tensor.data_ptr<float>();
-  float* temp = temp_tensor.data_ptr<float>();
-  int* idxs = idx_tensor.data_ptr<int>();
+  const float *dataset = points_tensor.data_ptr<float>();
+  float *temp = temp_tensor.data_ptr<float>();
+  int *idxs = idx_tensor.data_ptr<int>();
   FurthestPointSamplingWithDistForwardCUDAKernelLauncher(b, n, m, dataset, temp,
                                                          idxs);
 }
 
 void furthest_point_sampling_forward_impl(Tensor points_tensor,
                                           Tensor temp_tensor, Tensor idx_tensor,
                                           int b, int n, int m);
@@ -508,26 +508,51 @@
                                                     int n, int m);
 
 REGISTER_DEVICE_IMPL(furthest_point_sampling_forward_impl, CUDA,
                      furthest_point_sampling_forward_cuda);
 REGISTER_DEVICE_IMPL(furthest_point_sampling_with_dist_forward_impl, CUDA,
                      furthest_point_sampling_with_dist_forward_cuda);
 
-torch::Tensor fused_bias_leakyrelu_op(const torch::Tensor& input,
-                                      const torch::Tensor& bias,
-                                      const torch::Tensor& refer, int act,
+torch::Tensor fused_bias_leakyrelu_op(const torch::Tensor &input,
+                                      const torch::Tensor &bias,
+                                      const torch::Tensor &refer, int act,
                                       int grad, float alpha, float scale);
 
-torch::Tensor fused_bias_leakyrelu_op_impl(const torch::Tensor& input,
-                                           const torch::Tensor& bias,
-                                           const torch::Tensor& refer, int act,
+torch::Tensor fused_bias_leakyrelu_op_impl(const torch::Tensor &input,
+                                           const torch::Tensor &bias,
+                                           const torch::Tensor &refer, int act,
                                            int grad, float alpha, float scale);
 REGISTER_DEVICE_IMPL(fused_bias_leakyrelu_op_impl, CUDA,
                      fused_bias_leakyrelu_op);
 
+torch::Tensor bias_act_op_impl(const torch::Tensor &input,
+                               const torch::Tensor &bias,
+                               const torch::Tensor &xref,
+                               const torch::Tensor &yref,
+                               const torch::Tensor &dy, int grad, int dim,
+                               int act, float alpha, float gain, float clamp);
+
+torch::Tensor bias_act_op(const torch::Tensor &input, const torch::Tensor &bias,
+                          const torch::Tensor &xref, const torch::Tensor &yref,
+                          const torch::Tensor &dy, int grad, int dim, int act,
+                          float alpha, float gain, float clamp);
+
+REGISTER_DEVICE_IMPL(bias_act_op_impl, CUDA, bias_act_op);
+
+torch::Tensor filtered_lrelu_act_op_impl(torch::Tensor x, torch::Tensor si,
+                                         int sx, int sy, float gain,
+                                         float slope, float clamp,
+                                         bool writeSigns);
+
+torch::Tensor filtered_lrelu_act_op(torch::Tensor x, torch::Tensor si, int sx,
+                                    int sy, float gain, float slope,
+                                    float clamp, bool writeSigns);
+
+REGISTER_DEVICE_IMPL(filtered_lrelu_act_op_impl, CUDA, filtered_lrelu_act_op);
+
 void GatherPointsForwardCUDAKernelLauncher(int b, int c, int n, int npoints,
                                            const Tensor points,
                                            const Tensor idx, Tensor out);
 
 void GatherPointsBackwardCUDAKernelLauncher(int b, int c, int n, int npoints,
                                             const Tensor grad_out,
                                             const Tensor idx,
@@ -647,51 +672,51 @@
 
 void IoU3DBoxesOverlapBevForwardCUDAKernelLauncher(const int num_a,
                                                    const Tensor boxes_a,
                                                    const int num_b,
                                                    const Tensor boxes_b,
                                                    Tensor ans_overlap);
 
-void IoU3DNMS3DForwardCUDAKernelLauncher(const Tensor boxes, Tensor& keep,
-                                         Tensor& keep_num,
+void IoU3DNMS3DForwardCUDAKernelLauncher(const Tensor boxes, Tensor &keep,
+                                         Tensor &keep_num,
                                          float nms_overlap_thresh);
 
-void IoU3DNMS3DNormalForwardCUDAKernelLauncher(const Tensor boxes, Tensor& keep,
-                                               Tensor& keep_num,
+void IoU3DNMS3DNormalForwardCUDAKernelLauncher(const Tensor boxes, Tensor &keep,
+                                               Tensor &keep_num,
                                                float nms_overlap_thresh);
 
 void iou3d_boxes_overlap_bev_forward_cuda(const int num_a, const Tensor boxes_a,
                                           const int num_b, const Tensor boxes_b,
                                           Tensor ans_overlap) {
   IoU3DBoxesOverlapBevForwardCUDAKernelLauncher(num_a, boxes_a, num_b, boxes_b,
                                                 ans_overlap);
 };
 
-void iou3d_nms3d_forward_cuda(const Tensor boxes, Tensor& keep,
-                              Tensor& keep_num, float nms_overlap_thresh) {
+void iou3d_nms3d_forward_cuda(const Tensor boxes, Tensor &keep,
+                              Tensor &keep_num, float nms_overlap_thresh) {
   IoU3DNMS3DForwardCUDAKernelLauncher(boxes, keep, keep_num,
                                       nms_overlap_thresh);
 };
 
-void iou3d_nms3d_normal_forward_cuda(const Tensor boxes, Tensor& keep,
-                                     Tensor& keep_num,
+void iou3d_nms3d_normal_forward_cuda(const Tensor boxes, Tensor &keep,
+                                     Tensor &keep_num,
                                      float nms_overlap_thresh) {
   IoU3DNMS3DNormalForwardCUDAKernelLauncher(boxes, keep, keep_num,
                                             nms_overlap_thresh);
 };
 
 void iou3d_boxes_overlap_bev_forward_impl(const int num_a, const Tensor boxes_a,
                                           const int num_b, const Tensor boxes_b,
                                           Tensor ans_overlap);
 
-void iou3d_nms3d_forward_impl(const Tensor boxes, Tensor& keep,
-                              Tensor& keep_num, float nms_overlap_thresh);
+void iou3d_nms3d_forward_impl(const Tensor boxes, Tensor &keep,
+                              Tensor &keep_num, float nms_overlap_thresh);
 
-void iou3d_nms3d_normal_forward_impl(const Tensor boxes, Tensor& keep,
-                                     Tensor& keep_num,
+void iou3d_nms3d_normal_forward_impl(const Tensor boxes, Tensor &keep,
+                                     Tensor &keep_num,
                                      float nms_overlap_thresh);
 
 REGISTER_DEVICE_IMPL(iou3d_boxes_overlap_bev_forward_impl, CUDA,
                      iou3d_boxes_overlap_bev_forward_cuda);
 REGISTER_DEVICE_IMPL(iou3d_nms3d_forward_impl, CUDA, iou3d_nms3d_forward_cuda);
 REGISTER_DEVICE_IMPL(iou3d_nms3d_normal_forward_impl, CUDA,
                      iou3d_nms3d_normal_forward_cuda);
@@ -808,39 +833,39 @@
 REGISTER_DEVICE_IMPL(modulated_deformable_im2col_impl, CUDA,
                      modulated_deformable_im2col_cuda);
 REGISTER_DEVICE_IMPL(modulated_deformable_col2im_impl, CUDA,
                      modulated_deformable_col2im_cuda);
 REGISTER_DEVICE_IMPL(modulated_deformable_col2im_coord_impl, CUDA,
                      modulated_deformable_col2im_coord_cuda);
 
-Tensor ms_deform_attn_cuda_forward(const Tensor& value,
-                                   const Tensor& spatial_shapes,
-                                   const Tensor& level_start_index,
-                                   const Tensor& sampling_loc,
-                                   const Tensor& attn_weight,
+Tensor ms_deform_attn_cuda_forward(const Tensor &value,
+                                   const Tensor &spatial_shapes,
+                                   const Tensor &level_start_index,
+                                   const Tensor &sampling_loc,
+                                   const Tensor &attn_weight,
                                    const int im2col_step);
 
 void ms_deform_attn_cuda_backward(
-    const Tensor& value, const Tensor& spatial_shapes,
-    const Tensor& level_start_index, const Tensor& sampling_loc,
-    const Tensor& attn_weight, const Tensor& grad_output, Tensor& grad_value,
-    Tensor& grad_sampling_loc, Tensor& grad_attn_weight, const int im2col_step);
-
-Tensor ms_deform_attn_impl_forward(const Tensor& value,
-                                   const Tensor& spatial_shapes,
-                                   const Tensor& level_start_index,
-                                   const Tensor& sampling_loc,
-                                   const Tensor& attn_weight,
+    const Tensor &value, const Tensor &spatial_shapes,
+    const Tensor &level_start_index, const Tensor &sampling_loc,
+    const Tensor &attn_weight, const Tensor &grad_output, Tensor &grad_value,
+    Tensor &grad_sampling_loc, Tensor &grad_attn_weight, const int im2col_step);
+
+Tensor ms_deform_attn_impl_forward(const Tensor &value,
+                                   const Tensor &spatial_shapes,
+                                   const Tensor &level_start_index,
+                                   const Tensor &sampling_loc,
+                                   const Tensor &attn_weight,
                                    const int im2col_step);
 
 void ms_deform_attn_impl_backward(
-    const Tensor& value, const Tensor& spatial_shapes,
-    const Tensor& level_start_index, const Tensor& sampling_loc,
-    const Tensor& attn_weight, const Tensor& grad_output, Tensor& grad_value,
-    Tensor& grad_sampling_loc, Tensor& grad_attn_weight, const int im2col_step);
+    const Tensor &value, const Tensor &spatial_shapes,
+    const Tensor &level_start_index, const Tensor &sampling_loc,
+    const Tensor &attn_weight, const Tensor &grad_output, Tensor &grad_value,
+    Tensor &grad_sampling_loc, Tensor &grad_attn_weight, const int im2col_step);
 
 REGISTER_DEVICE_IMPL(ms_deform_attn_impl_forward, CUDA,
                      ms_deform_attn_cuda_forward);
 REGISTER_DEVICE_IMPL(ms_deform_attn_impl_backward, CUDA,
                      ms_deform_attn_cuda_backward);
 
 Tensor NMSCUDAKernelLauncher(Tensor boxes, Tensor scores, float iou_threshold,
@@ -1240,48 +1265,48 @@
                             int pooled_width, float spatial_scale);
 REGISTER_DEVICE_IMPL(roi_pool_forward_impl, CUDA, roi_pool_forward_cuda);
 REGISTER_DEVICE_IMPL(roi_pool_backward_impl, CUDA, roi_pool_backward_cuda);
 
 typedef enum { SUM = 0, MEAN = 1, MAX = 2 } reduce_t;
 
 std::vector<at::Tensor> DynamicPointToVoxelForwardCUDAKernelLauncher(
-    const at::Tensor& feats, const at::Tensor& coors,
+    const at::Tensor &feats, const at::Tensor &coors,
     const reduce_t reduce_type);
 
 void DynamicPointToVoxelBackwardCUDAKernelLauncher(
-    at::Tensor& grad_feats, const at::Tensor& grad_reduced_feats,
-    const at::Tensor& feats, const at::Tensor& reduced_feats,
-    const at::Tensor& coors_map, const at::Tensor& reduce_count,
+    at::Tensor &grad_feats, const at::Tensor &grad_reduced_feats,
+    const at::Tensor &feats, const at::Tensor &reduced_feats,
+    const at::Tensor &coors_map, const at::Tensor &reduce_count,
     const reduce_t reduce_type);
 
 std::vector<torch::Tensor> dynamic_point_to_voxel_forward_cuda(
-    const torch::Tensor& feats, const torch::Tensor& coors,
+    const torch::Tensor &feats, const torch::Tensor &coors,
     const reduce_t reduce_type) {
   return DynamicPointToVoxelForwardCUDAKernelLauncher(feats, coors,
                                                       reduce_type);
 };
 
 void dynamic_point_to_voxel_backward_cuda(
-    torch::Tensor& grad_feats, const torch::Tensor& grad_reduced_feats,
-    const torch::Tensor& feats, const torch::Tensor& reduced_feats,
-    const torch::Tensor& coors_idx, const torch::Tensor& reduce_count,
+    torch::Tensor &grad_feats, const torch::Tensor &grad_reduced_feats,
+    const torch::Tensor &feats, const torch::Tensor &reduced_feats,
+    const torch::Tensor &coors_idx, const torch::Tensor &reduce_count,
     const reduce_t reduce_type) {
   DynamicPointToVoxelBackwardCUDAKernelLauncher(grad_feats, grad_reduced_feats,
                                                 feats, reduced_feats, coors_idx,
                                                 reduce_count, reduce_type);
 };
 
 std::vector<torch::Tensor> dynamic_point_to_voxel_forward_impl(
-    const torch::Tensor& feats, const torch::Tensor& coors,
+    const torch::Tensor &feats, const torch::Tensor &coors,
     const reduce_t reduce_type);
 
 void dynamic_point_to_voxel_backward_impl(
-    torch::Tensor& grad_feats, const torch::Tensor& grad_reduced_feats,
-    const torch::Tensor& feats, const torch::Tensor& reduced_feats,
-    const torch::Tensor& coors_idx, const torch::Tensor& reduce_count,
+    torch::Tensor &grad_feats, const torch::Tensor &grad_reduced_feats,
+    const torch::Tensor &feats, const torch::Tensor &reduced_feats,
+    const torch::Tensor &coors_idx, const torch::Tensor &reduce_count,
     const reduce_t reduce_type);
 
 REGISTER_DEVICE_IMPL(dynamic_point_to_voxel_forward_impl, CUDA,
                      dynamic_point_to_voxel_forward_cuda);
 REGISTER_DEVICE_IMPL(dynamic_point_to_voxel_backward_impl, CUDA,
                      dynamic_point_to_voxel_backward_cuda);
 
@@ -1439,87 +1464,86 @@
 
 void tin_shift_forward_impl(Tensor input, Tensor shift, Tensor output);
 void tin_shift_backward_impl(Tensor grad_output, Tensor shift,
                              Tensor grad_input);
 REGISTER_DEVICE_IMPL(tin_shift_forward_impl, CUDA, tin_shift_forward_cuda);
 REGISTER_DEVICE_IMPL(tin_shift_backward_impl, CUDA, tin_shift_backward_cuda);
 
-torch::Tensor upfirdn2d_op(const torch::Tensor& input,
-                           const torch::Tensor& kernel, int up_x, int up_y,
-                           int down_x, int down_y, int pad_x0, int pad_x1,
-                           int pad_y0, int pad_y1);
-
-torch::Tensor upfirdn2d_op_impl(const torch::Tensor& input,
-                                const torch::Tensor& kernel, int up_x, int up_y,
-                                int down_x, int down_y, int pad_x0, int pad_x1,
-                                int pad_y0, int pad_y1);
+torch::Tensor upfirdn2d_op(torch::Tensor input, torch::Tensor filter, int upx,
+                           int upy, int downx, int downy, int padx0, int padx1,
+                           int pady0, int pady1, bool flip, float gain);
+
+torch::Tensor upfirdn2d_op_impl(torch::Tensor input, torch::Tensor filter,
+                                int upx, int upy, int downx, int downy,
+                                int padx0, int padx1, int pady0, int pady1,
+                                bool flip, float gain);
 REGISTER_DEVICE_IMPL(upfirdn2d_op_impl, CUDA, upfirdn2d_op);
 
 int HardVoxelizeForwardCUDAKernelLauncher(
-    const at::Tensor& points, at::Tensor& voxels, at::Tensor& coors,
-    at::Tensor& num_points_per_voxel, const std::vector<float> voxel_size,
+    const at::Tensor &points, at::Tensor &voxels, at::Tensor &coors,
+    at::Tensor &num_points_per_voxel, const std::vector<float> voxel_size,
     const std::vector<float> coors_range, const int max_points,
     const int max_voxels, const int NDim = 3);
 
 int NondeterministicHardVoxelizeForwardCUDAKernelLauncher(
-    const at::Tensor& points, at::Tensor& voxels, at::Tensor& coors,
-    at::Tensor& num_points_per_voxel, const std::vector<float> voxel_size,
+    const at::Tensor &points, at::Tensor &voxels, at::Tensor &coors,
+    at::Tensor &num_points_per_voxel, const std::vector<float> voxel_size,
     const std::vector<float> coors_range, const int max_points,
     const int max_voxels, const int NDim = 3);
 
 void DynamicVoxelizeForwardCUDAKernelLauncher(
-    const at::Tensor& points, at::Tensor& coors,
+    const at::Tensor &points, at::Tensor &coors,
     const std::vector<float> voxel_size, const std::vector<float> coors_range,
     const int NDim = 3);
 
-int hard_voxelize_forward_cuda(const at::Tensor& points, at::Tensor& voxels,
-                               at::Tensor& coors,
-                               at::Tensor& num_points_per_voxel,
+int hard_voxelize_forward_cuda(const at::Tensor &points, at::Tensor &voxels,
+                               at::Tensor &coors,
+                               at::Tensor &num_points_per_voxel,
                                const std::vector<float> voxel_size,
                                const std::vector<float> coors_range,
                                const int max_points, const int max_voxels,
                                const int NDim) {
   return HardVoxelizeForwardCUDAKernelLauncher(
       points, voxels, coors, num_points_per_voxel, voxel_size, coors_range,
       max_points, max_voxels, NDim);
 };
 
 int nondeterministic_hard_voxelize_forward_cuda(
-    const at::Tensor& points, at::Tensor& voxels, at::Tensor& coors,
-    at::Tensor& num_points_per_voxel, const std::vector<float> voxel_size,
+    const at::Tensor &points, at::Tensor &voxels, at::Tensor &coors,
+    at::Tensor &num_points_per_voxel, const std::vector<float> voxel_size,
     const std::vector<float> coors_range, const int max_points,
     const int max_voxels, const int NDim) {
   return NondeterministicHardVoxelizeForwardCUDAKernelLauncher(
       points, voxels, coors, num_points_per_voxel, voxel_size, coors_range,
       max_points, max_voxels, NDim);
 };
 
-void dynamic_voxelize_forward_cuda(const at::Tensor& points, at::Tensor& coors,
+void dynamic_voxelize_forward_cuda(const at::Tensor &points, at::Tensor &coors,
                                    const std::vector<float> voxel_size,
                                    const std::vector<float> coors_range,
                                    const int NDim) {
   DynamicVoxelizeForwardCUDAKernelLauncher(points, coors, voxel_size,
                                            coors_range, NDim);
 };
 
-int hard_voxelize_forward_impl(const at::Tensor& points, at::Tensor& voxels,
-                               at::Tensor& coors,
-                               at::Tensor& num_points_per_voxel,
+int hard_voxelize_forward_impl(const at::Tensor &points, at::Tensor &voxels,
+                               at::Tensor &coors,
+                               at::Tensor &num_points_per_voxel,
                                const std::vector<float> voxel_size,
                                const std::vector<float> coors_range,
                                const int max_points, const int max_voxels,
                                const int NDim);
 
 int nondeterministic_hard_voxelize_forward_impl(
-    const at::Tensor& points, at::Tensor& voxels, at::Tensor& coors,
-    at::Tensor& num_points_per_voxel, const std::vector<float> voxel_size,
+    const at::Tensor &points, at::Tensor &voxels, at::Tensor &coors,
+    at::Tensor &num_points_per_voxel, const std::vector<float> voxel_size,
     const std::vector<float> coors_range, const int max_points,
     const int max_voxels, const int NDim);
 
-void dynamic_voxelize_forward_impl(const at::Tensor& points, at::Tensor& coors,
+void dynamic_voxelize_forward_impl(const at::Tensor &points, at::Tensor &coors,
                                    const std::vector<float> voxel_size,
                                    const std::vector<float> coors_range,
                                    const int NDim);
 
 REGISTER_DEVICE_IMPL(hard_voxelize_forward_impl, CUDA,
                      hard_voxelize_forward_cuda);
 REGISTER_DEVICE_IMPL(nondeterministic_hard_voxelize_forward_impl, CUDA,
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
   auto output_n = output.view(
       {batch / im2col_step_, batch_n, num_query, num_heads, channels});
   auto per_value_size = spatial_size * num_heads * channels;
   auto per_sample_loc_size = num_query * num_heads * num_levels * num_point * 2;
   auto per_attn_weight_size = num_query * num_heads * num_levels * num_point;
   for (int n = 0; n < batch / im2col_step_; ++n) {
     auto columns = output_n.select(0, n);
-    AT_DISPATCH_FLOATING_TYPES(
+    AT_DISPATCH_FLOATING_TYPES_AND_HALF(
         value.scalar_type(), "ms_deform_attn_forward_cuda", ([&] {
           ms_deformable_im2col_cuda(
               at::cuda::getCurrentCUDAStream(),
               value.data_ptr<scalar_t>() + n * im2col_step_ * per_value_size,
               spatial_shapes.data_ptr<int64_t>(),
               level_start_index.data_ptr<int64_t>(),
               sampling_loc.data_ptr<scalar_t>() +
@@ -322,15 +322,15 @@
   auto per_sample_loc_size = num_query * num_heads * num_levels * num_point * 2;
   auto per_attn_weight_size = num_query * num_heads * num_levels * num_point;
   auto grad_output_n = grad_output.view(
       {batch / im2col_step_, batch_n, num_query, num_heads, channels});
 
   for (int n = 0; n < batch / im2col_step_; ++n) {
     auto grad_output_g = grad_output_n.select(0, n);
-    AT_DISPATCH_FLOATING_TYPES(
+    AT_DISPATCH_FLOATING_TYPES_AND_HALF(
         value.scalar_type(), "ms_deform_attn_backward_cuda", ([&] {
           ms_deformable_col2im_cuda(
               at::cuda::getCurrentCUDAStream(),
               grad_output_g.data_ptr<scalar_t>(),
               value.data_ptr<scalar_t>() + n * im2col_step_ * per_value_size,
               spatial_shapes.data_ptr<int64_t>(),
               level_start_index.data_ptr<int64_t>(),
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/deform_conv.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/gather_points.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/gather_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/group_points.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/group_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/info.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/info.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/iou3d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/iou3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/knn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/knn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/masked_conv2d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/masked_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,115 @@
 /*************************************************************************
- * Copyright (C) 2022 Cambricon.
+ * Copyright (C) 2022 by Cambricon.
  *
  * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
  * OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
  * MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
  * IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
  * CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
  * TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
  * SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  *************************************************************************/
+#include "mlu_common_helper.h"
 
-#include "pytorch_device_registry.hpp"
-#include "pytorch_mlu_helper.hpp"
+void RotatedFeatureAlignForwardMLUKernelLauncher(const Tensor features,
+                                                 const Tensor best_bboxes,
+                                                 const float spatial_scale,
+                                                 const int points,
+                                                 Tensor output) {
+  auto memory_format =
+      torch_mlu::cnnl::ops::get_channels_last_memory_format(features.dim());
+  auto features_ =
+      torch_mlu::cnnl::ops::cnnl_contiguous(features, memory_format);
+  auto best_bboxes_contiguous = torch_mlu::cnnl::ops::cnnl_contiguous(
+      best_bboxes, best_bboxes.suggest_memory_format());
+  auto output_contiguous =
+      torch_mlu::cnnl::ops::cnnl_contiguous(output, memory_format);
+
+  MluOpTensorDescriptor features_desc, best_bboxes_desc, output_desc;
+  features_desc.set_with_layout(features_, MLUOP_LAYOUT_NHWC);
+  best_bboxes_desc.set(best_bboxes_contiguous);
+  output_desc.set_with_layout(output_contiguous, MLUOP_LAYOUT_NHWC);
+
+  // get ptr of tensors
+  auto features_impl = torch_mlu::getMluTensorImpl(features_);
+  auto features_ptr = features_impl->cnnlMalloc();
+  auto best_bboxes_impl = torch_mlu::getMluTensorImpl(best_bboxes_contiguous);
+  auto best_bboxes_ptr = best_bboxes_impl->cnnlMalloc();
+  auto output_impl = torch_mlu::getMluTensorImpl(output_contiguous);
+  auto output_ptr = output_impl->cnnlMalloc();
 
-void KernelIou3d(cnrtDim3_t k_dim, cnrtFunctionType_t k_type, cnrtQueue_t queue,
-                 const cnrtDataType_t data_type_input, const void *boxes_dram,
-                 const int input_box_num, const float iou_threshold,
-                 void *workspace, void *output_size, void *output);
-
-int selectType(uint32_t use_job, int box_num_per_core) {
-  // the box_num_per_core should be at least 256, otherwise the real IO
-  // bandwidth would be very low
-  while (box_num_per_core < 256 && use_job >= 4) {
-    box_num_per_core *= 2;
-    use_job /= 2;
-  }
-  return use_job;
-}
-static cnnlStatus_t policyFunc(cnrtDim3_t *k_dim, cnrtFunctionType_t *k_type,
-                               int &core_num_per_class,
-                               const int input_box_num) {
-  uint32_t core_dim = torch_mlu::getDeviceAttr(cnrtAttrMcorePerCluster);
-  uint32_t job_limit = getJobLimitCapability();
-  uint32_t core_number = job_limit;
-
-  int box_num_per_core = (input_box_num + core_number - 1) / core_number;
-  int use_job = selectType(job_limit, box_num_per_core);
-  // initiate k_type as Union1
-  k_dim->x = core_dim;
-  k_dim->y = 1;
-  k_dim->z = 1;
-  *k_type = CNRT_FUNC_TYPE_UNION1;
-  switch (job_limit) {
-    case CN_KERNEL_CLASS_BLOCK:
-    case CN_KERNEL_CLASS_UNION:
-    case CN_KERNEL_CLASS_UNION2:
-    case CN_KERNEL_CLASS_UNION4:
-    case CN_KERNEL_CLASS_UNION8:
-    case CN_KERNEL_CLASS_UNION16: {
-      if (use_job < 4) {
-        k_dim->x = 1;
-        *k_type = CNRT_FUNC_TYPE_BLOCK;
-      } else if (use_job == 4) {
-        k_dim->x = core_dim;
-        *k_type = CNRT_FUNC_TYPE_UNION1;
-      } else {
-        k_dim->x = use_job;
-        *k_type = (cnrtFunctionType_t)use_job;
-      }
-    }; break;
-    default:
-      LOG(WARNING) << "[cnnlNms_v2]: got unsupported job limit number."
-                   << " Use default CN_KERNEL_CLASS_UNION1 with UNION1 task.";
-  }
-  return CNNL_STATUS_SUCCESS;
+  // get compute handle
+  auto handle = mluOpGetCurrentHandle();
+  mluOpRotatedFeatureAlignForward(
+      handle, features_desc.desc(), features_ptr, best_bboxes_desc.desc(),
+      best_bboxes_ptr, spatial_scale, points, output_desc.desc(), output_ptr);
+
+  output.copy_(output_contiguous);
 }
 
-void IoU3DNMS3DMLUKernelLauncher(Tensor boxes, Tensor &keep, Tensor &keep_num,
-                                 float iou_threshold) {
-  // dimension parameters check
-  TORCH_CHECK(boxes.dim() == 2, "boxes should be a 2d tensor, got ",
-              boxes.dim(), "D");
-  TORCH_CHECK(boxes.size(1) == 7,
-              "boxes should have 7 elements in dimension 1, got ",
-              boxes.size(1));
-
-  // data type check
-  TORCH_CHECK(
-      boxes.scalar_type() == at::kFloat || boxes.scalar_type() == at::kHalf,
-      "data type of boxes should be Float or Half, got ", boxes.scalar_type());
-
-  if (boxes.numel() == 0) {
-    return;
-  }
-  const size_t max_input_num = 2147483648;  // 2^31, 2G num
-  TORCH_CHECK(boxes.numel() < max_input_num,
-              "boxes.numel() should be less than 2147483648, got ",
-              boxes.numel());
-  int input_box_num = boxes.size(0);
-
-  cnrtDataType_t data_type_input = torch_mlu::toCnrtDtype(boxes.dtype());
-  cnrtDim3_t k_dim;
-  cnrtJobType_t k_type;
-
-  int core_num_per_class;
-  policyFunc(&k_dim, &k_type, core_num_per_class, input_box_num);
-
-  // transpose boxes (n, 7) to (7, n) for better performance
-  auto boxes_t = boxes.transpose(0, 1);
-  auto boxes_ = torch_mlu::cnnl::ops::cnnl_contiguous(boxes_t);
-
-  auto output = at::empty({input_box_num}, boxes.options().dtype(at::kLong));
-  auto output_size = at::empty({1}, boxes.options().dtype(at::kInt));
-
-  // workspace
-  const int info_num = 7;  // x, y,z, dx, dy, dz,angle
-  size_t space_size = 0;
-  if (boxes.scalar_type() == at::kHalf) {
-    space_size = input_box_num * sizeof(int16_t) * info_num +
-                 input_box_num * sizeof(float) + sizeof(float);
-  } else {
-    space_size = input_box_num * sizeof(float) * (info_num + 1) + sizeof(float);
-  }
-
-  auto workspace = at::empty(space_size, boxes.options().dtype(at::kByte));
-
-  // get compute queue
-  auto queue = torch_mlu::getCurQueue();
-
-  auto boxes_impl = torch_mlu::getMluTensorImpl(boxes_);
-  auto boxes_ptr = boxes_impl->cnnlMalloc();
-  auto workspace_impl = torch_mlu::getMluTensorImpl(workspace);
-  auto workspace_ptr = workspace_impl->cnnlMalloc();
-  auto output_impl = torch_mlu::getMluTensorImpl(keep);
-  auto output_ptr = output_impl->cnnlMalloc();
-  auto output_size_impl = torch_mlu::getMluTensorImpl(keep_num);
-  auto output_size_ptr = output_size_impl->cnnlMalloc();
+void RotatedFeatureAlignBackwardMLUKernelLauncher(const Tensor top_grad,
+                                                  const Tensor best_bboxes,
+                                                  const float spatial_scale,
+                                                  const int points,
+                                                  Tensor bottom_grad) {
+  auto memory_format =
+      torch_mlu::cnnl::ops::get_channels_last_memory_format(top_grad.dim());
+  auto top_grad_ =
+      torch_mlu::cnnl::ops::cnnl_contiguous(top_grad, memory_format);
+  auto best_bboxes_contiguous = torch_mlu::cnnl::ops::cnnl_contiguous(
+      best_bboxes, best_bboxes.suggest_memory_format());
+  auto bottom_grad_ =
+      torch_mlu::cnnl::ops::cnnl_contiguous(bottom_grad, memory_format);
+
+  // get ptr of tensors
+  auto top_grad_impl = torch_mlu::getMluTensorImpl(top_grad_);
+  auto top_grad_ptr = top_grad_impl->cnnlMalloc();
+  auto best_bboxes_impl = torch_mlu::getMluTensorImpl(best_bboxes_contiguous);
+  auto best_bboxes_ptr = best_bboxes_impl->cnnlMalloc();
+  auto bottom_grad_impl = torch_mlu::getMluTensorImpl(bottom_grad_);
+  auto bottom_grad_ptr = bottom_grad_impl->cnnlMalloc();
+
+  MluOpTensorDescriptor top_grad_desc, best_bboxes_desc, bottom_grad_desc;
+  top_grad_desc.set_with_layout(top_grad_, MLUOP_LAYOUT_NHWC);
+  best_bboxes_desc.set(best_bboxes_contiguous);
+  bottom_grad_desc.set_with_layout(bottom_grad_, MLUOP_LAYOUT_NHWC);
+
+  // get compute handle
+  auto handle = mluOpGetCurrentHandle();
+  mluOpRotatedFeatureAlignBackward(handle, top_grad_desc.desc(), top_grad_ptr,
+                                   best_bboxes_desc.desc(), best_bboxes_ptr,
+                                   spatial_scale, points,
+                                   bottom_grad_desc.desc(), bottom_grad_ptr);
+  bottom_grad.copy_(bottom_grad_);
+}
 
-  uint32_t core_dim = torch_mlu::getDeviceAttr(cnrtAttrMcorePerCluster);
-  CNLOG(INFO) << "Launch Kernel KernelIou3d<<<Union" << k_type / core_dim
-              << ", " << k_dim.x << ", " << k_dim.y << ", " << k_dim.z << ">>>";
-  KernelIou3d(k_dim, k_type, queue, data_type_input, boxes_ptr, input_box_num,
-              iou_threshold, workspace_ptr, output_size_ptr, output_ptr);
+void rotated_feature_align_forward_mlu(const Tensor features,
+                                       const Tensor best_bboxes,
+                                       const float spatial_scale,
+                                       const int points, Tensor output) {
+  RotatedFeatureAlignForwardMLUKernelLauncher(features, best_bboxes,
+                                              spatial_scale, points, output);
 }
 
-void iou3d_nms3d_forward_mlu(const Tensor boxes, Tensor &keep, Tensor &keep_num,
-                             float nms_overlap_thresh) {
-  IoU3DNMS3DMLUKernelLauncher(boxes, keep, keep_num, nms_overlap_thresh);
+void rotated_feature_align_backward_mlu(const Tensor top_grad,
+                                        const Tensor best_bboxes,
+                                        const float spatial_scale,
+                                        const int points, Tensor bottom_grad) {
+  RotatedFeatureAlignBackwardMLUKernelLauncher(
+      top_grad, best_bboxes, spatial_scale, points, bottom_grad);
 }
 
-void iou3d_nms3d_forward_impl(const Tensor boxes, Tensor &keep,
-                              Tensor &keep_num, float nms_overlap_thresh);
-REGISTER_DEVICE_IMPL(iou3d_nms3d_forward_impl, MLU, iou3d_nms3d_forward_mlu);
+void rotated_feature_align_forward_impl(const Tensor features,
+                                        const Tensor best_bboxes,
+                                        const float spatial_scale,
+                                        const int points, Tensor output);
+
+void rotated_feature_align_backward_impl(const Tensor top_grad,
+                                         const Tensor best_bboxes,
+                                         const float spatial_scale,
+                                         const int points, Tensor bottom_grad);
+
+REGISTER_DEVICE_IMPL(rotated_feature_align_forward_impl, MLU,
+                     rotated_feature_align_forward_mlu);
+REGISTER_DEVICE_IMPL(rotated_feature_align_backward_impl, MLU,
+                     rotated_feature_align_backward_mlu);
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,232 +1,275 @@
 /*************************************************************************
- * Copyright (C) 2022 by Cambricon.
+ * Copyright (C) 2022 Cambricon.
  *
  * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
  * OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
  * MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
  * IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
  * CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
  * TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
  * SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  *************************************************************************/
 #include "pytorch_device_registry.hpp"
 #include "pytorch_mlu_helper.hpp"
-#include "roi_align_rotated_utils.hpp"
 
-namespace {
-
-void policyFunc(int bin_num, cnrtDim3_t *k_dim, cnrtFunctionType_t *k_type) {
-  unsigned int core_num = torch_mlu::getDeviceAttr(cnrtAttrMcorePerCluster);
-  unsigned int cluster_num = torch_mlu::getDeviceAttr(cnrtAttrClusterCount);
+void KernelRoiPoolForward(cnrtDim3_t k_dim, cnrtFunctionType_t k_type,
+                          cnrtQueue_t queue, cnrtDataType_t data_type,
+                          const void *input_data, const void *input_rois,
+                          const int batch, const int channels, const int height,
+                          const int width, const int pooled_height,
+                          const int pooled_width, const int rois_num,
+                          const float spatial_scale, void *output_data,
+                          int *argmax);
+
+void KernelRoiPoolBackward(cnrtDim3_t k_dim, cnrtFunctionType_t k_type,
+                           cnrtQueue_t queue, cnrtDataType_t k_dtype,
+                           const void *grad_output_ptr, const void *rois_ptr,
+                           const int *argmax_ptr, void *grad_input_ptr,
+                           const int box_num, const int pooled_height,
+                           const int pooled_width, const int channels,
+                           const int batch, const int height, const int width,
+                           const float spatial_scale);
+
+// policy function for forward
+static void policyFuncForward(const int bin_num, cnrtDim3_t *k_dim,
+                              cnrtFunctionType_t *k_type) {
+  auto core_num = torch_mlu::getDeviceAttr(cnrtAttrMcorePerCluster);
+  auto cluster_num = torch_mlu::getDeviceAttr(cnrtAttrClusterCount);
   *k_type = CNRT_FUNC_TYPE_UNION1;
   k_dim->x = core_num;
-  unsigned int use_cluster = (bin_num + core_num - 1) / core_num;
+  unsigned int use_cluster = bin_num / core_num + (bin_num % core_num > 0);
   k_dim->y = use_cluster > cluster_num ? cluster_num : use_cluster;
   k_dim->z = 1;
 }
 
-}  // namespace
+void ROIPoolForwardMLUKernelLauncher(Tensor input, Tensor rois, Tensor output,
+                                     Tensor argmax, int pooled_height,
+                                     int pooled_width, float spatial_scale) {
+  // Check dtype.
+  TORCH_CHECK(
+      input.scalar_type() == at::kFloat || input.scalar_type() == at::kHalf,
+      "input type should be Float or Half, got ", input.scalar_type());
+  TORCH_CHECK(input.scalar_type() == rois.scalar_type(),
+              "rois should have the same type as input");
 
-void KernelRoiAlignRotatedForward(
-    cnrtDim3_t k_dim, cnrtFunctionType_t k_type, cnrtQueue_t queue,
-    const cnrtDataType_t d_type, const void *features, const void *rois,
-    void *output, const int batch, const int height, const int width,
-    const int channel, const int rois_num,
-    const RoiAlignRotatedParams roiAlignRotatedParams);
-
-void KernelRoiAlignRotatedBackward(
-    cnrtDim3_t k_dim, cnrtFunctionType_t k_type, cnrtQueue_t queue,
-    const cnrtDataType_t d_type, const void *top_grad, const void *rois,
-    void *bottom_grad, const int batch, const int height, const int width,
-    const int channel, const int rois_num,
-    const RoiAlignRotatedParams roiAlignRotatedParams);
-
-void ROIAlignRotatedForwardMLUKernelLauncher(Tensor input, Tensor rois,
-                                             Tensor output, int pooled_height,
-                                             int pooled_width,
-                                             float spatial_scale,
-                                             int sampling_ratio, bool aligned,
-                                             bool clockwise) {
-  TORCH_CHECK(((input.scalar_type() == output.scalar_type()) &&
-               (output.scalar_type() == rois.scalar_type())),
-              "data types of input, rois and output should be the same, ",
-              "but now input type is ", input.scalar_type(), ", rois type is ",
-              rois.scalar_type(), ", output type is ", output.scalar_type(),
-              ".");
+  // Check dtype relationship.
   TORCH_CHECK(
-      (input.scalar_type() == at::kFloat || input.scalar_type() == at::kHalf),
-      "input type should be Float or Half, got ", input.scalar_type(), ".");
+      argmax.scalar_type() == at::kLong || argmax.scalar_type() == at::kInt,
+      "argmax type should be Int or Long, got ", argmax.scalar_type());
 
-  TORCH_CHECK(input.dim() == 4, "input should be a 4d tensor, got ",
-              input.dim(), "D.");
-  TORCH_CHECK(rois.dim() == 2, "rois should be a 2d tensor, got ", rois.dim(),
-              "D.");
-  TORCH_CHECK(output.dim() == 4, "output should be a 4d tensor, got ",
-              output.dim(), "D.");
-
-  TORCH_CHECK((rois.size(0) == output.size(0)),
-              "the 1st dimensions of rois and output should be the same, ",
-              "but now the 1st dimension of rois is ", rois.size(0),
-              ", and output is ", output.size(0), ".");
-
-  TORCH_CHECK((input.size(1) == output.size(1)),
-              "the 2nd dimensions of input and output should be the same, ",
-              "but now the 2nd dimension of input is ", input.size(1),
-              ", and output is ", output.size(1), ".");
-
-  int channel = input.size(1);
-  int width = input.size(3);
-  int height = input.size(2);
-  int batch = input.size(0);
-  int rois_nums = rois.size(0);
-  cnrtDataType_t d_type = torch_mlu::toCnrtDtype(input.dtype());
-
-  // return if zero-elements
-  if (input.numel() == 0) {
-    CNLOG(INFO) << "Skip the zero-elements case.";
+  // Check shape.
+  TORCH_CHECK(input.dim() == 4, "input should be 4d tensor, got ", input.dim(),
+              "D");
+  TORCH_CHECK(rois.dim() == 2, "rois should be 2d tensor, got ", rois.dim(),
+              "D");
+  TORCH_CHECK(argmax.dim() == 4, "argmax should be 4d tensor, got ",
+              argmax.dim(), "D");
+
+  TORCH_CHECK(spatial_scale > 0 && spatial_scale <= 1,
+              "spatial_scale should be within (0, 1], got ", spatial_scale);
+
+  // compute kernel params
+  auto batch = input.size(0);
+  auto height = input.size(2);
+  auto width = input.size(3);
+  auto channels = input.size(1);
+  auto rois_num = output.size(0);
+
+  if (output.numel() == 0) {
+    output = at::zeros({rois_num, channels, pooled_height, pooled_width},
+                       input.options());
+    return;
+  }
+  if (argmax.numel() == 0) {
+    argmax = at::zeros({rois_num, channels, pooled_height, pooled_width},
+                       argmax.options());
     return;
   }
 
-  RoiAlignRotatedParams roiAlignRotatedParams{pooled_height,  pooled_width,
-                                              sampling_ratio, spatial_scale,
-                                              aligned,        clockwise};
-  cnrtDim3_t k_dim;
-  cnrtFunctionType_t k_type;
-  policyFunc(rois_nums * pooled_height * pooled_width, &k_dim, &k_type);
+  // zero element check
+  if (input.numel() == 0 || rois.numel() == 0 || output.numel() == 0 ||
+      argmax.numel() == 0) {
+    return;
+  }
 
   auto memory_format =
       torch_mlu::cnnl::ops::get_channels_last_memory_format(input.dim());
-  auto input_tensor =
-      torch_mlu::cnnl::ops::cnnl_contiguous(input, memory_format);
-  at::Tensor output_tmp =
-      at::empty({rois_nums, channel, pooled_height, pooled_width},
+  auto input_ = torch_mlu::cnnl::ops::cnnl_contiguous(input, memory_format);
+
+  at::Tensor output_ =
+      at::empty({rois_num, channels, pooled_height, pooled_width},
                 input.options(), memory_format);
+  at::Tensor argmax_ =
+      at::empty({rois_num, channels, pooled_height, pooled_width},
+                argmax.options(), memory_format);
+
+  // calculate task dimension
+  cnrtDim3_t k_dim;
+  cnrtFunctionType_t k_type;
+  policyFuncForward(rois_num * pooled_height * pooled_width, &k_dim, &k_type);
 
   // get compute queue
   auto queue = torch_mlu::getCurQueue();
 
   // get ptr of tensors
-  auto input_impl = torch_mlu::getMluTensorImpl(input_tensor);
+  auto input_impl = torch_mlu::getMluTensorImpl(input_);
   auto input_ptr = input_impl->cnnlMalloc();
   auto rois_impl = torch_mlu::getMluTensorImpl(rois);
   auto rois_ptr = rois_impl->cnnlMalloc();
-  auto output_impl = torch_mlu::getMluTensorImpl(output_tmp);
+  auto output_impl = torch_mlu::getMluTensorImpl(output_);
   auto output_ptr = output_impl->cnnlMalloc();
+  auto argmax_impl = torch_mlu::getMluTensorImpl(argmax_);
+  auto argmax_ptr = argmax_impl->cnnlMalloc();
+
+  // get comput dtype of input
+  cnrtDataType_t data_type = torch_mlu::toCnrtDtype(input_.dtype());
+
+  // launch kernel
+  CNLOG(INFO) << "Launch Kernel MLUKernelRoiPoolForward<<<" << k_dim.x << ", "
+              << k_dim.y << ", " << k_dim.z << ">>>";
+
+  KernelRoiPoolForward(k_dim, k_type, queue, data_type, input_ptr, rois_ptr,
+                       batch, channels, height, width, pooled_height,
+                       pooled_width, rois_num, spatial_scale, output_ptr,
+                       (int *)argmax_ptr);
+  output.copy_(output_);
+  argmax.copy_(argmax_);
+}
 
-  KernelRoiAlignRotatedForward(k_dim, k_type, queue, d_type, input_ptr,
-                               rois_ptr, output_ptr, batch, height, width,
-                               channel, rois_nums, roiAlignRotatedParams);
-  output.copy_(output_tmp);
-}
-
-void ROIAlignRotatedBackwardMLUKernelLauncher(
-    Tensor top_grad, Tensor rois, Tensor bottom_grad, int pooled_height,
-    int pooled_width, float spatial_scale, int sampling_ratio, bool aligned,
-    bool clockwise) {
-  TORCH_CHECK(((top_grad.scalar_type() == bottom_grad.scalar_type()) &&
-               (bottom_grad.scalar_type() == rois.scalar_type())),
-              "data types of top_grad, rois and bottom_grad should be ",
-              "the same, but now top_grad type is ", top_grad.scalar_type(),
-              ", rois type is ", rois.scalar_type(), ", bottom_grad type is ",
-              bottom_grad.scalar_type(), ".");
-  TORCH_CHECK((bottom_grad.scalar_type() == at::kFloat ||
-               bottom_grad.scalar_type() == at::kHalf),
-              "Data type of bottom_grad should be Float ro Half, got ",
-              bottom_grad.scalar_type(), ".");
-
-  TORCH_CHECK(bottom_grad.dim() == 4, "bottom_grad should be a 4d tensor, got ",
-              top_grad.dim(), "D.");
-  TORCH_CHECK(rois.dim() == 2, "rois should be a 2d tensor, got ", rois.dim(),
-              "D.");
-  TORCH_CHECK(top_grad.dim() == 4, "top_grad should be a 4d tensor, got ",
-              bottom_grad.dim(), "D.");
-
-  TORCH_CHECK((rois.size(0) == top_grad.size(0)),
-              "the 1st dimensions of rois and top_grad should be the same, ",
-              "but now the 1st dimension of rois is ", rois.size(0),
-              ", and top_grad is ", top_grad.size(0), ".");
-
-  TORCH_CHECK((bottom_grad.size(1) == top_grad.size(1)),
-              "the 2nd dimensions of bottom_grad and top_grad should be ",
-              "the same, but now the 2nd dimension of bottom_grad is ",
-              bottom_grad.size(1), ", and top_grad is ", top_grad.size(1), ".");
-
-  int channel = bottom_grad.size(1);
-  int width = bottom_grad.size(3);
-  int height = bottom_grad.size(2);
-  int batch = bottom_grad.size(0);
-  int rois_nums = rois.size(0);
-  cnrtDataType_t d_type = torch_mlu::toCnrtDtype(bottom_grad.dtype());
-
-  // return if zero-elements
-  if (bottom_grad.numel() == 0) {
-    CNLOG(INFO) << "Skip the zero-elements case.";
+// policy function for backward
+static void policyFuncBackward(cnrtDim3_t *k_dim, cnrtFunctionType_t *k_type) {
+  *k_type = CNRT_FUNC_TYPE_UNION1;
+  k_dim->x = torch_mlu::getDeviceAttr(cnrtAttrMcorePerCluster);
+  k_dim->y = torch_mlu::getDeviceAttr(cnrtAttrClusterCount);
+  k_dim->z = 1;
+}
+
+void ROIPoolBackwardMLUKernelLauncher(Tensor grad_output, Tensor rois,
+                                      Tensor argmax, Tensor grad_input,
+                                      int pooled_height, int pooled_width,
+                                      float spatial_scale) {
+  // Check dtype.
+  TORCH_CHECK(
+      argmax.scalar_type() == at::kLong || argmax.scalar_type() == at::kInt,
+      "argmax type should be Int or Long, got ", argmax.scalar_type());
+  TORCH_CHECK((grad_output.scalar_type() == at::kFloat ||
+               grad_output.scalar_type() == at::kHalf),
+              "grad_output type should be FLoat or Half, got ",
+              grad_output.scalar_type());
+
+  // Check dtype relationship.
+  TORCH_CHECK((rois.scalar_type() == grad_output.scalar_type()),
+              "rois should have the same type as grad_output");
+
+  // Check shape.
+  TORCH_CHECK(grad_output.dim() == 4, "grad_output should be 4d tensor, got ",
+              grad_output.dim(), "D");
+  TORCH_CHECK(rois.dim() == 2, "rois should be 2d tensor, got ", rois.dim(),
+              "D");
+  TORCH_CHECK(argmax.dim() == 4, "argmax should be 4d tensor, got ",
+              argmax.dim(), "D");
+
+  TORCH_CHECK(spatial_scale > 0 && spatial_scale <= 1,
+              "spatial_scale should be within (0, 1], got ", spatial_scale);
+
+  // Check relationship between tensor.
+  // Check the relationship of n.
+  TORCH_CHECK(grad_output.size(0) == rois.size(0),
+              "grad_output.size(0) = ", grad_output.size(0),
+              ", while rois.size(0) = ", rois.size(0),
+              ". They should be the same.");
+
+  // Check the relationship of channels.
+  TORCH_CHECK(grad_output.size(1) == argmax.size(1),
+              "grad_output.size(1) = ", grad_output.size(1),
+              ", while argmax.size(1) = ", argmax.size(1),
+              ". They should be the same.");
+
+  // Check the relationship of height and width.
+  TORCH_CHECK(grad_output.size(2) == argmax.size(2),
+              "argmax.size(2) = ", argmax.size(2),
+              ", while grad_output.size(2) = ", grad_output.size(2),
+              ". They should be the same.");
+  TORCH_CHECK(grad_output.size(3) == argmax.size(3),
+              "argmax.size(3) = ", argmax.size(3),
+              ", while grad_output.size(3) = ", grad_output.size(3),
+              ". They should be the same.");
+
+  // Check zero element.
+  if (grad_output.numel() == 0 || rois.numel() == 0 || argmax.numel() == 0 ||
+      grad_input.numel() == 0) {
+    // return if zero-element
     return;
   }
 
-  RoiAlignRotatedParams roiAlignRotatedParams{pooled_height,  pooled_width,
-                                              sampling_ratio, spatial_scale,
-                                              aligned,        clockwise};
-  cnrtDim3_t k_dim;
-  cnrtFunctionType_t k_type;
-  policyFunc(rois_nums * pooled_height * pooled_width, &k_dim, &k_type);
-
   auto memory_format =
-      torch_mlu::cnnl::ops::get_channels_last_memory_format(top_grad.dim());
-  auto top_grad_tensor =
-      torch_mlu::cnnl::ops::cnnl_contiguous(top_grad, memory_format);
-  at::Tensor bottom_grad_tmp = at::empty({batch, channel, height, width},
-                                         top_grad.options(), memory_format)
-                                   .zero_();
+      torch_mlu::cnnl::ops::get_channels_last_memory_format(grad_output.dim());
+  auto grad_output_ =
+      torch_mlu::cnnl::ops::cnnl_contiguous(grad_output, memory_format);
+  auto argmax_ = torch_mlu::cnnl::ops::cnnl_contiguous(argmax, memory_format);
+
+  int boxes_num = grad_output.size(0);
+  int no = grad_input.size(0);
+  int channels = grad_input.size(1);
+  int height = grad_input.size(2);
+  int width = grad_input.size(3);
+  auto grad_input_ = at::empty({no, channels, height, width},
+                               grad_input.options(), memory_format)
+                         .zero_();
+
+  // get tensor impl
+  auto grad_output_impl = torch_mlu::getMluTensorImpl(grad_output_);
+  auto rois_impl = torch_mlu::getMluTensorImpl(rois);
+  auto argmax_impl = torch_mlu::getMluTensorImpl(argmax_);
+  auto grad_input_impl = torch_mlu::getMluTensorImpl(grad_input_);
 
   // get compute queue
   auto queue = torch_mlu::getCurQueue();
 
-  // get ptr of tensors
-  auto bottom_grad_impl = torch_mlu::getMluTensorImpl(bottom_grad_tmp);
-  auto bottom_grad_ptr = bottom_grad_impl->cnnlMalloc();
-  auto rois_impl = torch_mlu::getMluTensorImpl(rois);
+  // get mlu ptr
+  auto grad_output_ptr = grad_output_impl->cnnlMalloc();
   auto rois_ptr = rois_impl->cnnlMalloc();
-  auto top_grad_impl = torch_mlu::getMluTensorImpl(top_grad_tensor);
-  auto top_grad_ptr = top_grad_impl->cnnlMalloc();
+  auto argmax_ptr = argmax_impl->cnnlMalloc();
+  auto grad_input_ptr = grad_input_impl->cnnlMalloc();
+
+  // calculate task dimension
+  cnrtDataType_t k_dtype = torch_mlu::toCnrtDtype(grad_input.dtype());
+  cnrtDim3_t k_dim;
+  cnrtFunctionType_t k_type;
+  policyFuncBackward(&k_dim, &k_type);
+
+  CNLOG(INFO) << "Launch Kernel MLUKernelRoiPoolBackward<<<" << k_dim.x << ", "
+              << k_dim.y << ", " << k_dim.z << ">>>";
+
+  KernelRoiPoolBackward(k_dim, k_type, queue, k_dtype, grad_output_ptr,
+                        rois_ptr, (int *)argmax_ptr, grad_input_ptr, boxes_num,
+                        pooled_height, pooled_width, channels, no, height,
+                        width, spatial_scale);
+
+  grad_input.copy_(grad_input_);
+}
+
+void roi_pool_forward_mlu(Tensor input, Tensor rois, Tensor output,
+                          Tensor argmax, int pooled_height, int pooled_width,
+                          float spatial_scale) {
+  ROIPoolForwardMLUKernelLauncher(input, rois, output, argmax, pooled_height,
+                                  pooled_width, spatial_scale);
+}
+
+void roi_pool_backward_mlu(Tensor grad_output, Tensor rois, Tensor argmax,
+                           Tensor grad_input, int pooled_height,
+                           int pooled_width, float spatial_scale) {
+  ROIPoolBackwardMLUKernelLauncher(grad_output, rois, argmax, grad_input,
+                                   pooled_height, pooled_width, spatial_scale);
+}
+
+void roi_pool_forward_impl(Tensor input, Tensor rois, Tensor output,
+                           Tensor argmax, int pooled_height, int pooled_width,
+                           float spatial_scale);
+
+void roi_pool_backward_impl(Tensor grad_output, Tensor rois, Tensor argmax,
+                            Tensor grad_input, int pooled_height,
+                            int pooled_width, float spatial_scale);
 
-  KernelRoiAlignRotatedBackward(k_dim, k_type, queue, d_type, top_grad_ptr,
-                                rois_ptr, bottom_grad_ptr, batch, height, width,
-                                channel, rois_nums, roiAlignRotatedParams);
-  bottom_grad.copy_(bottom_grad_tmp);
-}
-
-void roi_align_rotated_forward_mlu(Tensor input, Tensor rois, Tensor output,
-                                   int aligned_height, int aligned_width,
-                                   float spatial_scale, int sampling_ratio,
-                                   bool aligned, bool clockwise) {
-  ROIAlignRotatedForwardMLUKernelLauncher(input, rois, output, aligned_height,
-                                          aligned_width, spatial_scale,
-                                          sampling_ratio, aligned, clockwise);
-}
-
-void roi_align_rotated_backward_mlu(Tensor top_grad, Tensor rois,
-                                    Tensor bottom_grad, int aligned_height,
-                                    int aligned_width, float spatial_scale,
-                                    int sampling_ratio, bool aligned,
-                                    bool clockwise) {
-  ROIAlignRotatedBackwardMLUKernelLauncher(
-      top_grad, rois, bottom_grad, aligned_height, aligned_width, spatial_scale,
-      sampling_ratio, aligned, clockwise);
-}
-
-void roi_align_rotated_forward_impl(Tensor input, Tensor rois, Tensor output,
-                                    int aligned_height, int aligned_width,
-                                    float spatial_scale, int sampling_ratio,
-                                    bool aligned, bool clockwise);
-
-void roi_align_rotated_backward_impl(Tensor top_grad, Tensor rois,
-                                     Tensor bottom_grad, int aligned_height,
-                                     int aligned_width, float spatial_scale,
-                                     int sampling_ratio, bool aligned,
-                                     bool clockwise);
-
-REGISTER_DEVICE_IMPL(roi_align_rotated_forward_impl, MLU,
-                     roi_align_rotated_forward_mlu);
-REGISTER_DEVICE_IMPL(roi_align_rotated_backward_impl, MLU,
-                     roi_align_rotated_backward_mlu);
+REGISTER_DEVICE_IMPL(roi_pool_forward_impl, MLU, roi_pool_forward_mlu);
+REGISTER_DEVICE_IMPL(roi_pool_backward_impl, MLU, roi_pool_backward_mlu);
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/nms_quadri.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/nms_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/nms_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/nms_rotated.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -8,25 +8,45 @@
 
 #ifdef MMCV_WITH_CUDA
 Tensor nms_rotated_cuda(const Tensor dets, const Tensor scores,
                         const Tensor order, const Tensor dets_sorted,
                         const float iou_threshold, const int multi_label);
 #endif
 
+#ifdef MMCV_WITH_NPU
+Tensor nms_rotated_npu(const Tensor dets, const Tensor scores,
+                       const Tensor labels, const float iou_threshold);
+#endif
+
+#ifdef MMCV_WITH_MLU
+Tensor nms_rotated_mlu(const Tensor dets, const Tensor scores,
+                       const float iou_threshold);
+#endif
+
 // Interface for Python
 // inline is needed to prevent multiple function definitions when this header is
 // included by different cpps
 Tensor nms_rotated(const Tensor dets, const Tensor scores, const Tensor order,
-                   const Tensor dets_sorted, const float iou_threshold,
-                   const int multi_label) {
+                   const Tensor dets_sorted, const Tensor labels,
+                   const float iou_threshold, const int multi_label) {
   assert(dets.device().is_cuda() == scores.device().is_cuda());
   if (dets.device().is_cuda()) {
 #ifdef MMCV_WITH_CUDA
-    return nms_rotated_cuda(dets, scores, order, dets_sorted, iou_threshold,
-                            multi_label);
+    return nms_rotated_cuda(dets, scores, order, dets_sorted.contiguous(),
+                            iou_threshold, multi_label);
 #else
     AT_ERROR("Not compiled with GPU support");
 #endif
+  } else if (dets.device().type() == at::kXLA) {
+#ifdef MMCV_WITH_NPU
+    return nms_rotated_npu(dets, scores, labels, iou_threshold);
+#else
+    AT_ERROR("Not compiled with NPU support");
+#endif
+#ifdef MMCV_WITH_MLU
+  } else if (dets.device().type() == at::kMLU) {
+    return nms_rotated_mlu(dets, scores, iou_threshold);
+#endif
   }
 
-  return nms_rotated_cpu(dets, scores, iou_threshold);
+  return nms_rotated_cpu(dets.contiguous(), scores.contiguous(), iou_threshold);
 }
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -41,19 +41,19 @@
                                   int pooled_width, float spatial_scale,
                                   int sampling_ratio, float gamma) {
   c10::SmallVector<int64_t, 2> output_sizes = {pooled_height, pooled_width};
   at::IntArrayRef output_size = at::IntArrayRef(output_sizes);
   int64_t sampling_ratio_ = (int64_t)sampling_ratio;
   OpCommand cmd;
   cmd.Name("DeformableRoiPoolGrad")
-      .Input(grad_input)
+      .Input(grad_output)
       .Input(input)
       .Input(rois)
       .Input(offset)
-      .Output(grad_output)
+      .Output(grad_input)
       .Output(grad_offset)
       .Attr("output_size", output_size)
       .Attr("spatial_scale", spatial_scale)
       .Attr("sample_ratio", sampling_ratio_)
       .Attr("gamma", gamma)
       .Run();
 }
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #include "pytorch_npu_helper.hpp"
 
 using namespace NPU_NAME_SPACE;
 using namespace std;
 
 Tensor nms_npu(Tensor boxes, Tensor scores, float iou_threshold, int offset) {
-  at::Tensor boxed_offest = at_npu::native::OpPreparation::ApplyTensor(boxes);
-  at::Tensor ones_tensor =
-      at_npu::native::OpPreparation::ApplyTensor(boxes).fill_(1);
-  at::add_out(boxed_offest, boxes, ones_tensor, offset);
+  TORCH_CHECK((boxes.scalar_type() == at::ScalarType::Float),
+              "The type of boxes tensor passed in nms_npu should be float");
+  int64_t offset_64 = offset;
   at::Tensor iou_threshold_y = at_npu::native::OpPreparation::ApplyTensor(
                                    {}, boxes.options().dtype(at::kFloat), boxes)
                                    .fill_(iou_threshold);
   at::Tensor scores_threshold_y =
       at_npu::native::OpPreparation::ApplyTensor(
           {}, boxes.options().dtype(at::kFloat), boxes)
           .fill_(0);
@@ -25,14 +24,15 @@
   OpCommand cmd;
   cmd.Name("NonMaxSuppressionV3")
       .Input(boxes)
       .Input(scores)
       .Input(max_outputsize_y)
       .Input(iou_threshold_y)
       .Input(scores_threshold_y)
+      .Attr("offset", offset_64)
       .Output(output)
       .Run();
   auto outputsizeBool = at::gt(output, -1);
   auto outputsizeInt = outputsizeBool.to(at::ScalarType::Int);
   auto countLen = at::sum(outputsizeInt, at::ScalarType::Int);
   at::Tensor actual_output = output.slice(0, 0, countLen.item().toLong());
   actual_output = at_npu::native::NPUNativeFunctions::npu_dtype_cast(
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -7,28 +7,75 @@
                           Tensor argmax, int pooled_height, int pooled_width,
                           float spatial_scale) {
   int64_t pooled_height_64 = pooled_height;
   int64_t pooled_width_64 = pooled_width;
   int64_t pooled_channel = 1;
   at::Tensor roi_actual_num = at_npu::native::OpPreparation::ApplyTensor(
       {}, rois.options().dtype(at::kInt), rois);
+  if (input.sizes()[1] % 16 == 0) {
+    OpCommand cmd;
+    cmd.Name("RoiPoolingWithArgMax")
+        .Input(input)
+        .Input(rois)
+        .Input(roi_actual_num)
+        .Output(output)
+        .Output(argmax)
+        .Attr("pooled_h", pooled_height_64)
+        .Attr("pooled_w", pooled_width_64)
+        .Attr("spatial_scale_h", spatial_scale)
+        .Attr("spatial_scale_w", spatial_scale)
+        .Attr("pool_channel", pooled_channel)
+        .Run();
 
+  } else {
+    OpCommand cmd;
+    cmd.Name("RoiPoolingWithArgMax")
+        .Input(input)
+        .Input(rois)
+        .Input(roi_actual_num)
+        .Output(output)
+        .Output(argmax)
+        .Attr("pooled_h", pooled_height_64)
+        .Attr("pooled_w", pooled_width_64)
+        .Attr("spatial_scale_h", spatial_scale)
+        .Attr("spatial_scale_w", spatial_scale)
+        .Attr("pool_channel", pooled_channel)
+        .Attr("_exclude_engines", (string) "AiCore")
+        .Run();
+  }
+}
+
+void roi_pool_backward_npu(Tensor grad_output, Tensor rois, Tensor argmax,
+                           Tensor grad_input, int pooled_height,
+                           int pooled_width, float spatial_scale) {
+  int64_t pooled_height_64 = pooled_height;
+  int64_t pooled_width_64 = pooled_width;
+  int64_t pooled_channel = 1;
+  at::Tensor roi_actual_num = at_npu::native::OpPreparation::ApplyTensor(
+      {}, rois.options().dtype(at::kInt), rois);
+  at::Tensor x = at::ones_like(grad_input);
   OpCommand cmd;
-  cmd.Name("RoiPoolingWithArgMax")
-      .Input(input)
+  cmd.Name("RoiPoolingGradWithArgMax")
+      .Input(grad_output)
+      .Input(x)
       .Input(rois)
       .Input(roi_actual_num)
-      .Output(output)
-      .Output(argmax)
+      .Input(argmax)
+      .Output(grad_input)
       .Attr("pooled_h", pooled_height_64)
       .Attr("pooled_w", pooled_width_64)
       .Attr("spatial_scale_h", spatial_scale)
       .Attr("spatial_scale_w", spatial_scale)
       .Attr("pool_channel", pooled_channel)
       .Run();
 }
 
 void roi_pool_forward_impl(Tensor input, Tensor rois, Tensor output,
                            Tensor argmax, int pooled_height, int pooled_width,
                            float spatial_scale);
 
+void roi_pool_backward_impl(Tensor grad_output, Tensor rois, Tensor argmax,
+                            Tensor grad_input, int pooled_height,
+                            int pooled_width, float spatial_scale);
+
 REGISTER_NPU_IMPL(roi_pool_forward_impl, roi_pool_forward_npu);
+REGISTER_NPU_IMPL(roi_pool_backward_impl, roi_pool_backward_npu);
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/pixel_group.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/points_in_boxes.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/points_in_polygons.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/points_in_polygons.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/prroi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/prroi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/psamask.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/pybind.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/pybind.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -305,20 +305,20 @@
                                Tensor outGrad, Tensor indicePairs,
                                Tensor indiceNum);
 
 void box_iou_rotated(const Tensor boxes1, const Tensor boxes2, Tensor ious,
                      const int mode_flag, const bool aligned);
 
 Tensor nms_rotated(const Tensor dets, const Tensor scores, const Tensor order,
-                   const Tensor dets_sorted, const float iou_threshold,
-                   const int multi_label);
+                   const Tensor dets_sorted, const Tensor labels,
+                   const float iou_threshold, const int multi_label);
 
-Tensor upfirdn2d(const Tensor &input, const Tensor &kernel, int up_x, int up_y,
-                 int down_x, int down_y, int pad_x0, int pad_x1, int pad_y0,
-                 int pad_y1);
+Tensor upfirdn2d(torch::Tensor input, torch::Tensor filter, int upx, int upy,
+                 int downx, int downy, int padx0, int padx1, int pady0,
+                 int pady1, bool flip, float gain);
 
 Tensor fused_bias_leakyrelu(const Tensor &input, const Tensor &bias,
                             const Tensor &refer, int act, int grad, float alpha,
                             float scale);
 
 void roi_align_rotated_forward(Tensor input, Tensor rois, Tensor output,
                                int pooled_height, int pooled_width,
@@ -435,14 +435,28 @@
                               const Tensor idx1, const Tensor idx);
 
 void chamfer_distance_backward(const Tensor xyz1, const Tensor xyz2,
                                Tensor idx1, Tensor idx2, Tensor graddist1,
                                Tensor graddist2, Tensor gradxyz1,
                                Tensor gradxyz2);
 
+Tensor bias_act(const Tensor &input, const Tensor &bias, const Tensor &xref,
+                const Tensor &yref, const Tensor &dy, int grad, int dim,
+                int act, float alpha, float gain, float clamp);
+
+std::tuple<torch::Tensor, torch::Tensor, int> filtered_lrelu(
+    torch::Tensor x, torch::Tensor fu, torch::Tensor fd, torch::Tensor b,
+    torch::Tensor si, int up, int down, int px0, int px1, int py0, int py1,
+    int sx, int sy, float gain, float slope, float clamp, bool flip_filters,
+    bool writeSigns);
+
+torch::Tensor filtered_lrelu_act_(torch::Tensor x, torch::Tensor si, int sx,
+                                  int sy, float gain, float slope, float clamp,
+                                  bool writeSigns);
+
 void box_iou_quadri(const Tensor boxes1, const Tensor boxes2, Tensor ious,
                     const int mode_flag, const bool aligned);
 
 Tensor nms_quadri(const Tensor dets, const Tensor scores, const Tensor order,
                   const Tensor dets_sorted, const float iou_threshold,
                   const int multi_label);
 
@@ -454,17 +468,17 @@
 void bezier_align_backward(Tensor grad_output, Tensor rois, Tensor grad_input,
                            int aligned_height, int aligned_width,
                            float spatial_scale, int sampling_ratio,
                            bool aligned);
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
   m.def("upfirdn2d", &upfirdn2d, "upfirdn2d (CUDA)", py::arg("input"),
-        py::arg("kernel"), py::arg("up_x"), py::arg("up_y"), py::arg("down_x"),
-        py::arg("down_y"), py::arg("pad_x0"), py::arg("pad_x1"),
-        py::arg("pad_y0"), py::arg("pad_y1"));
+        py::arg("filter"), py::arg("upx"), py::arg("upy"), py::arg("downx"),
+        py::arg("downy"), py::arg("padx0"), py::arg("padx1"), py::arg("pady0"),
+        py::arg("pady1"), py::arg("flip"), py::arg("gain"));
   m.def("fused_bias_leakyrelu", &fused_bias_leakyrelu,
         "fused_bias_leakyrelu (CUDA)", py::arg("input"), py::arg("bias"),
         py::arg("empty"), py::arg("act"), py::arg("grad"), py::arg("alpha"),
         py::arg("scale"));
   m.def("gather_points_forward", &gather_points_forward,
         "gather_points_forward", py::arg("points_tensor"),
         py::arg("idx_tensor"), py::arg("out_tensor"), py::arg("b"),
@@ -754,15 +768,15 @@
   m.def("tin_shift_backward", &tin_shift_backward, "tin_shift backward",
         py::arg("grad_output"), py::arg("shift"), py::arg("grad_input"));
   m.def("box_iou_rotated", &box_iou_rotated, "IoU for rotated boxes",
         py::arg("boxes1"), py::arg("boxes2"), py::arg("ious"),
         py::arg("mode_flag"), py::arg("aligned"));
   m.def("nms_rotated", &nms_rotated, "NMS for rotated boxes", py::arg("dets"),
         py::arg("scores"), py::arg("order"), py::arg("dets_sorted"),
-        py::arg("iou_threshold"), py::arg("multi_label"));
+        py::arg("labels"), py::arg("iou_threshold"), py::arg("multi_label"));
   m.def("ball_query_forward", &ball_query_forward, "ball_query_forward",
         py::arg("new_xyz_tensor"), py::arg("xyz_tensor"), py::arg("idx_tensor"),
         py::arg("b"), py::arg("n"), py::arg("m"), py::arg("min_radius"),
         py::arg("max_radius"), py::arg("nsample"));
   m.def("stack_ball_query_forward", &stack_ball_query_forward,
         "stack_ball_query_forward", py::arg("new_xyz_tensor"),
         py::arg("new_xyz_batch_cnt"), py::arg("xyz_tensor"),
@@ -898,14 +912,28 @@
         py::arg("pooled_height"), py::arg("pooled_width"),
         py::arg("spatial_scale"));
   m.def("prroi_pool_coor_backward", &prroi_pool_coor_backward,
         "prroi_pool_coor_backward", py::arg("output"), py::arg("grad_output"),
         py::arg("input"), py::arg("rois"), py::arg("grad_rois"),
         py::arg("pooled_height"), py::arg("pooled_width"),
         py::arg("spatial_scale"));
+  m.def("bias_act", &bias_act, "bias_act (CUDA)", py::arg("input"),
+        py::arg("bias"), py::arg("xref"), py::arg("yref"), py::arg("dy"),
+        py::arg("grad"), py::arg("dim"), py::arg("act"), py::arg("alpha"),
+        py::arg("gain"), py::arg("clamp"));
+  m.def("filtered_lrelu", &filtered_lrelu, "filtered_lrelu (CUDA)",
+        py::arg("x"), py::arg("fu"), py::arg("fd"), py::arg("b"), py::arg("si"),
+        py::arg("up"), py::arg("down"), py::arg("px0"), py::arg("px1"),
+        py::arg("py0"), py::arg("py1"), py::arg("sx"), py::arg("sy"),
+        py::arg("gain"), py::arg("slope"), py::arg("clamp"),
+        py::arg("flip_filters"), py::arg("writeSigns"));
+  m.def("filtered_lrelu_act_", &filtered_lrelu_act_,
+        "filtered_lrelu_act_ (CUDA)", py::arg("x"), py::arg("si"),
+        py::arg("sx"), py::arg("sy"), py::arg("gain"), py::arg("slope"),
+        py::arg("clamp"), py::arg("writeSigns"));
   m.def("box_iou_quadri", &box_iou_quadri, "IoU for quadrilateral boxes",
         py::arg("boxes1"), py::arg("boxes2"), py::arg("ious"),
         py::arg("mode_flag"), py::arg("aligned"));
   m.def("nms_quadri", &nms_quadri, "NMS for quadrilateral boxes",
         py::arg("dets"), py::arg("scores"), py::arg("order"),
         py::arg("dets_sorted"), py::arg("iou_threshold"),
         py::arg("multi_label"));
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roi_pool.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/scatter_points.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/scatter_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/spconv_ops.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/spconv_ops.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,34 @@
     std::vector<int64_t> outPadding, int64_t _subM, int64_t _transpose) {
   return GetIndicePairsForwardCUDAKernelLauncher<NDim>(
       indices, batchSize, outSpatialShape, spatialShape, kernelSize, stride,
       padding, dilation, outPadding, _subM, _transpose);
 };
 
 template <unsigned NDim>
+std::vector<torch::Tensor> GetIndicePairsForwardMLUKernelLauncher(
+    torch::Tensor indices, int64_t batchSize,
+    std::vector<int64_t> outSpatialShape, std::vector<int64_t> spatialShape,
+    std::vector<int64_t> kernelSize, std::vector<int64_t> stride,
+    std::vector<int64_t> padding, std::vector<int64_t> dilation,
+    std::vector<int64_t> outPadding, int64_t _subM, int64_t _transpose);
+
+template <unsigned NDim>
+std::vector<torch::Tensor> get_indice_pairs_forward_mlu(
+    torch::Tensor indices, int64_t batchSize,
+    std::vector<int64_t> outSpatialShape, std::vector<int64_t> spatialShape,
+    std::vector<int64_t> kernelSize, std::vector<int64_t> stride,
+    std::vector<int64_t> padding, std::vector<int64_t> dilation,
+    std::vector<int64_t> outPadding, int64_t _subM, int64_t _transpose) {
+  return GetIndicePairsForwardMLUKernelLauncher<NDim>(
+      indices, batchSize, outSpatialShape, spatialShape, kernelSize, stride,
+      padding, dilation, outPadding, _subM, _transpose);
+}
+
+template <unsigned NDim>
 std::vector<torch::Tensor> GetIndicePairsBackwardCUDAKernelLauncher(
     torch::Tensor indices, torch::Tensor gridOut, int64_t batchSize,
     std::vector<int64_t> outSpatialShape, std::vector<int64_t> spatialShape,
     std::vector<int64_t> kernelSize, std::vector<int64_t> stride,
     std::vector<int64_t> padding, std::vector<int64_t> dilation,
     std::vector<int64_t> outPadding, int64_t _subM, int64_t _transpose);
 
@@ -68,14 +88,20 @@
 
     return get_indice_pairs_forward_cuda<NDim>(
         indices, batchSize, outSpatialShape, spatialShape, kernelSize, stride,
         padding, dilation, outPadding, _subM, _transpose);
 #else
     AT_ERROR("get_indice_pairs is not compiled with GPU support");
 #endif
+#ifdef MMCV_WITH_MLU
+  } else if (indices.device().type() == at::kMLU) {
+    return get_indice_pairs_forward_mlu<NDim>(
+        indices, batchSize, outSpatialShape, spatialShape, kernelSize, stride,
+        padding, dilation, outPadding, _subM, _transpose);
+#endif
   } else {
     AT_ERROR("get_indice_pairs is not implemented on CPU");
   }
 }
 
 template <unsigned NDim>
 std::vector<torch::Tensor> get_indice_pairs_backward(
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/spconv_utils.h` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/spconv_utils.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/sync_bn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/sync_bn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/three_interpolate.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/three_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/three_nn.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/three_nn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/tin_shift.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/tin_shift.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/csrc/pytorch/upfirdn2d.cpp` & `mmcv-lite-2.0.1/mmcv/ops/csrc/pytorch/upfirdn2d.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -98,21 +98,21 @@
 
 =======================================================================
 */
 
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 
-torch::Tensor upfirdn2d_op_impl(const torch::Tensor& input,
-                                const torch::Tensor& kernel, int up_x, int up_y,
-                                int down_x, int down_y, int pad_x0, int pad_x1,
-                                int pad_y0, int pad_y1) {
-  return DISPATCH_DEVICE_IMPL(upfirdn2d_op_impl, input, kernel, up_x, up_y,
-                              down_x, down_y, pad_x0, pad_x1, pad_y0, pad_y1);
+torch::Tensor upfirdn2d_op_impl(torch::Tensor input, torch::Tensor filter,
+                                int upx, int upy, int downx, int downy,
+                                int padx0, int padx1, int pady0, int pady1,
+                                bool flip, float gain) {
+  return DISPATCH_DEVICE_IMPL(upfirdn2d_op_impl, input, filter, upx, upy, downx,
+                              downy, padx0, padx1, pady0, pady1, flip, gain);
 }
 
-torch::Tensor upfirdn2d(const torch::Tensor& input, const torch::Tensor& kernel,
-                        int up_x, int up_y, int down_x, int down_y, int pad_x0,
-                        int pad_x1, int pad_y0, int pad_y1) {
-  return upfirdn2d_op_impl(input, kernel, up_x, up_y, down_x, down_y, pad_x0,
-                           pad_x1, pad_y0, pad_y1);
+torch::Tensor upfirdn2d(torch::Tensor input, torch::Tensor filter, int upx,
+                        int upy, int downx, int downy, int padx0, int padx1,
+                        int pady0, int pady1, bool flip, float gain) {
+  return upfirdn2d_op_impl(input, filter, upx, upy, downx, downy, padx0, padx1,
+                           pady0, pady1, flip, gain);
 }
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/deform_conv.py` & `mmcv-lite-2.0.1/mmcv/ops/deform_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         input_tensor, weight, offset_out, offset_all, sort_index_for_npu_bp = \
             ctx.saved_tensors
         grad_input, grad_weight, grad_offset_all, grad_bias = \
             torch.npu_deformable_conv2dbk(
                 input_tensor, grad_output, offset_out, weight, offset_all,
                 kernel_size=[weight.shape[3], weight.shape[2]],
                 stride=[1, 1, ctx.stride[0], ctx.stride[1]],
-                padding=[1, 1, ctx.padding[0], ctx.padding[1]],
+                padding=[ctx.padding[0], ctx.padding[0], ctx.padding[1],
+                         ctx.padding[1]],
                 dilation=[1, 1, ctx.dilation[0], ctx.dilation[1]],
                 groups=ctx.groups, deformable_groups=ctx.deform_groups,
                 modulated=True)
         grad_offset = grad_offset_all.index_select(1, sort_index_for_npu_bp)
         return grad_input, grad_offset, grad_weight, \
             None, None, None, None, None, None, None
 
@@ -104,16 +105,18 @@
             mask = torch.ones_like(mask_shape).to(input.device)
             bias = input.new_empty(0)
             output = ModulatedDeformConv2dFunction._npu_forward(
                 ctx, input, offset, mask, weight, bias)
             return output
         ctx.save_for_backward(input, offset, weight)
 
-        output = input.new_empty(
-            DeformConv2dFunction._output_size(ctx, input, weight))
+        output = input.new_empty([
+            int(i)
+            for i in DeformConv2dFunction._output_size(ctx, input, weight)
+        ])
 
         ctx.bufs_ = [input.new_empty(0), input.new_empty(0)]  # columns, ones
 
         cur_im2col_step = min(ctx.im2col_step, input.size(0))
         assert (input.size(0) % cur_im2col_step
                 ) == 0, 'batch size must be divisible by im2col_step'
         ext_module.deform_conv_forward(
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/deform_roi_pool.py` & `mmcv-lite-2.0.1/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/deprecated_wrappers.py` & `mmcv-lite-2.0.1/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/diff_iou_rotated.py` & `mmcv-lite-2.0.1/mmcv/ops/diff_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/focal_loss.py` & `mmcv-lite-2.0.1/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/furthest_point_sample.py` & `mmcv-lite-2.0.1/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/fused_bias_leakyrelu.py` & `mmcv-lite-2.0.1/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/gather_points.py` & `mmcv-lite-2.0.1/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/group_points.py` & `mmcv-lite-2.0.1/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/info.py` & `mmcv-lite-2.0.1/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/iou3d.py` & `mmcv-lite-2.0.1/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/knn.py` & `mmcv-lite-2.0.1/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/masked_conv.py` & `mmcv-lite-2.0.1/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/merge_cells.py` & `mmcv-lite-2.0.1/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/min_area_polygons.py` & `mmcv-lite-2.0.1/mmcv/ops/min_area_polygons.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/modulated_deform_conv.py` & `mmcv-lite-2.0.1/mmcv/ops/modulated_deform_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         output, offset_out = torch.npu_deformable_conv2d(
             input_tensor,
             weight,
             offset_all,
             conv2d_bias,
             kernel_size=[kernel_w, kernel_h],
             stride=[1, 1, ctx.stride[0], ctx.stride[1]],
-            padding=[1, 1, ctx.padding[0], ctx.padding[1]],
+            padding=[
+                ctx.padding[0], ctx.padding[0], ctx.padding[1], ctx.padding[1]
+            ],
             dilation=[1, 1, ctx.dilation[0], ctx.dilation[1]],
             groups=ctx.groups,
             deformable_groups=ctx.deform_groups,
             modulated=True)
         if weight.requires_grad or mask.requires_grad or offset.requires_grad \
                 or input_tensor.requires_grad:
             ctx.save_for_backward(input_tensor, weight, offset_out, offset_all,
@@ -80,15 +82,16 @@
         input_tensor, weight, offset_out, offset_all, sort_index_bp = \
             ctx.saved_tensors
         grad_input, grad_weight, grad_offset_all, grad_bias = \
             torch.npu_deformable_conv2dbk(
                 input_tensor, grad_output, offset_out, weight, offset_all,
                 kernel_size=[weight.shape[3], weight.shape[2]],
                 stride=[1, 1, ctx.stride[0], ctx.stride[1]],
-                padding=[1, 1, ctx.padding[0], ctx.padding[1]],
+                padding=[ctx.padding[0], ctx.padding[0], ctx.padding[1],
+                         ctx.padding[1]],
                 dilation=[1, 1, ctx.dilation[0], ctx.dilation[1]],
                 groups=ctx.groups, deformable_groups=ctx.deform_groups,
                 modulated=True)
         grad_offset = grad_offset_all.index_select(1, sort_index_bp)
         grad_mask = grad_offset_all[:, grad_offset.shape[1]:, :, :]
         if not ctx.with_bias:
             grad_bias = None
@@ -132,16 +135,18 @@
         bias = bias.type_as(input)  # type: ignore
         mask = mask.type_as(input)
         if ctx.device == 'npu':
             output = ModulatedDeformConv2dFunction._npu_forward(
                 ctx, input, offset, mask, weight, bias)
             return output
         ctx.save_for_backward(input, offset, mask, weight, bias)
-        output = input.new_empty(
-            ModulatedDeformConv2dFunction._output_size(ctx, input, weight))
+        output = input.new_empty([
+            int(i) for i in ModulatedDeformConv2dFunction._output_size(
+                ctx, input, weight)
+        ])
         ctx._bufs = [input.new_empty(0), input.new_empty(0)]
         ext_module.modulated_deform_conv_forward(
             input,
             weight,
             bias,
             ctx._bufs[0],
             offset,
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/multi_scale_deform_attn.py` & `mmcv-lite-2.0.1/mmcv/ops/multi_scale_deform_attn.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,26 @@
             im2col_step (torch.Tensor): The step used in image to column.
 
         Returns:
             torch.Tensor: has shape (bs, num_queries, embed_dims)
         """
 
         ctx.im2col_step = im2col_step
+
+        # When pytorch version >= 1.6.0, amp is adopted for fp16 mode;
+        # amp won't cast the type of sampling_locations, attention_weights
+        # (float32), but "value" is cast to float16, leading to the type
+        # mismatch with input (when it is float32) or weight.
+        # The flag for whether to use fp16 or amp is the type of "value",
+        # we cast sampling_locations and attention_weights to
+        # temporarily support fp16 and amp whatever the
+        # pytorch version is.
+        sampling_locations = sampling_locations.type_as(value)
+        attention_weights = attention_weights.type_as(value)
+
         output = ext_module.ms_deform_attn_forward(
             value,
             value_spatial_shapes,
             value_level_start_index,
             sampling_locations,
             attention_weights,
             im2col_step=ctx.im2col_step)
@@ -162,15 +174,15 @@
 
     `Deformable DETR: Deformable Transformers for End-to-End Object Detection.
     <https://arxiv.org/pdf/2010.04159.pdf>`_.
 
     Args:
         embed_dims (int): The embedding dimension of Attention.
             Default: 256.
-        num_heads (int): Parallel attention heads. Default: 64.
+        num_heads (int): Parallel attention heads. Default: 8.
         num_levels (int): The number of feature map used in
             Attention. Default: 4.
         num_points (int): The number of sampling points for
             each query in each head. Default: 4.
         im2col_step (int): The step used in image_to_column.
             Default: 64.
         dropout (float): A Dropout layer on `inp_identity`.
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/nms.py` & `mmcv-lite-2.0.1/mmcv/ops/nms.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,16 +289,17 @@
                                       dim=-1)
         else:
             max_coordinate = boxes.max()
             offsets = idxs.to(boxes) * (
                 max_coordinate + torch.tensor(1).to(boxes))
             boxes_for_nms = boxes + offsets[:, None]
 
-    nms_type = nms_cfg_.pop('type', 'nms')
-    nms_op = eval(nms_type)
+    nms_op = nms_cfg_.pop('type', 'nms')
+    if isinstance(nms_op, str):
+        nms_op = eval(nms_op)
 
     split_thr = nms_cfg_.pop('split_thr', 10000)
     # Won't split to multiple nms nodes when exporting to onnx
     if boxes_for_nms.shape[0] < split_thr:
         dets, keep = nms_op(boxes_for_nms, scores, **nms_cfg_)
         boxes = boxes[keep]
 
@@ -402,32 +403,51 @@
     if not clockwise:
         flip_mat = dets.new_ones(dets.shape[-1])
         flip_mat[-1] = -1
         dets_cw = dets * flip_mat
     else:
         dets_cw = dets
     multi_label = labels is not None
+    if labels is None:
+        input_labels = scores.new_empty(0, dtype=torch.int)
+    else:
+        input_labels = labels
+    if dets.device.type in ('npu', 'mlu'):
+        order = scores.new_empty(0, dtype=torch.long)
+        if dets.device.type == 'npu':
+            coefficient = 57.29578  # 180 / PI
+            for i in range(dets.size()[0]):
+                dets_cw[i][4] *= coefficient  # radians to angle
+        keep_inds = ext_module.nms_rotated(dets_cw, scores, order, dets_cw,
+                                           input_labels, iou_threshold,
+                                           multi_label)
+        dets = torch.cat((dets[keep_inds], scores[keep_inds].reshape(-1, 1)),
+                         dim=1)
+        return dets, keep_inds
+
     if multi_label:
         dets_wl = torch.cat((dets_cw, labels.unsqueeze(1)), 1)  # type: ignore
     else:
         dets_wl = dets_cw
     _, order = scores.sort(0, descending=True)
     dets_sorted = dets_wl.index_select(0, order)
 
     if torch.__version__ == 'parrots':
         keep_inds = ext_module.nms_rotated(
             dets_wl,
             scores,
             order,
             dets_sorted,
+            input_labels,
             iou_threshold=iou_threshold,
             multi_label=multi_label)
     else:
         keep_inds = ext_module.nms_rotated(dets_wl, scores, order, dets_sorted,
-                                           iou_threshold, multi_label)
+                                           input_labels, iou_threshold,
+                                           multi_label)
     dets = torch.cat((dets[keep_inds], scores[keep_inds].reshape(-1, 1)),
                      dim=1)
     return dets, keep_inds
 
 
 def nms_quadri(dets: Tensor,
                scores: Tensor,
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/pixel_group.py` & `mmcv-lite-2.0.1/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/point_sample.py` & `mmcv-lite-2.0.1/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/points_in_boxes.py` & `mmcv-lite-2.0.1/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/points_in_polygons.py` & `mmcv-lite-2.0.1/mmcv/ops/points_in_polygons.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/points_sampler.py` & `mmcv-lite-2.0.1/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/prroi_pool.py` & `mmcv-lite-2.0.1/mmcv/ops/prroi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/psa_mask.py` & `mmcv-lite-2.0.1/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/riroi_align_rotated.py` & `mmcv-lite-2.0.1/mmcv/ops/riroi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/roi_align.py` & `mmcv-lite-2.0.1/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/roi_align_rotated.py` & `mmcv-lite-2.0.1/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/roi_pool.py` & `mmcv-lite-2.0.1/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/roiaware_pool3d.py` & `mmcv-lite-2.0.1/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/roipoint_pool3d.py` & `mmcv-lite-2.0.1/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/rotated_feature_align.py` & `mmcv-lite-2.0.1/mmcv/ops/rotated_feature_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/saconv.py` & `mmcv-lite-2.0.1/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/scatter_points.py` & `mmcv-lite-2.0.1/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sparse_conv.py` & `mmcv-lite-2.0.1/mmcv/ops/sparse_conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sparse_functional.py` & `mmcv-lite-2.0.1/mmcv/ops/sparse_functional.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sparse_modules.py` & `mmcv-lite-2.0.1/mmcv/ops/sparse_modules.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sparse_ops.py` & `mmcv-lite-2.0.1/mmcv/ops/sparse_ops.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sparse_pool.py` & `mmcv-lite-2.0.1/mmcv/ops/sparse_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sparse_structure.py` & `mmcv-lite-2.0.1/mmcv/ops/sparse_structure.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/sync_bn.py` & `mmcv-lite-2.0.1/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/three_interpolate.py` & `mmcv-lite-2.0.1/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/three_nn.py` & `mmcv-lite-2.0.1/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/tin_shift.py` & `mmcv-lite-2.0.1/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/ops/voxelize.py` & `mmcv-lite-2.0.1/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/__init__.py` & `mmcv-lite-2.0.1/mmcv/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/base.py` & `mmcv-lite-2.0.1/mmcv/transforms/base.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/formatting.py` & `mmcv-lite-2.0.1/mmcv/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/loading.py` & `mmcv-lite-2.0.1/mmcv/transforms/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,17 @@
             img = mmcv.imfrombytes(
                 img_bytes, flag=self.color_type, backend=self.imdecode_backend)
         except Exception as e:
             if self.ignore_empty:
                 return None
             else:
                 raise e
+        # in some cases, images are not read successfully, the img would be
+        # `None`, refer to https://github.com/open-mmlab/mmpretrain/issues/1427
+        assert img is not None, f'failed to load image: {filename}'
         if self.to_float32:
             img = img.astype(np.float32)
 
         results['img'] = img
         results['img_shape'] = img.shape[:2]
         results['ori_shape'] = img.shape[:2]
         return results
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/processing.py` & `mmcv-lite-2.0.1/mmcv/transforms/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1396,15 +1396,15 @@
 
     - if ``scale`` is a tuple
 
     .. math::
         target\\_scale[0] \\sim Uniform([ratio\\_range[0], ratio\\_range[1]])
             * scale[0]
     .. math::
-        target\\_scale[0] \\sim Uniform([ratio\\_range[0], ratio\\_range[1]])
+        target\\_scale[1] \\sim Uniform([ratio\\_range[0], ratio\\_range[1]])
             * scale[1]
 
     Following the resize order of weight and height in cv2, ``ratio_range[0]``
     is for width, and ``ratio_range[1]`` is for height.
 
     - if ``keep_ratio`` is True, the minimum value of ``target_scale`` will be
       used to set the shorter side and the maximum value will be used to
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/utils.py` & `mmcv-lite-2.0.1/mmcv/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/transforms/wrappers.py` & `mmcv-lite-2.0.1/mmcv/transforms/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     def nullcontext(resource=None):
         try:
             yield resource
         finally:
             pass
 
 
+@TRANSFORMS.register_module()
 class Compose(BaseTransform):
     """Compose multiple transforms sequentially.
 
     Args:
         transforms (list[dict | callable]): Sequence of transform object or
             config dict to be composed.
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/utils/env.py` & `mmcv-lite-2.0.1/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/utils/ext_loader.py` & `mmcv-lite-2.0.1/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/utils/parrots_jit.py` & `mmcv-lite-2.0.1/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/version.py` & `mmcv-lite-2.0.1/mmcv/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '2.0.0rc4'
+__version__ = '2.0.1'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
@@ -26,10 +26,10 @@
     elif version.is_postrelease:
         release.extend(list(version.post))  # type: ignore
     else:
         release.extend([0, 0])
     return tuple(release)
 
 
-version_info = (2, 0, 0, 0, 'rc', 4)
+version_info = tuple(int(x) for x in __version__.split('.')[:3])
 
 __all__ = ['__version__', 'version_info', 'parse_version_info']
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv/video/__init__.py` & `mmcv-lite-2.0.1/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/video/io.py` & `mmcv-lite-2.0.1/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/video/optflow.py` & `mmcv-lite-2.0.1/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/video/processing.py` & `mmcv-lite-2.0.1/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/visualization/color.py` & `mmcv-lite-2.0.1/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/visualization/image.py` & `mmcv-lite-2.0.1/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv/visualization/optflow.py` & `mmcv-lite-2.0.1/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/PKG-INFO` & `mmcv-lite-2.0.1/mmcv_lite.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcv-lite
-Version: 2.0.0rc4
+Version: 2.0.1
 Summary: OpenMMLab Computer Vision Foundation
 Home-page: https://github.com/open-mmlab/mmcv
 Author: MMCV Contributors
 Author-email: openmmlab@gmail.com
 Keywords: computer vision
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmcv-lite-2.0.0rc4/mmcv_lite.egg-info/SOURCES.txt` & `mmcv-lite-2.0.1/mmcv_lite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 mmcv/cnn/bricks/padding.py
 mmcv/cnn/bricks/plugin.py
 mmcv/cnn/bricks/scale.py
 mmcv/cnn/bricks/swish.py
 mmcv/cnn/bricks/transformer.py
 mmcv/cnn/bricks/upsample.py
 mmcv/cnn/bricks/wrappers.py
+mmcv/cnn/rfsearch/__init__.py
+mmcv/cnn/rfsearch/operator.py
+mmcv/cnn/rfsearch/search.py
+mmcv/cnn/rfsearch/utils.py
 mmcv/cnn/utils/__init__.py
 mmcv/cnn/utils/flops_counter.py
 mmcv/cnn/utils/fuse_conv_bn.py
 mmcv/image/__init__.py
 mmcv/image/colorspace.py
 mmcv/image/geometric.py
 mmcv/image/io.py
@@ -44,28 +48,31 @@
 mmcv/image/photometric.py
 mmcv/ops/__init__.py
 mmcv/ops/active_rotated_filter.py
 mmcv/ops/assign_score_withk.py
 mmcv/ops/ball_query.py
 mmcv/ops/bbox.py
 mmcv/ops/bezier_align.py
+mmcv/ops/bias_act.py
 mmcv/ops/border_align.py
 mmcv/ops/box_iou_quadri.py
 mmcv/ops/box_iou_rotated.py
 mmcv/ops/carafe.py
 mmcv/ops/cc_attention.py
 mmcv/ops/chamfer_distance.py
 mmcv/ops/contour_expand.py
+mmcv/ops/conv2d_gradfix.py
 mmcv/ops/convex_iou.py
 mmcv/ops/corner_pool.py
 mmcv/ops/correlation.py
 mmcv/ops/deform_conv.py
 mmcv/ops/deform_roi_pool.py
 mmcv/ops/deprecated_wrappers.py
 mmcv/ops/diff_iou_rotated.py
+mmcv/ops/filtered_lrelu.py
 mmcv/ops/focal_loss.py
 mmcv/ops/furthest_point_sample.py
 mmcv/ops/fused_bias_leakyrelu.py
 mmcv/ops/gather_points.py
 mmcv/ops/group_points.py
 mmcv/ops/info.py
 mmcv/ops/iou3d.py
@@ -161,20 +168,15 @@
 mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/spconv/indice.cuh
 mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
-mmcv/ops/csrc/common/mlu/carafe_utils.hpp
 mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
-mmcv/ops/csrc/common/mlu/iou3d_utils.hpp
-mmcv/ops/csrc/common/mlu/nms_utils.hpp
-mmcv/ops/csrc/common/mlu/psamask_utils.hpp
-mmcv/ops/csrc/common/mlu/roi_align_rotated_utils.hpp
 mmcv/ops/csrc/common/mps/MPSDevice.h
 mmcv/ops/csrc/common/mps/MPSLibrary.h
 mmcv/ops/csrc/common/mps/MPSLibrary.mm
 mmcv/ops/csrc/common/mps/MPSStream.h
 mmcv/ops/csrc/common/mps/MPSUtils.h
 mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
 mmcv/ops/csrc/common/utils/spconv/prettyprint.h
@@ -324,26 +326,28 @@
 mmcv/ops/csrc/parrots/voxelization_parrots.cpp
 mmcv/ops/csrc/parrots/voxelization_pytorch.h
 mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
 mmcv/ops/csrc/pytorch/assign_score_withk.cpp
 mmcv/ops/csrc/pytorch/ball_query.cpp
 mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
 mmcv/ops/csrc/pytorch/bezier_align.cpp
+mmcv/ops/csrc/pytorch/bias_act.cpp
 mmcv/ops/csrc/pytorch/border_align.cpp
 mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
 mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
 mmcv/ops/csrc/pytorch/carafe.cpp
 mmcv/ops/csrc/pytorch/carafe_naive.cpp
 mmcv/ops/csrc/pytorch/chamfer_distance.cpp
 mmcv/ops/csrc/pytorch/contour_expand.cpp
 mmcv/ops/csrc/pytorch/convex_iou.cpp
 mmcv/ops/csrc/pytorch/correlation.cpp
 mmcv/ops/csrc/pytorch/deform_conv.cpp
 mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
 mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
+mmcv/ops/csrc/pytorch/filtered_lrelu.cpp
 mmcv/ops/csrc/pytorch/focal_loss.cpp
 mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
 mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
 mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
 mmcv/ops/csrc/pytorch/gather_points.cpp
 mmcv/ops/csrc/pytorch/group_points.cpp
 mmcv/ops/csrc/pytorch/info.cpp
@@ -376,14 +380,15 @@
 mmcv/ops/csrc/pytorch/sync_bn.cpp
 mmcv/ops/csrc/pytorch/three_interpolate.cpp
 mmcv/ops/csrc/pytorch/three_nn.cpp
 mmcv/ops/csrc/pytorch/tin_shift.cpp
 mmcv/ops/csrc/pytorch/upfirdn2d.cpp
 mmcv/ops/csrc/pytorch/voxelization.cpp
 mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
+mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp
 mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
 mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
 mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
 mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
 mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
 mmcv/ops/csrc/pytorch/cpu/nms.cpp
 mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
@@ -399,26 +404,28 @@
 mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
 mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
 mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
+mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
 mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
 mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
+mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu
 mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
@@ -451,37 +458,51 @@
 mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
 mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
 mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
+mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
 mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
+mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
 mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
 mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
+mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
+mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
 mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
 mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
 mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
+mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
 mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
+mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
 mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
+mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
 mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
+mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
 mmcv/transforms/__init__.py
 mmcv/transforms/base.py
 mmcv/transforms/builder.py
 mmcv/transforms/formatting.py
 mmcv/transforms/loading.py
 mmcv/transforms/processing.py
 mmcv/transforms/utils.py
@@ -501,8 +522,10 @@
 mmcv/visualization/optflow.py
 mmcv_lite.egg-info/PKG-INFO
 mmcv_lite.egg-info/SOURCES.txt
 mmcv_lite.egg-info/dependency_links.txt
 mmcv_lite.egg-info/not-zip-safe
 mmcv_lite.egg-info/requires.txt
 mmcv_lite.egg-info/top_level.txt
-requirements/runtime.txt
+requirements/runtime.txt
+tests/test_arraymisc.py
+tests/test_visualization.py
```

### Comparing `mmcv-lite-2.0.0rc4/setup.cfg` & `mmcv-lite-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.0.0rc4/setup.py` & `mmcv-lite-2.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import glob
 import os
 import platform
 import re
-from pkg_resources import DistributionNotFound, get_distribution
+from pkg_resources import DistributionNotFound, get_distribution, parse_version
 from setuptools import find_packages, setup
 
 EXT_TYPE = ''
 try:
     import torch
     if torch.__version__ == 'parrots':
         from parrots.utils.build_extension import BuildExtension
@@ -149,14 +149,17 @@
         define_macros = []
         include_dirs = []
         op_files = glob.glob('./mmcv/ops/csrc/pytorch/cuda/*.cu') +\
             glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp') +\
             glob.glob('./mmcv/ops/csrc/parrots/*.cpp')
         include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
         include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common/cuda'))
+        op_files.remove('./mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu')
+        op_files.remove('./mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp')
+        op_files.remove('./mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu')
         cuda_args = os.getenv('MMCV_CUDA_ARGS')
         extra_compile_args = {
             'nvcc': [cuda_args, '-std=c++14'] if cuda_args else ['-std=c++14'],
             'cxx': ['-std=c++14'],
         }
         if torch.cuda.is_available() or os.getenv('FORCE_CUDA', '0') == '1':
             define_macros += [('MMCV_WITH_CUDA', None)]
@@ -193,35 +196,65 @@
         # required key passed to PyTorch. Even if there is no flag passed
         # to cxx, users also need to pass an empty list to PyTorch.
         # Since PyTorch1.8.0, it has a default value so users do not need
         # to pass an empty list anymore.
         # More details at https://github.com/pytorch/pytorch/pull/45956
         extra_compile_args = {'cxx': []}
 
-        # Since the PR (https://github.com/open-mmlab/mmcv/pull/1463) uses
-        # c++14 features, the argument ['std=c++14'] must be added here.
-        # However, in the windows environment, some standard libraries
-        # will depend on c++17 or higher. In fact, for the windows
-        # environment, the compiler will choose the appropriate compiler
-        # to compile those cpp files, so there is no need to add the
-        # argument
         if platform.system() != 'Windows':
             extra_compile_args['cxx'] = ['-std=c++14']
+        else:
+            # TODO: In Windows, C++17 is chosen to compile extensions in
+            # PyTorch2.0 , but a compile error will be reported.
+            # As a temporary solution, force the use of C++14.
+            if parse_version(torch.__version__) >= parse_version('2.0.0'):
+                extra_compile_args['cxx'] = ['/std:c++14']
 
         include_dirs = []
+        library_dirs = []
+        libraries = []
 
+        extra_objects = []
+        extra_link_args = []
         is_rocm_pytorch = False
         try:
             from torch.utils.cpp_extension import ROCM_HOME
             is_rocm_pytorch = True if ((torch.version.hip is not None) and
                                        (ROCM_HOME is not None)) else False
         except ImportError:
             pass
 
-        if is_rocm_pytorch or torch.cuda.is_available() or os.getenv(
+        if os.getenv('MMCV_WITH_DIOPI', '0') == '1':
+            import mmengine  # NOQA: F401
+            from mmengine.utils.version_utils import digit_version
+            assert digit_version(mmengine.__version__) >= digit_version(
+                '0.7.4'), f'mmengine >= 0.7.4 is required \
+                but {mmengine.__version__} is installed'
+
+            print(f'Compiling {ext_name} with CPU and DIPU')
+            define_macros += [('MMCV_WITH_DIOPI', None)]
+            define_macros += [('DIOPI_ATTR_WEAK', None)]
+            op_files = glob.glob('./mmcv/ops/csrc/pytorch/*.cpp') + \
+                glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp')
+            extension = CppExtension
+            include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
+            dipu_root = os.getenv('DIPU_ROOT')
+            diopi_path = os.getenv('DIOPI_PATH')
+            dipu_path = os.getenv('DIPU_PATH')
+            vendor_include_dirs = os.getenv('VENDOR_INCLUDE_DIRS')
+            nccl_include_dirs = os.getenv('NCCL_INCLUDE_DIRS')
+            include_dirs.append(dipu_root)
+            include_dirs.append(diopi_path + '/include')
+            include_dirs.append(dipu_path + '/dist/include')
+            include_dirs.append(vendor_include_dirs)
+            if nccl_include_dirs:
+                include_dirs.append(nccl_include_dirs)
+            library_dirs += [dipu_root]
+            libraries += ['torch_dipu']
+        elif is_rocm_pytorch or torch.cuda.is_available() or os.getenv(
                 'FORCE_CUDA', '0') == '1':
             if is_rocm_pytorch:
                 define_macros += [('MMCV_WITH_HIP', None)]
             define_macros += [('MMCV_WITH_CUDA', None)]
             cuda_args = os.getenv('MMCV_CUDA_ARGS')
             extra_compile_args['nvcc'] = [cuda_args] if cuda_args else []
             op_files = glob.glob('./mmcv/ops/csrc/pytorch/*.cpp') + \
@@ -232,24 +265,109 @@
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/pytorch'))
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common/cuda'))
         elif (hasattr(torch, 'is_mlu_available') and
                 torch.is_mlu_available()) or \
                 os.getenv('FORCE_MLU', '0') == '1':
             from torch_mlu.utils.cpp_extension import MLUExtension
+
+            def get_mluops_version(file_path):
+                with open(file_path) as f:
+                    for line in f:
+                        if re.search('MLUOP_MAJOR', line):
+                            major = line.strip().split(' ')[2]
+                        if re.search('MLUOP_MINOR', line):
+                            minor = line.strip().split(' ')[2]
+                        if re.search('MLUOP_PATCHLEVEL', line):
+                            patchlevel = line.strip().split(' ')[2]
+                mluops_version = f'v{major}.{minor}.{patchlevel}'
+                return mluops_version
+
+            mmcv_mluops_version = get_mluops_version(
+                './mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h')
+            mlu_ops_path = os.getenv('MMCV_MLU_OPS_PATH')
+            if mlu_ops_path:
+                exists_mluops_version = get_mluops_version(
+                    mlu_ops_path + '/bangc-ops/mlu_op.h')
+                if exists_mluops_version != mmcv_mluops_version:
+                    print('the version of mlu-ops provided is %s,'
+                          ' while %s is needed.' %
+                          (exists_mluops_version, mmcv_mluops_version))
+                    exit()
+                try:
+                    if os.path.exists('mlu-ops'):
+                        if os.path.islink('mlu-ops'):
+                            os.remove('mlu-ops')
+                            os.symlink(mlu_ops_path, 'mlu-ops')
+                        elif os.path.abspath('mlu-ops') != mlu_ops_path:
+                            os.symlink(mlu_ops_path, 'mlu-ops')
+                    else:
+                        os.symlink(mlu_ops_path, 'mlu-ops')
+                except Exception:
+                    raise FileExistsError(
+                        'mlu-ops already exists, please move it out,'
+                        'or rename or remove it.')
+            else:
+                if not os.path.exists('mlu-ops'):
+                    import requests
+                    mluops_url = 'https://github.com/Cambricon/mlu-ops/' + \
+                        'archive/refs/tags/' + mmcv_mluops_version + '.zip'
+                    req = requests.get(mluops_url)
+                    with open('./mlu-ops.zip', 'wb') as f:
+                        try:
+                            f.write(req.content)
+                        except Exception:
+                            raise ImportError('failed to download mlu-ops')
+
+                    from zipfile import BadZipFile, ZipFile
+                    with ZipFile('./mlu-ops.zip', 'r') as archive:
+                        try:
+                            archive.extractall()
+                            dir_name = archive.namelist()[0].split('/')[0]
+                            os.rename(dir_name, 'mlu-ops')
+                        except BadZipFile:
+                            print('invalid mlu-ops.zip file')
+                else:
+                    exists_mluops_version = get_mluops_version(
+                        './mlu-ops/bangc-ops/mlu_op.h')
+                    if exists_mluops_version != mmcv_mluops_version:
+                        print('the version of provided mlu-ops is %s,'
+                              ' while %s is needed.' %
+                              (exists_mluops_version, mmcv_mluops_version))
+                        exit()
+
             define_macros += [('MMCV_WITH_MLU', None)]
-            mlu_args = os.getenv('MMCV_MLU_ARGS')
-            extra_compile_args['cncc'] = [mlu_args] if mlu_args else []
+            mlu_args = os.getenv('MMCV_MLU_ARGS', '-DNDEBUG ')
+            mluops_includes = []
+            mluops_includes.append('-I' +
+                                   os.path.abspath('./mlu-ops/bangc-ops'))
+            mluops_includes.append(
+                '-I' + os.path.abspath('./mlu-ops/bangc-ops/kernels'))
+            extra_compile_args['cncc'] = [mlu_args] + \
+                mluops_includes if mlu_args else mluops_includes
+            extra_compile_args['cxx'] += ['-fno-gnu-unique']
             op_files = glob.glob('./mmcv/ops/csrc/pytorch/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/pytorch/mlu/*.cpp') + \
-                glob.glob('./mmcv/ops/csrc/common/mlu/*.mlu')
+                glob.glob('./mmcv/ops/csrc/common/mlu/*.mlu') + \
+                glob.glob(
+                    './mlu-ops/bangc-ops/core/**/*.cpp', recursive=True) + \
+                glob.glob(
+                    './mlu-ops/bangc-ops/kernels/**/*.cpp', recursive=True) + \
+                glob.glob(
+                    './mlu-ops/bangc-ops/kernels/**/*.mlu', recursive=True)
+            extra_link_args = [
+                '-Wl,--whole-archive',
+                './mlu-ops/bangc-ops/kernels/kernel_wrapper/lib/libextops.a',
+                '-Wl,--no-whole-archive'
+            ]
             extension = MLUExtension
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common/mlu'))
+            include_dirs.append(os.path.abspath('./mlu-ops/bangc-ops'))
         elif (hasattr(torch.backends, 'mps')
               and torch.backends.mps.is_available()) or os.getenv(
                   'FORCE_MPS', '0') == '1':
             # objc compiler support
             from distutils.unixccompiler import UnixCCompiler
             if '.mm' not in UnixCCompiler.src_extensions:
                 UnixCCompiler.src_extensions.append('.mm')
@@ -303,15 +421,19 @@
             extra_compile_args['nvcc'] += ['-std=c++14']
 
         ext_ops = extension(
             name=ext_name,
             sources=op_files,
             include_dirs=include_dirs,
             define_macros=define_macros,
-            extra_compile_args=extra_compile_args)
+            extra_objects=extra_objects,
+            extra_compile_args=extra_compile_args,
+            library_dirs=library_dirs,
+            libraries=libraries,
+            extra_link_args=extra_link_args)
         extensions.append(ext_ops)
     return extensions
 
 
 setup(
     name='mmcv' if os.getenv('MMCV_WITH_OPS', '0') == '1' else 'mmcv-lite',
     version=get_version(),
```

