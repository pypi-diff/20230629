# Comparing `tmp/actinia-core-4.9.1.tar.gz` & `tmp/actinia-core-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actinia-core-4.9.1.tar", last modified: Wed Jun 14 12:52:15 2023, max compression
+gzip compressed data, was "actinia-core-4.9.2.tar", last modified: Thu Jun 29 15:14:13 2023, max compression
```

## Comparing `actinia-core-4.9.1.tar` & `actinia-core-4.9.2.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.876929 actinia-core-4.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-14 12:51:39.000000 actinia-core-4.9.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-06-14 12:51:39.000000 actinia-core-4.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-14 12:52:15.876929 actinia-core-4.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-14 12:51:39.000000 actinia-core-4.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-14 12:52:08.000000 actinia-core-4.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:52:15.876929 actinia-core-4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-14 12:51:39.000000 actinia-core-4.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.848929 actinia-core-4.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.852929 actinia-core-4.9.1/src/actinia_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.852929 actinia-core-4.9.1/src/actinia_core/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3104 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/cli/actinia_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12144 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/cli/actinia_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5432 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/cli/rq_custom_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/cli/webhook_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/cli/webhook_server_broken.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.856929 actinia-core-4.9.1/src/actinia_core/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/api_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/aws_sentinel_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    40540 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34970 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/google_satellite_bigquery_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/keycloak_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/landsat_processing_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    65904 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/process_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/process_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    17002 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/process_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/redis_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/redis_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    26500 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/sentinel_processing_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/common/user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/geodata_download_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/google_cloud_storage_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/grass_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/grass_modules_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/interim_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/list_grass_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/logging_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/mapset_merge_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/messages_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/redis_api_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/redis_fluentd_logger_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/redis_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/redis_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/request_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/resource_data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/resources_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/stac_exporter_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/stac_importer_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/storage_interface_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/storage_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/storage_interface_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/storage_interface_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/models/
--rw-r--r--   0 runner    (1001) docker     (123)    29234 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/models/process_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    44666 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/models/response_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/base/renderer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/download_cache_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_custom_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_processing_with_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/persistent_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/process_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/raster_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/raster_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/raster_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/resource_storage_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/vector_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    76693 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/raster_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/strds_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/vector_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.860929 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_with_export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_with_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_with_export/raster_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.864929 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/download_cache_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/location_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/map_layer_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/mapset_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/persistent_mapset_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/raster_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/raster_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/resource_storage_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/strds_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/strds_raster_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/vector_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.864929 actinia-core-4.9.1/src/actinia_core/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/download_cache_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/ephemeral_custom_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/ephemeral_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/ephemeral_processing_with_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/location_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/map_layer_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/mapset_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/persistent_mapset_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/persistent_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/process_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/raster_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/raster_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/raster_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/raster_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/raster_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/resource_storage_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/strds_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/strds_raster_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/strds_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/vector_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/processing/common/vector_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.868929 actinia-core-4.9.1/src/actinia_core/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/api_log_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.868929 actinia-core-4.9.1/src/actinia_core/rest/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/base_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/endpoint_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/map_layer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/renderer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/resource_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/base/user_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/download_cache_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/ephemeral_custom_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/ephemeral_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/ephemeral_processing_with_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/location_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/map_layer_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/mapset_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/mapsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/persistent_mapset_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/persistent_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/process_chain_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/process_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/raster_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/raster_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/raster_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/raster_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/raster_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/resource_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/resource_storage_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/resource_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/strds_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/strds_raster_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/strds_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/vector_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/rest/vector_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-14 12:51:39.000000 actinia-core-4.9.1/src/actinia_core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.852929 actinia-core-4.9.1/src/actinia_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-14 12:52:15.000000 actinia-core-4.9.1/src/actinia_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-14 12:52:15.000000 actinia-core-4.9.1/src/actinia_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:52:15.000000 actinia-core-4.9.1/src/actinia_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-14 12:52:15.000000 actinia-core-4.9.1/src/actinia_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-14 12:52:15.000000 actinia-core-4.9.1/src/actinia_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 12:52:15.000000 actinia-core-4.9.1/src/actinia_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:52:15.876929 actinia-core-4.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_api_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_mapset_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_mapset_merging_strds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_process_postgis_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_process_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_process_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_export_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_export_to_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_export_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    33657 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_mapset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_processing_stdout_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_async_raster_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_aws_sentinel_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_common_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_download_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_geodata_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_google_cloud_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    40380 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_job_resumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_location_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_mapset_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_mapsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_message_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_process_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_raster_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_raster_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_raster_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_raster_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_raster_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_raster_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_resource_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_resource_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    33069 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_resource_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_resource_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_strds_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_strds_raster_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_strds_raster_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_vector_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_vector_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_vector_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_vector_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_version_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-06-14 12:51:39.000000 actinia-core-4.9.1/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.678127 actinia-core-4.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 15:13:35.000000 actinia-core-4.9.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-06-29 15:13:35.000000 actinia-core-4.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-29 15:14:13.678127 actinia-core-4.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-29 15:13:35.000000 actinia-core-4.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-29 15:14:07.000000 actinia-core-4.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:14:13.678127 actinia-core-4.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 15:13:35.000000 actinia-core-4.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.646127 actinia-core-4.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.646127 actinia-core-4.9.2/src/actinia_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.650127 actinia-core-4.9.2/src/actinia_core/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3103 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/cli/actinia_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12138 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/cli/actinia_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5431 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/cli/rq_custom_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/cli/webhook_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/cli/webhook_server_broken.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.654127 actinia-core-4.9.2/src/actinia_core/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.654127 actinia-core-4.9.2/src/actinia_core/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/api_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/aws_sentinel_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40540 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34965 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/google_satellite_bigquery_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/keycloak_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/landsat_processing_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65895 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/process_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/process_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/process_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/redis_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/redis_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/sentinel_processing_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/common/user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/geodata_download_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/google_cloud_storage_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/grass_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/grass_modules_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/interim_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/list_grass_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/logging_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/mapset_merge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/messages_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/redis_api_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/redis_fluentd_logger_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/redis_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/redis_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/request_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/resource_data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/resources_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/stac_exporter_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/stac_importer_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/storage_interface_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/storage_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/storage_interface_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/storage_interface_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.654127 actinia-core-4.9.2/src/actinia_core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    29234 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/models/process_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44666 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/models/response_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.654127 actinia-core-4.9.2/src/actinia_core/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.654127 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.658127 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.658127 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/base/renderer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/download_cache_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_custom_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_processing_with_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/persistent_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/process_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/raster_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/raster_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/raster_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/resource_storage_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/vector_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76692 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.658127 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/raster_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/strds_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/vector_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.658127 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_with_export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_with_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_with_export/raster_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.658127 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/download_cache_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/location_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/map_layer_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/mapset_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/persistent_mapset_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/raster_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/raster_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/resource_storage_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/strds_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/strds_raster_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/vector_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.662127 actinia-core-4.9.2/src/actinia_core/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/download_cache_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/ephemeral_custom_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/ephemeral_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/ephemeral_processing_with_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/location_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/map_layer_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/mapset_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/persistent_mapset_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/persistent_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/process_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/raster_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/raster_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/raster_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/raster_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/raster_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/resource_storage_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/strds_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/strds_raster_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/strds_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/vector_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/processing/common/vector_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.666127 actinia-core-4.9.2/src/actinia_core/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/api_log_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.666127 actinia-core-4.9.2/src/actinia_core/rest/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/base_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/endpoint_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/map_layer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/renderer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17215 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/resource_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/base/user_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/download_cache_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/ephemeral_custom_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/ephemeral_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/ephemeral_processing_with_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/location_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/map_layer_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/mapset_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/mapsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/persistent_mapset_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/persistent_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/process_chain_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/process_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/raster_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/raster_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/raster_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/raster_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/raster_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25167 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/resource_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/resource_storage_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/resource_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/strds_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/strds_raster_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/strds_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/vector_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/rest/vector_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-29 15:13:35.000000 actinia-core-4.9.2/src/actinia_core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.650127 actinia-core-4.9.2/src/actinia_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-29 15:14:13.000000 actinia-core-4.9.2/src/actinia_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-29 15:14:13.000000 actinia-core-4.9.2/src/actinia_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:14:13.000000 actinia-core-4.9.2/src/actinia_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 15:14:13.000000 actinia-core-4.9.2/src/actinia_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-29 15:14:13.000000 actinia-core-4.9.2/src/actinia_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:14:13.000000 actinia-core-4.9.2/src/actinia_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:13.678127 actinia-core-4.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_api_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_mapset_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_mapset_merging_strds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_process_postgis_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_process_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_process_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20059 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_export_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_export_to_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_export_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33657 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_mapset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_processing_stdout_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_async_raster_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_aws_sentinel_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_common_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_download_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_geodata_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_google_cloud_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40376 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_job_resumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_location_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_mapset_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_mapsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_message_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_process_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_raster_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_raster_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_raster_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_raster_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_raster_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_raster_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_resource_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_resource_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33069 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_resource_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_resource_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_strds_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_strds_raster_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_strds_raster_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_vector_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_vector_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_vector_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_vector_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_version_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-06-29 15:13:35.000000 actinia-core-4.9.2/tests/test_webhook.py
```

### Comparing `actinia-core-4.9.1/LICENSE.txt` & `actinia-core-4.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/PKG-INFO` & `actinia-core-4.9.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: actinia-core
-Version: 4.9.1
-Summary: Actinia Core is an open source REST API for scalable, distributed, high performance processing of geographical data that uses mainly GRASS GIS for computational tasks
-Author: Carmen Tawalika, Anika Weinmann, Guido Riembauer, Markus Metz, Julia Haas, Marc Jansen, Jorge A. Herrera Maldonado, Sören Gebbert, Markus Neteler, Momen Mawad, and more
-Project-URL: Homepage, https://github.com/actinia-org/actinia_core
-Project-URL: Tutorial, https://actinia-org.github.io/actinia_core
-Project-URL: API_Docs, https://redocly.github.io/redoc/?url=https://actinia.mundialis.de/latest/swagger.json
-Keywords: processing,earth observation,cloud-based processing,rest api,gis,grass gis,osgeo
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: plugins
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
 # Actinia — The GRASS GIS REST API
 
 Software [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5879231.svg)](https://doi.org/10.5281/zenodo.5879231)
 Article [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2631917.svg)](https://doi.org/10.5281/zenodo.2631917)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Docker pulls](https://img.shields.io/docker/pulls/mundialis/actinia-core.svg)](https://hub.docker.com/r/mundialis/actinia-core)
 
@@ -69,14 +52,15 @@
 docker pull mundialis/actinia-core
 ```
 
 For own deployments or local dev-setup, see the `docker/` subfolder.
 
 Actinia is also available on [OSGeoLive](https://live.osgeo.org/en/overview/actinia_overview.html).
 
+
 ## Examples
 
 ### Data management
 
 * List all locations that are available in the actinia persistent database:
 
 ```bash
@@ -122,12 +106,74 @@
 To see a simple **list of endpoints** (and more), consult the "paths" section in the [API JSON](https://actinia.mundialis.de/api/v3/swagger.json); or, to list the available endpoints on command line, run
 
 ```bash
 # sudo npm install -g json
 curl -u 'demouser:gu3st!pa55w0rd' -X GET https://actinia.mundialis.de/api/v3/swagger.json | json paths | json -ka
 ```
 
+## Development
+
+### Use pre-commit
+
+It is highly recommended to install and use [pre-commit](https://pre-commit.com)
+before submitting any new or modified code or any other content. The pre-commit
+Git hooks set checks validity and executes automated formatting for
+a range of file formats, including Python. Pre-commit installs
+all necessary tools in a virtual environment upon first use.
+
+If you never used pre-commit before, you must start by installing it on your
+system. You only do it once:
+
+```bash
+python -m pip install pre-commit
+```
+
+Pre-commit must then be activated in the code repository. Change the directory
+to the root folder and use the `install` command:
+
+```bash
+cd <actinia-core_source_dir>
+
+# once per repo
+pre-commit install
+```
+
+Pre-commit will then be automatically triggered by the `git commit` command. If
+it finds any problem it will abort the commit and try to solve it automatically.
+In that case review the changes and run again `git add` and
+`git commit`.
+
+It is also possible to run pre-commit manually, e.g:
+
+```bash
+pre-commit run flake8 --all-files
+pre-commit run black --all-files
+# pre-commit run yamllint --all-files
+# pre-commit run markdownlint --all-files
+```
+
+Or to target a specific set of files:
+
+```bash
+pre-commit run --files src/*
+```
+
+The pre-commit hooks set is defined in
+[.pre-commit-config.yaml](.pre-commit-config.yaml).
+
+It is possible to temporally disable the pre-commit hooks in the repo, e.g. while
+working on older branches:
+
+```bash
+pre-commit uninstall
+```
+
+And to reactivate pre-commit again:
+
+```bash
+git switch main
+pre-commit install
+```
+
 ## Thanks to all contributors ❤
 
-<a href = "https://github.com/actinia-org/actinia-core/graphs/contributors">
-    <img src = "https://contrib.rocks/image?repo=actinia-org/actinia-core"/>
-</a>
+[![actinia-core contributors](https://contrib.rocks/image?repo=actinia-org/actinia-core "actinia-core contributors")](https://github.com/actinia-org/actinia-core/graphs/contributors)
```

### Comparing `actinia-core-4.9.1/pyproject.toml` & `actinia-core-4.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "actinia-core"
-version = "4.9.1"
+version = "4.9.2"
 description = "Actinia Core is an open source REST API for scalable, distributed, high performance processing of geographical data that uses mainly GRASS GIS for computational tasks"
 readme = "README.md"
 authors = [
     { name = "Carmen Tawalika"},
     { name = "Anika Weinmann"},
     { name = "Guido Riembauer"},
     { name = "Markus Metz"},
```

### Comparing `actinia-core-4.9.1/setup.py` & `actinia-core-4.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/__init__.py` & `actinia-core-4.9.2/src/actinia_core/__init__.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/cli/actinia_server.py` & `actinia-core-4.9.2/src/actinia_core/cli/actinia_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 __copyright__ = (
     "Copyright 2016-2023, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 def main():
-
     parser = argparse.ArgumentParser(
         description="Start actinia server. A running redis server"
         + " is required."
     )
 
     parser.add_argument(
         "--host",
```

### Comparing `actinia-core-4.9.1/src/actinia_core/cli/actinia_user.py` & `actinia-core-4.9.2/src/actinia_core/cli/actinia_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,14 @@
         host=server,
         port=port,
         password=redis_password,
     )
 
     # CREATE ############################
     if args.action == "create":
-
         if args.user_id is None:
             sys.stderr.write("You need to provide a user id\n")
             return
 
         if args.user_group is None:
             sys.stderr.write("You need to provide a user group\n")
             return
@@ -329,15 +328,14 @@
     # UPDATE ############################
     elif (
         args.action == "update"
         or args.action == "update_add"
         or args.action == "update_rm"
         or args.action == "update_rm_location"
     ):
-
         if args.user_id is None:
             sys.stderr.write("You need to provide a user id\n")
             return
 
         user = ActiniaUser(user_id=args.user_id)
 
         if user.exists() == 0:
@@ -358,46 +356,42 @@
             return
         else:
             sys.stderr.write("Unable to update the user <%s>\n" % args.user_id)
             return
 
     # DELETE ############################
     elif args.action == "delete":
-
         user = ActiniaUser(args.user_id)
 
         if user.exists() == 1:
             if user.delete() is True:
                 sys.stderr.write("User <%s> deleted\n" % args.user_id)
                 return
             else:
                 sys.stderr.write("Unable to delete user <%s>\n" % args.user_id)
                 return
         else:
             sys.stderr.write("User <%s> does not exist\n" % args.user_id)
 
     # SHOW ##############################
     elif args.action == "show":
-
         user = ActiniaUser(args.user_id)
 
         if user.exists() == 1:
             sys.stdout.write(str(user))
         else:
             sys.stderr.write("User <%s> does not exist\n" % args.user_id)
 
     # LIST ##############################
     elif args.action == "list":
-
         user = ActiniaUser(args.user_id)
         pprint.pprint(user.list_all_users())
 
     # PWCHECK ###########################
     elif args.action == "pwcheck":
-
         if args.user_id is None:
             sys.stderr.write("You need to provide a user id\n")
             return
 
         if args.password is None:
             sys.stderr.write("You need to provide a password\n")
             return
```

### Comparing `actinia-core-4.9.1/src/actinia_core/cli/rq_custom_worker.py` & `actinia-core-4.9.2/src/actinia_core/cli/rq_custom_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     with Connection(
         Redis(
             conf.REDIS_QUEUE_SERVER_URL,
             conf.REDIS_QUEUE_SERVER_PORT,
             password=conf.REDIS_QUEUE_SERVER_PASSWORD,
         )
     ):
-
         logger = logging.getLogger("rq.worker")
         logger.setLevel(logging.ERROR)
 
         node = platform.node()
 
         if conf.LOG_INTERFACE == "fluentd" and has_fluent is True:
             custom_format = {
```

### Comparing `actinia-core-4.9.1/src/actinia_core/cli/webhook_server.py` & `actinia-core-4.9.2/src/actinia_core/cli/webhook_server_broken.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,53 +25,60 @@
 """
 Dummy server to response HTTP code 200 to a POST call from an actinia webhook
 """
 import argparse
 import psutil
 from flask import Flask, make_response, jsonify, request, json
 from multiprocessing import Process
-from werkzeug.exceptions import BadRequest
+from werkzeug.exceptions import BadRequest, UnsupportedMediaType
 
 from pprint import pprint
 
 __license__ = "GPLv3"
 __author__ = "Soeren Gebbert, Anika Weinmann, Carmen Tawalika"
 __copyright__ = "Copyright 2016-2023, mundialis GmbH & Co. KG"
 __maintainer__ = "mundialis GmbH & Co. KG"
 
 
 flask_app = Flask(__name__)
 
 
 @flask_app.route("/webhook/finished", methods=["GET", "POST"])
 def finished():
+    port = request.server[1]
     try:
         pprint(json.loads(request.get_json()))
     except BadRequest:
         pass
+    except UnsupportedMediaType:
+        pass
     except TypeError:
         pass
-    return make_response(jsonify("OK"), 200)
+    sp = Process(target=shutdown_server, args=(port,))
+    sp.start()
+    return make_response(jsonify("Server shutting down..."), 200)
 
 
 @flask_app.route("/webhook/update", methods=["GET", "POST"])
 def update():
     try:
         pprint(json.loads(request.get_json()))
     except BadRequest:
         pass
+    except UnsupportedMediaType:
+        pass
     except TypeError:
         pass
     return make_response(jsonify("OK"), 200)
 
 
 def shutdown_server(port):
     for proc in psutil.process_iter():
         if (
-            proc.name() == "webhook-server"
+            proc.name() == "webhook-server-"
             and proc.as_dict()["connections"]
             and proc.as_dict()["connections"][0].laddr.port == port
         ):
             proc.kill()
 
 
 @flask_app.route("/shutdown", methods=["GET"])
@@ -79,18 +86,17 @@
     port = request.server[1]
     sp = Process(target=shutdown_server, args=(port,))
     sp.start()
     return make_response(jsonify("Server shutting down..."), 200)
 
 
 def main():
-
     parser = argparse.ArgumentParser(
-        description="Start a REST webhook server that exposes a GET/POST "
-        "endpoint which returns HTTP code 200 if called. The endpoints are: "
+        description="Start a webhook server that exposes GET/POST endpoints "
+        "which returns HTTP code 200 if called. The endpoints are: "
         " - /webhook/finished for finished callbacks "
         " - /webhook/update for status update callbacks"
     )
 
     parser.add_argument(
         "--host",
         type=str,
```

### Comparing `actinia-core-4.9.1/src/actinia_core/cli/webhook_server_broken.py` & `actinia-core-4.9.2/src/actinia_core/cli/webhook_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,56 +25,57 @@
 """
 Dummy server to response HTTP code 200 to a POST call from an actinia webhook
 """
 import argparse
 import psutil
 from flask import Flask, make_response, jsonify, request, json
 from multiprocessing import Process
-from werkzeug.exceptions import BadRequest
+from werkzeug.exceptions import BadRequest, UnsupportedMediaType
 
 from pprint import pprint
 
 __license__ = "GPLv3"
 __author__ = "Soeren Gebbert, Anika Weinmann, Carmen Tawalika"
 __copyright__ = "Copyright 2016-2023, mundialis GmbH & Co. KG"
 __maintainer__ = "mundialis GmbH & Co. KG"
 
 
 flask_app = Flask(__name__)
 
 
 @flask_app.route("/webhook/finished", methods=["GET", "POST"])
 def finished():
-    port = request.server[1]
     try:
         pprint(json.loads(request.get_json()))
     except BadRequest:
         pass
+    except UnsupportedMediaType:
+        pass
     except TypeError:
         pass
-    sp = Process(target=shutdown_server, args=(port,))
-    sp.start()
-    return make_response(jsonify("Server shutting down..."), 200)
+    return make_response(jsonify("OK"), 200)
 
 
 @flask_app.route("/webhook/update", methods=["GET", "POST"])
 def update():
     try:
         pprint(json.loads(request.get_json()))
     except BadRequest:
         pass
+    except UnsupportedMediaType:
+        pass
     except TypeError:
         pass
     return make_response(jsonify("OK"), 200)
 
 
 def shutdown_server(port):
     for proc in psutil.process_iter():
         if (
-            proc.name() == "webhook-server-"
+            proc.name() == "webhook-server"
             and proc.as_dict()["connections"]
             and proc.as_dict()["connections"][0].laddr.port == port
         ):
             proc.kill()
 
 
 @flask_app.route("/shutdown", methods=["GET"])
@@ -82,18 +83,17 @@
     port = request.server[1]
     sp = Process(target=shutdown_server, args=(port,))
     sp.start()
     return make_response(jsonify("Server shutting down..."), 200)
 
 
 def main():
-
     parser = argparse.ArgumentParser(
-        description="Start a webhook server that exposes GET/POST endpoints "
-        "which returns HTTP code 200 if called. The endpoints are: "
+        description="Start a REST webhook server that exposes a GET/POST "
+        "endpoint which returns HTTP code 200 if called. The endpoints are: "
         " - /webhook/finished for finished callbacks "
         " - /webhook/update for status update callbacks"
     )
 
     parser.add_argument(
         "--host",
         type=str,
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/api_logger.py` & `actinia-core-4.9.2/src/actinia_core/core/common/api_logger.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/app.py` & `actinia-core-4.9.2/src/actinia_core/core/common/app.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/aws_sentinel_interface.py` & `actinia-core-4.9.2/src/actinia_core/core/common/aws_sentinel_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,14 @@
         # S2A_MSIL1C_20171031T000721_N0206_R016_T01WCP_20171031T015145
 
         # Assign default bands
         if bands is None:
             bands = ["B04", "B08"]
 
         try:
-
             for band in bands:
                 if band not in self.sentinel_bands:
                     raise Exception("Unknown Sentinel-2 band name <%s>" % band)
 
             result = []
 
             for product_id in product_ids:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/config.py` & `actinia-core-4.9.2/src/actinia_core/core/common/config.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/exceptions.py` & `actinia-core-4.9.2/src/actinia_core/core/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/google_satellite_bigquery_interface.py` & `actinia-core-4.9.2/src/actinia_core/core/common/google_satellite_bigquery_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,14 @@
                 "south_lat": 50.67277,
                 "total_size": 161222513,
                 "west_lon": 153.20544
               }
             ]
         """
         try:
-
             self._start_clients()
             scene_id_query = None
             spacecraft_id_query = None
             temporal_query = None
             spatial_query = None
             cloud_cover_query = None
             has_where_statement = False
@@ -568,15 +567,14 @@
         # ]
 
         # Assign default bands
         if bands is None:
             bands = ["B1", "B2"]
 
         try:
-
             self._start_clients()
 
             for scene_id in scene_ids:
                 sensor_id = extract_sensor_id_from_scene_id(scene_id)
                 for band in bands:
                     if band not in self.landsat_scene_bands[sensor_id]:
                         raise Exception(
@@ -591,15 +589,14 @@
             )
 
             query_results = self.bigquery_client.query(query)
             result = {}
 
             if query_results.result():
                 for row in query_results.result():
-
                     scene_id, sensing_time, base_url = row
                     public_url = self.gcs_url + base_url[5:]
                     sensor_id = extract_sensor_id_from_scene_id(scene_id)
 
                     result[scene_id] = {}
                     result[scene_id]["timestamp"] = sensing_time
 
@@ -768,15 +765,14 @@
         # 20170208T092131_B01.jp2
 
         # Assign default bands
         if bands is None:
             bands = ["B04", "B08"]
 
         try:
-
             self._start_clients()
 
             for band in bands:
                 if band not in self.sentinel_bands:
                     raise Exception("Unknown Sentinel-2 band name <%s>" % band)
 
             # Select specific columns from the sentinel table
@@ -789,15 +785,14 @@
 
             rows = list(self.bigquery_client.query(query))  # API request
 
             result = {}
 
             if rows:
                 for row in rows:
-
                     (
                         granule_id,
                         product_id,
                         sensing_time,
                         datatake_identifier,
                         base_url,
                     ) = row
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/keycloak_user.py` & `actinia-core-4.9.2/src/actinia_core/core/common/keycloak_user.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/landsat_processing_library.py` & `actinia-core-4.9.2/src/actinia_core/core/common/landsat_processing_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,14 @@
         "oct",
         "nov",
         "dec",
     ]
 
     # Check for time zone info in the datetime object
     if dt.tzinfo is not None:
-
         tz = dt.tzinfo.utcoffset(0)
         if tz.seconds > 86400 / 2:
             tz = (tz.seconds - 86400) / 60
         else:
             tz = tz.seconds / 60
 
         string = "%.2i %s %.2i %.2i:%.2i:%.2i %+.4i" % (
@@ -315,15 +314,14 @@
             url = scene_id_to_google_url(self.scene_id, suffix)
 
             self.url_list.append(url)
             self.copy_file_list.append((temp_file_path, file_path))
             count += 1
 
     def get_import_process_list(self):
-
         count = 0
         import_commands = []
 
         for file_path in self.file_list:
             if "_MTL.TXT" not in file_path.upper():
                 raster_name = "%s%s" % (
                     self.scene_id,
@@ -338,15 +336,14 @@
                 )
                 import_commands.append(p)
                 count += 1
 
         return import_commands
 
     def get_i_landsat_toar_process_list(self, atcor_method):
-
         option = "uncorrected"
 
         if atcor_method == "DOS4":
             option = "dos4"
 
         if atcor_method == "DOS1":
             option = "dos1"
@@ -370,15 +367,14 @@
             id=f"top_of_atmosphere_{self.scene_id}",
             skip_permission_check=True,
         )
         toar_commands.append(p)
         return toar_commands
 
     def get_i_vi_process_list(self, atcor_method, processing_method):
-
         self.ndvi_name = "%s_%s_%s" % (
             self.scene_id,
             atcor_method,
             processing_method,
         )
 
         ndvi_commands = []
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/process_chain.py` & `actinia-core-4.9.2/src/actinia_core/core/common/process_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
         self.message_logger = message_logger
         self.import_descr_list = []
         self.webhook_finished = None
         self.webhook_update = None
         self.webhook_auth = None
 
     def process_chain_to_process_list(self, process_chain):
-
         if not process_chain:
             raise AsyncProcessError("Process chain is empty")
 
         if "list" in process_chain and "version" in process_chain:
             return self._process_chain_to_process_list(process_chain)
         else:
             return self._process_chain_to_process_list_legacy(process_chain)
@@ -184,15 +183,14 @@
             raise AsyncProcessError(
                 "List of processes to be executed is missing "
                 "in the process chain definition"
             )
 
         # Check for the webhooks
         if "webhooks" in process_chain:
-
             if "finished" in process_chain["webhooks"]:
                 self.webhook_finished = process_chain["webhooks"]["finished"]
                 self._check_if_webhook_exists(
                     self.webhook_finished, process_chain, "finished"
                 )
             else:
                 raise AsyncProcessError(
@@ -202,15 +200,14 @@
             if "update" in process_chain["webhooks"]:
                 self.webhook_update = process_chain["webhooks"]["update"]
                 self._check_if_webhook_exists(
                     self.webhook_update, process_chain, "update"
                 )
 
         for process_descr in process_chain["list"]:
-
             if "module" in process_descr:
                 module = self._create_module_process(process_descr)
                 if module:
                     process_list.append(module)
             elif "exe" in process_descr:
                 exe = self._create_exec_process(process_descr)
                 if exe:
@@ -764,15 +761,14 @@
 
         executable = module_descr["exe"]
 
         params = []
 
         if "params" in module_descr:
             for search_string in module_descr["params"]:
-
                 # Search for file identifiers and generate the temporary file
                 # path
                 if "$file" in search_string and "::" in search_string:
                     file_id = search_string.split("::")[1]
                     # Generate the temporary file path and store it in the dict
                     if file_id not in self.temporary_pc_files:
                         self.temporary_pc_files[
@@ -829,15 +825,14 @@
 
             # RASTER; VECTOR, FILE
             if (
                 entry["import_descr"]["type"].lower() == "raster"
                 or entry["import_descr"]["type"].lower() == "vector"
                 or entry["import_descr"]["type"].lower() == "file"
             ):
-
                 rvf_downimport_commands = (
                     self._get_raster_vector_file_download_import_command(entry)
                 )
                 downimp_list.extend(rvf_downimport_commands)
 
             # POSTGIS
             elif entry["import_descr"]["type"].lower() == "postgis":
@@ -926,15 +921,14 @@
                 "Missing module name in module description of id %s" % str(id)
             )
 
         module_name = module_descr["module"]
 
         if "inputs" in module_descr:
             for key in module_descr["inputs"]:
-
                 search_string = str(module_descr["inputs"][key])
 
                 # Search for file identifiers and generate the temporary file
                 # path
                 if "$file" in search_string and "::" in search_string:
                     file_id = search_string.split("::")[1]
                     # Generate the temporary file path and store it in the dict
@@ -945,15 +939,14 @@
 
                     param = "%s=%s" % (key, self.temporary_pc_files[file_id])
                 else:
                     param = "%s=%s" % (key, module_descr["inputs"][key])
                     # Check for mapset in input name and append it
                     # to the list of required mapsets
                     if "@" in str(module_descr["inputs"][key]):
-
                         # Mapset names are after an @ symbol
                         # Mapsets in expressions can be detected by replacing
                         # the symbols like *, +, :, /, {, (,},], ... by spaces
                         # and split the string by spaces, searching in each
                         # substring for @
 
                         symbols = [
@@ -993,15 +986,14 @@
                                         self.required_mapsets.append(mapset)
 
                 parameters.append(param)
 
         if "outputs" in module_descr:
             for key in module_descr["outputs"]:
                 if "name" in module_descr["outputs"][key]:
-
                     search_string = module_descr["outputs"][key]["name"]
 
                     # Search for file identifiers and generate the temporary
                     # file path
                     if "$file" in search_string and "::" in search_string:
                         file_id = search_string.split("::")[1]
                         # Generate the temporary file path and store it in the
@@ -1125,15 +1117,14 @@
                 "Missing executable name in module description of id %s"
                 % str(id)
             )
 
         executable = module_descr["executable"]
         if "parameters" in module_descr:
             for search_string in module_descr["parameters"]:
-
                 # Search for file identifiers and generate the temporary file
                 # path
                 if "$file" in search_string and "::" in search_string:
                     file_id = search_string.split("::")[1]
                     # Generate the temporary file path and store it in the dict
                     if file_id not in self.temporary_pc_files:
                         self.temporary_pc_files[
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/process_object.py` & `actinia-core-4.9.2/src/actinia_core/core/common/process_object.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/process_queue.py` & `actinia-core-4.9.2/src/actinia_core/core/common/process_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,14 @@
                             this with a termination or error message, if not
                             send a resource update
     - termination commits - Terminate the process and send an update to the
                             resource database about the termination
     """
 
     def __init__(self, func, timeout, resource_logger, args):
-
         self.process = Process(target=func, args=args)
         self.timeout = timeout
         self.config = args[0].config
         self.resource_id = args[0].resource_id
         self.iteration = args[0].iteration
         self.user_id = args[0].user_id
         self.api_info = args[0].api_info
@@ -238,15 +237,14 @@
         """Check the exitcode, if a non-zero exit code was received then
         send an update to the resource logger that something strange happened.
         Send only if the status of the resource is not "error", "terminated"
         or "timeout".
 
         """
         if self.process.exitcode is not None and self.process.exitcode != 0:
-
             # Check if the process noticed the error already
             response_data = self.resource_logger.get(
                 self.user_id, self.resource_id, self.iteration
             )
 
             if response_data is not None:
                 http_code, response_model = pickle.loads(response_data)
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/redis_base.py` & `actinia-core-4.9.2/src/actinia_core/core/common/redis_base.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/redis_interface.py` & `actinia-core-4.9.2/src/actinia_core/core/common/redis_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     if timeout > 2147483647:
         timeout = -1  # never exprire
     ret = queue.enqueue(
         func,
         *args,
         job_timeout=timeout,
         ttl=global_config.REDIS_QUEUE_JOB_TTL,
-        result_ttl=global_config.REDIS_QUEUE_JOB_TTL
+        result_ttl=global_config.REDIS_QUEUE_JOB_TTL,
     )
     log.info(ret)
 
 
 def enqueue_job(timeout, func, *args, queue_type_overwrite=None):
     """Write the provided function in a queue
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/sentinel_processing_library.py` & `actinia-core-4.9.2/src/actinia_core/core/common/sentinel_processing_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         "oct",
         "nov",
         "dec",
     ]
 
     # Check for time zone info in the datetime object
     if dt.tzinfo is not None:
-
         tz = dt.tzinfo.utcoffset(0)
         if tz.seconds > 86400 / 2:
             tz = (tz.seconds - 86400) / 60
         else:
             tz = tz.seconds / 60
 
         string = "%.2i %s %.2i %.2i:%.2i:%.2i %+.4i" % (
@@ -256,15 +255,14 @@
             )
             self.message_logger.info(
                 (gml_temp_file_name, self.gml_cache_file_name)
             )
 
         # Create file names, urls and check the download cache
         for band in self.bands:
-
             file_name = self.query_result[self.product_id][band]["file"]
             tile_name = self.query_result[self.product_id][band]["tile"]
             public_url = self.query_result[self.product_id][band]["public_url"]
 
             # This is the file path in the download cache directory
             file_path = os.path.join(self.user_download_cache_path, file_name)
 
@@ -376,15 +374,14 @@
             )
             self.message_logger.info(
                 (gml_temp_file_name, self.gml_cache_file_name)
             )
 
         # Create file names, urls and check the download cache
         for band in self.bands:
-
             file_name = self.query_result[self.product_id][band]["file"]
             tile_name = self.query_result[self.product_id][band]["tile"]
             public_url = self.query_result[self.product_id][band]["public_url"]
 
             # This is the file path in the download cache directory
             file_path = os.path.join(self.user_download_cache_path, file_name)
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/user.py` & `actinia-core-4.9.2/src/actinia_core/core/common/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     This class manages the user which are stored in the
     Redis database
     """
 
     db = redis_user_interface
 
     def read_from_db(self):
-
         creds = self.db.get_credentials(self.user_id)
         self.user_role = self.get_role()
         self.user_group = self.get_group()
         self.password_hash = self.get_password_hash()
 
         self.permissions = creds["permissions"]
         self.cell_limit = creds["permissions"]["cell_limit"]
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/common/user_base.py` & `actinia-core-4.9.2/src/actinia_core/core/common/user_base.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/geodata_download_importer.py` & `actinia-core-4.9.2/src/actinia_core/core/geodata_download_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,14 @@
                 dest = os.path.join(self.user_download_cache_path, file_name)
                 self.copy_file_list.append((source, dest))
             else:
                 source, dest = self.copy_file_list[count]
 
             # Download file only if it does not exist in the download cache
             if os.path.isfile(dest) is False:
-
                 p = get_wget_process(source, url)
                 download_commands.append(p)
                 if source != dest:
                     p = get_mv_process(source, dest)
                     download_commands.append(p)
             count += 1
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/google_cloud_storage_access.py` & `actinia-core-4.9.2/src/actinia_core/core/google_cloud_storage_access.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/grass_init.py` & `actinia-core-4.9.2/src/actinia_core/core/grass_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 import shutil
 import uuid
 from .messages_logger import MessageLogger
 
 __license__ = "GPLv3"
 __author__ = "Sören Gebbert"
 __copyright__ = (
-    "Copyright 2016-2018, Sören Gebbert and mundialis GmbH & Co. KG"
+    "Copyright 2016-2023, Sören Gebbert, Anika Weinmann and mundialis GmbH & "
+    "Co. KG"
 )
-__maintainer__ = "Sören Gebbert"
-__email__ = "soerengebbert@googlemail.com"
+__maintainer__ = "mundialis"
 
 
 class GrassInitError(Exception):
     """Exception that is thrown in case of a an
     initialization error of the GRASS environment
     """
 
@@ -83,15 +83,14 @@
             self.logger.error(message)
 
 
 class GrassEnvironment(ProcessLogging):
     """This class saves and sets grass environment variables"""
 
     def __init__(self):
-
         ProcessLogging.__init__(self)
         self.env = {
             "GISBASE": "",
             "GISRC": "",
             "LD_LIBRARY_PATH": "",
             "GRASS_ADDON_PATH": "",
             "GRASS_VERSION": "",
@@ -109,24 +108,24 @@
         Args:
             gisrc_path (str): Path to the GISRC file
             grass_gis_base (str): GRASS installation directory
             grass_addon_path (str): The path to GRASS addons
 
         """
         self.env["GIS_LOCK"] = str(os.getpid())
-        self.env["HOME"] = "/tmp/"
         self.env["GISBASE"] = grass_gis_base
+        self.env["HOME"] = os.getenv("HOME", "/tmp/")
         self.env["GRASS_MESSAGE_FORMAT"] = "plain"
         self.env["GRASS_SKIP_MAPSET_OWNER_CHECK"] = "1"
         self.env["GRASS_TGIS_RAISE_ON_ERROR"] = "1"
         self.env["GISRC"] = os.path.join(gisrc_path, "gisrc")
         self.env["LD_LIBRARY_PATH"] = str(
             os.path.join(self.env["GISBASE"], "lib")
         )
-        self.env["GRASS_VERSION"] = "7.7.svn"
+        self.env["GRASS_VERSION"] = "8"
         self.env["GRASS_ADDON_PATH"] = grass_addon_path
         self.env["GRASS_ADDON_BASE"] = grass_addon_path
         if os.name != "posix":
             self.env["PATH"] = str(
                 os.path.join(self.env["GISBASE"], "bin")
                 + ";"
                 + os.path.join(self.env["GISBASE"], "scripts")
@@ -162,26 +161,22 @@
             except Exception as e:
                 raise GrassInitError(
                     "Error getting grass environmental variables. Exception: "
                     + str(e)
                 )
 
     def set(self):
-        # # for debugging in ephemeral_processing.py (s. also process_queue.py)
-        # for var in [
-        #         'GISRC', 'GISBASE', 'LD_LIBRARY_PATH',
-        #         'GRASS_ADDON_PATH', 'GIS_LOCK']:
-        #     if var in os.environ:
-        #         del os.environ[var]
         for key in self.env:
-            try:
-                value = self.env[key]
-                origValue = os.getenv(key)
+            value = self.env[key]
+            # use self.env and enviroment variable values
+            if key in ["PATH", "PYTHONPATH"]:
+                origValue = os.getenv(key, None)
                 if origValue:
                     value += ":" + origValue
+            try:
                 os.putenv(key, value)
                 os.environ[key] = value
                 self.log_debug(key + "=" + value)
             except Exception as e:
                 raise GrassInitError(
                     "Error setting grass environmental variables. Exception: "
                     + str(e)
@@ -297,15 +292,14 @@
 
     def getFileName(self):
         return self.__windFile
 
 
 class GrassModuleRunner(ProcessLogging):
     def __init__(self, grassbase, grass_addon_path):
-
         ProcessLogging.__init__(self)
 
         self.grassbase = grassbase
         self.grass_addon_path = grass_addon_path
 
     def _run_process(
         self,
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/grass_modules_list.py` & `actinia-core-4.9.2/src/actinia_core/core/grass_modules_list.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/interim_results.py` & `actinia-core-4.9.2/src/actinia_core/core/interim_results.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/list_grass_modules.py` & `actinia-core-4.9.2/src/actinia_core/core/list_grass_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     This class creates a nested module dictionary based on keywords.
     The keyword depth is 2, if the second keyword is missing, the
     keyword "unspecific" is used as default.
     """
 
     def __init__(self, filename):
-
         self.modules_keyword_dict = {}
 
         file = QFile(filename)
         file.open(QIODevice.ReadOnly)
         self.xml = QXmlStreamReader(file)
 
         while not self.xml.atEnd():
@@ -70,21 +69,19 @@
         """
         Return the keyword dictionary
         :return:
         """
         return self.modules_keyword_dict
 
     def parse_module(self):
-
         module = None
         keywords = None
         description = None
 
         while self.xml.readNextStartElement():
-
             if self.xml.name() == "module":
                 module = self.xml.readElementText()
             elif self.xml.name() == "description":
                 description = self.xml.readElementText()
             elif self.xml.name() == "keywords":
                 keywords = self.xml.readElementText()
 
@@ -122,15 +119,14 @@
             for module in level_two:
                 entry = level_two[module]
                 print("    " + entry["module"])
                 print("      " + entry["description"])
 
 
 def main():
-
     grass_modules_xml_path = global_config.GRASS_MODULES_XML_PATH
     module_reader = GrassModuleReader(grass_modules_xml_path)
 
     file = open("grass_modules_list.py", "w")
     file.write("module_list=")
     file.write(str(module_reader.get()))
     file.close()
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/logging_interface.py` & `actinia-core-4.9.2/src/actinia_core/core/logging_interface.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/mapset_merge_utils.py` & `actinia-core-4.9.2/src/actinia_core/core/mapset_merge_utils.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/messages_logger.py` & `actinia-core-4.9.2/src/actinia_core/core/messages_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
     def __init__(self, config=None, user_id=None, fluent_sender=None):
         RedisFluentLoggerBase.__init__(
             self, config=config, user_id=user_id, fluent_sender=fluent_sender
         )
 
     def _log_message(self, log_level, message):
-
         node = platform.node()
         ctime = time.ctime()
 
         log_dict = {
             "node": node,
             "ctime": ctime,
             "user_id": self.user_id,
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/redis_api_log.py` & `actinia-core-4.9.2/src/actinia_core/core/redis_api_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     user_id_2 : log entry 1
                 log entry 2
                 log entry 3
 
     """
 
     def add(self, user_id, log_entry):
-        """Add a API log entry to a user specific  API log list in the Redis server
+        """Add a API log entry to a user specific  API log list in the Redis
+        server
 
         Args:
             user_id (str): The user id of the API log
             log_entry (str): A string
 
         Returns:
             int:
@@ -150,15 +151,14 @@
 
 
 # Create the Redis interface instance
 redis_api_log_interface = RedisAPILogInterface()
 
 
 def test_api_logging(r):
-
     user_id = "abcdefg"
 
     # Remove the loglist
     r.delete(user_id)
 
     ret = r.add(user_id, "API-log entry 1")
     if ret != 1:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/redis_fluentd_logger_base.py` & `actinia-core-4.9.2/src/actinia_core/core/redis_fluentd_logger_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 
 class RedisFluentLoggerBase(object):
     """Base class for all logger that use Redis and fluentd for logging"""
 
     def __init__(self, config=None, user_id=None, fluent_sender=None):
-
         if config is None:
             config = global_config
         if user_id is None:
             user_id = "Unknown"
 
         self.host = config.LOG_FLUENT_HOST
         self.port = config.LOG_FLUENT_PORT
@@ -61,15 +60,14 @@
         # The fluentd sender
         if fluent_sender is None and global_config.LOG_INTERFACE == "fluentd":
             self.fluent_sender = sender.FluentSender(
                 "actinia_logger", host=self.host, port=self.port
             )
 
     def _send_to_fluent(self, tag, data):
-
         try:
             cur_time = int(time.time())
             self.fluent_sender.emit_with_time(
                 tag, timestamp=cur_time, data=data
             )
         except Exception as e:
             log.error(
@@ -90,15 +88,14 @@
         ):
             print(
                 "WARNING: Some output might not be redirected to STDOUT:"
                 + " %s %s %s" % (tag, str(cur_time), str(data))
             )
 
     def _send_to_logging_interface(self, tag, data):
-
         if tag == "RESOURCE_LOG" and "status" in data:
             if data["status"] == "error":
                 log.error(data)
             elif data["status"] == "terminated":
                 log.warning(data)
             else:
                 log.info(data)
@@ -111,13 +108,12 @@
             try:
                 log.log(getattr(logging, tag), data)
             except AttributeError:
                 log.debug("Unknown log tag for logging: %s", tag)
                 log.info(data)
 
     def send_to_logger(self, tag, data):
-
         if global_config.LOG_INTERFACE == "fluentd":
             self._send_to_fluent(tag, data)
 
         # always send to logger as file logger (and stdout) is included here
         self._send_to_logging_interface(tag, data)
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/redis_lock.py` & `actinia-core-4.9.2/src/actinia_core/core/redis_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,14 @@
 
 
 # Create the Redis interface instance
 # redis_lock_interface = RedisLockingInterface()
 
 
 def test_locking(r):
-
     resource = "location/mapset"
 
     # Remove the lock if its present
     r.unlock(resource)
 
     ret = r.lock(resource, 5)
     if ret != 1:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/redis_resources.py` & `actinia-core-4.9.2/src/actinia_core/core/redis_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,14 @@
 
 
 # Create the Redis interface instance
 # redis_resource_interface = RedisResourceInterface()
 
 
 def test_resource_entries(r):
-
     resource_id = "abcdefg"
 
     # Remove the resource entry if it exist
     r.delete(resource_id)
 
     ret = r.set(resource_id, "JSON file", expiration=20)
     if ret != 1:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/redis_user.py` & `actinia-core-4.9.2/src/actinia_core/core/redis_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,14 @@
 
 
 # Create the Redis interface instance
 redis_user_interface = RedisUserInterface()
 
 
 def test_management(r):
-
     user_id = "Soeren"
     user_group = "test_1"
     password_hash = "hash"
     user_role = "admin"
     permissions = {
         "locations": {
             "NC": {"mapsets": ["PERMANWENT", "user1"]},
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/request_parser.py` & `actinia-core-4.9.2/src/actinia_core/core/request_parser.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/resource_data_container.py` & `actinia-core-4.9.2/src/actinia_core/core/resource_data_container.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/resources_logger.py` & `actinia-core-4.9.2/src/actinia_core/core/resources_logger.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/stac_exporter_interface.py` & `actinia-core-4.9.2/src/actinia_core/core/stac_exporter_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         """
 
         output_path = self._get_source_file(resource_url)
 
         self._stac_collection_initializer()
 
         if output_type == "raster":
-
             # Get parameters for STAC item
             extra_values = self._get_raster_parameters(output_path)
 
             # Checking if the input has WGS 84 CRS
             geom, bbox_raster = self._get_wgs84_parameters(extra_values)
 
             item_name = f"item-{filename}"
@@ -122,15 +121,14 @@
 
             # Create Catalog Object
             catalog = read_dict(catalog_dict)
 
             redis_items = self._save_items_redis(item, item_name)
 
             if redis_items:
-
                 # Add item to Catalog
                 catalog.add_item(item)
 
                 # Update redis catalog
                 self._update_catalog_redis(catalog)
 
                 return item.to_dict()
@@ -250,15 +248,14 @@
             geom = extra_values["geometry"]
             bbox_raster = extra_values["bbox"]
 
         return geom, bbox_raster
 
     @staticmethod
     def _update_catalog_redis(catalog):
-
         new_catalog = catalog.to_dict()
         redis_actinia_interface.update("result-catalog", new_catalog)
 
     @staticmethod
     def _set_processing_extention(item):
         input_item = item.to_dict()
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/stac_importer_interface.py` & `actinia-core-4.9.2/src/actinia_core/core/stac_importer_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,19 +50,18 @@
 except Exception:
     has_plugin = False
 
 
 class STACImporter:
     @staticmethod
     def _get_search_root(stac_collection_id):
-
         stac_from_actinia = callStacCollection(stac_collection_id)
         try:
             stac_json = json.loads(stac_from_actinia)
-        except (Exception):
+        except Exception:
             stac_json = stac_from_actinia
 
         for item in stac_json["links"]:
             if item["rel"] == "root":
                 stac_url = item["href"]
 
                 if "?" in stac_url:
@@ -73,15 +72,14 @@
                 else:
                     stac_root_search = stac_url + "/search"
 
         return stac_root_search
 
     @staticmethod
     def _apply_filter(stac_root_search, stac_name, interval, bbox, filter):
-
         search_body = {
             "collections": [stac_name],
         }
         search_body["query"] = filter
 
         search_body["bbox"] = bbox
 
@@ -100,15 +98,14 @@
             stac_search = requests.get(stac_root_search, json=search_body)
             full_filtered_result = stac_search.json()
 
             if (
                 "features" in full_filtered_result
                 and len(full_filtered_result["features"]) > 0
             ):
-
                 return full_filtered_result
             else:
                 raise AsyncProcessError("Not matched found")
 
     @staticmethod
     def _get_filtered_bands(stac_items, semantic_label):
         band_roots = {}
@@ -139,15 +136,14 @@
         stac_collection_id=None,
         semantic_label=None,
         interval=None,
         bbox=None,
         filter=None,
         strd_name=None,
     ):
-
         if has_plugin:
             try:
                 stac_name = stac_collection_id.split(".")[3]
             except Exception:
                 raise AsyncProcessError(
                     "The source has not the right structure"
                 )
@@ -254,15 +250,14 @@
         self,
         stac_entry,
         config=None,
         temp_file_path=None,
         message_logger=None,
         send_resource_update=None,
     ):
-
         """Helper method to get the stac import and download commands.
         Args:
             stac_entry (dict): stac_entry of the import description list
         Returns:
             stac_commands: The stac download and import commands
         """
         # Check for band information
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/storage_interface_aws_s3.py` & `actinia-core-4.9.2/src/actinia_core/core/storage_interface_aws_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
             region_name=self.config.S3_AWS_DEFAULT_REGION,
             aws_access_key_id=self.config.S3_AWS_ACCESS_KEY_ID,
             aws_secret_access_key=self.config.S3_AWS_SECRET_ACCESS_KEY,
         )
         self.s3_client = self.session.client("s3")
 
     def get_resource_urls(self):
-        """Return all resource urls that were generated when storing a resource on disk
+        """Return all resource urls that were generated when storing a resource
+        on disk
 
         Returns:
             (list): A list of urls
 
         """
         return self.resource_url_list
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/storage_interface_base.py` & `actinia-core-4.9.2/src/actinia_core/core/storage_interface_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,26 +58,27 @@
     @abstractmethod
     def setup(self):
         """Setup the resource storage"""
         pass
 
     @abstractmethod
     def get_resource_urls(self):
-        """Return all resource urls that were generated when storing a resource on disk
+        """Return all resource urls that were generated when storing a resource
+        on disk
 
         Returns:
             (list): A list of urls
 
         """
         return self.resource_url_list
 
     @abstractmethod
     def store_resource(self, file_path):
-        """Store a resource (file) at the user resource storage and return an URL
-        to the resource accessible via HTTP
+        """Store a resource (file) at the user resource storage and return an
+        URL to the resource accessible via HTTP
 
         Args:
             file_path:
 
         Returns:
             (str): the resource url that points to the stored resource
```

### Comparing `actinia-core-4.9.1/src/actinia_core/core/storage_interface_filesystem.py` & `actinia-core-4.9.2/src/actinia_core/core/storage_interface_filesystem.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/storage_interface_gcs.py` & `actinia-core-4.9.2/src/actinia_core/core/storage_interface_gcs.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/core/utils.py` & `actinia-core-4.9.2/src/actinia_core/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,17 +90,17 @@
     """
     read_allowed = path_is_in_allowed_read_paths(path)
     both_allowed = read_allowed and path_is_in_allowed_write_paths(path)
     return both_allowed
 
 
 def path_is_in_allowed_read_paths(path):
-    """Checks whether the passed path is a valid read path, uses the global_config
-    variables `GRASS_USER_DATABASE`, `GRASS_DATABASE` and `GRASS_RESOURCE_DIR`
-    for the check.
+    """Checks whether the passed path is a valid read path, uses the
+    global_config variables `GRASS_USER_DATABASE`, `GRASS_DATABASE` and
+    `GRASS_RESOURCE_DIR` for the check.
 
     Args:
         path (string): a normalized path
 
     Returns:
         (bool) Whether the passed path is a valid write path
     """
@@ -109,16 +109,17 @@
         global_config.GRASS_DATABASE,
         global_config.GRASS_RESOURCE_DIR,
     ]
     return any(path.startswith(allowed) for allowed in allowed_read_starts)
 
 
 def path_is_in_allowed_write_paths(path):
-    """Checks whether the passed path is a valid write path, uses the global_config
-    variables `GRASS_USER_DATABASE` and `GRASS_RESOURCE_DIR` for the check.
+    """Checks whether the passed path is a valid write path, uses the
+    global_config variables `GRASS_USER_DATABASE` and `GRASS_RESOURCE_DIR` for
+    the check.
 
     Args:
         path (string): a normalized path
 
     Returns:
         (bool) Whether the passed path is a valid write path
     """
```

### Comparing `actinia-core-4.9.1/src/actinia_core/endpoints.py` & `actinia-core-4.9.2/src/actinia_core/endpoints.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/health_check.py` & `actinia-core-4.9.2/src/actinia_core/health_check.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/main.py` & `actinia-core-4.9.2/src/actinia_core/main.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/models/process_chain.py` & `actinia-core-4.9.2/src/actinia_core/models/process_chain.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/models/response_models.py` & `actinia-core-4.9.2/src/actinia_core/models/response_models.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/base/renderer_base.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/base/renderer_base.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/download_cache_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/download_cache_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,21 +53,19 @@
         EphemeralProcessing.__init__(self, *args)
         self.user_download_cache_path = os.path.join(
             self.config.DOWNLOAD_CACHE, self.user_id
         )
         self.response_model_class = StorageResponseModel
 
     def _execute(self):
-
         self._setup()
 
         if os.path.exists(self.user_download_cache_path) and os.path.isdir(
             self.user_download_cache_path
         ):
-
             executable = "/usr/bin/du"
             args = ["-sb", self.user_download_cache_path]
 
             self._run_process(
                 Process(
                     exec_type="exec",
                     executable=executable,
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_custom_processing.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_custom_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_processing_with_export.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/ephemeral_processing_with_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         """
         # Export the layer
         suffix = ".tif"
         # Remove a potential mapset
         file_name = raster_name.split("@")[0] + suffix
 
         if use_raster_region is True:
-
             p = Process(
                 exec_type="grass",
                 executable="g.region",
                 executable_params=["raster=%s" % raster_name, "-g"],
                 id=f"exporter_region_{raster_name}",
                 stdin_source=None,
             )
@@ -407,15 +406,14 @@
         The temporary data will be finally removed.
 
         At the moment only raster layer export is supported.
 
         """
 
         for resource in self.resource_export_list:
-
             # Check for termination requests between the exports
             if (
                 bool(
                     self.resource_logger.get_termination(
                         self.user_id, self.resource_id, self.iteration
                     )
                 )
@@ -428,15 +426,14 @@
             # Raster export
             if resource["export"]["type"] in [
                 "raster",
                 "vector",
                 "file",
                 "strds",
             ]:
-
                 output_type = resource["export"]["type"]
                 output_path = None
 
                 # Legacy code
                 if "name" in resource:
                     file_name = resource["name"]
                 if "value" in resource:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/persistent_processing.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/persistent_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
         # accordingly
         if (
             os.path.exists(self.user_location_path)
             and os.path.isdir(self.user_location_path)
             and os.access(self.user_location_path, os.R_OK | os.X_OK | os.W_OK)
             is True
         ):
-
             self.orig_mapset_path = os.path.join(
                 self.user_location_path, mapset
             )
 
             if os.path.exists(self.orig_mapset_path) is True:
                 if (
                     os.access(
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/process_validation.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/process_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 
 class ProcessValidation(EphemeralProcessing):
     def __init__(self, *args):
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
 
         process_chain = (
             self._create_temporary_grass_environment_and_process_list()
         )
 
         result = []
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/raster_colors.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/raster_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 
 class EphemeralRasterColorsOutput(EphemeralProcessing):
     def __init__(self, *args):
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self, skip_permission_check=True):
-
         self._setup()
 
         raster_name = self.map_name
         self.required_mapsets.append(self.mapset_name)
 
         with NamedTemporaryFile(
             mode="w+", suffix=".color", dir=self.temp_file_path
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/raster_layer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/raster_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class EphemeralRasterInfo(EphemeralProcessing):
     def __init__(self, *args):
-
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self):
         """Read info from a raster layer
 
         Use a temporary mapset for processing
         """
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/raster_legend.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/raster_legend.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class EphemeralRasterLegend(EphemeralProcessing):
     def __init__(self, *args):
-
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self, skip_permission_check=True):
         """Render the raster legend with d.legend"""
         self._setup()
 
         self.required_mapsets.append(self.mapset_name)
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/resource_storage_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/resource_storage_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,21 +53,19 @@
         EphemeralProcessing.__init__(self, *args)
         self.response_model_class = StorageResponseModel
         self.user_resource_storage_path = os.path.join(
             self.config.GRASS_RESOURCE_DIR, self.user_id
         )
 
     def _execute(self):
-
         self._setup()
 
         if os.path.exists(self.user_resource_storage_path) and os.path.isdir(
             self.user_resource_storage_path
         ):
-
             executable = "/usr/bin/du"
             args = ["-sb", self.user_resource_storage_path]
 
             self._run_process(
                 Process(
                     exec_type="exec",
                     executable=executable,
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral/vector_layer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral/vector_layer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_processing.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1100,15 +1100,14 @@
         self.temp_mapset_path = os.path.join(
             self.temp_location_path, temp_mapset_name
         )
 
         # if interim_result_mapset is set copy the mapset from the interim
         # results
         if interim_result_mapset:
-
             self.message_logger.info(
                 "Rsync interim result mapset to temporary GRASS DB"
             )
             # change mapset name for groups, raster VRTs and tgis
             for directory in ["group", "cell_misc", "tgis"]:
                 change_mapsetname(
                     os.path.join(interim_result_mapset, directory),
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/raster_renderer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/raster_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         self._execute_process_list(process_list)
 
         self.module_results = result_file
 
 
 class EphemeralRasterRGBRenderer(EphemeralRendererBase):
     def __init__(self, *args):
-
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self, skip_permission_check=True):
         """Render three raster layer as rgb image
 
         Workflow:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/strds_renderer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/strds_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class EphemeralSTRDSRenderer(EphemeralRendererBase):
     def __init__(self, *args):
-
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self, skip_permission_check=True):
         """Render the raster map layers of a STRDS
 
         Workflow:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/vector_renderer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_renderer_base/vector_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class EphemeralVectorRenderer(EphemeralRendererBase):
     def __init__(self, *args):
-
         EphemeralProcessing.__init__(self, *args)
 
     def _execute(self, skip_permission_check=True):
         """Render the vector image
 
         Workflow:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/ephemeral_with_export/raster_export.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/ephemeral_with_export/raster_export.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/download_cache_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/download_cache_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,22 +42,20 @@
 __maintainer__ = "mundialis"
 
 
 class DownloadCacheDelete(PersistentProcessing):
     """Delete the whole download cache directory"""
 
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
         self.user_download_cache_path = os.path.join(
             self.config.DOWNLOAD_CACHE, self.user_id
         )
 
     def _execute(self):
-
         self._setup()
 
         if os.path.exists(self.user_download_cache_path) and os.path.isdir(
             self.user_download_cache_path
         ):
             executable = "/bin/rm"
             args = ["-rf", self.user_download_cache_path]
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/location_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/location_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 class PersistentLocationCreator(PersistentProcessing):
     """Create a new location based on EPSG code"""
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         new_location = self.location_name
 
         self.location_name = self.config.GRASS_DEFAULT_LOCATION
 
         self._setup()
 
         epsg_code = self.request_data["epsg"]
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/map_layer_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/map_layer_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     """
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
         self.response_model_class = StringListProcessingResultResponseModel
 
     def _execute(self):
-
         self._setup()
 
         args, layer_type = self.data
         self.required_mapsets.append(self.target_mapset_name)
 
         options = extract_glist_parameters(args)
 
@@ -88,19 +87,17 @@
         self.module_results = raster_layers_with_mapset
 
 
 class PersistentRemoveLayers(PersistentProcessing):
     """Remove layers in a mapset"""
 
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
 
         args, layer_type = self.data
         self.required_mapsets.append(self.target_mapset_name)
 
         options = extract_glist_parameters(args)
 
@@ -130,19 +127,17 @@
         self.finish_message = "Successfully removed %s layers." % layer_type
 
 
 class PersistentRenameLayers(PersistentProcessing):
     """Rename raster layers in a mapset"""
 
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
 
         args, layer_type = self.data
         self.required_mapsets.append(self.target_mapset_name)
 
         # List format must be
         # [(a, a_new),(b, b_new),(c, c_new), ...]
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/mapset_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/mapset_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
     ]
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
         self.response_model_class = MapsetInfoResponseModel
 
     def _execute(self):
-
         self._setup()
 
         pc = {
             "1": {"module": "g.region", "flags": "ug3"},
             "2": {"module": "g.proj", "flags": "fw"},
         }
 
@@ -165,15 +164,14 @@
 class PersistentMapsetCreator(PersistentProcessing):
     """Create a mapset in an existing location"""
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
         # Create temporary database
         self._create_temp_database()
 
         pc = {"1": {"module": "g.mapsets", "flags": "l"}}
 
         process_list = self._validate_process_chain(
@@ -217,15 +215,14 @@
     3. Check if the mapset exists
     """
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
 
         # For debug purpose
         # self.lock_interface.unlock(self.target_mapset_lock_id)
 
         if "PERMANENT" == self.target_mapset_name:
             raise AsyncProcessError(
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/persistent_mapset_merger.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/persistent_mapset_merger.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/raster_colors.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/raster_colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,17 @@
 class PersistentRasterColorsRules(PersistentProcessing):
     """Set the color table of a raster map from color rules
 
     Perform the processing in the original mapset
     """
 
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self, skip_permission_check=True):
-
         self._setup()
 
         raster_name = self.map_name
         self.required_mapsets.append(self.target_mapset_name)
 
         options = self.request_data
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/raster_layer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/raster_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         self.finish_message = (
             "Raster layer <%s> successfully removed." % raster_name
         )
 
 
 class PersistentRasterCreator(PersistentProcessing):
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
         """Create a specific raster layer
 
         This approach is complex, since the raster generation is performed in a
         localc temporary mapset that is later merged into the target mapset.
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/resource_storage_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/resource_storage_management.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,21 +51,19 @@
         PersistentProcessing.__init__(self, rdc)
         self.user_resource_storage_path = os.path.join(
             self.config.GRASS_RESOURCE_DIR, self.user_id
         )
         self.olderthan = args[1]
 
     def _execute(self):
-
         self._setup()
 
         if os.path.exists(self.user_resource_storage_path) and os.path.isdir(
             self.user_resource_storage_path
         ):
-
             if self.olderthan is None:
                 # delete all user resources
                 executable = "/bin/rm"
                 args = ["-rf", self.user_resource_storage_path]
             else:
                 # delete all user resources older than X days
                 executable = "/usr/bin/find"
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/strds_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/strds_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,20 +45,18 @@
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class PersistentSTRDSLister(PersistentProcessing):
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
         self.response_model_class = StringListProcessingResultResponseModel
 
     def _execute(self):
-
         self._setup()
 
         pc = {
             "1": {
                 "module": "t.list",
                 "inputs": {"type": "strds", "column": "name"},
             }
@@ -104,20 +102,18 @@
         self.module_results = mapset_lists
 
 
 class PersistentSTRDSInfo(PersistentProcessing):
     """Gather the STRDS information"""
 
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
         self.response_model_class = STRDSInfoResponseModel
 
     def _execute(self):
-
         self._setup()
 
         pc = {
             "1": {
                 "module": "t.info",
                 "inputs": {"type": "strds", "input": self.map_name},
                 "flags": "g",
@@ -192,15 +188,14 @@
 class PersistentSTRDSCreator(PersistentProcessing):
     """Create a STRDS"""
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
         self.required_mapsets.append(self.target_mapset_name)
 
         pc_1 = {}
         pc_1["1"] = {
             "module": "t.list",
             "inputs": {
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/strds_raster_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/strds_raster_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,18 @@
 __maintainer__ = "mundialis"
 
 
 class PersistentRasterSTRDSLister(PersistentProcessing):
     """List all mapsets in a location"""
 
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
         self.response_model_class = STRDSRasterListResponseModel
 
     def _execute(self):
-
         self._setup()
 
         result_file = tempfile.NamedTemporaryFile(
             dir=self.temp_file_path, delete=True
         )
 
         pc = {
@@ -120,15 +118,14 @@
 class PersistentRasterSTRDSRegisterer(PersistentProcessing):
     """Register a list of timestamped raster map layers in a STRDS"""
 
     def __init__(self, *args):
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
-
         self._setup()
 
         input_file = tempfile.NamedTemporaryFile(
             dir=self.temp_file_path, delete=True, mode="w"
         )
 
         for map_entry in self.request_data:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/actinia_processing/persistent/vector_layer.py` & `actinia-core-4.9.2/src/actinia_core/processing/actinia_processing/persistent/vector_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         self.finish_message = (
             "Vector layer <%s> successfully removed." % vector_name
         )
 
 
 class PersistentVectorCreator(PersistentProcessing):
     def __init__(self, *args):
-
         PersistentProcessing.__init__(self, *args)
 
     def _execute(self):
         """Create a specific vector layer
 
         This approach is complex, since the vector generation is performed in a
         local temporary mapset that is later merged into the target mapset.
```

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/download_cache_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/download_cache_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/ephemeral_custom_processing.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/ephemeral_custom_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/ephemeral_processing.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/ephemeral_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/ephemeral_processing_with_export.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/ephemeral_processing_with_export.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/location_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/location_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/map_layer_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/map_layer_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/mapset_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/mapset_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/persistent_mapset_merger.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/persistent_mapset_merger.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/persistent_processing.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/persistent_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/process_validation.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/process_validation.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/raster_colors.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/raster_colors.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/raster_export.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/raster_export.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/raster_layer.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/raster_layer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/raster_legend.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/raster_legend.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/raster_renderer.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/raster_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/resource_storage_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/resource_storage_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/strds_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/strds_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/strds_raster_management.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/strds_raster_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/strds_renderer.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/strds_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/utils.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/utils.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/vector_layer.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/vector_layer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/processing/common/vector_renderer.py` & `actinia-core-4.9.2/src/actinia_core/processing/common/vector_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/api_log_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/api_log_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
 class APILogResource(Resource):
     """API logg management"""
 
     decorators = [log_api_call, check_user_permissions, auth.login_required]
 
     def __init__(self):
-
         # Configuration
         Resource.__init__(self)
 
         self.api_logger = ApiLogger()
 
         # Store the user id and user role of the current user
         self.user_id = g.user.get_id()
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/base/base_login.py` & `actinia-core-4.9.2/src/actinia_core/rest/base/base_login.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/base/endpoint_config.py` & `actinia-core-4.9.2/src/actinia_core/rest/base/endpoint_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     """
 
     def decorator(func):
         endpoint_class, method = func.__qualname__.split(".")
 
         @wraps(func)
         def wrapper(*args, **kwargs):
-
             if check_endpoint(method, endpoint_class=endpoint_class):
                 result = func(*args, **kwargs)
                 return result
             else:
                 return make_response(
                     jsonify(
                         SimpleResponseModel(
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/base/map_layer_base.py` & `actinia-core-4.9.2/src/actinia_core/rest/base/map_layer_base.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/base/renderer_base.py` & `actinia-core-4.9.2/src/actinia_core/rest/base/renderer_base.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/base/resource_base.py` & `actinia-core-4.9.2/src/actinia_core/rest/base/resource_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,14 @@
         """Check if the Payload is a JSON document
 
         Return: bool:
             True in case of success, False otherwise
         """
         # First check for the data field and create JSON from it
         if hasattr(request, "data") is True:
-
             try:
                 self.request_data = json_loads(request.data)
             except Exception as e:
                 self.create_error_response(
                     message="No JSON data in request: Exception: %s" % str(e)
                 )
                 return False
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/base/user_auth.py` & `actinia-core-4.9.2/src/actinia_core/rest/base/user_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,14 @@
     Returns:
         function: The decorator functions
 
     """
 
     @wraps(f)
     def decorated_function(*args, **kwargs):
-
         location_name = None
         mapset_name = None
         module_name = None
 
         if "location_name" in kwargs:
             location_name = kwargs["location_name"]
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/download_cache_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/download_cache_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/ephemeral_custom_processing.py` & `actinia-core-4.9.2/src/actinia_core/rest/ephemeral_custom_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/ephemeral_processing.py` & `actinia-core-4.9.2/src/actinia_core/rest/ephemeral_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/ephemeral_processing_with_export.py` & `actinia-core-4.9.2/src/actinia_core/rest/ephemeral_processing_with_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         ResourceBase.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint("post", ephemeral_processing_with_export.post_doc)
     )
     def post(self, location_name):
-        """Execute a user defined process chain in an ephemeral location/mapset and
-        store the processing result in an Amazon S3 bucket
+        """Execute a user defined process chain in an ephemeral location/mapset
+        and store the processing result in an Amazon S3 bucket
         """
         rdc = self.preprocess(has_json=True, location_name=location_name)
         rdc.set_storage_model_to_s3()
 
         enqueue_job(self.job_timeout, start_job, rdc)
 
         html_code, response_model = pickle.loads(self.response_data)
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/location_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/location_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/map_layer_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/map_layer_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/mapset_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/mapset_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/mapsets.py` & `actinia-core-4.9.2/src/actinia_core/rest/mapsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     """Get all locked mapsets"""
 
     decorators = [log_api_call, check_user_permissions, auth.login_required]
 
     @endpoint_decorator()
     @swagger.doc(check_endpoint("get", mapsets.get_doc))
     def get(self):
-
         if "status" in request.args:
             if request.args["status"] == "locked":
                 if self.user.has_superadmin_role() is False:
                     return make_response(
                         jsonify(
                             SimpleResponseModel(
                                 status="error",
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/persistent_mapset_merger.py` & `actinia-core-4.9.2/src/actinia_core/rest/persistent_mapset_merger.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/persistent_processing.py` & `actinia-core-4.9.2/src/actinia_core/rest/persistent_processing.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/process_chain_monitoring.py` & `actinia-core-4.9.2/src/actinia_core/rest/process_chain_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 __license__ = "GPLv3"
 __author__ = "Anika Weinmann, Carmen Tawalika"
 __copyright__ = "Copyright 2021, mundialis GmbH & Co. KG"
 __maintainer__ = "mundialis"
 
 
 def create_scatter_plot(x, y, xlabel, ylabel, title):
-
     plt.clf()
     plt.scatter(x, y, s=(np.pi * 5), c=(1, 0, 0))
     plt.title(title, fontsize=14)
     plt.xlabel(xlabel, fontsize=12)
     plt.ylabel(ylabel, fontsize=12)
     y_up = (max(y) + 9) // 10 * 10
     plt.ylim(0, y_up)
@@ -77,15 +76,14 @@
 
 class MapsetSizeResource(ResourceManager):
     """
     This class returns the mapset sizes of a resource
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManager.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint("get", process_chain_monitoring.mapset_size_get_doc)
     )
@@ -140,15 +138,14 @@
 
 class MapsetSizeDiffResource(ResourceManager):
     """
     This class returns the step-by-step mapset size differences of a resource
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManager.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint("get", process_chain_monitoring.mapset_sizediff_get_doc)
     )
@@ -204,15 +201,14 @@
 
 class MaxMapsetSizeResource(ResourceManager):
     """
     This class returns the maximum mapset size of a resource
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManager.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint("get", process_chain_monitoring.mapset_maxsize_get_doc)
     )
@@ -268,15 +264,14 @@
 
 class MapsetSizeRenderResource(ResourceManager):
     """
     This class renders the mapset sizes of a resource
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManager.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint(
             "get", process_chain_monitoring.mapset_render_sizes_get_doc
@@ -350,15 +345,14 @@
 
 class MapsetSizeDiffRenderResource(ResourceManager):
     """
     This class renders the step-by-step mapset size differences of a resource
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManager.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint(
             "get", process_chain_monitoring.mapset_render_sizediff_get_doc
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/process_validation.py` & `actinia-core-4.9.2/src/actinia_core/rest/process_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 __copyright__ = (
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class AsyncProcessValidationResource(ResourceBase):
-
     decorators = [log_api_call, auth.login_required]
 
     @endpoint_decorator()
     @swagger.doc(check_endpoint("post", process_validation.post_doc))
     def post(self, location_name):
         """Validate a process chain asynchronously, check the provided sources
         and the mapsets."""
@@ -68,15 +67,14 @@
             enqueue_job(self.job_timeout, start_job, rdc)
 
         html_code, response_model = pickle.loads(self.response_data)
         return make_response(jsonify(response_model), html_code)
 
 
 class SyncProcessValidationResource(ResourceBase):
-
     decorators = [log_api_call, auth.login_required]
 
     @endpoint_decorator()
     @swagger.doc(check_endpoint("post", process_validation.post_doc))
     def post(self, location_name):
         """Validate a process chain synchronously, check the provided sources
         and the mapsets."""
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/raster_colors.py` & `actinia-core-4.9.2/src/actinia_core/rest/raster_colors.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/raster_export.py` & `actinia-core-4.9.2/src/actinia_core/rest/raster_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     def post(self, location_name, mapset_name, raster_name):
         """Export an existing raster map layer as GeoTiff."""
         return self._execute(location_name, mapset_name, raster_name, False)
 
     def _execute(
         self, location_name, mapset_name, raster_name, use_raster_region
     ):
-
         rdc = self.preprocess(
             has_json=False,
             location_name=location_name,
             mapset_name=mapset_name,
             map_name=raster_name,
         )
         if rdc:
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/raster_layer.py` & `actinia-core-4.9.2/src/actinia_core/rest/raster_layer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/raster_legend.py` & `actinia-core-4.9.2/src/actinia_core/rest/raster_legend.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/raster_renderer.py` & `actinia-core-4.9.2/src/actinia_core/rest/raster_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/resource_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/resource_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 class ResourceManagerBase(Resource):
     """Base class for resource management"""
 
     decorators = [log_api_call, auth.login_required]
 
     def __init__(self):
-
         # Configuration
         Resource.__init__(self)
 
         kwargs = dict()
         kwargs["host"] = global_config.REDIS_SERVER_URL
         kwargs["port"] = global_config.REDIS_SERVER_PORT
         if (
@@ -191,15 +190,14 @@
     """
     This class is responsible to answer status requests
     of asynchronous processes (resources) and
     to request the termination of a resource
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManagerBase.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(check_endpoint("get", resource_management.resource_get_doc))
     def get(self, user_id, resource_id):
         """Get the status of a resource."""
@@ -589,15 +587,14 @@
 
     TODO: This methods must be secured by checking the user id. Only admins
     can terminate and list resources from other users.
 
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManagerBase.__init__(self)
 
     def _get_resource_list(self, user_id, type_="all"):
         """
         Get a list of resources that have been generated by the calling user
         """
@@ -683,15 +680,14 @@
     """
     This class is responsible to answer status requests
     of asynchronous processes (resources) and
     to request the termination of a resource with iterations
     """
 
     def __init__(self):
-
         # Configuration
         ResourceManagerBase.__init__(self)
 
     @endpoint_decorator()
     @swagger.doc(
         check_endpoint("get", resource_management.resource_iteration_get_doc)
     )
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/resource_storage_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/resource_storage_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 __copyright__ = (
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class SyncResourceStorageResource(ResourceBase):
-
     decorators = [
         log_api_call,
         check_user_permissions,
         check_admin_role,
         auth.login_required,
     ]
 
@@ -125,12 +124,12 @@
             enqueue_job(
                 self.job_timeout,
                 start_resource_storage_remove,
                 rdc,
                 olderthan,
                 queue_type_overwrite=True,
             )
-            http_code, response_model = self.wait_until_finish()
+            http_code, response_model = pickle.loads(self.response_data)
         else:
             http_code, response_model = pickle.loads(self.response_data)
 
         return make_response(jsonify(response_model), http_code)
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/resource_streamer.py` & `actinia-core-4.9.2/src/actinia_core/rest/resource_streamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,14 @@
             [resource_export_path, file_name], "w"
         )
 
         if (
             os.path.exists(resource_export_file_path) is True
             and os.access(resource_export_file_path, os.R_OK) is True
         ):
-
             return send_from_directory(
                 resource_export_path, file_name, as_attachment=True
             )
         else:
             return make_response(
                 jsonify(
                     {"status": "error", "message": "Resource does not exist"}
```

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/strds_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/strds_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/strds_raster_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/strds_raster_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/strds_renderer.py` & `actinia-core-4.9.2/src/actinia_core/rest/strds_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/user_api_key.py` & `actinia-core-4.9.2/src/actinia_core/rest/user_api_key.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/user_management.py` & `actinia-core-4.9.2/src/actinia_core/rest/user_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/vector_layer.py` & `actinia-core-4.9.2/src/actinia_core/rest/vector_layer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/rest/vector_renderer.py` & `actinia-core-4.9.2/src/actinia_core/rest/vector_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core/testsuite.py` & `actinia-core-4.9.2/src/actinia_core/testsuite.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
         server_test = bool(os.environ["ACTINIA_SERVER_TEST"])
 
     if "ACTINIA_CUSTOM_TEST_CFG" in os.environ:
         custom_actinia_cfg = str(os.environ["ACTINIA_CUSTOM_TEST_CFG"])
 
     @classmethod
     def setUpClass(cls):
-
         if cls.server_test is False and cls.custom_actinia_cfg is False:
             global_config.REDIS_SERVER_SERVER = "localhost"
             global_config.REDIS_SERVER_PORT = 7000
             global_config.GRASS_RESOURCE_DIR = "/tmp"
             global_config.DOWNLOAD_CACHE = "/tmp/download_cache"
             global_config.REDIS_QUEUE_SERVER_URL = "localhost"
             global_config.REDIS_QUEUE_SERVER_PORT = 6379
@@ -233,15 +232,14 @@
         role="guest",
         group="group",
         password="abcdefgh",
         accessible_datasets=None,
         process_num_limit=1000,
         process_time_limit=6000,
     ):
-
         auth = bytes("%s:%s" % (name, password), "utf-8")
 
         # We need to create an HTML basic authorization header
         cls.auth_header[role] = Headers()
         cls.auth_header[role].add(
             "Authorization", "Basic " + base64.b64encode(auth).decode()
         )
@@ -263,15 +261,14 @@
         user.add_accessible_modules(["uname", "sleep"])
         cls.users_list.append(user)
 
         return name, group, cls.auth_header[role]
 
     @classmethod
     def tearDownClass(cls):
-
         for user in cls.users_list:
             user.delete()
 
         if cls.server_test is False:
             redis_interface.disconnect()
 
     def setUp(self):
@@ -362,15 +359,14 @@
                 (f"Message is {resp_data['message']}"),
             )
 
         time.sleep(0.4)
         return resp_data
 
     def assertRasterInfo(self, location, mapset, raster, ref_info, header):
-
         url = (
             f"{URL_PREFIX}/locations/{location}/mapsets/{mapset}/"
             f"raster_layers/{raster}"
         )
         rv = self.server.get(url, headers=header)
         resp = json_loads(rv.data.decode())
         info = resp["process_results"]
@@ -384,15 +380,14 @@
                 (
                     f"RasterInfoAssertion failed:"
                     f" value {key}:{val} does not match reference"
                 ),
             )
 
     def assertVectorInfo(self, location, mapset, vector, ref_info, header):
-
         url = (
             f"{URL_PREFIX}/locations/{location}/mapsets/{mapset}/"
             f"vector_layers/{vector}"
         )
         rv = self.server.get(url, headers=header)
         resp = json_loads(rv.data.decode())
         info = resp["process_results"]
```

### Comparing `actinia-core-4.9.1/src/actinia_core/version.py` & `actinia-core-4.9.2/src/actinia_core/version.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core.egg-info/PKG-INFO` & `actinia-core-4.9.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actinia-core
-Version: 4.9.1
+Version: 4.9.2
 Summary: Actinia Core is an open source REST API for scalable, distributed, high performance processing of geographical data that uses mainly GRASS GIS for computational tasks
 Author: Carmen Tawalika, Anika Weinmann, Guido Riembauer, Markus Metz, Julia Haas, Marc Jansen, Jorge A. Herrera Maldonado, Sören Gebbert, Markus Neteler, Momen Mawad, and more
 Project-URL: Homepage, https://github.com/actinia-org/actinia_core
 Project-URL: Tutorial, https://actinia-org.github.io/actinia_core
 Project-URL: API_Docs, https://redocly.github.io/redoc/?url=https://actinia.mundialis.de/latest/swagger.json
 Keywords: processing,earth observation,cloud-based processing,rest api,gis,grass gis,osgeo
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -69,14 +69,15 @@
 docker pull mundialis/actinia-core
 ```
 
 For own deployments or local dev-setup, see the `docker/` subfolder.
 
 Actinia is also available on [OSGeoLive](https://live.osgeo.org/en/overview/actinia_overview.html).
 
+
 ## Examples
 
 ### Data management
 
 * List all locations that are available in the actinia persistent database:
 
 ```bash
@@ -122,12 +123,74 @@
 To see a simple **list of endpoints** (and more), consult the "paths" section in the [API JSON](https://actinia.mundialis.de/api/v3/swagger.json); or, to list the available endpoints on command line, run
 
 ```bash
 # sudo npm install -g json
 curl -u 'demouser:gu3st!pa55w0rd' -X GET https://actinia.mundialis.de/api/v3/swagger.json | json paths | json -ka
 ```
 
+## Development
+
+### Use pre-commit
+
+It is highly recommended to install and use [pre-commit](https://pre-commit.com)
+before submitting any new or modified code or any other content. The pre-commit
+Git hooks set checks validity and executes automated formatting for
+a range of file formats, including Python. Pre-commit installs
+all necessary tools in a virtual environment upon first use.
+
+If you never used pre-commit before, you must start by installing it on your
+system. You only do it once:
+
+```bash
+python -m pip install pre-commit
+```
+
+Pre-commit must then be activated in the code repository. Change the directory
+to the root folder and use the `install` command:
+
+```bash
+cd <actinia-core_source_dir>
+
+# once per repo
+pre-commit install
+```
+
+Pre-commit will then be automatically triggered by the `git commit` command. If
+it finds any problem it will abort the commit and try to solve it automatically.
+In that case review the changes and run again `git add` and
+`git commit`.
+
+It is also possible to run pre-commit manually, e.g:
+
+```bash
+pre-commit run flake8 --all-files
+pre-commit run black --all-files
+# pre-commit run yamllint --all-files
+# pre-commit run markdownlint --all-files
+```
+
+Or to target a specific set of files:
+
+```bash
+pre-commit run --files src/*
+```
+
+The pre-commit hooks set is defined in
+[.pre-commit-config.yaml](.pre-commit-config.yaml).
+
+It is possible to temporally disable the pre-commit hooks in the repo, e.g. while
+working on older branches:
+
+```bash
+pre-commit uninstall
+```
+
+And to reactivate pre-commit again:
+
+```bash
+git switch main
+pre-commit install
+```
+
 ## Thanks to all contributors ❤
 
-<a href = "https://github.com/actinia-org/actinia-core/graphs/contributors">
-    <img src = "https://contrib.rocks/image?repo=actinia-org/actinia-core"/>
-</a>
+[![actinia-core contributors](https://contrib.rocks/image?repo=actinia-org/actinia-core "actinia-core contributors")](https://github.com/actinia-org/actinia-core/graphs/contributors)
```

### Comparing `actinia-core-4.9.1/src/actinia_core.egg-info/SOURCES.txt` & `actinia-core-4.9.2/src/actinia_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/src/actinia_core.egg-info/requires.txt` & `actinia-core-4.9.2/src/actinia_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_api_logging.py` & `actinia-core-4.9.2/tests/test_api_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         self.log = ApiLogger()
         self.request_object = DummyHTTPRequest()
 
     def tearDown(self):
         self.app_context.pop()
 
     def test_logging(self):
-
         ret = self.log.add_entry(
             user_id=self.user_id, http_request=self.request_object
         )
 
         self.assertTrue(ret, "add_entry does not work")
 
         ret = self.log.add_entry(
```

### Comparing `actinia-core-4.9.1/tests/test_async_mapset_merging.py` & `actinia-core-4.9.2/tests/test_async_mapset_merging.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_mapset_merging_strds.py` & `actinia-core-4.9.2/tests/test_async_mapset_merging_strds.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,14 @@
         },
     ],
     "version": "1",
 }
 
 
 class AsyncMapsetMergingSTRDS(ActiniaResourceTestCaseBase):
-
     user_mapset = mapset_name
     raster_dict_modis = {
         "MOD11B3.A2015001.h11v05.single_LST_Day_6km": "2015-01-01 00:00:00",
         "MOD11B3.A2015032.h11v05.single_LST_Day_6km": "2015-02-01 00:00:00",
         "MOD11B3.A2015060.h11v05.single_LST_Day_6km": "2015-03-01 00:00:00",
     }
     raster_dict_modis2 = {
@@ -313,15 +312,14 @@
         self.assertEqual(
             raster_times,
             raster_times,
             "STRDS times and raster names are not correct in test mapset",
         )
 
     def test_create_strds_in_persistent_user_db(self):
-
         rv = self.server.post(
             f"{URL_PREFIX}/locations/nc_spm_08/mapsets/{self.user_mapset}/"
             "processing_async",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_create_strds1),
             content_type="application/json",
         )
@@ -370,15 +368,14 @@
 
         # check if strds 'modis' is in mapset
         self.check_strds_in_mapset(["modis"])
         # check if correct maps are listed i strds 'modis'
         self.check_modis_strds(self.raster_dict_modis, "modis")
 
     def test_create_strds_in_persistent_user_db_2(self):
-
         rv = self.server.post(
             f"{URL_PREFIX}/locations/nc_spm_08/mapsets/{self.user_mapset}/"
             "processing_async",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_create_strds1),
             content_type="application/json",
         )
@@ -408,15 +405,14 @@
         # check if strds 'modis' and 'modis2' is in mapset
         self.check_strds_in_mapset(["modis", "modis2"])
         # check if correct maps are listed in strds 'modis' and 'modis2'
         self.check_modis_strds(self.raster_dict_modis, "modis")
         self.check_modis_strds(self.raster_dict_modis2, "modis2")
 
     def test_create_strds_in_persistent_user_db_3(self):
-
         rv = self.server.post(
             f"{URL_PREFIX}/locations/nc_spm_08/mapsets/{self.user_mapset}/"
             "processing_async",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_create_strds1),
             content_type="application/json",
         )
```

### Comparing `actinia-core-4.9.1/tests/test_async_process_postgis_import_export.py` & `actinia-core-4.9.2/tests/test_async_process_postgis_import_export.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_process_validation.py` & `actinia-core-4.9.2/tests/test_async_process_validation.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_process_validation_errors.py` & `actinia-core-4.9.2/tests/test_async_process_validation_errors.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_processing.py` & `actinia-core-4.9.2/tests/test_async_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,30 +169,28 @@
         "verbose": True,
     },
 }
 
 
 class AsyncProcessTestCase(ActiniaResourceTestCaseBase):
     def test_async_processing(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
             rv,
             headers=self.admin_auth_header,
             http_status=200,
             status="finished",
         )
 
     def test_async_processing_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain),
             content_type="application/json",
         )
         print(rv.data)
