# Comparing `tmp/intel_extension_for_deepspeed-0.1.dev20230613-py3-none-any.whl.zip` & `tmp/intel_extension_for_deepspeed-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,69 +1,75 @@
-Zip file size: 109220 bytes, number of entries: 67
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/__init__.py
--rw-r--r--  2.0 unx     7299 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/xpu_accelerator.py
--rwxr-xr-x  2.0 unx      320 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/__init__.py
--rw-r--r--  2.0 unx     6974 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/builder.py
--rw-r--r--  2.0 unx      752 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/cpu_adagrad.py
--rw-r--r--  2.0 unx      810 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/cpu_adam.py
--rw-r--r--  2.0 unx      845 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/fused_adam.py
--rw-r--r--  2.0 unx      475 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/quantizer.py
--rw-r--r--  2.0 unx     1952 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/transformer.py
--rwxr-xr-x  2.0 unx     1285 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/transformer_inference.py
--rw-r--r--  2.0 unx      553 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/utils.py
--rw-r--r--  2.0 unx     7481 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/adagrad/cpu_adagrad.dp.cpp
--rw-r--r--  2.0 unx    34107 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/adam/cpu_adam.dp.cpp
--rw-r--r--  2.0 unx     1007 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/adam/custom_sycl_kernel.dp.cpp
--rw-r--r--  2.0 unx      781 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--  2.0 unx     8589 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/adam/multi_tensor_adam.dp.cpp
--rw-r--r--  2.0 unx     1259 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/Timer.hpp
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/common.hpp
--rw-r--r--  2.0 unx     5015 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/context.hpp
--rw-r--r--  2.0 unx     2183 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/cpu_adagrad.hpp
--rw-r--r--  2.0 unx     4675 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/cpu_adam.hpp
--rw-r--r--  2.0 unx    11342 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/custom_sycl_layers.hpp
--rw-r--r--  2.0 unx     2250 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/dropout.hpp
--rw-r--r--  2.0 unx     6100 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/ds_transformer_sycl.hpp
--rw-r--r--  2.0 unx     4392 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/feed_forward.hpp
--rw-r--r--  2.0 unx     1041 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/gelu.hpp
--rw-r--r--  2.0 unx     9971 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/gemm_test.hpp
--rw-r--r--  2.0 unx     1243 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/general_kernels.hpp
--rw-r--r--  2.0 unx     8611 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/multi_tensor_apply.dp.hpp
--rw-r--r--  2.0 unx     7050 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/normalize_layer.hpp
--rw-r--r--  2.0 unx     1134 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/onednn_wrappers.hpp
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/onemkl_wrappers.hpp
--rw-r--r--  2.0 unx     1640 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/softmax.hpp
--rw-r--r--  2.0 unx     9923 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/strided_batch_gemm.hpp
--rw-r--r--  2.0 unx     5770 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/includes/type_shim.hpp
--rw-r--r--  2.0 unx    44729 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/dropout_kernels.dp.cpp
--rw-r--r--  2.0 unx     3614 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_dropout_sycl.dp.cpp
--rw-r--r--  2.0 unx     3033 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_feedforward_sycl.dp.cpp
--rw-r--r--  2.0 unx     1595 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_gelu_sycl.dp.cpp
--rw-r--r--  2.0 unx     4685 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_layer_reorder_sycl.dp.cpp
--rw-r--r--  2.0 unx     6224 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_normalize_sycl.dp.cpp
--rw-r--r--  2.0 unx     1568 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_softmax_sycl.dp.cpp
--rw-r--r--  2.0 unx     4387 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_stridedbatchgemm_sycl.dp.cpp
--rw-r--r--  2.0 unx    48959 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_transformer_sycl.dp.cpp
--rw-r--r--  2.0 unx    17623 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/gelu_kernels.dp.cpp
--rw-r--r--  2.0 unx    20424 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/general_kernels.dp.cpp
--rw-r--r--  2.0 unx   107734 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/normalize_kernels.dp.cpp
--rw-r--r--  2.0 unx     4454 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/onednn_wrappers.dp.cpp
--rw-r--r--  2.0 unx     6030 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/onemkl_wrappers.dp.cpp
--rw-r--r--  2.0 unx    35537 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/softmax_kernels.dp.cpp
--rw-r--r--  2.0 unx    38144 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/transform_kernels.dp.cpp
--rw-r--r--  2.0 unx    13069 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/gelu.cpp
--rw-r--r--  2.0 unx     9623 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onednn_wrappers.cpp
--rw-r--r--  2.0 unx     5341 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp
--rw-r--r--  2.0 unx    17804 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/layer_norm.cpp
--rw-r--r--  2.0 unx    30737 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--  2.0 unx    26518 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/softmax.cpp
--rw-r--r--  2.0 unx     6136 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/dnnl_ext.hpp
--rw-r--r--  2.0 unx     7692 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_context.hpp
--rw-r--r--  2.0 unx      933 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onednn_wrappers.hpp
--rw-r--r--  2.0 unx     1292 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onemkl_wrappers.hpp
--rw-r--r--  2.0 unx     9833 b- defN 23-Jun-14 05:08 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/lru_cache.hpp
--rw-r--r--  2.0 unx     1074 b- defN 23-Jun-14 05:12 intel_extension_for_deepspeed-0.1.dev20230613.dist-info/LICENSE
--rw-r--r--  2.0 unx      171 b- defN 23-Jun-14 05:12 intel_extension_for_deepspeed-0.1.dev20230613.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 05:12 intel_extension_for_deepspeed-0.1.dev20230613.dist-info/WHEEL
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-14 05:12 intel_extension_for_deepspeed-0.1.dev20230613.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8697 b- defN 23-Jun-14 05:12 intel_extension_for_deepspeed-0.1.dev20230613.dist-info/RECORD
-67 files, 648183 bytes uncompressed, 94238 bytes compressed:  85.5%
+Zip file size: 120094 bytes, number of entries: 73
+-rw-rw-r--  2.0 unx       45 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/__init__.py
+-rw-rw-r--  2.0 unx     7299 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/xpu_accelerator.py
+-rwxrwxr-x  2.0 unx      320 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/__init__.py
+-rw-rw-r--  2.0 unx     7188 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/builder.py
+-rw-rw-r--  2.0 unx      752 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/cpu_adagrad.py
+-rw-rw-r--  2.0 unx      810 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/cpu_adam.py
+-rw-rw-r--  2.0 unx      845 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/fused_adam.py
+-rw-rw-r--  2.0 unx      475 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/quantizer.py
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/transformer.py
+-rwxrwxr-x  2.0 unx     1320 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/transformer_inference.py
+-rw-rw-r--  2.0 unx      553 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/utils.py
+-rw-rw-r--  2.0 unx     7481 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/adagrad/cpu_adagrad.dp.cpp
+-rw-rw-r--  2.0 unx    34107 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/adam/cpu_adam.dp.cpp
+-rw-rw-r--  2.0 unx     1007 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/adam/custom_sycl_kernel.dp.cpp
+-rw-rw-r--  2.0 unx      781 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/adam/fused_adam_frontend.cpp
+-rw-rw-r--  2.0 unx     8589 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/adam/multi_tensor_adam.dp.cpp
+-rw-rw-r--  2.0 unx     1259 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/Timer.hpp
+-rw-rw-r--  2.0 unx      926 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/common.hpp
+-rw-rw-r--  2.0 unx     5015 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/context.hpp
+-rw-rw-r--  2.0 unx     2183 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/cpu_adagrad.hpp
+-rw-rw-r--  2.0 unx     4675 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/cpu_adam.hpp
+-rw-rw-r--  2.0 unx    11342 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/custom_sycl_layers.hpp
+-rw-rw-r--  2.0 unx     2250 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/dropout.hpp
+-rw-rw-r--  2.0 unx     6100 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/ds_transformer_sycl.hpp
+-rw-rw-r--  2.0 unx     4392 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/feed_forward.hpp
+-rw-rw-r--  2.0 unx     1041 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/gelu.hpp
+-rw-rw-r--  2.0 unx     9971 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/gemm_test.hpp
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/general_kernels.hpp
+-rw-rw-r--  2.0 unx     8611 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/multi_tensor_apply.dp.hpp
+-rw-rw-r--  2.0 unx     7050 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/normalize_layer.hpp
+-rw-rw-r--  2.0 unx     1134 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/onednn_wrappers.hpp
+-rw-rw-r--  2.0 unx     2601 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/onemkl_wrappers.hpp
+-rw-rw-r--  2.0 unx     1640 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/softmax.hpp
+-rw-rw-r--  2.0 unx     9923 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/strided_batch_gemm.hpp
+-rw-rw-r--  2.0 unx     5770 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/includes/type_shim.hpp
+-rw-rw-r--  2.0 unx    44729 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/dropout_kernels.dp.cpp
+-rw-rw-r--  2.0 unx     3614 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_dropout_sycl.dp.cpp
+-rw-rw-r--  2.0 unx     3033 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_feedforward_sycl.dp.cpp
+-rw-rw-r--  2.0 unx     1595 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_gelu_sycl.dp.cpp
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_layer_reorder_sycl.dp.cpp
+-rw-rw-r--  2.0 unx     6224 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_normalize_sycl.dp.cpp
+-rw-rw-r--  2.0 unx     1568 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_softmax_sycl.dp.cpp
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_stridedbatchgemm_sycl.dp.cpp
+-rw-rw-r--  2.0 unx    48959 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/ds_transformer_sycl.dp.cpp
+-rw-rw-r--  2.0 unx    17623 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/gelu_kernels.dp.cpp
+-rw-rw-r--  2.0 unx    20424 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/general_kernels.dp.cpp
+-rw-rw-r--  2.0 unx   107734 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/normalize_kernels.dp.cpp
+-rw-rw-r--  2.0 unx     4454 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/onednn_wrappers.dp.cpp
+-rw-rw-r--  2.0 unx     6030 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/onemkl_wrappers.dp.cpp
+-rw-rw-r--  2.0 unx    35537 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/softmax_kernels.dp.cpp
+-rw-rw-r--  2.0 unx    38144 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/transform_kernels.dp.cpp
+-rw-rw-r--  2.0 unx    13077 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/gelu.cpp
+-rw-rw-r--  2.0 unx     9625 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onednn_wrappers.cpp
+-rw-rw-r--  2.0 unx     5343 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp
+-rw-rw-r--  2.0 unx    17814 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/layer_norm.cpp
+-rw-rw-r--  2.0 unx     2760 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pointwise_ops.cpp
+-rw-rw-r--  2.0 unx    31783 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-rw-r--  2.0 unx    26524 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/softmax.cpp
+-rw-rw-r--  2.0 unx     2004 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/compatible.hpp
+-rw-rw-r--  2.0 unx     8412 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/conversion_utils.hpp
+-rw-rw-r--  2.0 unx     6136 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/dnnl_ext.hpp
+-rw-rw-r--  2.0 unx     7694 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_context.hpp
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onednn_wrappers.hpp
+-rw-rw-r--  2.0 unx     1292 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onemkl_wrappers.hpp
+-rw-rw-r--  2.0 unx     2680 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_sycl_layers.hpp
+-rw-rw-r--  2.0 unx     9833 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/lru_cache.hpp
+-rw-rw-r--  2.0 unx    15298 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/memory_access_utils.hpp
+-rw-rw-r--  2.0 unx    16305 b- defN 23-Jun-29 08:46 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/reduction_utils.hpp
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-29 08:47 intel_extension_for_deepspeed-0.9.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2035 b- defN 23-Jun-29 08:47 intel_extension_for_deepspeed-0.9.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 08:47 intel_extension_for_deepspeed-0.9.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       30 b- defN 23-Jun-29 08:47 intel_extension_for_deepspeed-0.9.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9568 b- defN 23-Jun-29 08:47 intel_extension_for_deepspeed-0.9.4.dist-info/RECORD
+73 files, 699702 bytes uncompressed, 103604 bytes compressed:  85.2%
```

## zipnote {}

```diff
@@ -159,44 +159,62 @@
 
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp
 Comment: 
 
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/layer_norm.cpp
 Comment: 
 
+Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pointwise_ops.cpp
+Comment: 
+
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pt_binding.cpp
 Comment: 
 
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/softmax.cpp
 Comment: 
 
+Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/compatible.hpp
+Comment: 
+
+Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/conversion_utils.hpp
+Comment: 
+
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/dnnl_ext.hpp
 Comment: 
 
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_context.hpp
 Comment: 
 
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onednn_wrappers.hpp
 Comment: 
 
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onemkl_wrappers.hpp
 Comment: 
 
+Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_sycl_layers.hpp
+Comment: 
+
 Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/lru_cache.hpp
 Comment: 
 
-Filename: intel_extension_for_deepspeed-0.1.dev20230613.dist-info/LICENSE
+Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/memory_access_utils.hpp
+Comment: 
+
+Filename: intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/reduction_utils.hpp
+Comment: 
+
+Filename: intel_extension_for_deepspeed-0.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: intel_extension_for_deepspeed-0.1.dev20230613.dist-info/METADATA
+Filename: intel_extension_for_deepspeed-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: intel_extension_for_deepspeed-0.1.dev20230613.dist-info/WHEEL
+Filename: intel_extension_for_deepspeed-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: intel_extension_for_deepspeed-0.1.dev20230613.dist-info/top_level.txt
+Filename: intel_extension_for_deepspeed-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: intel_extension_for_deepspeed-0.1.dev20230613.dist-info/RECORD
+Filename: intel_extension_for_deepspeed-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## intel_extension_for_deepspeed/op_builder/builder.py

