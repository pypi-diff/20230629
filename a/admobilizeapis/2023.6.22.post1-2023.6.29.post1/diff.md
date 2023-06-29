# Comparing `tmp/admobilizeapis-2023.6.22.post1.tar.gz` & `tmp/admobilizeapis-2023.6.29.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/admobilizeapis-2023.6.22.post1.tar", last modified: Thu Jun 22 05:58:54 2023, max compression
+gzip compressed data, was "dist/admobilizeapis-2023.6.29.post1.tar", last modified: Thu Jun 29 17:16:05 2023, max compression
```

## Comparing `admobilizeapis-2023.6.22.post1.tar` & `admobilizeapis-2023.6.29.post1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10932 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/wifi_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25837 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    35932 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4194 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/model_pb2.py
--rw-r--r--   0 root         (0) root         (0)    25636 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     6478 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5528 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15461 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28693 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10609 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28083 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18992 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20392 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    99455 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    76701 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13543 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    41623 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29786 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9576 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14877 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15271 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22477 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/driver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/maloseye_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    14646 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    31149 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28346 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15801 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21203 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18378 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24106 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/entity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/admobilize_types_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/entity_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22301 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29481 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24348 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21841 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16356 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)     6814 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/README.md
--rw-r--r--   0 root         (0) root         (0)     1293 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/google/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10932 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/wifi_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35932 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    26810 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28693 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28083 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18992 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20392 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    99455 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    76701 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    41623 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15271 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6954 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22477 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/driver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/maloseye_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    14646 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    31149 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28346 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24106 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/entity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/admobilize_types_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/common/entity_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)    22301 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21841 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)     6814 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-06-29 17:16:04.000000 admobilizeapis-2023.6.29.post1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 17:16:05.000000 admobilizeapis-2023.6.29.post1/setup.cfg
```

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/wifi_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/wifi/v1/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/model_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/vision/v1/vision_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!admobilize/vision/v1/vision.proto\x12\x14\x61\x64mobilize.vision.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"%\n\x04Size\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\"@\n\tRectangle\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\r\n\x05width\x18\x03 \x01(\x02\x12\x0e\n\x06height\x18\x04 \x01(\x02\"\xa0\x01\n\x12VehicleRecognition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05\x62rand\x18\x02 \x01(\t\x12\r\n\x05model\x18\x03 \x01(\t\x12\x0c\n\x04year\x18\x04 \x01(\x05\x12<\n\x03tag\x18\x05 \x01(\x0e\x32/.admobilize.vision.v1.EnumVehicleRecognitionTag\x12\x12\n\nconfidence\x18\x06 \x01(\x02\"\xfb\n\n\x11\x46\x61\x63ialRecognition\x12;\n\x03tag\x18\x01 \x01(\x0e\x32..admobilize.vision.v1.EnumFacialRecognitionTag\x12\x12\n\nconfidence\x18\x02 \x01(\x02\x12\x0b\n\x03\x61ge\x18\x03 \x01(\x05\x12\x43\n\tage_class\x18\r \x01(\x0e\x32\x30.admobilize.vision.v1.FacialRecognition.AgeClass\x12>\n\x06gender\x18\x04 \x01(\x0e\x32..admobilize.vision.v1.FacialRecognition.Gender\x12@\n\x07\x65motion\x18\x05 \x01(\x0e\x32/.admobilize.vision.v1.FacialRecognition.Emotion\x12\x1b\n\x0f\x66\x61\x63\x65_descriptor\x18\x06 \x03(\x02\x42\x02\x10\x01\x12\x0f\n\x07\x66\x61\x63\x65_id\x18\x07 \x01(\t\x12\x10\n\x08pose_yaw\x18\x08 \x01(\x02\x12\x11\n\tpose_roll\x18\t \x01(\x02\x12\x12\n\npose_pitch\x18\n \x01(\x02\x12\x12\n\nis_looking\x18\x0e \x01(\x08\x12O\n\rbasic_feature\x18\x0b \x01(\x0b\x32\x38.admobilize.vision.v1.FacialRecognition.BasicFaceFeature\x12\x0f\n\x07is_face\x18\x0c \x01(\x08\x12\x12\n\nhave_glass\x18\x0f \x01(\x08\x12\r\n\x05\x62\x65\x61rd\x18\x10 \x01(\x08\x12\x0c\n\x04mask\x18\x13 \x01(\x08\x12\r\n\x05spoof\x18\x14 \x01(\x08\x12@\n\x07glasses\x18\x11 \x01(\x0e\x32/.admobilize.vision.v1.FacialRecognition.Glasses\x12\x45\n\nface_shape\x18\x12 \x01(\x0e\x32\x31.admobilize.vision.v1.FacialRecognition.FaceShape\x1a\xc8\x01\n\x10\x42\x61sicFaceFeature\x12*\n\x05mouth\x18\x01 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12-\n\x08left_eye\x18\x02 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12.\n\tright_eye\x18\x03 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12)\n\x04nose\x18\x04 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\"[\n\x08\x41geClass\x12\x19\n\x15\x41GE_CLASS_NOT_DEFINED\x10\x00\x12\x0c\n\x08\x43HILDREN\x10\x01\x12\x0f\n\x0bYOUNG_ADULT\x10\x02\x12\t\n\x05\x41\x44ULT\x10\x03\x12\n\n\x06SENIOR\x10\x04\"6\n\x06Gender\x12\x16\n\x12GENDER_NOT_DEFINED\x10\x00\x12\x08\n\x04MALE\x10\x01\x12\n\n\x06\x46\x45MALE\x10\x02\"\x8c\x01\n\x07\x45motion\x12\x17\n\x13\x45MOTION_NOT_DEFINED\x10\x00\x12\t\n\x05\x41NGRY\x10\x01\x12\x0b\n\x07\x44ISGUST\x10\x02\x12\x0c\n\x08\x43ONFUSED\x10\x03\x12\t\n\x05HAPPY\x10\x04\x12\x07\n\x03SAD\x10\x05\x12\r\n\tSURPRISED\x10\x06\x12\x08\n\x04\x43\x41LM\x10\x07\x12\x08\n\x04\x46\x45\x41R\x10\x08\x12\x0b\n\x07NEUTRAL\x10\t\"P\n\x07Glasses\x12\x17\n\x13GLASSES_NOT_DEFINED\x10\x00\x12\x0b\n\x07GLASSES\x10\x01\x12\x0e\n\nNO_GLASSES\x10\x02\x12\x0f\n\x0bSUN_GLASSES\x10\x03\"Z\n\tFaceShape\x12\x15\n\x11SHAPE_NOT_DEFINED\x10\x00\x12\t\n\x05HEART\x10\x01\x12\n\n\x06OBLONG\x10\x02\x12\x08\n\x04OVAL\x10\x03\x12\t\n\x05ROUND\x10\x04\x12\n\n\x06SQUARE\x10\x05\"\x9b\x01\n\nZoneConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x07point_a\x18\x02 \x01(\x0b\x32\x1b.admobilize.vision.v1.Point\x12,\n\x07point_b\x18\x03 \x01(\x0b\x32\x1b.admobilize.vision.v1.Point\x12\x0e\n\x06height\x18\x04 \x01(\x05\x12\x13\n\x0breal_height\x18\x05 \x01(\x02\"|\n\nAreaConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x05point\x18\x02 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12\x34\n\x0f\x63ount_direction\x18\x03 \x01(\x0b\x32\x1b.admobilize.vision.v1.Point\"\xb0\x01\n\x11\x41reaAndZoneConfig\x12.\n\x04\x61rea\x18\x01 \x03(\x0b\x32 .admobilize.vision.v1.AreaConfig\x12.\n\x04zone\x18\x02 \x03(\x0b\x32 .admobilize.vision.v1.ZoneConfig\x12;\n\x12region_of_interest\x18\x03 \x03(\x0b\x32\x1f.admobilize.vision.v1.Rectangle\"c\n\rVehicleConfig\x12\x12\n\ncamera_url\x18\x01 \x01(\t\x12>\n\rarea_and_zone\x18\x02 \x01(\x0b\x32\'.admobilize.vision.v1.AreaAndZoneConfig\"\xbc\x02\n\x0bVisionEvent\x12+\n\x03tag\x18\x01 \x01(\x0e\x32\x1e.admobilize.vision.v1.EventTag\x12\x13\n\x0btracking_id\x18\x02 \x01(\x04\x12\x14\n\x0csession_time\x18\x03 \x01(\x02\x12\x12\n\ndwell_time\x18\x04 \x01(\x02\x12\x0f\n\x07\x61rea_id\x18\x05 \x01(\x04\x12\x0f\n\x07zone_id\x18\x06 \x01(\x04\x12;\n\x0ezone_direction\x18\x07 \x01(\x0e\x32#.admobilize.vision.v1.ZoneDirection\x12\r\n\x05speed\x18\x08 \x01(\x02\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x11\n\tzone_name\x18\x0b \x01(\t\"\xed\x03\n\x14RectangularDetection\x12?\n\talgorithm\x18\x01 \x01(\x0e\x32,.admobilize.vision.v1.EnumDetectionAlgorithm\x12\x31\n\x08location\x18\x02 \x01(\x0b\x32\x1f.admobilize.vision.v1.Rectangle\x12\x33\n\x03tag\x18\x03 \x01(\x0e\x32&.admobilize.vision.v1.EnumDetectionTag\x12\x12\n\nconfidence\x18\x04 \x01(\x02\x12\x43\n\x12\x66\x61\x63ial_recognition\x18\x05 \x03(\x0b\x32\'.admobilize.vision.v1.FacialRecognition\x12\x45\n\x13vehicle_recognition\x18\t \x03(\x0b\x32(.admobilize.vision.v1.VehicleRecognition\x12\r\n\x05speed\x18\n \x01(\x02\x12\r\n\x05image\x18\x06 \x01(\x0c\x12\x13\n\x0bimage_small\x18\x07 \x01(\x0c\x12\x0c\n\x04type\x18\x0c \x01(\t\x12\x13\n\x0btracking_id\x18\x08 \x01(\x04\x12\x0c\n\x04uuid\x18\x0b \x01(\t\x12\x10\n\x08\x64istance\x18\r \x01(\x02\x12\x16\n\x0e\x61ttention_time\x18\x0e \x01(\x02\":\n\tImageList\x12\x12\n\nimage_data\x18\x01 \x03(\x0c\x12\x19\n\x11\x66rames_per_second\x18\x02 \x01(\x05\"]\n\x05Video\x12\x12\n\nvideo_data\x18\x01 \x01(\x0c\x12\x33\n\x05\x63odec\x18\x02 \x01(\x0e\x32$.admobilize.vision.v1.EnumVideoCodec\x12\x0b\n\x03tag\x18\x03 \x03(\t\"s\n\x05Image\x12\r\n\x05image\x18\x01 \x01(\x0c\x12\x31\n\x06\x66ormat\x18\x02 \x01(\x0e\x32!.admobilize.vision.v1.ImageFormat\x12(\n\x04size\x18\x03 \x01(\x0b\x32\x1a.admobilize.vision.v1.Size\"\xe7\x01\n\tFrameData\x12\n\n\x02id\x18\x01 \x01(\x04\x12.\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x08sections\x18\x04 \x03(\x0b\x32-.admobilize.vision.v1.FrameData.SectionsEntry\x1a/\n\rSectionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"@\n\rFrameDataList\x12/\n\x06\x66rames\x18\x01 \x03(\x0b\x32\x1f.admobilize.vision.v1.FrameData\"\x98\x03\n\x0cVisionResult\x12\x42\n\x0erect_detection\x18\x01 \x03(\x0b\x32*.admobilize.vision.v1.RectangularDetection\x12\x37\n\x0cvision_event\x18\x04 \x03(\x0b\x32!.admobilize.vision.v1.VisionEvent\x12\x31\n\x0cresult_image\x18\x05 \x01(\x0b\x32\x1b.admobilize.vision.v1.Image\x12\x37\n\x12result_image_small\x18\x06 \x01(\x0b\x32\x1b.admobilize.vision.v1.Image\x12\r\n\x05image\x18\x02 \x01(\x0c\x12\x13\n\x0bimage_small\x18\x03 \x01(\x0c\x12\x0c\n\x04uuid\x18\x07 \x01(\t\x12\x33\n\nframe_data\x18\x08 \x01(\x0b\x32\x1f.admobilize.vision.v1.FrameData\x12\x38\n\rmoment_of_day\x18\t \x01(\x0e\x32!.admobilize.vision.v1.MomentOfDay\"`\n\x0eModelInference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x1d\n\x15single_inference_time\x18\x02 \x01(\x02\x12\x1b\n\x13real_inference_time\x18\x03 \x01(\x02\"`\n\x1c\x46\x61\x63\x65\x43rowdInferenceTimeResult\x12\x12\n\ncount_face\x18\x01 \x01(\x04\x12\x14\n\x0c\x63ount_person\x18\x02 \x01(\x04\x12\x16\n\x0einference_time\x18\x03 \x01(\x02\"\x9e\x01\n\x16VisionEvaluationResult\x12\x34\n\x06models\x18\x01 \x03(\x0b\x32$.admobilize.vision.v1.ModelInference\x12N\n\x12\x66\x61\x63\x65_crowd_results\x18\x02 \x03(\x0b\x32\x32.admobilize.vision.v1.FaceCrowdInferenceTimeResult\"N\n\x10VisionResultList\x12:\n\x0evision_results\x18\x01 \x03(\x0b\x32\".admobilize.vision.v1.VisionResult*\x81\x02\n\x18\x45numFacialRecognitionTag\x12\"\n\x1e\x46\x41\x43IAL_RECOGNITION_NOT_DEFINED\x10\x00\x12\x07\n\x03\x41GE\x10\x01\x12\x0b\n\x07\x45MOTION\x10\x02\x12\n\n\x06GENDER\x10\x03\x12\x0b\n\x07\x46\x41\x43\x45_ID\x10\x04\x12\r\n\tHEAD_POSE\x10\x05\x12\x11\n\rFACE_FEATURES\x10\x06\x12\x13\n\x0f\x46\x41\x43\x45_DESCRIPTOR\x10\x07\x12\x0b\n\x07IS_FACE\x10\x08\x12\x0e\n\nHAVE_GLASS\x10\t\x12\t\n\x05\x42\x45\x41RD\x10\n\x12\x0e\n\nTYPE_GLASS\x10\x0b\x12\x0e\n\nFACE_SHAPE\x10\x0c\x12\x08\n\x04MASK\x10\r\x12\t\n\x05SPOOF\x10\x0e*P\n\x19\x45numVehicleRecognitionTag\x12#\n\x1fVEHICLE_RECOGNITION_NOT_DEFINED\x10\x00\x12\x0e\n\nFAMILY_CAR\x10\x01*J\n\rZoneDirection\x12\x1e\n\x1aZONE_DIRECTION_NOT_DEFINED\x10\x00\x12\x0b\n\x07\x46ORWARD\x10\x01\x12\x0c\n\x08\x42\x41\x43KWARD\x10\x02*\x85\x01\n\x08\x45ventTag\x12\x15\n\x11\x45VENT_NOT_DEFINED\x10\x00\x12\x12\n\x0eTRACKING_START\x10\x01\x12\x10\n\x0cTRACKING_END\x10\x02\x12\x0e\n\nAREA_ENTER\x10\x03\x12\r\n\tAREA_EXIT\x10\x04\x12\x0e\n\nZONE_ENTER\x10\x05\x12\r\n\tZONE_EXIT\x10\x06*\x8e\x01\n\x10\x45numDetectionTag\x12\x19\n\x15\x44\x45TECTION_NOT_DEFINED\x10\x00\x12\x08\n\x04\x46\x41\x43\x45\x10\x01\x12\x0e\n\nHAND_THUMB\x10\x02\x12\r\n\tHAND_PALM\x10\x03\x12\x0e\n\nHAND_PINCH\x10\x04\x12\r\n\tHAND_FIST\x10\x05\x12\n\n\x06PERSON\x10\x06\x12\x0b\n\x07VEHICLE\x10\x07*a\n\x16\x45numDetectionAlgorithm\x12#\n\x1f\x44\x45TECTION_ALGORITHM_NOT_DEFINED\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x15\n\x11\x46IRST_ALTERNATIVE\x10\x02*x\n\x0e\x45numVideoCodec\x12\x1b\n\x17VIDEO_CODEC_NOT_DEFINED\x10\x00\x12\x19\n\x15UNDEFINED_VIDEO_CODEC\x10\x01\x12\x08\n\x04H264\x10\x02\x12\x08\n\x04MP4V\x10\x03\x12\x08\n\x04RV24\x10\x04\x12\x07\n\x03VP8\x10\x05\x12\x07\n\x03VP9\x10\x06*o\n\x0bImageFormat\x12\x1c\n\x18IMAGE_FORMAT_NOT_DEFINED\x10\x00\x12\x0f\n\x0bUNSPECIFIED\x10\x01\x12\x10\n\x0c\x46ORMAT_8URGB\x10\x02\x12\x10\n\x0c\x46ORMAT_8UBGR\x10\x03\x12\r\n\tFORMAT_8U\x10\x04*@\n\x0bMomentOfDay\x12\x1d\n\x19MOMENT_OF_DAY_NOT_DEFINED\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x01\x12\t\n\x05NIGHT\x10\x02\x42\x80\x01\n\x1e\x63om.admobilize.proto.vision.v1B\x0bVisionProtoP\x01Z8bitbucket.org/admobilize/admobilizeapis-go/pkg/vision/v1\xaa\x02\x14\x41\x64Mobilize.Vision.V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!admobilize/vision/v1/vision.proto\x12\x14\x61\x64mobilize.vision.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"%\n\x04Size\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\"@\n\tRectangle\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\r\n\x05width\x18\x03 \x01(\x02\x12\x0e\n\x06height\x18\x04 \x01(\x02\"\xa0\x01\n\x12VehicleRecognition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05\x62rand\x18\x02 \x01(\t\x12\r\n\x05model\x18\x03 \x01(\t\x12\x0c\n\x04year\x18\x04 \x01(\x05\x12<\n\x03tag\x18\x05 \x01(\x0e\x32/.admobilize.vision.v1.EnumVehicleRecognitionTag\x12\x12\n\nconfidence\x18\x06 \x01(\x02\"\xfb\n\n\x11\x46\x61\x63ialRecognition\x12;\n\x03tag\x18\x01 \x01(\x0e\x32..admobilize.vision.v1.EnumFacialRecognitionTag\x12\x12\n\nconfidence\x18\x02 \x01(\x02\x12\x0b\n\x03\x61ge\x18\x03 \x01(\x05\x12\x43\n\tage_class\x18\r \x01(\x0e\x32\x30.admobilize.vision.v1.FacialRecognition.AgeClass\x12>\n\x06gender\x18\x04 \x01(\x0e\x32..admobilize.vision.v1.FacialRecognition.Gender\x12@\n\x07\x65motion\x18\x05 \x01(\x0e\x32/.admobilize.vision.v1.FacialRecognition.Emotion\x12\x1b\n\x0f\x66\x61\x63\x65_descriptor\x18\x06 \x03(\x02\x42\x02\x10\x01\x12\x0f\n\x07\x66\x61\x63\x65_id\x18\x07 \x01(\t\x12\x10\n\x08pose_yaw\x18\x08 \x01(\x02\x12\x11\n\tpose_roll\x18\t \x01(\x02\x12\x12\n\npose_pitch\x18\n \x01(\x02\x12\x12\n\nis_looking\x18\x0e \x01(\x08\x12O\n\rbasic_feature\x18\x0b \x01(\x0b\x32\x38.admobilize.vision.v1.FacialRecognition.BasicFaceFeature\x12\x0f\n\x07is_face\x18\x0c \x01(\x08\x12\x12\n\nhave_glass\x18\x0f \x01(\x08\x12\r\n\x05\x62\x65\x61rd\x18\x10 \x01(\x08\x12\x0c\n\x04mask\x18\x13 \x01(\x08\x12\r\n\x05spoof\x18\x14 \x01(\x08\x12@\n\x07glasses\x18\x11 \x01(\x0e\x32/.admobilize.vision.v1.FacialRecognition.Glasses\x12\x45\n\nface_shape\x18\x12 \x01(\x0e\x32\x31.admobilize.vision.v1.FacialRecognition.FaceShape\x1a\xc8\x01\n\x10\x42\x61sicFaceFeature\x12*\n\x05mouth\x18\x01 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12-\n\x08left_eye\x18\x02 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12.\n\tright_eye\x18\x03 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12)\n\x04nose\x18\x04 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\"[\n\x08\x41geClass\x12\x19\n\x15\x41GE_CLASS_NOT_DEFINED\x10\x00\x12\x0c\n\x08\x43HILDREN\x10\x01\x12\x0f\n\x0bYOUNG_ADULT\x10\x02\x12\t\n\x05\x41\x44ULT\x10\x03\x12\n\n\x06SENIOR\x10\x04\"6\n\x06Gender\x12\x16\n\x12GENDER_NOT_DEFINED\x10\x00\x12\x08\n\x04MALE\x10\x01\x12\n\n\x06\x46\x45MALE\x10\x02\"\x8c\x01\n\x07\x45motion\x12\x17\n\x13\x45MOTION_NOT_DEFINED\x10\x00\x12\t\n\x05\x41NGRY\x10\x01\x12\x0b\n\x07\x44ISGUST\x10\x02\x12\x0c\n\x08\x43ONFUSED\x10\x03\x12\t\n\x05HAPPY\x10\x04\x12\x07\n\x03SAD\x10\x05\x12\r\n\tSURPRISED\x10\x06\x12\x08\n\x04\x43\x41LM\x10\x07\x12\x08\n\x04\x46\x45\x41R\x10\x08\x12\x0b\n\x07NEUTRAL\x10\t\"P\n\x07Glasses\x12\x17\n\x13GLASSES_NOT_DEFINED\x10\x00\x12\x0b\n\x07GLASSES\x10\x01\x12\x0e\n\nNO_GLASSES\x10\x02\x12\x0f\n\x0bSUN_GLASSES\x10\x03\"Z\n\tFaceShape\x12\x15\n\x11SHAPE_NOT_DEFINED\x10\x00\x12\t\n\x05HEART\x10\x01\x12\n\n\x06OBLONG\x10\x02\x12\x08\n\x04OVAL\x10\x03\x12\t\n\x05ROUND\x10\x04\x12\n\n\x06SQUARE\x10\x05\"\x9b\x01\n\nZoneConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x07point_a\x18\x02 \x01(\x0b\x32\x1b.admobilize.vision.v1.Point\x12,\n\x07point_b\x18\x03 \x01(\x0b\x32\x1b.admobilize.vision.v1.Point\x12\x0e\n\x06height\x18\x04 \x01(\x05\x12\x13\n\x0breal_height\x18\x05 \x01(\x02\"|\n\nAreaConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x05point\x18\x02 \x03(\x0b\x32\x1b.admobilize.vision.v1.Point\x12\x34\n\x0f\x63ount_direction\x18\x03 \x01(\x0b\x32\x1b.admobilize.vision.v1.Point\"\xb0\x01\n\x11\x41reaAndZoneConfig\x12.\n\x04\x61rea\x18\x01 \x03(\x0b\x32 .admobilize.vision.v1.AreaConfig\x12.\n\x04zone\x18\x02 \x03(\x0b\x32 .admobilize.vision.v1.ZoneConfig\x12;\n\x12region_of_interest\x18\x03 \x03(\x0b\x32\x1f.admobilize.vision.v1.Rectangle\"c\n\rVehicleConfig\x12\x12\n\ncamera_url\x18\x01 \x01(\t\x12>\n\rarea_and_zone\x18\x02 \x01(\x0b\x32\'.admobilize.vision.v1.AreaAndZoneConfig\"2\n\x0bHeatmapData\x12\t\n\x01x\x18\x01 \x01(\r\x12\t\n\x01y\x18\x02 \x01(\r\x12\r\n\x05value\x18\x03 \x01(\x02\"j\n\x07Heatmap\x12.\n\nresolution\x18\x01 \x01(\x0b\x32\x1a.admobilize.vision.v1.Size\x12/\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32!.admobilize.vision.v1.HeatmapData\"\xec\x02\n\x0bVisionEvent\x12+\n\x03tag\x18\x01 \x01(\x0e\x32\x1e.admobilize.vision.v1.EventTag\x12\x13\n\x0btracking_id\x18\x02 \x01(\x04\x12\x14\n\x0csession_time\x18\x03 \x01(\x02\x12\x12\n\ndwell_time\x18\x04 \x01(\x02\x12\x0f\n\x07\x61rea_id\x18\x05 \x01(\x04\x12\x0f\n\x07zone_id\x18\x06 \x01(\x04\x12;\n\x0ezone_direction\x18\x07 \x01(\x0e\x32#.admobilize.vision.v1.ZoneDirection\x12\r\n\x05speed\x18\x08 \x01(\x02\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x11\n\tzone_name\x18\x0b \x01(\t\x12.\n\x07heatmap\x18\x0c \x01(\x0b\x32\x1d.admobilize.vision.v1.Heatmap\"\xed\x03\n\x14RectangularDetection\x12?\n\talgorithm\x18\x01 \x01(\x0e\x32,.admobilize.vision.v1.EnumDetectionAlgorithm\x12\x31\n\x08location\x18\x02 \x01(\x0b\x32\x1f.admobilize.vision.v1.Rectangle\x12\x33\n\x03tag\x18\x03 \x01(\x0e\x32&.admobilize.vision.v1.EnumDetectionTag\x12\x12\n\nconfidence\x18\x04 \x01(\x02\x12\x43\n\x12\x66\x61\x63ial_recognition\x18\x05 \x03(\x0b\x32\'.admobilize.vision.v1.FacialRecognition\x12\x45\n\x13vehicle_recognition\x18\t \x03(\x0b\x32(.admobilize.vision.v1.VehicleRecognition\x12\r\n\x05speed\x18\n \x01(\x02\x12\r\n\x05image\x18\x06 \x01(\x0c\x12\x13\n\x0bimage_small\x18\x07 \x01(\x0c\x12\x0c\n\x04type\x18\x0c \x01(\t\x12\x13\n\x0btracking_id\x18\x08 \x01(\x04\x12\x0c\n\x04uuid\x18\x0b \x01(\t\x12\x10\n\x08\x64istance\x18\r \x01(\x02\x12\x16\n\x0e\x61ttention_time\x18\x0e \x01(\x02\":\n\tImageList\x12\x12\n\nimage_data\x18\x01 \x03(\x0c\x12\x19\n\x11\x66rames_per_second\x18\x02 \x01(\x05\"]\n\x05Video\x12\x12\n\nvideo_data\x18\x01 \x01(\x0c\x12\x33\n\x05\x63odec\x18\x02 \x01(\x0e\x32$.admobilize.vision.v1.EnumVideoCodec\x12\x0b\n\x03tag\x18\x03 \x03(\t\"s\n\x05Image\x12\r\n\x05image\x18\x01 \x01(\x0c\x12\x31\n\x06\x66ormat\x18\x02 \x01(\x0e\x32!.admobilize.vision.v1.ImageFormat\x12(\n\x04size\x18\x03 \x01(\x0b\x32\x1a.admobilize.vision.v1.Size\"\xe7\x01\n\tFrameData\x12\n\n\x02id\x18\x01 \x01(\x04\x12.\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x08sections\x18\x04 \x03(\x0b\x32-.admobilize.vision.v1.FrameData.SectionsEntry\x1a/\n\rSectionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"@\n\rFrameDataList\x12/\n\x06\x66rames\x18\x01 \x03(\x0b\x32\x1f.admobilize.vision.v1.FrameData\"\x98\x03\n\x0cVisionResult\x12\x42\n\x0erect_detection\x18\x01 \x03(\x0b\x32*.admobilize.vision.v1.RectangularDetection\x12\x37\n\x0cvision_event\x18\x04 \x03(\x0b\x32!.admobilize.vision.v1.VisionEvent\x12\x31\n\x0cresult_image\x18\x05 \x01(\x0b\x32\x1b.admobilize.vision.v1.Image\x12\x37\n\x12result_image_small\x18\x06 \x01(\x0b\x32\x1b.admobilize.vision.v1.Image\x12\r\n\x05image\x18\x02 \x01(\x0c\x12\x13\n\x0bimage_small\x18\x03 \x01(\x0c\x12\x0c\n\x04uuid\x18\x07 \x01(\t\x12\x33\n\nframe_data\x18\x08 \x01(\x0b\x32\x1f.admobilize.vision.v1.FrameData\x12\x38\n\rmoment_of_day\x18\t \x01(\x0e\x32!.admobilize.vision.v1.MomentOfDay\"`\n\x0eModelInference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x1d\n\x15single_inference_time\x18\x02 \x01(\x02\x12\x1b\n\x13real_inference_time\x18\x03 \x01(\x02\"`\n\x1c\x46\x61\x63\x65\x43rowdInferenceTimeResult\x12\x12\n\ncount_face\x18\x01 \x01(\x04\x12\x14\n\x0c\x63ount_person\x18\x02 \x01(\x04\x12\x16\n\x0einference_time\x18\x03 \x01(\x02\"\x9e\x01\n\x16VisionEvaluationResult\x12\x34\n\x06models\x18\x01 \x03(\x0b\x32$.admobilize.vision.v1.ModelInference\x12N\n\x12\x66\x61\x63\x65_crowd_results\x18\x02 \x03(\x0b\x32\x32.admobilize.vision.v1.FaceCrowdInferenceTimeResult\"N\n\x10VisionResultList\x12:\n\x0evision_results\x18\x01 \x03(\x0b\x32\".admobilize.vision.v1.VisionResult*\x81\x02\n\x18\x45numFacialRecognitionTag\x12\"\n\x1e\x46\x41\x43IAL_RECOGNITION_NOT_DEFINED\x10\x00\x12\x07\n\x03\x41GE\x10\x01\x12\x0b\n\x07\x45MOTION\x10\x02\x12\n\n\x06GENDER\x10\x03\x12\x0b\n\x07\x46\x41\x43\x45_ID\x10\x04\x12\r\n\tHEAD_POSE\x10\x05\x12\x11\n\rFACE_FEATURES\x10\x06\x12\x13\n\x0f\x46\x41\x43\x45_DESCRIPTOR\x10\x07\x12\x0b\n\x07IS_FACE\x10\x08\x12\x0e\n\nHAVE_GLASS\x10\t\x12\t\n\x05\x42\x45\x41RD\x10\n\x12\x0e\n\nTYPE_GLASS\x10\x0b\x12\x0e\n\nFACE_SHAPE\x10\x0c\x12\x08\n\x04MASK\x10\r\x12\t\n\x05SPOOF\x10\x0e*P\n\x19\x45numVehicleRecognitionTag\x12#\n\x1fVEHICLE_RECOGNITION_NOT_DEFINED\x10\x00\x12\x0e\n\nFAMILY_CAR\x10\x01*J\n\rZoneDirection\x12\x1e\n\x1aZONE_DIRECTION_NOT_DEFINED\x10\x00\x12\x0b\n\x07\x46ORWARD\x10\x01\x12\x0c\n\x08\x42\x41\x43KWARD\x10\x02*\x85\x01\n\x08\x45ventTag\x12\x15\n\x11\x45VENT_NOT_DEFINED\x10\x00\x12\x12\n\x0eTRACKING_START\x10\x01\x12\x10\n\x0cTRACKING_END\x10\x02\x12\x0e\n\nAREA_ENTER\x10\x03\x12\r\n\tAREA_EXIT\x10\x04\x12\x0e\n\nZONE_ENTER\x10\x05\x12\r\n\tZONE_EXIT\x10\x06*\x8e\x01\n\x10\x45numDetectionTag\x12\x19\n\x15\x44\x45TECTION_NOT_DEFINED\x10\x00\x12\x08\n\x04\x46\x41\x43\x45\x10\x01\x12\x0e\n\nHAND_THUMB\x10\x02\x12\r\n\tHAND_PALM\x10\x03\x12\x0e\n\nHAND_PINCH\x10\x04\x12\r\n\tHAND_FIST\x10\x05\x12\n\n\x06PERSON\x10\x06\x12\x0b\n\x07VEHICLE\x10\x07*a\n\x16\x45numDetectionAlgorithm\x12#\n\x1f\x44\x45TECTION_ALGORITHM_NOT_DEFINED\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x15\n\x11\x46IRST_ALTERNATIVE\x10\x02*x\n\x0e\x45numVideoCodec\x12\x1b\n\x17VIDEO_CODEC_NOT_DEFINED\x10\x00\x12\x19\n\x15UNDEFINED_VIDEO_CODEC\x10\x01\x12\x08\n\x04H264\x10\x02\x12\x08\n\x04MP4V\x10\x03\x12\x08\n\x04RV24\x10\x04\x12\x07\n\x03VP8\x10\x05\x12\x07\n\x03VP9\x10\x06*o\n\x0bImageFormat\x12\x1c\n\x18IMAGE_FORMAT_NOT_DEFINED\x10\x00\x12\x0f\n\x0bUNSPECIFIED\x10\x01\x12\x10\n\x0c\x46ORMAT_8URGB\x10\x02\x12\x10\n\x0c\x46ORMAT_8UBGR\x10\x03\x12\r\n\tFORMAT_8U\x10\x04*@\n\x0bMomentOfDay\x12\x1d\n\x19MOMENT_OF_DAY_NOT_DEFINED\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x01\x12\t\n\x05NIGHT\x10\x02\x42\x80\x01\n\x1e\x63om.admobilize.proto.vision.v1B\x0bVisionProtoP\x01Z8bitbucket.org/admobilize/admobilizeapis-go/pkg/vision/v1\xaa\x02\x14\x41\x64Mobilize.Vision.V1b\x06proto3')
 
 _ENUMFACIALRECOGNITIONTAG = DESCRIPTOR.enum_types_by_name['EnumFacialRecognitionTag']
 EnumFacialRecognitionTag = enum_type_wrapper.EnumTypeWrapper(_ENUMFACIALRECOGNITIONTAG)
 _ENUMVEHICLERECOGNITIONTAG = DESCRIPTOR.enum_types_by_name['EnumVehicleRecognitionTag']
 EnumVehicleRecognitionTag = enum_type_wrapper.EnumTypeWrapper(_ENUMVEHICLERECOGNITIONTAG)
 _ZONEDIRECTION = DESCRIPTOR.enum_types_by_name['ZoneDirection']
 ZoneDirection = enum_type_wrapper.EnumTypeWrapper(_ZONEDIRECTION)
@@ -97,14 +97,16 @@
 _VEHICLERECOGNITION = DESCRIPTOR.message_types_by_name['VehicleRecognition']
 _FACIALRECOGNITION = DESCRIPTOR.message_types_by_name['FacialRecognition']
 _FACIALRECOGNITION_BASICFACEFEATURE = _FACIALRECOGNITION.nested_types_by_name['BasicFaceFeature']
 _ZONECONFIG = DESCRIPTOR.message_types_by_name['ZoneConfig']
 _AREACONFIG = DESCRIPTOR.message_types_by_name['AreaConfig']
 _AREAANDZONECONFIG = DESCRIPTOR.message_types_by_name['AreaAndZoneConfig']
 _VEHICLECONFIG = DESCRIPTOR.message_types_by_name['VehicleConfig']
+_HEATMAPDATA = DESCRIPTOR.message_types_by_name['HeatmapData']
+_HEATMAP = DESCRIPTOR.message_types_by_name['Heatmap']
 _VISIONEVENT = DESCRIPTOR.message_types_by_name['VisionEvent']
 _RECTANGULARDETECTION = DESCRIPTOR.message_types_by_name['RectangularDetection']
 _IMAGELIST = DESCRIPTOR.message_types_by_name['ImageList']
 _VIDEO = DESCRIPTOR.message_types_by_name['Video']
 _IMAGE = DESCRIPTOR.message_types_by_name['Image']
 _FRAMEDATA = DESCRIPTOR.message_types_by_name['FrameData']
 _FRAMEDATA_SECTIONSENTRY = _FRAMEDATA.nested_types_by_name['SectionsEntry']
@@ -186,14 +188,28 @@
 VehicleConfig = _reflection.GeneratedProtocolMessageType('VehicleConfig', (_message.Message,), {
   'DESCRIPTOR' : _VEHICLECONFIG,
   '__module__' : 'admobilize.vision.v1.vision_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.vision.v1.VehicleConfig)
   })
 _sym_db.RegisterMessage(VehicleConfig)
 
+HeatmapData = _reflection.GeneratedProtocolMessageType('HeatmapData', (_message.Message,), {
+  'DESCRIPTOR' : _HEATMAPDATA,
+  '__module__' : 'admobilize.vision.v1.vision_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.vision.v1.HeatmapData)
+  })
+_sym_db.RegisterMessage(HeatmapData)
+
+Heatmap = _reflection.GeneratedProtocolMessageType('Heatmap', (_message.Message,), {
+  'DESCRIPTOR' : _HEATMAP,
+  '__module__' : 'admobilize.vision.v1.vision_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.vision.v1.Heatmap)
+  })
+_sym_db.RegisterMessage(Heatmap)
+
 VisionEvent = _reflection.GeneratedProtocolMessageType('VisionEvent', (_message.Message,), {
   'DESCRIPTOR' : _VISIONEVENT,
   '__module__' : 'admobilize.vision.v1.vision_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.vision.v1.VisionEvent)
   })
 _sym_db.RegisterMessage(VisionEvent)
 
@@ -286,32 +302,32 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.admobilize.proto.vision.v1B\013VisionProtoP\001Z8bitbucket.org/admobilize/admobilizeapis-go/pkg/vision/v1\252\002\024AdMobilize.Vision.V1'
   _FACIALRECOGNITION.fields_by_name['face_descriptor']._options = None
   _FACIALRECOGNITION.fields_by_name['face_descriptor']._serialized_options = b'\020\001'
   _FRAMEDATA_SECTIONSENTRY._options = None
   _FRAMEDATA_SECTIONSENTRY._serialized_options = b'8\001'
-  _ENUMFACIALRECOGNITIONTAG._serialized_start=4597
-  _ENUMFACIALRECOGNITIONTAG._serialized_end=4854
-  _ENUMVEHICLERECOGNITIONTAG._serialized_start=4856
-  _ENUMVEHICLERECOGNITIONTAG._serialized_end=4936
-  _ZONEDIRECTION._serialized_start=4938
-  _ZONEDIRECTION._serialized_end=5012
-  _EVENTTAG._serialized_start=5015
-  _EVENTTAG._serialized_end=5148
-  _ENUMDETECTIONTAG._serialized_start=5151
-  _ENUMDETECTIONTAG._serialized_end=5293
-  _ENUMDETECTIONALGORITHM._serialized_start=5295
-  _ENUMDETECTIONALGORITHM._serialized_end=5392
-  _ENUMVIDEOCODEC._serialized_start=5394
-  _ENUMVIDEOCODEC._serialized_end=5514
-  _IMAGEFORMAT._serialized_start=5516
-  _IMAGEFORMAT._serialized_end=5627
-  _MOMENTOFDAY._serialized_start=5629
-  _MOMENTOFDAY._serialized_end=5693
+  _ENUMFACIALRECOGNITIONTAG._serialized_start=4805
+  _ENUMFACIALRECOGNITIONTAG._serialized_end=5062
+  _ENUMVEHICLERECOGNITIONTAG._serialized_start=5064
+  _ENUMVEHICLERECOGNITIONTAG._serialized_end=5144
+  _ZONEDIRECTION._serialized_start=5146
+  _ZONEDIRECTION._serialized_end=5220
+  _EVENTTAG._serialized_start=5223
+  _EVENTTAG._serialized_end=5356
+  _ENUMDETECTIONTAG._serialized_start=5359
+  _ENUMDETECTIONTAG._serialized_end=5501
+  _ENUMDETECTIONALGORITHM._serialized_start=5503
+  _ENUMDETECTIONALGORITHM._serialized_end=5600
+  _ENUMVIDEOCODEC._serialized_start=5602
+  _ENUMVIDEOCODEC._serialized_end=5722
+  _IMAGEFORMAT._serialized_start=5724
+  _IMAGEFORMAT._serialized_end=5835
+  _MOMENTOFDAY._serialized_start=5837
+  _MOMENTOFDAY._serialized_end=5901
   _POINT._serialized_start=92
   _POINT._serialized_end=121
   _SIZE._serialized_start=123
   _SIZE._serialized_end=160
   _RECTANGLE._serialized_start=162
   _RECTANGLE._serialized_end=226
   _VEHICLERECOGNITION._serialized_start=229
@@ -334,34 +350,38 @@
   _ZONECONFIG._serialized_end=1953
   _AREACONFIG._serialized_start=1955
   _AREACONFIG._serialized_end=2079
   _AREAANDZONECONFIG._serialized_start=2082
   _AREAANDZONECONFIG._serialized_end=2258
   _VEHICLECONFIG._serialized_start=2260
   _VEHICLECONFIG._serialized_end=2359
-  _VISIONEVENT._serialized_start=2362
-  _VISIONEVENT._serialized_end=2678
-  _RECTANGULARDETECTION._serialized_start=2681
-  _RECTANGULARDETECTION._serialized_end=3174
-  _IMAGELIST._serialized_start=3176
-  _IMAGELIST._serialized_end=3234
-  _VIDEO._serialized_start=3236
-  _VIDEO._serialized_end=3329
-  _IMAGE._serialized_start=3331
-  _IMAGE._serialized_end=3446
-  _FRAMEDATA._serialized_start=3449
-  _FRAMEDATA._serialized_end=3680
-  _FRAMEDATA_SECTIONSENTRY._serialized_start=3633
-  _FRAMEDATA_SECTIONSENTRY._serialized_end=3680
-  _FRAMEDATALIST._serialized_start=3682
-  _FRAMEDATALIST._serialized_end=3746
-  _VISIONRESULT._serialized_start=3749
-  _VISIONRESULT._serialized_end=4157
-  _MODELINFERENCE._serialized_start=4159
-  _MODELINFERENCE._serialized_end=4255
-  _FACECROWDINFERENCETIMERESULT._serialized_start=4257
-  _FACECROWDINFERENCETIMERESULT._serialized_end=4353
-  _VISIONEVALUATIONRESULT._serialized_start=4356
-  _VISIONEVALUATIONRESULT._serialized_end=4514
-  _VISIONRESULTLIST._serialized_start=4516
-  _VISIONRESULTLIST._serialized_end=4594
+  _HEATMAPDATA._serialized_start=2361
+  _HEATMAPDATA._serialized_end=2411
+  _HEATMAP._serialized_start=2413
+  _HEATMAP._serialized_end=2519
+  _VISIONEVENT._serialized_start=2522
+  _VISIONEVENT._serialized_end=2886
+  _RECTANGULARDETECTION._serialized_start=2889
+  _RECTANGULARDETECTION._serialized_end=3382
+  _IMAGELIST._serialized_start=3384
+  _IMAGELIST._serialized_end=3442
+  _VIDEO._serialized_start=3444
+  _VIDEO._serialized_end=3537
+  _IMAGE._serialized_start=3539
+  _IMAGE._serialized_end=3654
+  _FRAMEDATA._serialized_start=3657
+  _FRAMEDATA._serialized_end=3888
+  _FRAMEDATA_SECTIONSENTRY._serialized_start=3841
+  _FRAMEDATA_SECTIONSENTRY._serialized_end=3888
+  _FRAMEDATALIST._serialized_start=3890
+  _FRAMEDATALIST._serialized_end=3954
+  _VISIONRESULT._serialized_start=3957
+  _VISIONRESULT._serialized_end=4365
+  _MODELINFERENCE._serialized_start=4367
+  _MODELINFERENCE._serialized_end=4463
+  _FACECROWDINFERENCETIMERESULT._serialized_start=4465
+  _FACECROWDINFERENCETIMERESULT._serialized_end=4561
+  _VISIONEVALUATIONRESULT._serialized_start=4564
+  _VISIONEVALUATIONRESULT._serialized_end=4722
+  _VISIONRESULTLIST._serialized_start=4724
+  _VISIONRESULTLIST._serialized_end=4802
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/driver_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/maloseye_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/malos/v1/maloseye_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/common/entity_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/common/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/common/admobilize_types_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/common/admobilize_types_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/common/job_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/common/job_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py` & `admobilizeapis-2023.6.29.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/PKG-INFO` & `admobilizeapis-2023.6.29.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.6.22.post1
+Version: 2023.6.29.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/SOURCES.txt` & `admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/PKG-INFO` & `admobilizeapis-2023.6.29.post1/admobilizeapis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.6.22.post1
+Version: 2023.6.29.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.6.22.post1/README.md` & `admobilizeapis-2023.6.29.post1/README.md`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.22.post1/setup.py` & `admobilizeapis-2023.6.29.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_requires = ["google-api-core >= 1.6.0, < 2.0.0dev", "protobuf >= 3.6.0, < 4.0"]
 
 extras_require = {"grpc": ["grpcio>=1.2.0"]}
 
 setup(
     name="admobilizeapis",
-    version='2023.06.22r1',
+    version='2023.06.29r1',
     author="AdMobilize Team",
     author_email="devel@admobilize.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
```