@@ -242,15 +240,14 @@
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
         self.assertEqual(resp["status"], "terminated")
 
         time.sleep(1)
 
     def test_async_processing_large_region(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_region),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -298,15 +295,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_async_processing_error_3(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_3),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -314,15 +310,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_async_processing_error_4(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_4),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -348,15 +343,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_async_processing_error_6(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_5),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -364,15 +358,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_async_processing_error_7(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_6),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
```

### Comparing `actinia-core-4.9.1/tests/test_async_processing_2.py` & `actinia-core-4.9.2/tests/test_async_processing_2.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_processing_custom.py` & `actinia-core-4.9.2/tests/test_async_processing_custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 __maintainer__ = "Sören Gebbert"
 __email__ = "soerengebbert@googlemail.com"
 
 
 class AsyncProcessCustomTestCaseAdmin(ActiniaResourceTestCaseBase):
     def test_async_processing(self):
-
         rv = self.server.post(
             URL_PREFIX + "/custom_process/uname",
             headers=self.admin_auth_header,
             data=json_dumps(["-a"]),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(rv, headers=self.admin_auth_header)
```

### Comparing `actinia-core-4.9.1/tests/test_async_processing_export.py` & `actinia-core-4.9.2/tests/test_async_processing_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,15 +321,14 @@
         "verbose": True,
     },
 }
 
 
 class AsyncProcessExportTestCaseUser(ActiniaResourceTestCaseBase):
     def test_async_processing(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_short),
             content_type="application/json",
         )
         resp = self.waitAsyncStatusAssertHTTP(
@@ -401,15 +400,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_termination_1(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_short_long_run),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -425,15 +423,14 @@
             headers=self.admin_auth_header,
             http_status=200,
             status="terminated",
             message_check="AsyncProcessTermination:",
         )
 
     def test_termination_2(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_short_long_run),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -449,15 +446,14 @@
             headers=self.user_auth_header,
             http_status=200,
             status="terminated",
             message_check="AsyncProcessTermination:",
         )
 
     def test_termination_3(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.root_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -473,15 +469,14 @@
             headers=self.root_auth_header,
             http_status=200,
             status="terminated",
             message_check="AsyncProcessTermination:",
         )
 
     def test_error_1(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_1),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -489,15 +484,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_error_2(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_2),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -505,15 +499,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_error_3(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_3),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -521,15 +514,14 @@
             headers=self.user_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_error_4(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.user_auth_header,
             data=json_dumps(process_chain_error_4),
             content_type="application/json",
         )
 