```diff
@@ -42,22 +42,22 @@
     def cxx_args(self):
         cxx_flags = ['-fsycl', '-fsycl-targets=spir64_gen', '-g', '-gdwarf-4', '-O3', '-std=c++17', '-fPIC', '-DMKL_ILP64', '-fno-strict-aliasing']
         if os.environ.get('USE_MKL_GEMM'):
             cxx_flags.append('-DUSE_MKL_GEMM')
         return cxx_flags
 
     def extra_ldflags(self):
-        return ['-fPIC', '-Wl,-export-dynamic']
+        return ['-fPIC', '-fsycl', '-fsycl-targets=spir64_gen', '-fsycl-max-parallel-link-jobs=8', '-Xs "-options -cl-poison-unsupported-fp64-kernels,cl-intel-enable-auto-large-GRF-mode"', '-Xs "-device pvc"', '-Wl,-export-dynamic']
 
     def fixed_aotflags(self):
         return ['-fsycl', '-fsycl-targets=spir64_gen', '-fsycl-max-parallel-link-jobs=8', '-Xs', "-options -cl-poison-unsupported-fp64-kernels,cl-intel-enable-auto-large-GRF-mode", '-Xs', "-device pvc"]
 
     def load(self, verbose=True):
         from deepspeed.git_version_info import installed_ops, torch_info  # noqa: F401
-        if installed_ops[self.name]:
+        if installed_ops.get(self.name, False):
             return importlib.import_module(self.absolute_name())
         else:
             return self.jit_load(verbose)
 
     def jit_load(self, verbose=True):
         if not self.is_compatible(verbose):
             raise RuntimeError(
@@ -130,15 +130,15 @@
         SYCL_KERNEL_PATH)
     if not os.path.exists(sycl_link_path):
         # Create directory and link for sycl kernel:
         #   deepspeed/ops/SYCL_KERNEL_PATH-->../../SYCL_KERNEL_PATH
         sycl_dir_path = os.path.join(os.path.dirname(sycl_link_path),
                                      "../../" + SYCL_KERNEL_PATH)
 
-        os.mkdir(sycl_dir_path)
+        os.makedirs(sycl_dir_path, exist_ok=True)
         os.symlink("../../" + SYCL_KERNEL_PATH, sycl_link_path, True)
         print("Create directory and link for sycl kernel:{}-->{}".format(
             sycl_link_path,
             sycl_dir_path))
 
     import filecmp
     if (os.path.exists(abs_target_path) and filecmp.cmp(abs_target_path,
```

## intel_extension_for_deepspeed/op_builder/transformer_inference.py

```diff
@@ -19,16 +19,14 @@
         return [
             sycl_kernel_path('csrc/transformer/inference/csrc/softmax.cpp'),
             sycl_kernel_path('csrc/transformer/inference/csrc/pt_binding.cpp'),
             sycl_kernel_path('csrc/transformer/inference/csrc/gelu.cpp'),
             sycl_kernel_path('csrc/transformer/inference/csrc/inference_onednn_wrappers.cpp'),
             sycl_kernel_path('csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp'),
             sycl_kernel_path('csrc/transformer/inference/csrc/layer_norm.cpp'),
+            sycl_kernel_path('csrc/transformer/inference/csrc/pointwise_ops.cpp'),
         ]
 
-    def extra_ldflags(self):
-        return []
-
     def include_paths(self):
         includes = [sycl_kernel_include('csrc/transformer/inference/includes'), 'csrc/transformer/inference/includes']
         return includes
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/gelu.cpp

```diff
@@ -1,15 +1,15 @@
 /*
 Copyright 2022 The Microsoft DeepSpeed Team
 */
 
-#include "compatible.h"
-#include "conversion_utils.h"
-#include "memory_access_utils.h"
-#include "inference_sycl_layers.h"
+#include "compatible.hpp"
+#include "conversion_utils.hpp"
+#include "memory_access_utils.hpp"
+#include "inference_sycl_layers.hpp"
 
 #define MAX_CAP 4
 #define MAX_SEQ 2048
 
 inline float gelu(const float x) {
   const float sqrt_param = 0.79788456080286535587989211986876f;
   const float mul_param = 0.044715;
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onednn_wrappers.cpp

```diff
@@ -1,10 +1,10 @@
 #include <ATen/ATen.h>
 #include "inference_onednn_wrappers.hpp"
-#include "inference_sycl_layers.h"
+#include "inference_sycl_layers.hpp"
 
 struct hash_pair {
   static size_t hash_combine( size_t lhs, size_t rhs ) {
     lhs ^= rhs + 0x9e3779b9 + (lhs << 6) + (lhs >> 2);
     return lhs;
   }
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp

```diff
@@ -1,10 +1,10 @@
 #include <ATen/ATen.h>
 #include "inference_onemkl_wrappers.hpp"
-#include "inference_sycl_layers.h"
+#include "inference_sycl_layers.hpp"
 
 
 template <typename T>
 int onemkl_matmul_ex(sycl::queue handle,
                    oneapi::mkl::transpose transa,
                    oneapi::mkl::transpose transb,
                    int m,
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/layer_norm.cpp

```diff
@@ -1,16 +1,16 @@
 /*
 Copyright 2022 The Microsoft DeepSpeed Team
 */
 
-#include "compatible.h"
-#include "conversion_utils.h"
-#include "memory_access_utils.h"
-#include "reduction_utils.h"
-#include "inference_sycl_layers.h"
+#include "compatible.hpp"
+#include "conversion_utils.hpp"
+#include "memory_access_utils.hpp"
+#include "reduction_utils.hpp"
+#include "inference_sycl_layers.hpp"
 
 using rop = reduce::ROpType;
 
 namespace ln {
 constexpr int granularity = 16;
 } // namespace ln
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pt_binding.cpp

```diff
@@ -1,15 +1,15 @@
 #include <torch/extension.h>
 #include <stdexcept>
 #include <vector>
-#include "compatible.h"
+#include "compatible.hpp"
 #include "inference_context.hpp"
 #include "inference_onednn_wrappers.hpp"
 #include "inference_onemkl_wrappers.hpp"
-#include "inference_sycl_layers.h"
+#include "inference_sycl_layers.hpp"
 
 // NOTE: This activation function type enum should be always in sync
 // with the python counterpart, otherwise the casting from python binding
 // will be incorrect.
 enum class ActivationFuncType { UNKNOWN = 0, GELU = 1, ReLU = 2 };
 
 enum class TransformerType : uint8_t { UNKNOWN = 0, GPTType = 1, BERTType = 2 };
@@ -685,17 +685,41 @@
                             (T*)weight.data_ptr(),
                             (T*)output.data_ptr());
 #endif
     }
     return output;
 }
 