@@ -565,15 +557,14 @@
                 "HTML status code is wrong %i" % rv.status_code,
             )
         time.sleep(1)
 
 
 class AsyncProcessExportTestCaseAdmin(ActiniaResourceTestCaseBase):
     def test_async_processing(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = self.waitAsyncStatusAssertHTTP(
@@ -592,15 +583,14 @@
                 "HTML status code is wrong %i" % rv.status_code,
             )
             self.assertEqual(
                 rv.mimetype, "image/tiff", "Wrong mimetype %s" % rv.mimetype
             )
 
     def test_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -616,15 +606,14 @@
             headers=self.admin_auth_header,
             http_status=200,
             status="terminated",
             message_check="AsyncProcessTermination:",
         )
 
     def test_error_1(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_error_1),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -632,15 +621,14 @@
             headers=self.admin_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_error_2(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_error_2),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -648,15 +636,14 @@
             headers=self.admin_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_error_3(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_error_3),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
@@ -664,15 +651,14 @@
             headers=self.admin_auth_header,
             http_status=400,
             status="error",
             message_check="AsyncProcessError:",
         )
 
     def test_error_4(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_error_4),
             content_type="application/json",
         )
         self.waitAsyncStatusAssertHTTP(
```

### Comparing `actinia-core-4.9.1/tests/test_async_processing_export_file.py` & `actinia-core-4.9.2/tests/test_async_processing_export_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,14 @@
                 "application/zip",
                 "Wrong mimetype %s" % rv.mimetype,
             )
             print(rv.headers)
             print(rv.iter_encoded())
 
     def test_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(file_export),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -155,15 +154,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_async_processing_export(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_s3",
             headers=self.admin_auth_header,
             data=json_dumps(file_export),
             content_type="application/json",
         )
         resp = self.waitAsyncStatusAssertHTTP(
@@ -186,15 +184,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_s3",
             headers=self.admin_auth_header,
             data=json_dumps(file_export),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -223,15 +220,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_async_processing_export(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_gcs",
             headers=self.admin_auth_header,
             data=json_dumps(file_export),
             content_type="application/json",
         )
         resp = self.waitAsyncStatusAssertHTTP(
@@ -254,15 +250,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_gcs",
             headers=self.admin_auth_header,
             data=json_dumps(file_export),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
```

### Comparing `actinia-core-4.9.1/tests/test_async_processing_export_to_storage.py` & `actinia-core-4.9.2/tests/test_async_processing_export_to_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         },
     },
 }
 
 
 class AsyncProcessExport2TestCaseAdmin(ActiniaResourceTestCaseBase):
     def test_async_processing_export(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = self.waitAsyncStatusAssertHTTP(
@@ -154,15 +153,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_s3",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
@@ -191,15 +189,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_async_processing_export(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_gcs",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = self.waitAsyncStatusAssertHTTP(
@@ -222,15 +219,14 @@
     @unittest.skipIf(
         "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ
         and "GOOGLE_CLOUD_PROJECT" not in os.environ,
         "Test is skipped because 'GOOGLE_APPLICATION_CREDENTIALS' and "
         "'GOOGLE_CLOUD_PROJECT' not set",
     )
     def test_termination(self):
-
         rv = self.server.post(
             URL_PREFIX + "/locations/nc_spm_08/processing_async_export_gcs",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
         resp = json_loads(rv.data)
```

### Comparing `actinia-core-4.9.1/tests/test_async_processing_export_vector.py` & `actinia-core-4.9.2/tests/test_async_processing_export_vector.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_processing_import_export.py` & `actinia-core-4.9.2/tests/test_async_processing_import_export.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_processing_mapset.py` & `actinia-core-4.9.2/tests/test_async_processing_mapset.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         "verbose": True,
     },
 }
 
 
 class AsyncProcessMapsetTestCaseAdmin(ActiniaResourceTestCaseBase):
     def check_remove_test_mapset(self):
-
         rv = self.server.get(
             URL_PREFIX + "/locations/nc_spm_08/mapsets",
             headers=self.user_auth_header,
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
@@ -445,15 +444,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_4_create_global_mapset(self):
-
         rv = self.server.post(
             URL_PREFIX
             + "/locations/nc_spm_08/mapsets/PERMANENT/processing_async",
             headers=self.admin_auth_header,
             data=json_dumps(process_chain_long),
             content_type="application/json",
         )
```

### Comparing `actinia-core-4.9.1/tests/test_async_processing_stdout_parser.py` & `actinia-core-4.9.2/tests/test_async_processing_stdout_parser.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_async_raster_export.py` & `actinia-core-4.9.2/tests/test_async_raster_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 __maintainer__ = "Sören Gebbert"
 __email__ = "soerengebbert@googlemail.com"
 
 
 class RasterAsyncExport(ActiniaResourceTestCaseBase):
     def test_export(self):
-
         rv = self.server.post(
             f"{URL_PREFIX}/locations/nc_spm_08/mapsets/PERMANENT/raster_layers"
             "/elevation/geotiff_async",
             headers=self.user_auth_header,
         )
         resp = self.waitAsyncStatusAssertHTTP(
             rv, headers=self.user_auth_header
@@ -68,15 +67,14 @@
                 rv.mimetype, "image/tiff", "Wrong mimetype %s" % rv.mimetype
             )
             print(rv.headers)
 
         time.sleep(1)
 
     def test_export_region(self):
-
         rv = self.server.post(
             f"{URL_PREFIX}/locations/nc_spm_08/mapsets/PERMANENT/raster_layers"
             "/elevation/geotiff_async_orig",
             headers=self.user_auth_header,
         )
         resp = self.waitAsyncStatusAssertHTTP(
             rv, headers=self.user_auth_header
@@ -97,15 +95,14 @@
                 rv.mimetype, "image/tiff", "Wrong mimetype %s" % rv.mimetype
             )
             print(rv.headers)
 
         time.sleep(1)
 
     def test_export_error(self):
-
         rv = self.server.post(
             f"{URL_PREFIX}/locations/nc_spm_08/mapsets/PERMANENT/"
             "raster_layers/elevationion/geotiff_async",
             headers=self.user_auth_header,
         )
         self.waitAsyncStatusAssertHTTP(
             rv,
```

### Comparing `actinia-core-4.9.1/tests/test_aws_sentinel_interface.py` & `actinia-core-4.9.2/tests/test_aws_sentinel_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,16 @@
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def validate_result(self, result, bands):
-
         for scene in result:
             for tile in scene["tiles"]:
-
                 url = tile["info"]
                 response = urlopen(url)
                 mime_type = magic.from_buffer(
                     response.read(256), mime=True
                 ).lower()
                 print(mime_type)
                 self.assertTrue(mime_type in ["text/plain"])
```

### Comparing `actinia-core-4.9.1/tests/test_common_base.py` & `actinia-core-4.9.2/tests/test_common_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 # Set this variable to use a actinia config file in a docker container
 if "ACTINIA_CUSTOM_TEST_CFG" in os.environ:
     custom_actinia_cfg = str(os.environ["ACTINIA_CUSTOM_TEST_CFG"])
 
 
 def setup_environment():
-
     # If docker config
     if custom_actinia_cfg is not False:
         global_config.read(custom_actinia_cfg)
         return
 
     global redis_pid
     # Set the port to the test redis server
@@ -98,15 +97,14 @@
 class CommonTestCaseBase(unittest.TestCase):
     """
     This is the base class for the common testing
     """
 
     @classmethod
     def setUpClass(cls):
-
         if custom_actinia_cfg is not False:
             global_config.read(custom_actinia_cfg)
             print(global_config)
         else:
             global_config.REDIS_SERVER_URL = "localhost"
             global_config.REDIS_SERVER_PORT = 7000
```

### Comparing `actinia-core-4.9.1/tests/test_configuration.py` & `actinia-core-4.9.2/tests/test_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,29 +40,27 @@
     This class tests the user interface, the creation and deletion
     of a user entry in a Redis database
     """
 
     file_name = "/tmp/actinia_test.cfg"
 
     def test_change_loglevel(self):
-
         c = Configuration()
 
         c.write(self.file_name)
         c.read(self.file_name)
 
         c.LOG_LEVEL = 1
         c.write(self.file_name)
         c.LOG_LEVEL = 4
         c.read(self.file_name)
 
         self.assertEqual(c.LOG_LEVEL, 1)
 
     def test_read_write_exceptions(self):
-
         c = Configuration()
         self.assertRaises(IOError, c.read, "/dk/l/K/D/V/l/d/g")
         self.assertRaises(IOError, c.write, "/dk/l/K/D/V/l/d/g")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `actinia-core-4.9.1/tests/test_download_cache.py` & `actinia-core-4.9.2/tests/test_download_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 __maintainer__ = "Sören Gebbert"
 __email__ = "soerengebbert@googlemail.com"
 
 
 class DownloadCacheTestCase(ActiniaResourceTestCaseBase):
     def test_download_cache(self):
-
         global_config.DOWNLOAD_CACHE = "/tmp/dcache_tmp"
         global_config.DOWNLOAD_CACHE_QUOTA = 1
         try:
             os.mkdir(global_config.DOWNLOAD_CACHE)
         except Exception:  # more precise exception gladly accepted
             pass
 
@@ -115,15 +114,14 @@
         self.assertTrue("quota" in json_load(rv.data)["process_results"])
         self.assertTrue("free" in json_load(rv.data)["process_results"])
         self.assertTrue(
             "free_percent" in json_load(rv.data)["process_results"]
         )
 
     def test_download_cache_error_1(self):
-
         if os.path.isdir("/tmp/dcache_tmp_nope") is True:
             os.rmdir("/tmp/dcache_tmp_nope")
 
         global_config.DOWNLOAD_CACHE = "/tmp/dcache_tmp_nope"
         global_config.DOWNLOAD_CACHE_QUOTA = 1
 
         rv = self.server.get(
@@ -136,15 +134,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_download_cache_error_2(self):
-
         if os.path.isdir("/tmp/dcache_tmp_nope") is True:
             os.rmdir("/tmp/dcache_tmp_nope")
 
         global_config.DOWNLOAD_CACHE = "/tmp/dcache_tmp_nope"
         global_config.DOWNLOAD_CACHE_QUOTA = 1
 
         rv = self.server.delete(
```

### Comparing `actinia-core-4.9.1/tests/test_geodata_import.py` & `actinia-core-4.9.2/tests/test_geodata_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
     def tearDown(self):
         if os.path.isdir(self.cache_dir) is True:
             shutil.rmtree(self.cache_dir)
         pass
 
     def _run_process(self, process):
-
         print("Run process: " + str(process))
 
         inputlist = list()
         inputlist.append(process.executable)
         inputlist.extend(process.executable_params)
 
         proc = subprocess.Popen(
@@ -104,15 +103,14 @@
         proc.wait()
 
         self.assertEqual(
             0, proc.returncode, "Error while running %s" % process.executable
         )
 
     def test_download_commands_gml(self):
-
         gml = additional_external_data["census_wake2000_gml"]
 
         gddl = GeoDataDownloadImportSupport(
             config=global_config,
             temp_file_path="/tmp",
             download_cache=self.cache_dir,
             send_resource_update=update_dummy,
@@ -134,15 +132,14 @@
 
         for url, file_path, file_name in import_file_info:
             p = gddl.get_vector_import_command(file_name, "test")
             print(p)
             self.assertEqual("v.import", p.executable)
 
     def test_download_commands_gml_zip(self):
-
         url_list = []
 
         gml = additional_external_data["census_wake2000_gml"]
         gml_zip = additional_external_data["census_wake2000_zip"]
         tif = additional_external_data["geology_30m_tif"]
         tif_zip = additional_external_data["geology_30m_zip"]
 
@@ -167,15 +164,14 @@
         for p in pl:
             self._run_process(p)
 
         for url, file_path, file_name in import_file_info:
             gddl.perform_file_validation(filepath=file_name)
 
     def test_download_commands_tif(self):
-
         tif_list = []
         tif_list.append(additional_external_data["geology_30m_tif"])
         tif_list.append(additional_external_data["geology_30m_tif"])
         tif_list.append(additional_external_data["geology_30m_tif"])
         tif_list.append(additional_external_data["geology_30m_tif"])
         tif_list.append(additional_external_data["geology_30m_tif"])
         tif_list.append(additional_external_data["geology_30m_tif"])
@@ -205,15 +201,14 @@
 
         for url, file_path, file_name in import_file_info:
             p = gddl.get_raster_import_command(file_name, "test")
             print(p)
             self.assertEqual("r.import", p.executable)
 
     def test_landsat_download_commands(self):
-
         lp = LandsatProcessing(
             config=global_config,
             temp_file_path="/tmp",
             scene_id="LC08_L1GT_001004_20130910_20170502_01_T2",
             download_cache=self.cache_dir,
             send_resource_update=update_dummy,
             message_logger=MessageDummy(),
```

### Comparing `actinia-core-4.9.1/tests/test_google_cloud_interfaces.py` & `actinia-core-4.9.2/tests/test_google_cloud_interfaces.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_job_resumption.py` & `actinia-core-4.9.2/tests/test_job_resumption.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,14 @@
             "stdout": {"id": "r_info_map2", "format": "kv", "delimiter": "="},
         },
     ],
 }
 
 
 class JobResumptionProcessingTestCase(ActiniaResourceTestCaseBase):
-
     cfg_file = os.environ.get(
         "ACTINIA_CUSTOM_TEST_CFG", "/etc/default/actinia"
     )
     tmp_cfg_file = "%s_tmp" % cfg_file
     save_interim_results_value = None
     endpoint = "/locations/nc_spm_08/processing_async"
     resource_user_id = None
@@ -915,15 +914,14 @@
                     resp_data3[str(iteration)],
                     "'iteration' is in response",
                 )
             del rv3, resp_data3
 
 
 class JobResumptionProcessingExportTestCase(JobResumptionProcessingTestCase):
-
     endpoint = "/locations/nc_spm_08/processing_async_export"
     resource_user_id = None
     resource_resource_id = None
 
     def test_job_resumption_exporter(self):
         """
         Test job resumption with processing_async_export endpoint and exporter
@@ -1075,15 +1073,14 @@
         self.__class__.resource_user_id = rv_user_id
         self.__class__.resource_resource_id = rv_resource_id
 
 
 class JobResumptionPersistentProcessingTestCase(
     JobResumptionProcessingTestCase
 ):
-
     location = "nc_spm_08"
     mapset = "test_mapset"
     endpoint = "/locations/%s/mapsets/%s/processing_async" % (location, mapset)
     resource_user_id = None
     resource_resource_id = None
     mapset_created = True
 
@@ -1150,15 +1147,14 @@
         super(
             JobResumptionPersistentProcessingTestCase, self
         ).test_resource_endpoints()
         self.__class__.mapset_created = False
 
 
 class JobResumptionErrorTestCase(ActiniaResourceTestCaseBase):
-
     endpoint = "/locations/nc_spm_08/processing_async"
 
     def test_job_resumption_config_error(self):
         """Test if the job resumption fails if save_interim_results is set to
         False in the actinia.cfg
         """
         tpl = Template(json_dumps(process_chain_1))
```

### Comparing `actinia-core-4.9.1/tests/test_location_management.py` & `actinia-core-4.9.2/tests/test_location_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_location_creation_and_deletion(self):
-
         # Delete a potentially existing location
         rv = self.server.delete(
             URL_PREFIX + "/locations/test_location",
             headers=self.admin_auth_header,
         )
 
         # Create new location as admin
@@ -172,15 +171,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_location_creation_and_deletion_as_user(self):
-
         # Delete a potentially existing location
         rv = self.server.delete(
             URL_PREFIX + "/locations/test_location",
             headers=self.user_auth_header,
         )
 
         # Create new location as user
@@ -252,15 +250,14 @@
         self.assertEqual(
             rv.mimetype,
             "application/json",
             "Location redeletion by user: Wrong mimetype %s" % rv.mimetype,
         )
 
     def test_location_creation_and_deletion_as_guest(self):
-
         # ERROR: Try to create a location as guest
         rv = self.server.post(
             URL_PREFIX + "/locations/test_location_user",
             data=json_dumps({"epsg": "4326"}),
             content_type="application/json",
             headers=self.guest_auth_header,
         )
```

### Comparing `actinia-core-4.9.1/tests/test_login.py` & `actinia-core-4.9.2/tests/test_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,60 +280,56 @@
             rv.status_code,
             200,
             f"HTML status code is wrong {rv.status_code} for get user from a "
             "admin.",
         )
 
     def test_token_generation_admin(self):
-
         rv = self.server.get(
             URL_PREFIX + "/token", headers=self.admin_auth_header
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_api_key_generation_admin(self):
-
         rv = self.server.get(
             URL_PREFIX + "/api_key", headers=self.admin_auth_header
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_token_generation_user(self):
-
         rv = self.server.get(
             URL_PREFIX + "/token", headers=self.user_auth_header
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_token_generation_user_expire(self):
-
         rv = self.server.get(
             URL_PREFIX + "/token?expiration_time=3600",
             headers=self.user_auth_header,
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
@@ -341,58 +337,54 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_token_generation_guest(self):
-
         rv = self.server.get(
             URL_PREFIX + "/token", headers=self.guest_auth_header
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_token_generation_wrong_no_auth(self):
-
         rv = self.server.get(URL_PREFIX + "/token")
         print(rv.data)
         self.assertEqual(
             rv.status_code,
             401,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "text/html", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_api_key_generation_wrong_user(self):
-
         rv = self.server.get(
             URL_PREFIX + "/api_key", headers=self.user_auth_header
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
             401,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_token_generation_user_expire_error(self):
-
         rv = self.server.get(
             URL_PREFIX + "/token?expiration_time=1000000000",
             headers=self.user_auth_header,
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
@@ -400,15 +392,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_token_generation_user_expire_wrong(self):
-
         rv = self.server.get(
             URL_PREFIX + "/token?expiration_time=blablub",
             headers=self.user_auth_header,
         )
         print(rv.data)
         self.assertEqual(
             rv.status_code,
```

### Comparing `actinia-core-4.9.1/tests/test_mapset_management.py` & `actinia-core-4.9.2/tests/test_mapset_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_mapsets.py` & `actinia-core-4.9.2/tests/test_mapsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 __license__ = "GPLv3"
 __author__ = "Julia Haas, Guido Riembauer"
 __copyright__ = "Copyright 2021 mundialis GmbH & Co. KG"
 __maintainer__ = "mundialis"
 
 
 class MapsetsTestCase(ActiniaResourceTestCaseBase):
-
     test_mapsets = [str(uuid.uuid4()), str(uuid.uuid4())]
     test_user = f"test_user_{str(uuid.uuid4())}"
     accessible_datasets = {
         "nc_spm_08": ["PERMANENT"],
         "latlong_wgs84": ["PERMANENT"],
     }
     ref_mapsets = []
```

### Comparing `actinia-core-4.9.1/tests/test_message_logger.py` & `actinia-core-4.9.2/tests/test_message_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 class MessageLoggerTestCase(unittest.TestCase):
     """
     This class tests the user interface, the creation and deletion
     of a user entry in a Redis database
     """
 
     def test_change_loglevel(self):
-
         c = Configuration()
         c.LOG_LEVEL = 4
 
         logger = MessageLogger(config=c, user_id="soeren")
         logger.debug("debug")
         logger.info("info")
         logger.warning("warning")
@@ -78,15 +77,14 @@
         logger = MessageLogger(config=c, user_id="soeren")
         logger.debug("debug")
         logger.info("info")
         logger.warning("warning")
         logger.error("error")
 
     def test_fluentd(self):
-
         c = Configuration()
         c.LOG_LEVEL = 4
         c.LOG_INTERFACE = "fluentd"
 
         logger = MessageLogger(config=c, user_id="soeren")
         logger.debug("debug")
         logger.info("info")
```

### Comparing `actinia-core-4.9.1/tests/test_process_queue.py` & `actinia-core-4.9.2/tests/test_process_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
             map_name="map_name",
         )
 
     def tearDown(self):
         self.app_context.pop()
 
     def otest_1(self):
-
         create_process_queue(config=global_config, use_logger=False)
 
         args = deepcopy(self.rdc)
         args.api_info = 0
 
         args = deepcopy(self.rdc)
         args.api_info = 1
@@ -140,15 +139,14 @@
 
         time.sleep(10)
         stop_process_queue()
 
         return
 
     def otest_2(self):
-
         create_process_queue(config=global_config, use_logger=False)
 
         args = deepcopy(self.rdc)
         args.api_info = 0
 
         enqueue_job(30, job_with_exception, args)
```

### Comparing `actinia-core-4.9.1/tests/test_raster_colors.py` & `actinia-core-4.9.2/tests/test_raster_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
         colors = json_load(rv.data)["process_results"]
         self.assertTrue(len(colors) == 8)
 
     def test_raster_layer_set_colors(self):
-
         new_mapset = "raster_test_mapset"
         self.create_new_mapset(new_mapset)
 
         # Create
         postbody = {
             "list": [
                 {
```

### Comparing `actinia-core-4.9.1/tests/test_raster_layer.py` & `actinia-core-4.9.2/tests/test_raster_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     "Copyright 2016-2018, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "Sören Gebbert"
 __email__ = "soerengebbert@googlemail.com"
 
 
 class RasterLayerTestCase(ActiniaResourceTestCaseBase):
-
     # TODO create test for CREATION (upload)
 
     def test_raster_layer_info(self):
         rv = self.server.get(
             URL_PREFIX
             + "/locations/nc_spm_08/mapsets/PERMANENT/raster_layers/elevation",
             headers=self.user_auth_header,
```

### Comparing `actinia-core-4.9.1/tests/test_raster_layers.py` & `actinia-core-4.9.2/tests/test_raster_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
         map_list = json_loads(rv.data)["process_results"]
         self.assertTrue(len(map_list) == 0)
 
     def test_remove_raster_layers_pattern(self):
-
         new_mapset = "raster_test_mapset"
         self.create_new_mapset(new_mapset)
 
         map_list = ["test_delete_layer_1", "test_delete_layer_2"]
 
         # Create raster layers
         for map_name in map_list:
@@ -220,15 +219,14 @@
                 + "/locations/nc_spm_08/mapsets/%s/raster_layers/%s"
                 % (new_mapset, map_name),
                 headers=self.user_auth_header,
             )
             print(rv.data.decode())
 
     def test_rename_raster_layers(self):
-
         new_mapset = "raster_test_mapset"
         self.create_new_mapset(new_mapset)
 
         map_list = ["test_rename_layer_1", "test_rename_layer_2"]
         new_map_list = ["test_rename_layer_1_new", "test_rename_layer_2_new"]
         rename_map_list = [
             ("test_rename_layer_1", "test_rename_layer_1_new"),
```

### Comparing `actinia-core-4.9.1/tests/test_raster_legend.py` & `actinia-core-4.9.2/tests/test_raster_legend.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_raster_renderer.py` & `actinia-core-4.9.2/tests/test_raster_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_raster_upload.py` & `actinia-core-4.9.2/tests/test_raster_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __license__ = "GPLv3"
 __author__ = "Anika Weinmann, Guido Riembauer"
 __copyright__ = "Copyright 2016-2021, mundialis GmbH & Co. KG"
 __maintainer__ = "mundialis GmbH & Co. KG"
 
 
 class UploadRasterLayerTestCase(ActiniaResourceTestCaseBase):
-
     location = "nc_spm_08"
     mapset = "PERMANENT"
     tmp_mapset = "mapset_upload"
     raster = "elev_ned_30m"
     raster_url = additional_external_data["elev_ned_30m_tif"]
     local_raster = f"/tmp/{raster}.tif"
```

### Comparing `actinia-core-4.9.1/tests/test_resource_base.py` & `actinia-core-4.9.2/tests/test_resource_base.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_resource_logging.py` & `actinia-core-4.9.2/tests/test_resource_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         self.log = ResourceLogger(*redis_args)
         del redis_args
 
     def tearDown(self):
         self.app_context.pop()
 
     def test_logging(self):
-
         ret = self.log.commit(
             user_id=self.user_id,
             resource_id=self.resource_id,
             iteration=1,
             document=self.document,
         )
 
@@ -111,15 +110,14 @@
         ret = self.log.delete(
             user_id=self.user_id, resource_id=self.resource_id
         )
 
         self.assertFalse(ret)
 
     def test_list(self):
-
         user = "lisa"
         resource = "a"
         ret = self.log.commit(
             user_id=user,
             resource_id=resource,
             iteration=1,
             document=self.document,
@@ -180,15 +178,14 @@
         ret = self.log.get_user_resources("franky")
         print(ret)
 
         ret = self.log.get_user_resources("klaus")
         print(ret)
 
     def test_termination(self):
-
         ret = self.log.commit_termination(
             user_id=self.user_id, resource_id=self.resource_id
         )
 
         self.assertTrue(ret)
 
         ret = self.log.get_termination(
```

### Comparing `actinia-core-4.9.1/tests/test_resource_management.py` & `actinia-core-4.9.2/tests/test_resource_management.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_resource_storage.py` & `actinia-core-4.9.2/tests/test_resource_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "Copyright 2016-2022, Sören Gebbert and mundialis GmbH & Co. KG"
 )
 __maintainer__ = "mundialis"
 
 
 class ResourceStorageTestCase(ActiniaResourceTestCaseBase):
     def test_resource_storage(self):
-
         global_config.GRASS_RESOURCE_DIR = "/tmp/rstorage_tmp"
         global_config.GRASS_RESOURCE_QUOTA = 1
         try:
             os.mkdir(global_config.GRASS_RESOURCE_DIR)
         except Exception:  # more precise exception gladly accepted
             pass
 
@@ -85,14 +84,15 @@
         self.assertTrue(
             "free_percent" in json_load(rv.data)["process_results"]
         )
 
         rv = self.server.delete(
             URL_PREFIX + "/resource_storage", headers=self.admin_auth_header
         )
+        self.waitAsyncStatusAssertHTTP(rv, headers=self.admin_auth_header)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
@@ -114,15 +114,14 @@
         self.assertTrue("quota" in json_load(rv.data)["process_results"])
         self.assertTrue("free" in json_load(rv.data)["process_results"])
         self.assertTrue(
             "free_percent" in json_load(rv.data)["process_results"]
         )
 
     def test_resource_storage_error_1(self):
-
         global_config.GRASS_RESOURCE_DIR = "/tmp/rstorage_tmp_nope"
         global_config.GRASS_RESOURCE_QUOTA = 1
 
         rv = self.server.get(
             URL_PREFIX + "/resource_storage", headers=self.admin_auth_header
         )
         self.assertEqual(
@@ -131,32 +130,32 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_resource_storage_error_2(self):
-
         global_config.GRASS_RESOURCE_DIR = "/tmp/rstorage_tmp_nope"
         global_config.GRASS_RESOURCE_QUOTA = 1
 
         rv = self.server.delete(
             URL_PREFIX + "/resource_storage", headers=self.admin_auth_header
         )
-        self.assertEqual(
-            rv.status_code,
-            400,
-            "HTML status code is wrong %i" % rv.status_code,
+        self.waitAsyncStatusAssertHTTP(
+            rv,
+            headers=self.admin_auth_header,
+            http_status=400,
+            status="error",
+            message_check="AsyncProcessError:",
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_resource_storage_delete_olderthan(self):
-
         global_config.GRASS_RESOURCE_DIR = "/tmp/rstorage_tmp"
         global_config.GRASS_RESOURCE_QUOTA = 1
         try:
             os.mkdir(global_config.GRASS_RESOURCE_DIR)
         except Exception:  # more precise exception gladly accepted
             pass
 
@@ -203,28 +202,31 @@
         )
 
         # delete files older than 10 days
         rv = self.server.delete(
             URL_PREFIX + "/resource_storage?olderthan=10",
             headers=self.admin_auth_header,
         )
+        self.waitAsyncStatusAssertHTTP(rv, headers=self.admin_auth_header)
+        self.waitAsyncStatusAssertHTTP(rv, headers=self.admin_auth_header)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
         # check files
         files = os.listdir(admin_resource_path)
         self.assertIn("file1.txt", files, "'file1.txt' not in resource path")
         self.assertNotIn("file2.txt", files, "'file2.txt' in resource path")
 
         # clean up resource storage
         rv = self.server.delete(
             URL_PREFIX + "/resource_storage", headers=self.admin_auth_header
         )
+        self.waitAsyncStatusAssertHTTP(rv, headers=self.admin_auth_header)
         self.assertEqual(
             rv.status_code,
             200,
             "HTML status code is wrong %i" % rv.status_code,
         )
```

### Comparing `actinia-core-4.9.1/tests/test_strds_management.py` & `actinia-core-4.9.2/tests/test_strds_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
         )
 
         start_time = json_loads(rv.data)["process_results"]["start_time"]
 
         self.assertEqual(start_time, "'2015-01-01 00:00:00'")
 
     def test_strds_create_remove(self):
-
         new_mapset = "strds_test"
         self.create_new_mapset(mapset_name=new_mapset, location_name=location)
 
         # Create success
         rv = self.server.post(
             URL_PREFIX
             + "/locations/%s/mapsets/%s/strds/test_strds"
```

### Comparing `actinia-core-4.9.1/tests/test_strds_raster_management.py` & `actinia-core-4.9.2/tests/test_strds_raster_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_strds_creation_error(self):
-
         # This must fail, global mapsets are not allowed to modify
         rv = self.server.post(
             f"{URL_PREFIX}/locations/{location}/mapsets/{strds_mapset}/strds/"
             "test_strds_register",
             headers=self.admin_auth_header,
             data=json_dumps(
                 {
@@ -138,15 +137,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_strds_create_register_unregister_1(self):
-
         self.create_new_mapset(new_mapset, location)
 
         # Create success
         rv = self.server.post(
             f"{URL_PREFIX}/locations/{location}/mapsets/{new_mapset}/strds/"
             "test_strds_register",
             headers=self.admin_auth_header,
```

### Comparing `actinia-core-4.9.1/tests/test_strds_raster_renderer.py` & `actinia-core-4.9.2/tests/test_strds_raster_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
             "HTML status code is wrong %i" % rv.status_code,
         )
         self.assertEqual(
             rv.mimetype, "application/json", "Wrong mimetype %s" % rv.mimetype
         )
 
     def test_strds_render_1(self):
-
         new_mapset = "strds_render_test"
         self.create_new_mapset(new_mapset, location)
 
         # Create success
         rv = self.server.post(
             f"{URL_PREFIX}/locations/{location}/mapsets/{new_mapset}/strds/"
             "test_strds_register",
```

### Comparing `actinia-core-4.9.1/tests/test_user_management.py` & `actinia-core-4.9.2/tests/test_user_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         self.password = "1234"
         self.user_group = "test"
 
     def tearDown(self):
         self.app_context.pop()
 
     def test_create_delete_user(self):
-
         # Make sure the user database is empty
         user = ActiniaUser(self.user_id)
         if user.exists():
             print("Delete existing user")
             user.delete()
 
         # Create a new user
```

### Comparing `actinia-core-4.9.1/tests/test_vector_layer.py` & `actinia-core-4.9.2/tests/test_vector_layer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_vector_layers.py` & `actinia-core-4.9.2/tests/test_vector_layers.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_vector_renderer.py` & `actinia-core-4.9.2/tests/test_vector_renderer.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_vector_upload.py` & `actinia-core-4.9.2/tests/test_vector_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
       }
     }
   ]
 }"""
 
 
 class UploadVectorLayerTestCase(ActiniaResourceTestCaseBase):
-
     location = "nc_spm_08"
     mapset = "PERMANENT"
     tmp_mapset = "mapset_upload"
     vector = "testvector"
     local_geojson = f"/tmp/{vector}.geojson"
     gpkg_file = "/src/actinia_core/tests/data/nc_test_poly.gpkg"
     zipped_shp_file = "/src/actinia_core/tests/data/nc_test_poly.zip"
```

### Comparing `actinia-core-4.9.1/tests/test_version_health.py` & `actinia-core-4.9.2/tests/test_version_health.py`

 * *Files identical despite different names*

### Comparing `actinia-core-4.9.1/tests/test_webhook.py` & `actinia-core-4.9.2/tests/test_webhook.py`

 * *Files identical despite different names*