+#define DISPATCH_VECTOR_ADD(T_TYPE, C_TYPE)                                         \
+    if (a.scalar_type() == at::k##T_TYPE) {                                         \
+        launch_vector_add<C_TYPE>((C_TYPE*)(a.data_ptr()),                          \
+                                  (const C_TYPE*)(a.data_ptr()),                    \
+                                  (const C_TYPE*)(b.data_ptr()),                    \
+                                  gamma,                                            \
+                                  total_elems,                                      \
+                                  InferenceContext::Instance().GetCurrentStream()); \
+    }
+
+at::Tensor& _vector_add(at::Tensor& a, at::Tensor& b, float gamma)
+{
+    const int total_elems = a.numel();
+
+    DISPATCH_VECTOR_ADD(Float, float)
+    DISPATCH_VECTOR_ADD(Half, sycl::half)
+#ifdef BF16_AVAILABLE
+    DISPATCH_VECTOR_ADD(BFloat16, bf16)
+#endif
+
+    return a;
+}
+
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
     m.def("layer_norm", &ds_layer_norm, "DeepSpeed layer norm (SYCL)");
+    m.def("_vector_add", &_vector_add, "DeepSpeed vector add (SYCL)");
     m.def(
         "_layer_norm_residual", &ds_layer_norm_residual, "DeepSpeed layer norm + residual (SYCL)");
 
 #define DEF_OPS(_name, _dtype)                                                                    \
     m.def("softmax_" #_name, &ds_softmax<_dtype>, "DeepSpeed SoftMax with " #_name " (SYCL)");    \
     m.def("layer_norm_" #_name, &ds_layer_norm_test<_dtype>, "DeepSpeed layer norm (SYCL)");      \
     m.def("qkv_gemm_" #_name, &ds_qkv_gemm<_dtype>, "DeepSpeed qkv gemm with " #_name " (SYCL)"); \
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/softmax.cpp

```diff
@@ -1,14 +1,14 @@
 /*
 Copyright 2022 The Microsoft DeepSpeed Team
 */
 
-#include "compatible.h"
-#include "conversion_utils.h"
-#include "inference_sycl_layers.h"
+#include "compatible.hpp"
+#include "conversion_utils.hpp"
+#include "inference_sycl_layers.hpp"
 
 #define MAX_REG_SIZE 8
 #define minus_infinity -10000.0
 
 template <typename T, int iterations>
 class attn_softmax_v2 {
 private:
```

## intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_context.hpp

```diff
@@ -7,15 +7,15 @@
 #include <torch/library.h>
 #include <cassert>
 #include <iostream>
 #include <oneapi/mkl.hpp>
 #include <oneapi/mkl/rng/device.hpp>
 #include <vector>
 
-#include "compatible.h"
+#include "compatible.hpp"
 
 #define MEGABYTE (1024 * 1024)
 #define GIGABYTE (1024 * 1024 * 1024)
 
 #define WARP_SIZE 32
 #define ONEMKL_OP_T oneapi::mkl::transpose::trans
 #define ONEMKL_OP_N oneapi::mkl::transpose::nontrans
```

## Comparing `intel_extension_for_deepspeed-0.1.dev20230613.dist-info/LICENSE` & `intel_extension_for_deepspeed-0.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intel_extension_for_deepspeed-0.1.dev20230613.dist-info/RECORD` & `intel_extension_for_deepspeed-0.9.4.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 intel_extension_for_deepspeed/__init__.py,sha256=eRXXGht7jJuSYtwPiAj2FFomy1E7Cl-942LV1Rh5yP8,45
 intel_extension_for_deepspeed/xpu_accelerator.py,sha256=q0A2pJEI_gD_0aK0NA6rAVchmsKGT94hz-Sl1mp805Q,7299
 intel_extension_for_deepspeed/op_builder/__init__.py,sha256=ZnNT45UrFIpDyTDMN3qd1W1S-Wt6K4eLhQAAFXuwXwc,320
-intel_extension_for_deepspeed/op_builder/builder.py,sha256=RJA9yz9hBt7NDvjVHL4shWbvnqNFQUDUtnd59JxLwLA,6974
+intel_extension_for_deepspeed/op_builder/builder.py,sha256=_p1XMztAda57s03LUujfnvWZL_FVW63w14kdJQO_Di8,7188
 intel_extension_for_deepspeed/op_builder/cpu_adagrad.py,sha256=utJC5S6Kje42LtOeQjNx_P_-v0nUpmAN7CWtzJ5J4bY,752
 intel_extension_for_deepspeed/op_builder/cpu_adam.py,sha256=gHbFS7INlZvoQGw0N5GaAZxBZ_DlPh9NHyqiz_OU4M8,810
 intel_extension_for_deepspeed/op_builder/fused_adam.py,sha256=Sc6rQ92OBFuoMTkQi5DI2cArBwj8cFEqWvv4HOakymw,845
 intel_extension_for_deepspeed/op_builder/quantizer.py,sha256=Jr0blK6pg5M9EOKnx14AEwuJtHiNzIdzo6t4Y5Snuoc,475
 intel_extension_for_deepspeed/op_builder/transformer.py,sha256=uyQLI7qnkfRQjXiMBJtcN83BQKCv0gZbRLudDu3LdEY,1952
-intel_extension_for_deepspeed/op_builder/transformer_inference.py,sha256=g3Exz1mB4PfrkIqH_wbOMt3Ovb3Q8K0wntqG4wFhnpw,1285
+intel_extension_for_deepspeed/op_builder/transformer_inference.py,sha256=Kawvd-aTEScN2bPZZHCrk_O_B9C_XQl5tS9xhwiXZLY,1320
 intel_extension_for_deepspeed/op_builder/utils.py,sha256=J2_e1m856JLlXUUdNqmo68-XVDhsB_LrhT7OATD2tU4,553
 intel_extension_for_deepspeed/op_builder/csrc/adagrad/cpu_adagrad.dp.cpp,sha256=ASt1bkWBZQ4hjMioOB50Q2UeG_FPTit78DAempnMnaQ,7481
 intel_extension_for_deepspeed/op_builder/csrc/adam/cpu_adam.dp.cpp,sha256=S-GZeijHUv2KQq_yc8xLq6kbWkvM9S90AGVgIlvQKKw,34107
 intel_extension_for_deepspeed/op_builder/csrc/adam/custom_sycl_kernel.dp.cpp,sha256=zrjPsCQwxvC0intZ7w48aueFR3Y3wq6DzWGzbuWegjw,1007
 intel_extension_for_deepspeed/op_builder/csrc/adam/fused_adam_frontend.cpp,sha256=aej8fOlCteij8LmoBffBRygnzQ8PeHBE1i1UKn9LOyQ,781
 intel_extension_for_deepspeed/op_builder/csrc/adam/multi_tensor_adam.dp.cpp,sha256=coV7QtvotuQQHMtnbAIVP00RMoh2j_7OwplnHBlItig,8589
 intel_extension_for_deepspeed/op_builder/csrc/includes/Timer.hpp,sha256=WJgv-LUkB2h0s93vTccwrRtG_8xp4tJVJq8VwT986Zc,1259
@@ -45,23 +45,29 @@
 intel_extension_for_deepspeed/op_builder/csrc/transformer/gelu_kernels.dp.cpp,sha256=47MMgCFZgw0PakMd1GWhPNDQxgRls-Le1yXPB9c0FwE,17623
 intel_extension_for_deepspeed/op_builder/csrc/transformer/general_kernels.dp.cpp,sha256=wcHJtAAd2HNsgGpSE9NS9iFZDEwrA72CRT1bZRUoh60,20424
 intel_extension_for_deepspeed/op_builder/csrc/transformer/normalize_kernels.dp.cpp,sha256=uqc4EzgZQpqtJKaQtPtq0qkQeCWtpwrSnBbetYJOrBA,107734
 intel_extension_for_deepspeed/op_builder/csrc/transformer/onednn_wrappers.dp.cpp,sha256=RmP1Xdp2-dr62thsYgZwoLDaZnmCd6Cc_WZwX9GEQTI,4454
 intel_extension_for_deepspeed/op_builder/csrc/transformer/onemkl_wrappers.dp.cpp,sha256=aPtWf-x4VSsRWkkbSN5pgY68Y38bwarasyS4Eps9R_8,6030
 intel_extension_for_deepspeed/op_builder/csrc/transformer/softmax_kernels.dp.cpp,sha256=y3XaCKLhLMtxKNQixYgOFThz0x4UcDqPDuRpYXM3Ek8,35537
 intel_extension_for_deepspeed/op_builder/csrc/transformer/transform_kernels.dp.cpp,sha256=g0MiZI7E-CLExdTreH18b5Z2GLyftyM-_oP2M6xc89o,38144
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/gelu.cpp,sha256=OBOiGQcs_JFLGnoGwvZaj74jtCFOa-Y8CY42QDOz4Rs,13069
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onednn_wrappers.cpp,sha256=a7kPk21uMGjMIDSJPJrNRXuL0lQi2gw4haK49ulS-zY,9623
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp,sha256=CN6GZOlDQg3rVI3Ech_L4MbrN0Lo0qiW6lhpI8G2jvo,5341
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/layer_norm.cpp,sha256=wwr2dAwQ9cCgny4Ngy1iP4i6CqK6V6tXBwX7-eDcPec,17804
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pt_binding.cpp,sha256=Ow6kjSk7xGy2o_W8kFaMycgtrBK-4W20PSiGNn84IZY,30737
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/softmax.cpp,sha256=etjY3oMFYlP4dcWit4Kgjnqz6j8A5A1MAfofn74Ylz0,26518
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/gelu.cpp,sha256=01QLGqe0Va3kXzyaB6rkFQER5zcYl-f24Ll_ekbQPBc,13077
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onednn_wrappers.cpp,sha256=1tF9qQPRcmiijnlAWj48OyfelDP1CDLHbLvrIG2aJFA,9625
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/inference_onemkl_wrappers.cpp,sha256=srNBugmsi3ZC14AWULTwrb8ajgZ1hZ5hItjeF4ZJaQA,5343
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/layer_norm.cpp,sha256=vbhzkI7Ft4vb_ZkZ_WpadlYd3a9AkVVArmaS4-7ZMw8,17814
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pointwise_ops.cpp,sha256=hkCQAST8hqaQ69nS4ttwKKm8aT2fh-me0CnZMH-1PP8,2760
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/pt_binding.cpp,sha256=fdkDFOYXceaY7RuzFjXoNSJbZrmtvH1iGablDytD480,31783
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/csrc/softmax.cpp,sha256=OkpaVqHct8yOpeXOai0ifzmMY79Cg-GTid3r3COGcuI,26524
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/compatible.hpp,sha256=lp83O5GQ5GFspxyUGEcw5SBc-wCDgr9sUsM35vismDs,2004
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/conversion_utils.hpp,sha256=ekheG8tFj0c8ZkbOBszyng9lshyUDrlsnLlPI9eiEx4,8412
 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/dnnl_ext.hpp,sha256=RqPk2MPbfErzAQom8cwceKeGDoeYviOIJqzWAoCAmwc,6136
-intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_context.hpp,sha256=UbaNUtF7tHZlwNvrpLQU_MPXalXZEE3FXFjBetFY3M4,7692
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_context.hpp,sha256=EVM061vAcj9himEk0oW6C4l0DtiW3Is7f3BhrWuguDU,7694
 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onednn_wrappers.hpp,sha256=EKBGpbA-mqmXhJ3BOXBrNl-Ah-EpEU1PFEtZSrhOwjM,933
 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_onemkl_wrappers.hpp,sha256=uLh2BMj_Bak2k39DG1qaBUqp4_RFHPzbgbXU91HS7AM,1292
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/inference_sycl_layers.hpp,sha256=UDCLIXoGhxDDaIMAMtuwqKlbFB_fiD3pixzTAvPE1lg,2680
 intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/lru_cache.hpp,sha256=hjk1R8ai4b-BJsJVkMdxB3e8nogzWb8oqxJCheTjlk8,9833
-intel_extension_for_deepspeed-0.1.dev20230613.dist-info/LICENSE,sha256=DohMgz3056mBB4lSpGqjJ2n625t8Frf3K3iOM5861SU,1074
-intel_extension_for_deepspeed-0.1.dev20230613.dist-info/METADATA,sha256=hwZVcW8JiUIaK4qsG36O9pJRYAyWF8xnf8MxPp5Y7KE,171
-intel_extension_for_deepspeed-0.1.dev20230613.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-intel_extension_for_deepspeed-0.1.dev20230613.dist-info/top_level.txt,sha256=6hxaNxb_WJodZP9hMUFFkrHWi45Td4KdtbIsF10xKqA,30
-intel_extension_for_deepspeed-0.1.dev20230613.dist-info/RECORD,,
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/memory_access_utils.hpp,sha256=viLGljnPSbc33zby8WBhGjZW2kxuyDCdkSa4yRjZX7k,15298
+intel_extension_for_deepspeed/op_builder/csrc/transformer/inference/includes/reduction_utils.hpp,sha256=A2YUoaSY876KfSrg__EooDksfvFZJ_7rJYw8ebwkjFc,16305
+intel_extension_for_deepspeed-0.9.4.dist-info/LICENSE,sha256=DohMgz3056mBB4lSpGqjJ2n625t8Frf3K3iOM5861SU,1074
+intel_extension_for_deepspeed-0.9.4.dist-info/METADATA,sha256=xoCO7EqMOrbFy5JE8hDthmHio5-cThAF-9ZdL5nD-2k,2035
+intel_extension_for_deepspeed-0.9.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+intel_extension_for_deepspeed-0.9.4.dist-info/top_level.txt,sha256=6hxaNxb_WJodZP9hMUFFkrHWi45Td4KdtbIsF10xKqA,30
+intel_extension_for_deepspeed-0.9.4.dist-info/RECORD,,
```

