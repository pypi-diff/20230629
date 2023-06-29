# Comparing `tmp/google-cloud-securitycenter-1.8.0.tar.gz` & `tmp/google-cloud-securitycenter-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-securitycenter-1.8.0.tar", last modified: Tue Jan 18 16:08:05 2022, max compression
+gzip compressed data, was "google-cloud-securitycenter-1.9.0.tar", last modified: Mon Feb 28 22:53:33 2022, max compression
```

## Comparing `google-cloud-securitycenter-1.8.0.tar` & `google-cloud-securitycenter-1.9.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.951387 google-cloud-securitycenter-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3957 2022-01-18 16:08:05.951387 google-cloud-securitycenter-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2994 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.927399 google-cloud-securitycenter-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.931397 google-cloud-securitycenter-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.931397 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter/
--rw-rw-r--   0 root         (0)     1003     7501 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter/__init__.py
--rw-rw-r--   0 root         (0)     1003       88 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.931397 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/
--rw-rw-r--   0 root         (0)     1003     5450 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8523 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       88 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.931397 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.935395 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/
--rw-rw-r--   0 root         (0)     1003      769 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/__init__.py
--rw-rw-r--   0 root         (0)     1003   126588 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/async_client.py
--rw-rw-r--   0 root         (0)     1003   140635 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/client.py
--rw-rw-r--   0 root         (0)     1003    37695 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.935395 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    25602 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/base.py
--rw-rw-r--   0 root         (0)     1003    49760 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    50867 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.939393 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/
--rw-rw-r--   0 root         (0)     1003     3776 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7695 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/asset.py
--rw-rw-r--   0 root         (0)     1003     2247 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/external_system.py
--rw-rw-r--   0 root         (0)     1003     9292 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/finding.py
--rw-rw-r--   0 root         (0)     1003     1339 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/folder.py
--rw-rw-r--   0 root         (0)     1003     1472 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/indicator.py
--rw-rw-r--   0 root         (0)     1003     3811 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/mute_config.py
--rw-rw-r--   0 root         (0)     1003     3921 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/notification_config.py
--rw-rw-r--   0 root         (0)     1003     1917 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/notification_message.py
--rw-rw-r--   0 root         (0)     1003     3652 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/organization_settings.py
--rw-rw-r--   0 root         (0)     1003     2467 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/resource.py
--rw-rw-r--   0 root         (0)     1003     1567 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/run_asset_discovery_response.py
--rw-rw-r--   0 root         (0)     1003     2857 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/security_marks.py
--rw-rw-r--   0 root         (0)     1003    63693 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/securitycenter_service.py
--rw-rw-r--   0 root         (0)     1003     2770 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/source.py
--rw-rw-r--   0 root         (0)     1003     7516 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/vulnerability.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.939393 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/
--rw-rw-r--   0 root         (0)     1003     3137 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5073 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       88 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.939393 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.939393 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/
--rw-rw-r--   0 root         (0)     1003      769 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/__init__.py
--rw-rw-r--   0 root         (0)     1003    78167 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/async_client.py
--rw-rw-r--   0 root         (0)     1003    87927 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/client.py
--rw-rw-r--   0 root         (0)     1003    26881 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.939393 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18201 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33481 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34252 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.943391 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2178 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5210 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/asset.py
--rw-rw-r--   0 root         (0)     1003     5363 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/finding.py
--rw-rw-r--   0 root         (0)     1003     3412 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/organization_settings.py
--rw-rw-r--   0 root         (0)     1003     1581 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/run_asset_discovery_response.py
--rw-rw-r--   0 root         (0)     1003     2219 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/security_marks.py
--rw-rw-r--   0 root         (0)     1003    32832 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/securitycenter_service.py
--rw-rw-r--   0 root         (0)     1003     2320 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/source.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.943391 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     4078 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6511 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       88 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.943391 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.943391 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/
--rw-rw-r--   0 root         (0)     1003      769 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/__init__.py
--rw-rw-r--   0 root         (0)     1003   102143 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/async_client.py
--rw-rw-r--   0 root         (0)     1003   113362 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/client.py
--rw-rw-r--   0 root         (0)     1003    32750 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.943391 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21965 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/base.py
--rw-rw-r--   0 root         (0)     1003    40357 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41247 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2873 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7765 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/asset.py
--rw-rw-r--   0 root         (0)     1003     6489 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/finding.py
--rw-rw-r--   0 root         (0)     1003     1346 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/folder.py
--rw-rw-r--   0 root         (0)     1003     4290 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/notification_config.py
--rw-rw-r--   0 root         (0)     1003     1943 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/notification_message.py
--rw-rw-r--   0 root         (0)     1003     3673 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/organization_settings.py
--rw-rw-r--   0 root         (0)     1003     2229 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/resource.py
--rw-rw-r--   0 root         (0)     1003     1585 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/run_asset_discovery_response.py
--rw-rw-r--   0 root         (0)     1003     2871 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/security_marks.py
--rw-rw-r--   0 root         (0)     1003    54054 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/securitycenter_service.py
--rw-rw-r--   0 root         (0)     1003     2762 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/source.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/
--rw-r--r--   0 root         (0)     1003     3957 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5587 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      119 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-01-18 16:08:05.000000 google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/scripts/
--rw-rw-r--   0 root         (0)     1003     8069 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/scripts/fixup_securitycenter_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     7209 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/scripts/fixup_securitycenter_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003     7592 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/scripts/fixup_securitycenter_v1p1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-01-18 16:08:05.951387 google-cloud-securitycenter-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2893 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.947389 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   372462 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1/test_security_center.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.951387 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   226403 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1beta1/test_security_center.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:05.951387 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   296631 2022-01-18 16:05:31.000000 google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1p1beta1/test_security_center.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.738988 google-cloud-securitycenter-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3957 2022-02-28 22:53:33.738988 google-cloud-securitycenter-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2994 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.714988 google-cloud-securitycenter-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.714988 google-cloud-securitycenter-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.718988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter/
+-rw-rw-r--   0 root         (0)     1003     7665 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter/__init__.py
+-rw-rw-r--   0 root         (0)     1003       88 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.718988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/
+-rw-rw-r--   0 root         (0)     1003     5554 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8523 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       88 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.718988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.722988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/
+-rw-rw-r--   0 root         (0)     1003      769 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/__init__.py
+-rw-rw-r--   0 root         (0)     1003   147503 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/async_client.py
+-rw-rw-r--   0 root         (0)     1003   161814 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/client.py
+-rw-rw-r--   0 root         (0)     1003    37695 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.722988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25602 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    49936 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    51043 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.726988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3862 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2266 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/access.py
+-rw-rw-r--   0 root         (0)     1003     7695 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/asset.py
+-rw-rw-r--   0 root         (0)     1003     2247 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/external_system.py
+-rw-rw-r--   0 root         (0)     1003     9929 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/finding.py
+-rw-rw-r--   0 root         (0)     1003     1339 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/folder.py
+-rw-rw-r--   0 root         (0)     1003     1472 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/indicator.py
+-rw-rw-r--   0 root         (0)     1003     3811 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/mute_config.py
+-rw-rw-r--   0 root         (0)     1003     3921 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/notification_config.py
+-rw-rw-r--   0 root         (0)     1003     1917 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/notification_message.py
+-rw-rw-r--   0 root         (0)     1003     3652 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/organization_settings.py
+-rw-rw-r--   0 root         (0)     1003     2435 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/resource.py
+-rw-rw-r--   0 root         (0)     1003     1567 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/run_asset_discovery_response.py
+-rw-rw-r--   0 root         (0)     1003     2857 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/security_marks.py
+-rw-rw-r--   0 root         (0)     1003    63710 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/securitycenter_service.py
+-rw-rw-r--   0 root         (0)     1003     2770 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/source.py
+-rw-rw-r--   0 root         (0)     1003     7489 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/vulnerability.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.726988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     3137 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5073 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       88 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.726988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.726988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/
+-rw-rw-r--   0 root         (0)     1003      769 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/__init__.py
+-rw-rw-r--   0 root         (0)     1003    91179 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/async_client.py
+-rw-rw-r--   0 root         (0)     1003   101203 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/client.py
+-rw-rw-r--   0 root         (0)     1003    26881 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.726988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18201 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33657 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34428 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.730988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2178 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5210 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/asset.py
+-rw-rw-r--   0 root         (0)     1003     5363 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/finding.py
+-rw-rw-r--   0 root         (0)     1003     3412 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/organization_settings.py
+-rw-rw-r--   0 root         (0)     1003     1581 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/run_asset_discovery_response.py
+-rw-rw-r--   0 root         (0)     1003     2219 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/security_marks.py
+-rw-rw-r--   0 root         (0)     1003    32832 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/securitycenter_service.py
+-rw-rw-r--   0 root         (0)     1003     2320 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/source.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.730988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     4078 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6511 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       88 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.730988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.730988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/
+-rw-rw-r--   0 root         (0)     1003      769 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/__init__.py
+-rw-rw-r--   0 root         (0)     1003   118393 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/async_client.py
+-rw-rw-r--   0 root         (0)     1003   129876 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/client.py
+-rw-rw-r--   0 root         (0)     1003    32750 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.730988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21965 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    40533 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41423 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2873 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7765 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/asset.py
+-rw-rw-r--   0 root         (0)     1003     6489 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/finding.py
+-rw-rw-r--   0 root         (0)     1003     1346 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/folder.py
+-rw-rw-r--   0 root         (0)     1003     4290 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/notification_config.py
+-rw-rw-r--   0 root         (0)     1003     1943 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/notification_message.py
+-rw-rw-r--   0 root         (0)     1003     3673 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/organization_settings.py
+-rw-rw-r--   0 root         (0)     1003     2229 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/resource.py
+-rw-rw-r--   0 root         (0)     1003     1585 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/run_asset_discovery_response.py
+-rw-rw-r--   0 root         (0)     1003     2871 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/security_marks.py
+-rw-rw-r--   0 root         (0)     1003    54054 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/securitycenter_service.py
+-rw-rw-r--   0 root         (0)     1003     2762 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/source.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/
+-rw-r--r--   0 root         (0)     1003     3957 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5634 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      119 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-02-28 22:53:33.000000 google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     8069 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/scripts/fixup_securitycenter_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     7209 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/scripts/fixup_securitycenter_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     7592 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/scripts/fixup_securitycenter_v1p1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-02-28 22:53:33.738988 google-cloud-securitycenter-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2893 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.734988 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   380552 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1/test_security_center.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.738988 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   234437 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1beta1/test_security_center.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-02-28 22:53:33.738988 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   304665 2022-02-28 22:50:43.000000 google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1p1beta1/test_security_center.py
```

### Comparing `google-cloud-securitycenter-1.8.0/LICENSE` & `google-cloud-securitycenter-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycenter-1.8.0/MANIFEST.in` & `google-cloud-securitycenter-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycenter-1.8.0/PKG-INFO` & `google-cloud-securitycenter-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-securitycenter
-Version: 1.8.0
+Version: 1.9.0
 Summary: Cloud Security Command Center API client library
 Home-page: https://github.com/googleapis/python-securitycenter
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-securitycenter-1.8.0/README.rst` & `google-cloud-securitycenter-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,14 +17,16 @@
 from google.cloud.securitycenter_v1.services.security_center.client import (
     SecurityCenterClient,
 )
 from google.cloud.securitycenter_v1.services.security_center.async_client import (
     SecurityCenterAsyncClient,
 )
 
+from google.cloud.securitycenter_v1.types.access import Access
+from google.cloud.securitycenter_v1.types.access import Geolocation
 from google.cloud.securitycenter_v1.types.asset import Asset
 from google.cloud.securitycenter_v1.types.external_system import ExternalSystem
 from google.cloud.securitycenter_v1.types.finding import Finding
 from google.cloud.securitycenter_v1.types.folder import Folder
 from google.cloud.securitycenter_v1.types.indicator import Indicator
 from google.cloud.securitycenter_v1.types.mute_config import MuteConfig
 from google.cloud.securitycenter_v1.types.notification_config import NotificationConfig
@@ -149,14 +151,16 @@
 from google.cloud.securitycenter_v1.types.vulnerability import Cvssv3
 from google.cloud.securitycenter_v1.types.vulnerability import Reference
 from google.cloud.securitycenter_v1.types.vulnerability import Vulnerability
 
 __all__ = (
     "SecurityCenterClient",
     "SecurityCenterAsyncClient",
+    "Access",
+    "Geolocation",
     "Asset",
     "ExternalSystem",
     "Finding",
     "Folder",
     "Indicator",
     "MuteConfig",
     "NotificationConfig",
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from .services.security_center import SecurityCenterClient
 from .services.security_center import SecurityCenterAsyncClient
 
+from .types.access import Access
+from .types.access import Geolocation
 from .types.asset import Asset
 from .types.external_system import ExternalSystem
 from .types.finding import Finding
 from .types.folder import Folder
 from .types.indicator import Indicator
 from .types.mute_config import MuteConfig
 from .types.notification_config import NotificationConfig
@@ -70,28 +72,30 @@
 from .types.vulnerability import Cve
 from .types.vulnerability import Cvssv3
 from .types.vulnerability import Reference
 from .types.vulnerability import Vulnerability
 
 __all__ = (
     "SecurityCenterAsyncClient",
+    "Access",
     "Asset",
     "BulkMuteFindingsRequest",
     "BulkMuteFindingsResponse",
     "CreateFindingRequest",
     "CreateMuteConfigRequest",
     "CreateNotificationConfigRequest",
     "CreateSourceRequest",
     "Cve",
     "Cvssv3",
     "DeleteMuteConfigRequest",
     "DeleteNotificationConfigRequest",
     "ExternalSystem",
     "Finding",
     "Folder",
+    "Geolocation",
     "GetMuteConfigRequest",
     "GetNotificationConfigRequest",
     "GetOrganizationSettingsRequest",
     "GetSourceRequest",
     "GroupAssetsRequest",
     "GroupAssetsResponse",
     "GroupFindingsRequest",
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/gapic_metadata.json` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/async_client.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/async_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Sequence, Tuple, Type, Union
+from typing import Dict, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -30,14 +30,15 @@
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.securitycenter_v1.services.security_center import pagers
+from google.cloud.securitycenter_v1.types import access
 from google.cloud.securitycenter_v1.types import external_system as gcs_external_system
 from google.cloud.securitycenter_v1.types import finding
 from google.cloud.securitycenter_v1.types import finding as gcs_finding
 from google.cloud.securitycenter_v1.types import indicator
 from google.cloud.securitycenter_v1.types import mute_config
 from google.cloud.securitycenter_v1.types import mute_config as gcs_mute_config
 from google.cloud.securitycenter_v1.types import notification_config
@@ -157,14 +158,50 @@
         Returns:
             SecurityCenterAsyncClient: The constructed client.
         """
         return SecurityCenterClient.from_service_account_file.__func__(SecurityCenterAsyncClient, filename, *args, **kwargs)  # type: ignore
 
     from_service_account_json = from_service_account_file
 
+    @classmethod
+    def get_mtls_endpoint_and_cert_source(
+        cls, client_options: Optional[ClientOptions] = None
+    ):
+        """Return the API endpoint and client cert source for mutual TLS.
+
+        The client cert source is determined in the following order:
+        (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
+        client cert source is None.
+        (2) if `client_options.client_cert_source` is provided, use the provided one; if the
+        default client cert source exists, use the default one; otherwise the client cert
+        source is None.
+
+        The API endpoint is determined in the following order:
+        (1) if `client_options.api_endpoint` if provided, use the provided one.
+        (2) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is "always", use the
+        default mTLS endpoint; if the environment variabel is "never", use the default API
+        endpoint; otherwise if client cert source exists, use the default mTLS endpoint, otherwise
+        use the default API endpoint.
+
+        More details can be found at https://google.aip.dev/auth/4114.
+
+        Args:
+            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+                client. Only the `api_endpoint` and `client_cert_source` properties may be used
+                in this method.
+
+        Returns:
+            Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
+                client cert source to use.
+
+        Raises:
+            google.auth.exceptions.MutualTLSChannelError: If any errors happen.
+        """
+        return SecurityCenterClient.get_mtls_endpoint_and_cert_source(client_options)  # type: ignore
+
     @property
     def transport(self) -> SecurityCenterTransport:
         """Returns the transport used by the client instance.
 
         Returns:
             SecurityCenterTransport: The transport used by the client instance.
         """
@@ -231,14 +268,38 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Kicks off an LRO to bulk mute findings for a parent
         based on a filter. The parent can be either an
         organization, folder or project. The findings matched by
         the filter will be muted after the LRO is done.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_bulk_mute_findings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.BulkMuteFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.bulk_mute_findings(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.BulkMuteFindingsRequest, dict]):
                 The request object. Request message for bulk findings
                 update.
                 Note:
                 1. If multiple bulk update requests match the same
                 resource, the order in which they get executed is not
@@ -267,15 +328,15 @@
                 The result type for the operation will be
                 :class:`google.cloud.securitycenter_v1.types.BulkMuteFindingsResponse`
                 The response to a BulkMute request. Contains the LRO
                 information.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -323,14 +384,33 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Creates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_source():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.CreateSourceRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                response = client.create_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.CreateSourceRequest, dict]):
                 The request object. Request message for creating a
                 source.
             parent (:class:`str`):
                 Required. Resource name of the new source's parent. Its
                 format should be "organizations/[organization_id]".
@@ -359,15 +439,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, and other tools.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -411,14 +491,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates a finding. The corresponding source must
         exist for finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_finding():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.CreateFindingRequest(
+                    parent="parent_value",
+                    finding_id="finding_id_value",
+                )
+
+                # Make the request
+                response = client.create_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.CreateFindingRequest, dict]):
                 The request object. Request message for creating a
                 finding.
             parent (:class:`str`):
                 Required. Resource name of the new finding's parent. Its
                 format should be
@@ -461,15 +562,15 @@
                 analysis, policy testing, and
                 enforcement. For example, a cross-site
                 scripting (XSS) vulnerability in an App
                 Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, finding_id, finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -514,14 +615,38 @@
         mute_config_id: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_mute_config.MuteConfig:
         r"""Creates a mute config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                mute_config = securitycenter_v1.MuteConfig()
+                mute_config.filter = "filter_value"
+
+                request = securitycenter_v1.CreateMuteConfigRequest(
+                    parent="parent_value",
+                    mute_config=mute_config,
+                    mute_config_id="mute_config_id_value",
+                )
+
+                # Make the request
+                response = client.create_mute_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.CreateMuteConfigRequest, dict]):
                 The request object. Request message for creating a mute
                 config.
             parent (:class:`str`):
                 Required. Resource name of the new mute configs's
                 parent. Its format is "organizations/[organization_id]",
@@ -558,15 +683,15 @@
             google.cloud.securitycenter_v1.types.MuteConfig:
                 A mute config is a Cloud SCC resource
                 that contains the configuration to mute
                 create/update events of findings.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, mute_config, mute_config_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -613,14 +738,34 @@
         notification_config: gcs_notification_config.NotificationConfig = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Creates a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.CreateNotificationConfigRequest(
+                    parent="parent_value",
+                    config_id="config_id_value",
+                )
+
+                # Make the request
+                response = client.create_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.CreateNotificationConfigRequest, dict]):
                 The request object. Request message for creating a
                 notification config.
             parent (:class:`str`):
                 Required. Resource name of the new notification config's
                 parent. Its format is "organizations/[organization_id]".
@@ -661,15 +806,15 @@
                 A notification config is a Cloud SCC
                 resource that contains the configuration
                 to send notifications for create/update
                 events of findings, assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, config_id, notification_config])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -712,14 +857,30 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes an existing mute config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_delete_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.DeleteMuteConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_mute_config(request=request)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.DeleteMuteConfigRequest, dict]):
                 The request object. Request message for deleting a mute
                 config.
             name (:class:`str`):
                 Required. Name of the mute config to delete. Its format
                 is organizations/{organization}/muteConfigs/{config_id},
@@ -732,15 +893,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -780,14 +941,30 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_delete_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.DeleteNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_notification_config(request=request)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.DeleteNotificationConfigRequest, dict]):
                 The request object. Request message for deleting a
                 notification config.
             name (:class:`str`):
                 Required. Name of the notification config to delete. Its
                 format is
@@ -799,15 +976,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -846,14 +1023,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_iam_policy():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.get_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
@@ -925,15 +1122,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -982,14 +1179,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> mute_config.MuteConfig:
         r"""Gets a mute config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetMuteConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_mute_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.GetMuteConfigRequest, dict]):
                 The request object. Request message for retrieving a
                 mute config.
             name (:class:`str`):
                 Required. Name of the mute config to retrieve. Its
                 format is
@@ -1010,15 +1226,15 @@
             google.cloud.securitycenter_v1.types.MuteConfig:
                 A mute config is a Cloud SCC resource
                 that contains the configuration to mute
                 create/update events of findings.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1059,14 +1275,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification_config.NotificationConfig:
         r"""Gets a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.GetNotificationConfigRequest, dict]):
                 The request object. Request message for getting a
                 notification config.
             name (:class:`str`):
                 Required. Name of the notification config to get. Its
                 format is
@@ -1088,15 +1323,15 @@
                 A notification config is a Cloud SCC
                 resource that contains the configuration
                 to send notifications for create/update
                 events of findings, assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1147,14 +1382,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> organization_settings.OrganizationSettings:
         r"""Gets the settings for an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_organization_settings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetOrganizationSettingsRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.GetOrganizationSettingsRequest, dict]):
                 The request object. Request message for getting
                 organization settings.
             name (:class:`str`):
                 Required. Name of the organization to get organization
                 settings for. Its format is
@@ -1173,15 +1427,15 @@
             google.cloud.securitycenter_v1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1230,14 +1484,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> source.Source:
         r"""Gets a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_source():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetSourceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.GetSourceRequest, dict]):
                 The request object. Request message for getting a
                 source.
             name (:class:`str`):
                 Required. Relative resource name of the source. Its
                 format is
@@ -1259,15 +1532,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, and other tools.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1316,14 +1589,36 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.GroupAssetsAsyncPager:
         r"""Filters an organization's assets and  groups them by
         their specified properties.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_group_assets():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GroupAssetsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.GroupAssetsRequest, dict]):
                 The request object. Request message for grouping by
                 assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1392,14 +1687,36 @@
         their specified properties.
 
         To group across all sources provide a ``-`` as the source id.
         Example: /v1/organizations/{organization_id}/sources/-/findings,
         /v1/folders/{folder_id}/sources/-/findings,
         /v1/projects/{project_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_group_findings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GroupFindingsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.GroupFindingsRequest, dict]):
                 The request object. Request message for grouping by
                 findings.
             parent (:class:`str`):
                 Required. Name of the source to groupBy. Its format is
                 "organizations/[organization_id]/sources/[source_id]",
@@ -1447,15 +1764,15 @@
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, group_by])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1511,14 +1828,34 @@
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAssetsAsyncPager:
         r"""Lists an organization's assets.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_assets():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListAssetsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.ListAssetsRequest, dict]):
                 The request object. Request message for listing assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -1580,14 +1917,35 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFindingsAsyncPager:
         r"""Lists an organization or source's findings.
 
         To list across all sources provide a ``-`` as the source id.
         Example: /v1/organizations/{organization_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_findings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.ListFindingsRequest, dict]):
                 The request object. Request message for listing
                 findings.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1649,14 +2007,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListMuteConfigsAsyncPager:
         r"""Lists mute configs.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_mute_configs():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListMuteConfigsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_mute_configs(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.ListMuteConfigsRequest, dict]):
                 The request object. Request message for listing  mute
                 configs at a given scope e.g. organization, folder or
                 project.
             parent (:class:`str`):
                 Required. The parent, which owns the collection of mute
@@ -1679,15 +2057,15 @@
                 configs.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1734,14 +2112,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationConfigsAsyncPager:
         r"""Lists notification configs.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_notification_configs():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListNotificationConfigsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_notification_configs(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.ListNotificationConfigsRequest, dict]):
                 The request object. Request message for listing
                 notification configs.
             parent (:class:`str`):
                 Required. Name of the organization to list notification
                 configs. Its format is
@@ -1762,15 +2160,15 @@
                 notification configs.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1825,14 +2223,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListSourcesAsyncPager:
         r"""Lists all sources belonging to an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_sources():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListSourcesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_sources(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.ListSourcesRequest, dict]):
                 The request object. Request message for listing sources.
             parent (:class:`str`):
                 Required. Resource name of the parent of sources to
                 list. Its format should be
                 "organizations/[organization_id], folders/[folder_id],
@@ -1852,15 +2270,15 @@
                 Response message for listing sources.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1920,14 +2338,38 @@
         r"""Runs asset discovery. The discovery is tracked with a
         long-running operation.
 
         This API can only be called with limited frequency for an
         organization. If it is called too frequently the caller will
         receive a TOO_MANY_REQUESTS error.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_run_asset_discovery():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.RunAssetDiscoveryRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.run_asset_discovery(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.RunAssetDiscoveryRequest, dict]):
                 The request object. Request message for running asset
                 discovery for an organization.
             parent (:class:`str`):
                 Required. Name of the organization to run asset
                 discovery for. Its format is
@@ -1948,15 +2390,15 @@
 
                 The result type for the operation will be
                 :class:`google.cloud.securitycenter_v1.types.RunAssetDiscoveryResponse`
                 Response of asset discovery run
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2005,14 +2447,34 @@
         start_time: timestamp_pb2.Timestamp = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_set_finding_state():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.SetFindingStateRequest(
+                    name="name_value",
+                    state="INACTIVE",
+                )
+
+                # Make the request
+                response = client.set_finding_state(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.SetFindingStateRequest, dict]):
                 The request object. Request message for updating a
                 finding's state.
             name (:class:`str`):
                 Required. The relative resource name of the finding.
                 See:
@@ -2053,15 +2515,15 @@
                 analysis, policy testing, and
                 enforcement. For example, a cross-site
                 scripting (XSS) vulnerability in an App
                 Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, state, start_time])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2105,14 +2567,34 @@
         mute: finding.Finding.Mute = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the mute state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_set_mute():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.SetMuteRequest(
+                    name="name_value",
+                    mute="UNDEFINED",
+                )
+
+                # Make the request
+                response = client.set_mute(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.SetMuteRequest, dict]):
                 The request object. Request message for updating a
                 finding's mute status.
             name (:class:`str`):
                 Required. The relative resource name of the finding.
                 See:
@@ -2148,15 +2630,15 @@
                 analysis, policy testing, and
                 enforcement. For example, a cross-site
                 scripting (XSS) vulnerability in an App
                 Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, mute])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2198,14 +2680,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_set_iam_policy():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.SetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.set_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
@@ -2277,15 +2779,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2326,14 +2828,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Returns the permissions that a caller has on the
         specified source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_test_iam_permissions():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.TestIamPermissionsRequest(
+                    resource="resource_value",
+                    permissions=['permissions_value_1', 'permissions_value_2'],
+                )
+
+                # Make the request
+                response = client.test_iam_permissions(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
@@ -2359,15 +2882,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.iam_policy_pb2.TestIamPermissionsResponse:
                 Response message for TestIamPermissions method.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource, permissions])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2419,14 +2942,32 @@
         update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_external_system.ExternalSystem:
         r"""Updates external system. This is for a given finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_external_system():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateExternalSystemRequest(
+                )
+
+                # Make the request
+                response = client.update_external_system(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateExternalSystemRequest, dict]):
                 The request object. Request message for updating a
                 ExternalSystem resource.
             external_system (:class:`google.cloud.securitycenter_v1.types.ExternalSystem`):
                 Required. The external system
                 resource to update.
@@ -2452,15 +2993,15 @@
         Returns:
             google.cloud.securitycenter_v1.types.ExternalSystem:
                 Representation of third party
                 SIEM/SOAR fields within SCC.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([external_system, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2504,14 +3045,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates or updates a finding. The corresponding
         source must exist for a finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_finding():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateFindingRequest(
+                )
+
+                # Make the request
+                response = client.update_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateFindingRequest, dict]):
                 The request object. Request message for updating or
                 creating a finding.
             finding (:class:`google.cloud.securitycenter_v1.types.Finding`):
                 Required. The finding resource to update or create if it
                 does not already exist. parent, security_marks, and
@@ -2540,15 +3100,15 @@
                 analysis, policy testing, and
                 enforcement. For example, a cross-site
                 scripting (XSS) vulnerability in an App
                 Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2590,14 +3150,36 @@
         update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_mute_config.MuteConfig:
         r"""Updates a mute config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                mute_config = securitycenter_v1.MuteConfig()
+                mute_config.filter = "filter_value"
+
+                request = securitycenter_v1.UpdateMuteConfigRequest(
+                    mute_config=mute_config,
+                )
+
+                # Make the request
+                response = client.update_mute_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateMuteConfigRequest, dict]):
                 The request object. Request message for updating a mute
                 config.
             mute_config (:class:`google.cloud.securitycenter_v1.types.MuteConfig`):
                 Required. The mute config being
                 updated.
@@ -2623,15 +3205,15 @@
             google.cloud.securitycenter_v1.types.MuteConfig:
                 A mute config is a Cloud SCC resource
                 that contains the configuration to mute
                 create/update events of findings.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([mute_config, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2678,14 +3260,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Updates a notification config. The following update fields are
         allowed: description, pubsub_topic, streaming_config.filter
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateNotificationConfigRequest(
+                )
+
+                # Make the request
+                response = client.update_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateNotificationConfigRequest, dict]):
                 The request object. Request message for updating a
                 notification config.
             notification_config (:class:`google.cloud.securitycenter_v1.types.NotificationConfig`):
                 Required. The notification config to
                 update.
@@ -2715,15 +3316,15 @@
                 A notification config is a Cloud SCC
                 resource that contains the configuration
                 to send notifications for create/update
                 events of findings, assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([notification_config, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2768,14 +3369,32 @@
         organization_settings: gcs_organization_settings.OrganizationSettings = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_organization_settings.OrganizationSettings:
         r"""Updates an organization's settings.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_organization_settings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateOrganizationSettingsRequest(
+                )
+
+                # Make the request
+                response = client.update_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateOrganizationSettingsRequest, dict]):
                 The request object. Request message for updating an
                 organization's settings.
             organization_settings (:class:`google.cloud.securitycenter_v1.types.OrganizationSettings`):
                 Required. The organization settings
                 resource to update.
@@ -2793,15 +3412,15 @@
             google.cloud.securitycenter_v1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([organization_settings])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2842,14 +3461,32 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Updates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_source():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateSourceRequest(
+                )
+
+                # Make the request
+                response = client.update_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateSourceRequest, dict]):
                 The request object. Request message for updating a
                 source.
             source (:class:`google.cloud.securitycenter_v1.types.Source`):
                 Required. The source resource to
                 update.
@@ -2870,15 +3507,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, and other tools.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2919,14 +3556,32 @@
         security_marks: gcs_security_marks.SecurityMarks = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_security_marks.SecurityMarks:
         r"""Updates security marks.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_security_marks():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateSecurityMarksRequest(
+                )
+
+                # Make the request
+                response = client.update_security_marks(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1.types.UpdateSecurityMarksRequest, dict]):
                 The request object. Request message for updating a
                 SecurityMarks resource.
             security_marks (:class:`google.cloud.securitycenter_v1.types.SecurityMarks`):
                 Required. The security marks resource
                 to update.
@@ -2949,15 +3604,15 @@
                 Center organization -- they can be
                 modified and viewed by all users who
                 have proper permissions on the
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([security_marks])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/client.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,36 +32,33 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
-from google.cloud.securitycenter_v1.services.security_center import pagers
-from google.cloud.securitycenter_v1.types import external_system as gcs_external_system
-from google.cloud.securitycenter_v1.types import finding
-from google.cloud.securitycenter_v1.types import finding as gcs_finding
-from google.cloud.securitycenter_v1.types import indicator
-from google.cloud.securitycenter_v1.types import mute_config
-from google.cloud.securitycenter_v1.types import mute_config as gcs_mute_config
-from google.cloud.securitycenter_v1.types import notification_config
-from google.cloud.securitycenter_v1.types import (
+from google.cloud.securitycenter_v1p1beta1.services.security_center import pagers
+from google.cloud.securitycenter_v1p1beta1.types import finding
+from google.cloud.securitycenter_v1p1beta1.types import finding as gcs_finding
+from google.cloud.securitycenter_v1p1beta1.types import notification_config
+from google.cloud.securitycenter_v1p1beta1.types import (
     notification_config as gcs_notification_config,
 )
-from google.cloud.securitycenter_v1.types import organization_settings
-from google.cloud.securitycenter_v1.types import (
+from google.cloud.securitycenter_v1p1beta1.types import organization_settings
+from google.cloud.securitycenter_v1p1beta1.types import (
     organization_settings as gcs_organization_settings,
 )
-from google.cloud.securitycenter_v1.types import run_asset_discovery_response
-from google.cloud.securitycenter_v1.types import security_marks
-from google.cloud.securitycenter_v1.types import security_marks as gcs_security_marks
-from google.cloud.securitycenter_v1.types import securitycenter_service
-from google.cloud.securitycenter_v1.types import source
-from google.cloud.securitycenter_v1.types import source as gcs_source
-from google.cloud.securitycenter_v1.types import vulnerability
+from google.cloud.securitycenter_v1p1beta1.types import run_asset_discovery_response
+from google.cloud.securitycenter_v1p1beta1.types import security_marks
+from google.cloud.securitycenter_v1p1beta1.types import (
+    security_marks as gcs_security_marks,
+)
+from google.cloud.securitycenter_v1p1beta1.types import securitycenter_service
+from google.cloud.securitycenter_v1p1beta1.types import source
+from google.cloud.securitycenter_v1p1beta1.types import source as gcs_source
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import SecurityCenterTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import SecurityCenterGrpcTransport
@@ -98,15 +95,15 @@
 
         # No transport is requested; return the default (that is, the first one
         # in the dictionary).
         return next(iter(cls._transport_registry.values()))
 
 
 class SecurityCenterClient(metaclass=SecurityCenterClientMeta):
-    """V1 APIs for Security Center service."""
+    """V1p1Beta1 APIs for Security Center service."""
 
     @staticmethod
     def _get_default_mtls_endpoint(api_endpoint):
         """Converts api endpoint to mTLS endpoint.
 
         Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
         "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
@@ -198,35 +195,14 @@
         """Parses a asset path into its component segments."""
         m = re.match(
             r"^organizations/(?P<organization>.+?)/assets/(?P<asset>.+?)$", path
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def external_system_path(
-        organization: str, source: str, finding: str, externalsystem: str,
-    ) -> str:
-        """Returns a fully-qualified external_system string."""
-        return "organizations/{organization}/sources/{source}/findings/{finding}/externalSystems/{externalsystem}".format(
-            organization=organization,
-            source=source,
-            finding=finding,
-            externalsystem=externalsystem,
-        )
-
-    @staticmethod
-    def parse_external_system_path(path: str) -> Dict[str, str]:
-        """Parses a external_system path into its component segments."""
-        m = re.match(
-            r"^organizations/(?P<organization>.+?)/sources/(?P<source>.+?)/findings/(?P<finding>.+?)/externalSystems/(?P<externalsystem>.+?)$",
-            path,
-        )
-        return m.groupdict() if m else {}
-
-    @staticmethod
     def finding_path(organization: str, source: str, finding: str,) -> str:
         """Returns a fully-qualified finding string."""
         return "organizations/{organization}/sources/{source}/findings/{finding}".format(
             organization=organization, source=source, finding=finding,
         )
 
     @staticmethod
@@ -235,30 +211,14 @@
         m = re.match(
             r"^organizations/(?P<organization>.+?)/sources/(?P<source>.+?)/findings/(?P<finding>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def mute_config_path(organization: str, mute_config: str,) -> str:
-        """Returns a fully-qualified mute_config string."""
-        return "organizations/{organization}/muteConfigs/{mute_config}".format(
-            organization=organization, mute_config=mute_config,
-        )
-
-    @staticmethod
-    def parse_mute_config_path(path: str) -> Dict[str, str]:
-        """Parses a mute_config path into its component segments."""
-        m = re.match(
-            r"^organizations/(?P<organization>.+?)/muteConfigs/(?P<mute_config>.+?)$",
-            path,
-        )
-        return m.groupdict() if m else {}
-
-    @staticmethod
     def notification_config_path(organization: str, notification_config: str,) -> str:
         """Returns a fully-qualified notification_config string."""
         return "organizations/{organization}/notificationConfigs/{notification_config}".format(
             organization=organization, notification_config=notification_config,
         )
 
     @staticmethod
@@ -382,14 +342,81 @@
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
 
+    @classmethod
+    def get_mtls_endpoint_and_cert_source(
+        cls, client_options: Optional[client_options_lib.ClientOptions] = None
+    ):
+        """Return the API endpoint and client cert source for mutual TLS.
+
+        The client cert source is determined in the following order:
+        (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
+        client cert source is None.
+        (2) if `client_options.client_cert_source` is provided, use the provided one; if the
+        default client cert source exists, use the default one; otherwise the client cert
+        source is None.
+
+        The API endpoint is determined in the following order:
+        (1) if `client_options.api_endpoint` if provided, use the provided one.
+        (2) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is "always", use the
+        default mTLS endpoint; if the environment variabel is "never", use the default API
+        endpoint; otherwise if client cert source exists, use the default mTLS endpoint, otherwise
+        use the default API endpoint.
+
+        More details can be found at https://google.aip.dev/auth/4114.
+
+        Args:
+            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+                client. Only the `api_endpoint` and `client_cert_source` properties may be used
+                in this method.
+
+        Returns:
+            Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
+                client cert source to use.
+
+        Raises:
+            google.auth.exceptions.MutualTLSChannelError: If any errors happen.
+        """
+        if client_options is None:
+            client_options = client_options_lib.ClientOptions()
+        use_client_cert = os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false")
+        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
+        if use_client_cert not in ("true", "false"):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        if use_mtls_endpoint not in ("auto", "never", "always"):
+            raise MutualTLSChannelError(
+                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
+            )
+
+        # Figure out the client cert source to use.
+        client_cert_source = None
+        if use_client_cert == "true":
+            if client_options.client_cert_source:
+                client_cert_source = client_options.client_cert_source
+            elif mtls.has_default_client_cert_source():
+                client_cert_source = mtls.default_client_cert_source()
+
+        # Figure out which api endpoint to use.
+        if client_options.api_endpoint is not None:
+            api_endpoint = client_options.api_endpoint
+        elif use_mtls_endpoint == "always" or (
+            use_mtls_endpoint == "auto" and client_cert_source
+        ):
+            api_endpoint = cls.DEFAULT_MTLS_ENDPOINT
+        else:
+            api_endpoint = cls.DEFAULT_ENDPOINT
+
+        return api_endpoint, client_cert_source
+
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, SecurityCenterTransport, None] = None,
         client_options: Optional[client_options_lib.ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
@@ -432,231 +459,130 @@
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
 
-        # Create SSL credentials for mutual TLS if needed.
-        if os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") not in (
-            "true",
-            "false",
-        ):
-            raise ValueError(
-                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
-            )
-        use_client_cert = (
-            os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") == "true"
+        api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
+            client_options
         )
 
-        client_cert_source_func = None
-        is_mtls = False
-        if use_client_cert:
-            if client_options.client_cert_source:
-                is_mtls = True
-                client_cert_source_func = client_options.client_cert_source
-            else:
-                is_mtls = mtls.has_default_client_cert_source()
-                if is_mtls:
-                    client_cert_source_func = mtls.default_client_cert_source()
-                else:
-                    client_cert_source_func = None
-
-        # Figure out which api endpoint to use.
-        if client_options.api_endpoint is not None:
-            api_endpoint = client_options.api_endpoint
-        else:
-            use_mtls_env = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
-            if use_mtls_env == "never":
-                api_endpoint = self.DEFAULT_ENDPOINT
-            elif use_mtls_env == "always":
-                api_endpoint = self.DEFAULT_MTLS_ENDPOINT
-            elif use_mtls_env == "auto":
-                if is_mtls:
-                    api_endpoint = self.DEFAULT_MTLS_ENDPOINT
-                else:
-                    api_endpoint = self.DEFAULT_ENDPOINT
-            else:
-                raise MutualTLSChannelError(
-                    "Unsupported GOOGLE_API_USE_MTLS_ENDPOINT value. Accepted "
-                    "values: never, auto, always"
-                )
+        api_key_value = getattr(client_options, "api_key", None)
+        if api_key_value and credentials:
+            raise ValueError(
+                "client_options.api_key and credentials are mutually exclusive"
+            )
 
         # Save or instantiate the transport.
         # Ordinarily, we provide the transport, but allowing a custom transport
         # instance provides an extensibility point for unusual situations.
         if isinstance(transport, SecurityCenterTransport):
             # transport is a SecurityCenterTransport instance.
-            if credentials or client_options.credentials_file:
+            if credentials or client_options.credentials_file or api_key_value:
                 raise ValueError(
                     "When providing a transport instance, "
                     "provide its credentials directly."
                 )
             if client_options.scopes:
                 raise ValueError(
                     "When providing a transport instance, provide its scopes "
                     "directly."
                 )
             self._transport = transport
         else:
+            import google.auth._default  # type: ignore
+
+            if api_key_value and hasattr(
+                google.auth._default, "get_api_key_credentials"
+            ):
+                credentials = google.auth._default.get_api_key_credentials(
+                    api_key_value
+                )
+
             Transport = type(self).get_transport_class(transport)
             self._transport = Transport(
                 credentials=credentials,
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
                 always_use_jwt_access=True,
             )
 
-    def bulk_mute_findings(
+    def create_source(
         self,
-        request: Union[securitycenter_service.BulkMuteFindingsRequest, dict] = None,
+        request: Union[securitycenter_service.CreateSourceRequest, dict] = None,
         *,
         parent: str = None,
+        source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> operation.Operation:
-        r"""Kicks off an LRO to bulk mute findings for a parent
-        based on a filter. The parent can be either an
-        organization, folder or project. The findings matched by
-        the filter will be muted after the LRO is done.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.BulkMuteFindingsRequest, dict]):
-                The request object. Request message for bulk findings
-                update.
-                Note:
-                1. If multiple bulk update requests match the same
-                resource, the order in which they get executed is not
-                defined.
-                2. Once a bulk operation is started, there is no way to
-                stop it.
-            parent (str):
-                Required. The parent, at which bulk action needs to be
-                applied. Its format is
-                "organizations/[organization_id]",
-                "folders/[folder_id]", "projects/[project_id]".
-
-                This corresponds to the ``parent`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.api_core.operation.Operation:
-                An object representing a long-running operation.
-
-                The result type for the operation will be
-                :class:`google.cloud.securitycenter_v1.types.BulkMuteFindingsResponse`
-                The response to a BulkMute request. Contains the LRO
-                information.
-
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([parent])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.BulkMuteFindingsRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.BulkMuteFindingsRequest):
-            request = securitycenter_service.BulkMuteFindingsRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
+    ) -> gcs_source.Source:
+        r"""Creates a source.
 
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.bulk_mute_findings]
+        .. code-block:: python
 
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+            from google.cloud import securitycenter_v1p1beta1
 
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+            def sample_create_source():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
 
-        # Wrap the response in an operation future.
-        response = operation.from_gapic(
-            response,
-            self._transport.operations_client,
-            securitycenter_service.BulkMuteFindingsResponse,
-            metadata_type=empty_pb2.Empty,
-        )
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.CreateSourceRequest(
+                    parent="parent_value",
+                )
 
-        # Done; return the response.
-        return response
+                # Make the request
+                response = client.create_source(request=request)
 
-    def create_source(
-        self,
-        request: Union[securitycenter_service.CreateSourceRequest, dict] = None,
-        *,
-        parent: str = None,
-        source: gcs_source.Source = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> gcs_source.Source:
-        r"""Creates a source.
+                # Handle the response
+                print(response)
 
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.CreateSourceRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateSourceRequest, dict]):
                 The request object. Request message for creating a
                 source.
             parent (str):
                 Required. Resource name of the new source's parent. Its
                 format should be "organizations/[organization_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            source (google.cloud.securitycenter_v1.types.Source):
+            source (google.cloud.securitycenter_v1p1beta1.types.Source):
                 Required. The Source being created, only the
                 display_name and description will be used. All other
                 fields will be ignored.
 
                 This corresponds to the ``source`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.Source:
+            google.cloud.securitycenter_v1p1beta1.types.Source:
                 Security Command Center finding
                 source. A finding source is an entity or
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
-                monitor, and other tools.
+                monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -700,65 +626,83 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates a finding. The corresponding source must
         exist for finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_create_finding():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.CreateFindingRequest(
+                    parent="parent_value",
+                    finding_id="finding_id_value",
+                )
+
+                # Make the request
+                response = client.create_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.CreateFindingRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateFindingRequest, dict]):
                 The request object. Request message for creating a
                 finding.
             parent (str):
                 Required. Resource name of the new finding's parent. Its
                 format should be
                 "organizations/[organization_id]/sources/[source_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             finding_id (str):
                 Required. Unique identifier provided
                 by the client within the parent scope.
-                It must be alphanumeric and less than or
-                equal to 32 characters and greater than
-                0 characters in length.
 
                 This corresponds to the ``finding_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            finding (google.cloud.securitycenter_v1.types.Finding):
+            finding (google.cloud.securitycenter_v1p1beta1.types.Finding):
                 Required. The Finding being created. The name and
                 security_marks will be ignored as they are both output
                 only fields on this resource.
 
                 This corresponds to the ``finding`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.Finding:
+            google.cloud.securitycenter_v1p1beta1.types.Finding:
                 Security Command Center finding.
                 A finding is a record of assessment data
-                like security, risk, health, or privacy,
-                that is ingested into Security Command
-                Center for presentation, notification,
+                (security, risk, health or privacy)
+                ingested into Security Command Center
+                for presentation, notification,
                 analysis, policy testing, and
-                enforcement. For example, a cross-site
-                scripting (XSS) vulnerability in an App
-                Engine application is a finding.
+                enforcement. For example, an XSS
+                vulnerability in an App Engine
+                application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, finding_id, finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -790,111 +734,14 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
-    def create_mute_config(
-        self,
-        request: Union[securitycenter_service.CreateMuteConfigRequest, dict] = None,
-        *,
-        parent: str = None,
-        mute_config: gcs_mute_config.MuteConfig = None,
-        mute_config_id: str = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> gcs_mute_config.MuteConfig:
-        r"""Creates a mute config.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.CreateMuteConfigRequest, dict]):
-                The request object. Request message for creating a mute
-                config.
-            parent (str):
-                Required. Resource name of the new mute configs's
-                parent. Its format is "organizations/[organization_id]",
-                "folders/[folder_id]", or "projects/[project_id]".
-
-                This corresponds to the ``parent`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            mute_config (google.cloud.securitycenter_v1.types.MuteConfig):
-                Required. The mute config being
-                created.
-
-                This corresponds to the ``mute_config`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            mute_config_id (str):
-                Required. Unique identifier provided
-                by the client within the parent scope.
-                It must consist of lower case letters,
-                numbers, and hyphen, with the first
-                character a letter, the last a letter or
-                a number, and a 63 character maximum.
-
-                This corresponds to the ``mute_config_id`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.cloud.securitycenter_v1.types.MuteConfig:
-                A mute config is a Cloud SCC resource
-                that contains the configuration to mute
-                create/update events of findings.
-
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([parent, mute_config, mute_config_id])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.CreateMuteConfigRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.CreateMuteConfigRequest):
-            request = securitycenter_service.CreateMuteConfigRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
-            if mute_config is not None:
-                request.mute_config = mute_config
-            if mute_config_id is not None:
-                request.mute_config_id = mute_config_id
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.create_mute_config]
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
-
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
-
-        # Done; return the response.
-        return response
-
     def create_notification_config(
         self,
         request: Union[
             securitycenter_service.CreateNotificationConfigRequest, dict
         ] = None,
         *,
         parent: str = None,
@@ -902,37 +749,56 @@
         notification_config: gcs_notification_config.NotificationConfig = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Creates a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_create_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.CreateNotificationConfigRequest(
+                    parent="parent_value",
+                    config_id="config_id_value",
+                )
+
+                # Make the request
+                response = client.create_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.CreateNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateNotificationConfigRequest, dict]):
                 The request object. Request message for creating a
                 notification config.
             parent (str):
                 Required. Resource name of the new notification config's
                 parent. Its format is "organizations/[organization_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             config_id (str):
-                Required.
-                Unique identifier provided by the client
-                within the parent scope. It must be
-                between 1 and 128 characters, and
-                contains alphanumeric characters,
+                Required. Unique identifier provided
+                by the client within the parent scope.
+                It must be between 1 and 128 characters,
+                and contains alphanumeric characters,
                 underscores or hyphens only.
 
                 This corresponds to the ``config_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            notification_config (google.cloud.securitycenter_v1.types.NotificationConfig):
+            notification_config (google.cloud.securitycenter_v1p1beta1.types.NotificationConfig):
                 Required. The notification config
                 being created. The name and the service
                 account will be ignored as they are both
                 output only fields on this resource.
 
                 This corresponds to the ``notification_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -940,25 +806,26 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.NotificationConfig:
-                Cloud Security Command Center (Cloud
-                SCC) notification configs.
-                A notification config is a Cloud SCC
-                resource that contains the configuration
-                to send notifications for create/update
-                events of findings, assets and etc.
+            google.cloud.securitycenter_v1p1beta1.types.NotificationConfig:
+                Security Command Center notification
+                configs.
+                A notification config is a Security
+                Command Center resource that contains
+                the configuration to send notifications
+                for create/update events of findings,
+                assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, config_id, notification_config])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -994,95 +861,45 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
-    def delete_mute_config(
-        self,
-        request: Union[securitycenter_service.DeleteMuteConfigRequest, dict] = None,
-        *,
-        name: str = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> None:
-        r"""Deletes an existing mute config.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.DeleteMuteConfigRequest, dict]):
-                The request object. Request message for deleting a mute
-                config.
-            name (str):
-                Required. Name of the mute config to delete. Its format
-                is organizations/{organization}/muteConfigs/{config_id},
-                folders/{folder}/muteConfigs/{config_id}, or
-                projects/{project}/muteConfigs/{config_id}
-
-                This corresponds to the ``name`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([name])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.DeleteMuteConfigRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.DeleteMuteConfigRequest):
-            request = securitycenter_service.DeleteMuteConfigRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if name is not None:
-                request.name = name
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.delete_mute_config]
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
-        )
-
     def delete_notification_config(
         self,
         request: Union[
             securitycenter_service.DeleteNotificationConfigRequest, dict
         ] = None,
         *,
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_delete_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.DeleteNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_notification_config(request=request)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.DeleteNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.DeleteNotificationConfigRequest, dict]):
                 The request object. Request message for deleting a
                 notification config.
             name (str):
                 Required. Name of the notification config to delete. Its
                 format is
                 "organizations/[organization_id]/notificationConfigs/[config_id]".
 
@@ -1092,15 +909,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1143,14 +960,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_iam_policy():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.get_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
@@ -1222,15 +1059,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1257,104 +1094,48 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
-    def get_mute_config(
-        self,
-        request: Union[securitycenter_service.GetMuteConfigRequest, dict] = None,
-        *,
-        name: str = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> mute_config.MuteConfig:
-        r"""Gets a mute config.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.GetMuteConfigRequest, dict]):
-                The request object. Request message for retrieving a
-                mute config.
-            name (str):
-                Required. Name of the mute config to retrieve. Its
-                format is
-                organizations/{organization}/muteConfigs/{config_id},
-                folders/{folder}/muteConfigs/{config_id}, or
-                projects/{project}/muteConfigs/{config_id}
-
-                This corresponds to the ``name`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.cloud.securitycenter_v1.types.MuteConfig:
-                A mute config is a Cloud SCC resource
-                that contains the configuration to mute
-                create/update events of findings.
-
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([name])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.GetMuteConfigRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.GetMuteConfigRequest):
-            request = securitycenter_service.GetMuteConfigRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if name is not None:
-                request.name = name
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.get_mute_config]
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
-
-        # Done; return the response.
-        return response
-
     def get_notification_config(
         self,
         request: Union[
             securitycenter_service.GetNotificationConfigRequest, dict
         ] = None,
         *,
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification_config.NotificationConfig:
         r"""Gets a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.GetNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.GetNotificationConfigRequest, dict]):
                 The request object. Request message for getting a
                 notification config.
             name (str):
                 Required. Name of the notification config to get. Its
                 format is
                 "organizations/[organization_id]/notificationConfigs/[config_id]".
 
@@ -1364,25 +1145,26 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.NotificationConfig:
-                Cloud Security Command Center (Cloud
-                SCC) notification configs.
-                A notification config is a Cloud SCC
-                resource that contains the configuration
-                to send notifications for create/update
-                events of findings, assets and etc.
+            google.cloud.securitycenter_v1p1beta1.types.NotificationConfig:
+                Security Command Center notification
+                configs.
+                A notification config is a Security
+                Command Center resource that contains
+                the configuration to send notifications
+                for create/update events of findings,
+                assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1423,16 +1205,35 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> organization_settings.OrganizationSettings:
         r"""Gets the settings for an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_organization_settings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetOrganizationSettingsRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.GetOrganizationSettingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.GetOrganizationSettingsRequest, dict]):
                 The request object. Request message for getting
                 organization settings.
             name (str):
                 Required. Name of the organization to get organization
                 settings for. Its format is
                 "organizations/[organization_id]/organizationSettings".
 
@@ -1442,22 +1243,22 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.OrganizationSettings:
+            google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1500,16 +1301,35 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> source.Source:
         r"""Gets a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_source():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetSourceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.GetSourceRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.GetSourceRequest, dict]):
                 The request object. Request message for getting a
                 source.
             name (str):
                 Required. Relative resource name of the source. Its
                 format is
                 "organizations/[organization_id]/source/[source_id]".
 
@@ -1519,25 +1339,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.Source:
+            google.cloud.securitycenter_v1p1beta1.types.Source:
                 Security Command Center finding
                 source. A finding source is an entity or
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
-                monitor, and other tools.
+                monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1576,26 +1396,48 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.GroupAssetsPager:
         r"""Filters an organization's assets and  groups them by
         their specified properties.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_group_assets():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GroupAssetsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.GroupAssetsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.GroupAssetsRequest, dict]):
                 The request object. Request message for grouping by
                 assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.GroupAssetsPager:
+            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.GroupAssetsPager:
                 Response message for grouping by
                 assets.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1643,16 +1485,38 @@
         their specified properties.
 
         To group across all sources provide a ``-`` as the source id.
         Example: /v1/organizations/{organization_id}/sources/-/findings,
         /v1/folders/{folder_id}/sources/-/findings,
         /v1/projects/{project_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_group_findings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GroupFindingsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.GroupFindingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.GroupFindingsRequest, dict]):
                 The request object. Request message for grouping by
                 findings.
             parent (str):
                 Required. Name of the source to groupBy. Its format is
                 "organizations/[organization_id]/sources/[source_id]",
                 folders/[folder_id]/sources/[source_id], or
                 projects/[project_id]/sources/[source_id]. To groupBy
@@ -1689,24 +1553,24 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.GroupFindingsPager:
+            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.GroupFindingsPager:
                 Response message for group by
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, group_by])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1746,44 +1610,86 @@
         # Done; return the response.
         return response
 
     def list_assets(
         self,
         request: Union[securitycenter_service.ListAssetsRequest, dict] = None,
         *,
+        parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAssetsPager:
         r"""Lists an organization's assets.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_assets():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListAssetsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.ListAssetsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListAssetsRequest, dict]):
                 The request object. Request message for listing assets.
+            parent (str):
+                Required. Name of the organization assets should belong
+                to. Its format is "organizations/[organization_id],
+                folders/[folder_id], or projects/[project_id]".
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.ListAssetsPager:
+            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListAssetsPager:
                 Response message for listing assets.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
         # Minor optimization to avoid making a copy if the user passes
         # in a securitycenter_service.ListAssetsRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.ListAssetsRequest):
             request = securitycenter_service.ListAssetsRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.list_assets]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -1803,149 +1709,116 @@
         # Done; return the response.
         return response
 
     def list_findings(
         self,
         request: Union[securitycenter_service.ListFindingsRequest, dict] = None,
         *,
+        parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFindingsPager:
         r"""Lists an organization or source's findings.
 
         To list across all sources provide a ``-`` as the source id.
-        Example: /v1/organizations/{organization_id}/sources/-/findings
+        Example:
+        /v1p1beta1/organizations/{organization_id}/sources/-/findings
 
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.ListFindingsRequest, dict]):
-                The request object. Request message for listing
-                findings.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
 
-        Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.ListFindingsPager:
-                Response message for listing
-                findings.
-                Iterating over this object will yield
-                results and resolve additional pages
-                automatically.
+        .. code-block:: python
 
-        """
-        # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.ListFindingsRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.ListFindingsRequest):
-            request = securitycenter_service.ListFindingsRequest(request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.list_findings]
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+            from google.cloud import securitycenter_v1p1beta1
 
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+            def sample_list_findings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
 
-        # This method is paged; wrap the response in a pager, which provides
-        # an `__iter__` convenience method.
-        response = pagers.ListFindingsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
-        )
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListFindingsRequest(
+                    parent="parent_value",
+                )
 
-        # Done; return the response.
-        return response
+                # Make the request
+                page_result = client.list_findings(request=request)
 
-    def list_mute_configs(
-        self,
-        request: Union[securitycenter_service.ListMuteConfigsRequest, dict] = None,
-        *,
-        parent: str = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.ListMuteConfigsPager:
-        r"""Lists mute configs.
+                # Handle the response
+                for response in page_result:
+                    print(response)
 
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.ListMuteConfigsRequest, dict]):
-                The request object. Request message for listing  mute
-                configs at a given scope e.g. organization, folder or
-                project.
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListFindingsRequest, dict]):
+                The request object. Request message for listing
+                findings.
             parent (str):
-                Required. The parent, which owns the collection of mute
-                configs. Its format is
-                "organizations/[organization_id]",
-                "folders/[folder_id]", "projects/[project_id]".
+                Required. Name of the source the findings belong to. Its
+                format is
+                "organizations/[organization_id]/sources/[source_id],
+                folders/[folder_id]/sources/[source_id], or
+                projects/[project_id]/sources/[source_id]". To list
+                across all sources provide a source_id of ``-``. For
+                example: organizations/{organization_id}/sources/-,
+                folders/{folder_id}/sources/- or
+                projects/{projects_id}/sources/-
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.ListMuteConfigsPager:
-                Response message for listing mute
-                configs.
+            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListFindingsPager:
+                Response message for listing
+                findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.ListMuteConfigsRequest.
+        # in a securitycenter_service.ListFindingsRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.ListMuteConfigsRequest):
-            request = securitycenter_service.ListMuteConfigsRequest(request)
+        if not isinstance(request, securitycenter_service.ListFindingsRequest):
+            request = securitycenter_service.ListFindingsRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.list_mute_configs]
+        rpc = self._transport._wrapped_methods[self._transport.list_findings]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
-        response = pagers.ListMuteConfigsPager(
+        response = pagers.ListFindingsPager(
             method=rpc, request=request, response=response, metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def list_notification_configs(
@@ -1957,16 +1830,36 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationConfigsPager:
         r"""Lists notification configs.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_notification_configs():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListNotificationConfigsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_notification_configs(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.ListNotificationConfigsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListNotificationConfigsRequest, dict]):
                 The request object. Request message for listing
                 notification configs.
             parent (str):
                 Required. Name of the organization to list notification
                 configs. Its format is
                 "organizations/[organization_id]".
 
@@ -1976,24 +1869,24 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.ListNotificationConfigsPager:
+            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListNotificationConfigsPager:
                 Response message for listing
                 notification configs.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2042,16 +1935,36 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListSourcesPager:
         r"""Lists all sources belonging to an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_sources():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListSourcesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_sources(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.ListSourcesRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListSourcesRequest, dict]):
                 The request object. Request message for listing sources.
             parent (str):
                 Required. Resource name of the parent of sources to
                 list. Its format should be
                 "organizations/[organization_id], folders/[folder_id],
                 or projects/[project_id]".
 
@@ -2061,23 +1974,23 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.services.security_center.pagers.ListSourcesPager:
+            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListSourcesPager:
                 Response message for listing sources.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2127,16 +2040,40 @@
         r"""Runs asset discovery. The discovery is tracked with a
         long-running operation.
 
         This API can only be called with limited frequency for an
         organization. If it is called too frequently the caller will
         receive a TOO_MANY_REQUESTS error.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_run_asset_discovery():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.RunAssetDiscoveryRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.run_asset_discovery(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.RunAssetDiscoveryRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.RunAssetDiscoveryRequest, dict]):
                 The request object. Request message for running asset
                 discovery for an organization.
             parent (str):
                 Required. Name of the organization to run asset
                 discovery for. Its format is
                 "organizations/[organization_id]".
 
@@ -2150,20 +2087,20 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.securitycenter_v1.types.RunAssetDiscoveryResponse`
+                :class:`google.cloud.securitycenter_v1p1beta1.types.RunAssetDiscoveryResponse`
                 Response of asset discovery run
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2212,29 +2149,49 @@
         start_time: timestamp_pb2.Timestamp = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_set_finding_state():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.SetFindingStateRequest(
+                    name="name_value",
+                    state="INACTIVE",
+                )
+
+                # Make the request
+                response = client.set_finding_state(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.SetFindingStateRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.SetFindingStateRequest, dict]):
                 The request object. Request message for updating a
                 finding's state.
             name (str):
                 Required. The relative resource name of the finding.
                 See:
                 https://cloud.google.com/apis/design/resource_names#relative_resource_name
                 Example:
                 "organizations/{organization_id}/sources/{source_id}/finding/{finding_id}".
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state (google.cloud.securitycenter_v1.types.Finding.State):
+            state (google.cloud.securitycenter_v1p1beta1.types.Finding.State):
                 Required. The desired State of the
                 finding.
 
                 This corresponds to the ``state`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             start_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -2247,28 +2204,28 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.Finding:
+            google.cloud.securitycenter_v1p1beta1.types.Finding:
                 Security Command Center finding.
                 A finding is a record of assessment data
-                like security, risk, health, or privacy,
-                that is ingested into Security Command
-                Center for presentation, notification,
+                (security, risk, health or privacy)
+                ingested into Security Command Center
+                for presentation, notification,
                 analysis, policy testing, and
-                enforcement. For example, a cross-site
-                scripting (XSS) vulnerability in an App
-                Engine application is a finding.
+                enforcement. For example, an XSS
+                vulnerability in an App Engine
+                application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, state, start_time])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2300,118 +2257,45 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
-    def set_mute(
+    def set_iam_policy(
         self,
-        request: Union[securitycenter_service.SetMuteRequest, dict] = None,
+        request: Union[iam_policy_pb2.SetIamPolicyRequest, dict] = None,
         *,
-        name: str = None,
-        mute: finding.Finding.Mute = None,
+        resource: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> finding.Finding:
-        r"""Updates the mute state of a finding.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.SetMuteRequest, dict]):
-                The request object. Request message for updating a
-                finding's mute status.
-            name (str):
-                Required. The relative resource name of the finding.
-                See:
-                https://cloud.google.com/apis/design/resource_names#relative_resource_name
-                Example:
-                "organizations/{organization_id}/sources/{source_id}/finding/{finding_id}",
-                "folders/{folder_id}/sources/{source_id}/finding/{finding_id}",
-                "projects/{project_id}/sources/{source_id}/finding/{finding_id}".
-
-                This corresponds to the ``name`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            mute (google.cloud.securitycenter_v1.types.Finding.Mute):
-                Required. The desired state of the
-                Mute.
-
-                This corresponds to the ``mute`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.cloud.securitycenter_v1.types.Finding:
-                Security Command Center finding.
-                A finding is a record of assessment data
-                like security, risk, health, or privacy,
-                that is ingested into Security Command
-                Center for presentation, notification,
-                analysis, policy testing, and
-                enforcement. For example, a cross-site
-                scripting (XSS) vulnerability in an App
-                Engine application is a finding.
+    ) -> policy_pb2.Policy:
+        r"""Sets the access control policy on the specified
+        Source.
 
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([name, mute])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.SetMuteRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.SetMuteRequest):
-            request = securitycenter_service.SetMuteRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if name is not None:
-                request.name = name
-            if mute is not None:
-                request.mute = mute
+        .. code-block:: python
 
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.set_mute]
+            from google.cloud import securitycenter_v1p1beta1
 
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
+            def sample_set_iam_policy():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
 
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.SetIamPolicyRequest(
+                    resource="resource_value",
+                )
 
-        # Done; return the response.
-        return response
+                # Make the request
+                response = client.set_iam_policy(request=request)
 
-    def set_iam_policy(
-        self,
-        request: Union[iam_policy_pb2.SetIamPolicyRequest, dict] = None,
-        *,
-        resource: str = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> policy_pb2.Policy:
-        r"""Sets the access control policy on the specified
-        Source.
+                # Handle the response
+                print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             resource (str):
                 REQUIRED: The resource for which the
@@ -2484,15 +2368,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2532,14 +2416,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Returns the permissions that a caller has on the
         specified source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_test_iam_permissions():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.TestIamPermissionsRequest(
+                    resource="resource_value",
+                    permissions=['permissions_value_1', 'permissions_value_2'],
+                )
+
+                # Make the request
+                response = client.test_iam_permissions(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
@@ -2565,15 +2470,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.iam_policy_pb2.TestIamPermissionsResponse:
                 Response message for TestIamPermissions method.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource, permissions])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2602,150 +2507,99 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
-    def update_external_system(
+    def update_finding(
         self,
-        request: Union[securitycenter_service.UpdateExternalSystemRequest, dict] = None,
+        request: Union[securitycenter_service.UpdateFindingRequest, dict] = None,
         *,
-        external_system: gcs_external_system.ExternalSystem = None,
+        finding: gcs_finding.Finding = None,
         update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> gcs_external_system.ExternalSystem:
-        r"""Updates external system. This is for a given finding.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateExternalSystemRequest, dict]):
-                The request object. Request message for updating a
-                ExternalSystem resource.
-            external_system (google.cloud.securitycenter_v1.types.ExternalSystem):
-                Required. The external system
-                resource to update.
-
-                This corresponds to the ``external_system`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
-                The FieldMask to use when updating
-                the external system resource.
-                If empty all mutable fields will be
-                updated.
-
-                This corresponds to the ``update_mask`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
+    ) -> gcs_finding.Finding:
+        r"""Creates or updates a finding. The corresponding
+        source must exist for a finding creation to succeed.
 
-        Returns:
-            google.cloud.securitycenter_v1.types.ExternalSystem:
-                Representation of third party
-                SIEM/SOAR fields within SCC.
 
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([external_system, update_mask])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
+        .. code-block:: python
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.UpdateExternalSystemRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.UpdateExternalSystemRequest):
-            request = securitycenter_service.UpdateExternalSystemRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if external_system is not None:
-                request.external_system = external_system
-            if update_mask is not None:
-                request.update_mask = update_mask
+            from google.cloud import securitycenter_v1p1beta1
 
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.update_external_system]
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata(
-                (("external_system.name", request.external_system.name),)
-            ),
-        )
+            def sample_update_finding():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
 
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateFindingRequest(
+                )
 
-        # Done; return the response.
-        return response
+                # Make the request
+                response = client.update_finding(request=request)
 
-    def update_finding(
-        self,
-        request: Union[securitycenter_service.UpdateFindingRequest, dict] = None,
-        *,
-        finding: gcs_finding.Finding = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> gcs_finding.Finding:
-        r"""Creates or updates a finding. The corresponding
-        source must exist for a finding creation to succeed.
+                # Handle the response
+                print(response)
 
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateFindingRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateFindingRequest, dict]):
                 The request object. Request message for updating or
                 creating a finding.
-            finding (google.cloud.securitycenter_v1.types.Finding):
+            finding (google.cloud.securitycenter_v1p1beta1.types.Finding):
                 Required. The finding resource to update or create if it
                 does not already exist. parent, security_marks, and
                 update_time will be ignored.
 
                 In the case of creation, the finding id portion of the
                 name must be alphanumeric and less than or equal to 32
                 characters and greater than 0 characters in length.
 
                 This corresponds to the ``finding`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                The FieldMask to use when updating the finding resource.
+                This field should not be specified when creating a
+                finding.
+
+                When updating a finding, an empty mask is treated as
+                updating all mutable fields and replacing
+                source_properties. Individual source_properties can be
+                added/updated by using "source_properties." in the field
+                mask.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.Finding:
+            google.cloud.securitycenter_v1p1beta1.types.Finding:
                 Security Command Center finding.
                 A finding is a record of assessment data
-                like security, risk, health, or privacy,
-                that is ingested into Security Command
-                Center for presentation, notification,
+                (security, risk, health or privacy)
+                ingested into Security Command Center
+                for presentation, notification,
                 analysis, policy testing, and
-                enforcement. For example, a cross-site
-                scripting (XSS) vulnerability in an App
-                Engine application is a finding.
+                enforcement. For example, an XSS
+                vulnerability in an App Engine
+                application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([finding])
+        has_flattened_params = any([finding, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
@@ -2754,109 +2608,26 @@
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.UpdateFindingRequest):
             request = securitycenter_service.UpdateFindingRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if finding is not None:
                 request.finding = finding
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.update_finding]
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata(
-                (("finding.name", request.finding.name),)
-            ),
-        )
-
-        # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
-
-        # Done; return the response.
-        return response
-
-    def update_mute_config(
-        self,
-        request: Union[securitycenter_service.UpdateMuteConfigRequest, dict] = None,
-        *,
-        mute_config: gcs_mute_config.MuteConfig = None,
-        update_mask: field_mask_pb2.FieldMask = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> gcs_mute_config.MuteConfig:
-        r"""Updates a mute config.
-
-        Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateMuteConfigRequest, dict]):
-                The request object. Request message for updating a mute
-                config.
-            mute_config (google.cloud.securitycenter_v1.types.MuteConfig):
-                Required. The mute config being
-                updated.
-
-                This corresponds to the ``mute_config`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
-                The list of fields to be updated.
-                If empty all mutable fields will be
-                updated.
-
-                This corresponds to the ``update_mask`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.cloud.securitycenter_v1.types.MuteConfig:
-                A mute config is a Cloud SCC resource
-                that contains the configuration to mute
-                create/update events of findings.
-
-        """
-        # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([mute_config, update_mask])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
-        # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.UpdateMuteConfigRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.UpdateMuteConfigRequest):
-            request = securitycenter_service.UpdateMuteConfigRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if mute_config is not None:
-                request.mute_config = mute_config
             if update_mask is not None:
                 request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.update_mute_config]
+        rpc = self._transport._wrapped_methods[self._transport.update_finding]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
-                (("mute_config.name", request.mute_config.name),)
+                (("finding.name", request.finding.name),)
             ),
         )
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
@@ -2873,19 +2644,38 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Updates a notification config. The following update fields are
         allowed: description, pubsub_topic, streaming_config.filter
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateNotificationConfigRequest(
+                )
+
+                # Make the request
+                response = client.update_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateNotificationConfigRequest, dict]):
                 The request object. Request message for updating a
                 notification config.
-            notification_config (google.cloud.securitycenter_v1.types.NotificationConfig):
+            notification_config (google.cloud.securitycenter_v1p1beta1.types.NotificationConfig):
                 Required. The notification config to
                 update.
 
                 This corresponds to the ``notification_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
@@ -2900,25 +2690,26 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.NotificationConfig:
-                Cloud Security Command Center (Cloud
-                SCC) notification configs.
-                A notification config is a Cloud SCC
-                resource that contains the configuration
-                to send notifications for create/update
-                events of findings, assets and etc.
+            google.cloud.securitycenter_v1p1beta1.types.NotificationConfig:
+                Security Command Center notification
+                configs.
+                A notification config is a Security
+                Command Center resource that contains
+                the configuration to send notifications
+                for create/update events of findings,
+                assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([notification_config, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2967,40 +2758,58 @@
         organization_settings: gcs_organization_settings.OrganizationSettings = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_organization_settings.OrganizationSettings:
         r"""Updates an organization's settings.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_organization_settings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateOrganizationSettingsRequest(
+                )
+
+                # Make the request
+                response = client.update_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateOrganizationSettingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateOrganizationSettingsRequest, dict]):
                 The request object. Request message for updating an
                 organization's settings.
-            organization_settings (google.cloud.securitycenter_v1.types.OrganizationSettings):
+            organization_settings (google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings):
                 Required. The organization settings
                 resource to update.
 
                 This corresponds to the ``organization_settings`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.OrganizationSettings:
+            google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([organization_settings])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -3039,51 +2848,79 @@
         return response
 
     def update_source(
         self,
         request: Union[securitycenter_service.UpdateSourceRequest, dict] = None,
         *,
         source: gcs_source.Source = None,
+        update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Updates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_source():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateSourceRequest(
+                )
+
+                # Make the request
+                response = client.update_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateSourceRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateSourceRequest, dict]):
                 The request object. Request message for updating a
                 source.
-            source (google.cloud.securitycenter_v1.types.Source):
+            source (google.cloud.securitycenter_v1p1beta1.types.Source):
                 Required. The source resource to
                 update.
 
                 This corresponds to the ``source`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                The FieldMask to use when updating
+                the source resource.
+                If empty all mutable fields will be
+                updated.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.Source:
+            google.cloud.securitycenter_v1p1beta1.types.Source:
                 Security Command Center finding
                 source. A finding source is an entity or
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
-                monitor, and other tools.
+                monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([source])
+        has_flattened_params = any([source, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
@@ -3092,14 +2929,16 @@
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.UpdateSourceRequest):
             request = securitycenter_service.UpdateSourceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if source is not None:
                 request.source = source
+            if update_mask is not None:
+                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_source]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -3116,53 +2955,84 @@
         return response
 
     def update_security_marks(
         self,
         request: Union[securitycenter_service.UpdateSecurityMarksRequest, dict] = None,
         *,
         security_marks: gcs_security_marks.SecurityMarks = None,
+        update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_security_marks.SecurityMarks:
         r"""Updates security marks.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_security_marks():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateSecurityMarksRequest(
+                )
+
+                # Make the request
+                response = client.update_security_marks(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1.types.UpdateSecurityMarksRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateSecurityMarksRequest, dict]):
                 The request object. Request message for updating a
                 SecurityMarks resource.
-            security_marks (google.cloud.securitycenter_v1.types.SecurityMarks):
+            security_marks (google.cloud.securitycenter_v1p1beta1.types.SecurityMarks):
                 Required. The security marks resource
                 to update.
 
                 This corresponds to the ``security_marks`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                The FieldMask to use when updating the security marks
+                resource.
+
+                The field mask must not contain duplicate fields. If
+                empty or set to "marks", all marks will be replaced.
+                Individual marks can be updated using
+                "marks.<mark_key>".
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1.types.SecurityMarks:
+            google.cloud.securitycenter_v1p1beta1.types.SecurityMarks:
                 User specified security marks that
                 are attached to the parent Security
                 Command Center resource. Security marks
                 are scoped within a Security Command
                 Center organization -- they can be
                 modified and viewed by all users who
                 have proper permissions on the
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([security_marks])
+        has_flattened_params = any([security_marks, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
@@ -3171,14 +3041,16 @@
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.UpdateSecurityMarksRequest):
             request = securitycenter_service.UpdateSecurityMarksRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if security_marks is not None:
                 request.security_marks = security_marks
+            if update_mask is not None:
+                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_security_marks]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/pagers.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/base.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -176,16 +176,19 @@
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
+                # use the credentials which are saved
                 credentials=self._credentials,
-                credentials_file=credentials_file,
+                # Set ``credentials_file`` to ``None`` here as
+                # the credentials that we saved earlier should be used.
+                credentials_file=None,
                 scopes=self._scopes,
                 ssl_credentials=self._ssl_channel_credentials,
                 quota_project_id=quota_project_id,
                 options=[
                     ("grpc.max_send_message_length", -1),
                     ("grpc.max_receive_message_length", -1),
                 ],
@@ -250,15 +253,15 @@
     @property
     def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
-        # Sanity check: Only create a new client if we do not already have one.
+        # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
             self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc_asyncio.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -221,16 +221,19 @@
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
+                # use the credentials which are saved
                 credentials=self._credentials,
-                credentials_file=credentials_file,
+                # Set ``credentials_file`` to ``None`` here as
+                # the credentials that we saved earlier should be used.
+                credentials_file=None,
                 scopes=self._scopes,
                 ssl_credentials=self._ssl_channel_credentials,
                 quota_project_id=quota_project_id,
                 options=[
                     ("grpc.max_send_message_length", -1),
                     ("grpc.max_receive_message_length", -1),
                 ],
@@ -252,15 +255,15 @@
     @property
     def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
-        # Sanity check: Only create a new client if we do not already have one.
+        # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
             self._operations_client = operations_v1.OperationsAsyncClient(
                 self.grpc_channel
             )
 
         # Return the client from cache.
         return self._operations_client
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from .access import (
+    Access,
+    Geolocation,
+)
 from .asset import Asset
 from .external_system import ExternalSystem
 from .finding import Finding
 from .folder import Folder
 from .indicator import Indicator
 from .mute_config import MuteConfig
 from .notification_config import NotificationConfig
@@ -69,14 +73,16 @@
     Cve,
     Cvssv3,
     Reference,
     Vulnerability,
 )
 
 __all__ = (
+    "Access",
+    "Geolocation",
     "Asset",
     "ExternalSystem",
     "Finding",
     "Folder",
     "Indicator",
     "MuteConfig",
     "NotificationConfig",
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/asset.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/external_system.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/external_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/finding.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/finding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import proto  # type: ignore
 
+from google.cloud.securitycenter_v1.types import access as gcs_access
 from google.cloud.securitycenter_v1.types import external_system
 from google.cloud.securitycenter_v1.types import indicator as gcs_indicator
 from google.cloud.securitycenter_v1.types import security_marks as gcs_security_marks
 from google.cloud.securitycenter_v1.types import vulnerability as gcs_vulnerability
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
@@ -75,24 +76,24 @@
             characters or underscores only.
         security_marks (google.cloud.securitycenter_v1.types.SecurityMarks):
             Output only. User specified security marks.
             These marks are entirely managed by the user and
             come from the SecurityMarks resource that
             belongs to the finding.
         event_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time at which the event took place, or
-            when an update to the finding occurred. For
-            example, if the finding represents an open
-            firewall it would capture the time the detector
-            believes the firewall became open. The accuracy
-            is determined by the detector. If the finding
-            were to be resolved afterward, this time would
-            reflect when the finding was resolved. Must not
-            be set to a value greater than the current
-            timestamp.
+            The time the finding was first detected. If
+            an existing finding is updated, then this is the
+            time the update occurred. For example, if the
+            finding represents an open firewall, this
+            property captures the time the detector believes
+            the firewall became open. The accuracy is
+            determined by the detector. If the finding is
+            later resolved, then this time reflects when the
+            finding was resolved. This must not be set to a
+            value greater than the current timestamp.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The time at which the finding was created in
             Security Command Center.
         severity (google.cloud.securitycenter_v1.types.Finding.Severity):
             The severity of the finding. This field is
             managed by the source that writes the finding.
         canonical_name (str):
@@ -102,14 +103,16 @@
             or
             "projects/{project_number}/sources/{source_id}/findings/{finding_id}",
             depending on the closest CRM ancestor of the resource
             associated with the finding.
         mute (google.cloud.securitycenter_v1.types.Finding.Mute):
             Indicates the mute state of a finding (either
             unspecified, muted, unmuted or undefined).
+            Unlike other attributes of a finding, a finding
+            provider shouldn't set the value of mute.
         finding_class (google.cloud.securitycenter_v1.types.Finding.FindingClass):
             The class of the finding.
         indicator (google.cloud.securitycenter_v1.types.Indicator):
             Represents what's commonly known as an Indicator of
             compromise (IoC) in computer forensics. This is an artifact
             observed on a network or in an operating system that, with
             high confidence, indicates a computer intrusion. Reference:
@@ -122,18 +125,24 @@
         mute_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The most recent time this
             finding was muted or unmuted.
         external_systems (Sequence[google.cloud.securitycenter_v1.types.Finding.ExternalSystemsEntry]):
             Output only. Third party SIEM/SOAR fields
             within SCC, contains external system information
             and external system finding fields.
+        access (google.cloud.securitycenter_v1.types.Access):
+            Access details associated to the Finding,
+            such as more information on the caller, which
+            method was accessed, from where, etc.
         mute_initiator (str):
             First known as mute_annotation. Records additional
             information about the mute operation e.g. mute config that
-            muted the finding, user who muted the finding, etc.
+            muted the finding, user who muted the finding, etc. Unlike
+            other attributes of a finding, a finding provider shouldn't
+            set the value of mute.
     """
 
     class State(proto.Enum):
         r"""The state of the finding."""
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         INACTIVE = 2
@@ -187,11 +196,12 @@
     )
     mute_update_time = proto.Field(
         proto.MESSAGE, number=21, message=timestamp_pb2.Timestamp,
     )
     external_systems = proto.MapField(
         proto.STRING, proto.MESSAGE, number=22, message=external_system.ExternalSystem,
     )
+    access = proto.Field(proto.MESSAGE, number=26, message=gcs_access.Access,)
     mute_initiator = proto.Field(proto.STRING, number=28,)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/folder.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/indicator.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/indicator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/mute_config.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/mute_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/notification_config.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/notification_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/notification_message.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/notification_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/organization_settings.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/organization_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/resource.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,16 +30,15 @@
         name (str):
             The full resource name of the resource. See:
             https://cloud.google.com/apis/design/resource_names#full_resource_name
         project (str):
             The full resource name of project that the
             resource belongs to.
         project_display_name (str):
-            The human readable name of project that the
-            resource belongs to.
+            The project id that the resource belongs to.
         parent (str):
             The full resource name of resource's parent.
         parent_display_name (str):
             The human readable name of resource's parent.
         type_ (str):
             The full resource type of the resource.
         folders (Sequence[google.cloud.securitycenter_v1.types.Folder]):
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/run_asset_discovery_response.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/run_asset_discovery_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/security_marks.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/security_marks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/securitycenter_service.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/securitycenter_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1329,16 +1329,15 @@
                 name (str):
                     The full resource name of the resource. See:
                     https://cloud.google.com/apis/design/resource_names#full_resource_name
                 project_name (str):
                     The full resource name of project that the
                     resource belongs to.
                 project_display_name (str):
-                    The human readable name of project that the
-                    resource belongs to.
+                    The project id that the resource belongs to.
                 parent_name (str):
                     The full resource name of resource's parent.
                 parent_display_name (str):
                     The human readable name of resource's parent.
                 type_ (str):
                     The full resource type of the resource.
                 folders (Sequence[google.cloud.securitycenter_v1.types.Folder]):
@@ -1580,15 +1579,16 @@
             or set to "marks", all marks will be replaced. Individual
             marks can be updated using "marks.<mark_key>".
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             The time at which the updated SecurityMarks
             take effect. If not set uses current server
             time.  Updates will be applied to the
             SecurityMarks that are active immediately
-            preceding this time.
+            preceding this time. Must be smaller or equal to
+            the server time.
     """
 
     security_marks = proto.Field(
         proto.MESSAGE, number=1, message=gcs_security_marks.SecurityMarks,
     )
     update_mask = proto.Field(
         proto.MESSAGE, number=2, message=field_mask_pb2.FieldMask,
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/source.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1/types/vulnerability.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/types/vulnerability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -41,21 +41,20 @@
 
     Attributes:
         id (str):
             The unique identifier for the vulnerability.
             e.g. CVE-2021-34527
         references (Sequence[google.cloud.securitycenter_v1.types.Reference]):
             Additional information about the CVE.
-            e.g. https://cve.mitre.org/cgi-
-            bin/cvename.cgi?name=CVE-2021-34527
+            e.g.
+            https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-34527
         cvssv3 (google.cloud.securitycenter_v1.types.Cvssv3):
             Describe Common Vulnerability Scoring System
             specified at
-            https://www.first.org/cvss/v3.1/specification-
-            document
+            https://www.first.org/cvss/v3.1/specification-document
     """
 
     id = proto.Field(proto.STRING, number=1,)
     references = proto.RepeatedField(proto.MESSAGE, number=2, message="Reference",)
     cvssv3 = proto.Field(proto.MESSAGE, number=3, message="Cvssv3",)
 
 
@@ -63,16 +62,15 @@
     r"""Additional Links
 
     Attributes:
         source (str):
             Source of the reference e.g. NVD
         uri (str):
             Uri for the mentioned source e.g.
-            https://cve.mitre.org/cgi-
-            bin/cvename.cgi?name=CVE-2021-34527.
+            https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-34527.
     """
 
     source = proto.Field(proto.STRING, number=1,)
     uri = proto.Field(proto.STRING, number=2,)
 
 
 class Cvssv3(proto.Message):
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/gapic_metadata.json` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/async_client.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/async_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Sequence, Tuple, Type, Union
+from typing import Dict, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -134,14 +134,50 @@
         Returns:
             SecurityCenterAsyncClient: The constructed client.
         """
         return SecurityCenterClient.from_service_account_file.__func__(SecurityCenterAsyncClient, filename, *args, **kwargs)  # type: ignore
 
     from_service_account_json = from_service_account_file
 
+    @classmethod
+    def get_mtls_endpoint_and_cert_source(
+        cls, client_options: Optional[ClientOptions] = None
+    ):
+        """Return the API endpoint and client cert source for mutual TLS.
+
+        The client cert source is determined in the following order:
+        (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
+        client cert source is None.
+        (2) if `client_options.client_cert_source` is provided, use the provided one; if the
+        default client cert source exists, use the default one; otherwise the client cert
+        source is None.
+
+        The API endpoint is determined in the following order:
+        (1) if `client_options.api_endpoint` if provided, use the provided one.
+        (2) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is "always", use the
+        default mTLS endpoint; if the environment variabel is "never", use the default API
+        endpoint; otherwise if client cert source exists, use the default mTLS endpoint, otherwise
+        use the default API endpoint.
+
+        More details can be found at https://google.aip.dev/auth/4114.
+
+        Args:
+            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+                client. Only the `api_endpoint` and `client_cert_source` properties may be used
+                in this method.
+
+        Returns:
+            Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
+                client cert source to use.
+
+        Raises:
+            google.auth.exceptions.MutualTLSChannelError: If any errors happen.
+        """
+        return SecurityCenterClient.get_mtls_endpoint_and_cert_source(client_options)  # type: ignore
+
     @property
     def transport(self) -> SecurityCenterTransport:
         """Returns the transport used by the client instance.
 
         Returns:
             SecurityCenterTransport: The transport used by the client instance.
         """
@@ -206,14 +242,33 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Creates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_create_source():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.CreateSourceRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                response = client.create_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.CreateSourceRequest, dict]):
                 The request object. Request message for creating a
                 source.
             parent (:class:`str`):
                 Required. Resource name of the new source's parent. Its
                 format should be "organizations/[organization_id]".
@@ -242,15 +297,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -294,14 +349,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates a finding. The corresponding source must
         exist for finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_create_finding():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.CreateFindingRequest(
+                    parent="parent_value",
+                    finding_id="finding_id_value",
+                )
+
+                # Make the request
+                response = client.create_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.CreateFindingRequest, dict]):
                 The request object. Request message for creating a
                 finding.
             parent (:class:`str`):
                 Required. Resource name of the new finding's parent. Its
                 format should be
@@ -344,15 +420,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, finding_id, finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -396,14 +472,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_get_iam_policy():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.get_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
@@ -475,15 +571,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -534,14 +630,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> organization_settings.OrganizationSettings:
         r"""Gets the settings for an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_get_organization_settings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GetOrganizationSettingsRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GetOrganizationSettingsRequest, dict]):
                 The request object. Request message for getting
                 organization settings.
             name (:class:`str`):
                 Required. Name of the organization to get organization
                 settings for. Its format is
@@ -560,15 +675,15 @@
             google.cloud.securitycenter_v1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -617,14 +732,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> source.Source:
         r"""Gets a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_get_source():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GetSourceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GetSourceRequest, dict]):
                 The request object. Request message for getting a
                 source.
             name (:class:`str`):
                 Required. Relative resource name of the source. Its
                 format is
@@ -646,15 +780,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -703,14 +837,36 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.GroupAssetsAsyncPager:
         r"""Filters an organization's assets and  groups them by
         their specified properties.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_group_assets():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GroupAssetsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GroupAssetsRequest, dict]):
                 The request object. Request message for grouping by
                 assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -778,14 +934,36 @@
         r"""Filters an organization or source's findings and groups them by
         their specified properties.
 
         To group across all sources provide a ``-`` as the source id.
         Example:
         /v1beta1/organizations/{organization_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_group_findings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GroupFindingsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GroupFindingsRequest, dict]):
                 The request object. Request message for grouping by
                 findings.
             parent (:class:`str`):
                 Required. Name of the source to groupBy. Its format is
                 "organizations/[organization_id]/sources/[source_id]".
@@ -824,15 +1002,15 @@
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, group_by])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -888,14 +1066,34 @@
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAssetsAsyncPager:
         r"""Lists an organization's assets.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_list_assets():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.ListAssetsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.ListAssetsRequest, dict]):
                 The request object. Request message for listing assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -958,14 +1156,35 @@
     ) -> pagers.ListFindingsAsyncPager:
         r"""Lists an organization or source's findings.
 
         To list across all sources provide a ``-`` as the source id.
         Example:
         /v1beta1/organizations/{organization_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_list_findings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.ListFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.ListFindingsRequest, dict]):
                 The request object. Request message for listing
                 findings.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1027,14 +1246,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListSourcesAsyncPager:
         r"""Lists all sources belonging to an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_list_sources():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.ListSourcesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_sources(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.ListSourcesRequest, dict]):
                 The request object. Request message for listing sources.
             parent (:class:`str`):
                 Required. Resource name of the parent of sources to
                 list. Its format should be
                 "organizations/[organization_id]".
@@ -1053,15 +1292,15 @@
                 Response message for listing sources.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1121,14 +1360,38 @@
         r"""Runs asset discovery. The discovery is tracked with a
         long-running operation.
 
         This API can only be called with limited frequency for an
         organization. If it is called too frequently the caller will
         receive a TOO_MANY_REQUESTS error.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_run_asset_discovery():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.RunAssetDiscoveryRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.run_asset_discovery(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.RunAssetDiscoveryRequest, dict]):
                 The request object. Request message for running asset
                 discovery for an organization.
             parent (:class:`str`):
                 Required. Name of the organization to run asset
                 discovery for. Its format is
@@ -1159,15 +1422,15 @@
                       }
 
                    The JSON representation for Empty is empty JSON
                    object {}.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1216,14 +1479,34 @@
         start_time: timestamp_pb2.Timestamp = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_set_finding_state():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.SetFindingStateRequest(
+                    name="name_value",
+                    state="INACTIVE",
+                )
+
+                # Make the request
+                response = client.set_finding_state(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.SetFindingStateRequest, dict]):
                 The request object. Request message for updating a
                 finding's state.
             name (:class:`str`):
                 Required. The relative resource name of the finding.
                 See:
@@ -1264,15 +1547,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, state, start_time])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1316,14 +1599,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_set_iam_policy():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.SetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.set_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
@@ -1395,15 +1698,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1444,14 +1747,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Returns the permissions that a caller has on the
         specified source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_test_iam_permissions():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.TestIamPermissionsRequest(
+                    resource="resource_value",
+                    permissions=['permissions_value_1', 'permissions_value_2'],
+                )
+
+                # Make the request
+                response = client.test_iam_permissions(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
@@ -1477,15 +1801,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.iam_policy_pb2.TestIamPermissionsResponse:
                 Response message for TestIamPermissions method.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource, permissions])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1537,14 +1861,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates or updates a finding. The corresponding
         source must exist for a finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_finding():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateFindingRequest(
+                )
+
+                # Make the request
+                response = client.update_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateFindingRequest, dict]):
                 The request object. Request message for updating or
                 creating a finding.
             finding (:class:`google.cloud.securitycenter_v1beta1.types.Finding`):
                 Required. The finding resource to update or create if it
                 does not already exist. parent, security_marks, and
@@ -1573,15 +1916,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1624,14 +1967,32 @@
         organization_settings: gcs_organization_settings.OrganizationSettings = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_organization_settings.OrganizationSettings:
         r"""Updates an organization's settings.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_organization_settings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateOrganizationSettingsRequest(
+                )
+
+                # Make the request
+                response = client.update_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateOrganizationSettingsRequest, dict]):
                 The request object. Request message for updating an
                 organization's settings.
             organization_settings (:class:`google.cloud.securitycenter_v1beta1.types.OrganizationSettings`):
                 Required. The organization settings
                 resource to update.
@@ -1649,15 +2010,15 @@
             google.cloud.securitycenter_v1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([organization_settings])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1698,14 +2059,32 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Updates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_source():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateSourceRequest(
+                )
+
+                # Make the request
+                response = client.update_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateSourceRequest, dict]):
                 The request object. Request message for updating a
                 source.
             source (:class:`google.cloud.securitycenter_v1beta1.types.Source`):
                 Required. The source resource to
                 update.
@@ -1726,15 +2105,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1775,14 +2154,32 @@
         security_marks: gcs_security_marks.SecurityMarks = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_security_marks.SecurityMarks:
         r"""Updates security marks.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_security_marks():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateSecurityMarksRequest(
+                )
+
+                # Make the request
+                response = client.update_security_marks(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateSecurityMarksRequest, dict]):
                 The request object. Request message for updating a
                 SecurityMarks resource.
             security_marks (:class:`google.cloud.securitycenter_v1beta1.types.SecurityMarks`):
                 Required. The security marks resource
                 to update.
@@ -1805,15 +2202,15 @@
                 Center organization -- they can be
                 modified and viewed by all users who
                 have proper permissions on the
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([security_marks])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/client.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -309,14 +309,81 @@
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
 
+    @classmethod
+    def get_mtls_endpoint_and_cert_source(
+        cls, client_options: Optional[client_options_lib.ClientOptions] = None
+    ):
+        """Return the API endpoint and client cert source for mutual TLS.
+
+        The client cert source is determined in the following order:
+        (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
+        client cert source is None.
+        (2) if `client_options.client_cert_source` is provided, use the provided one; if the
+        default client cert source exists, use the default one; otherwise the client cert
+        source is None.
+
+        The API endpoint is determined in the following order:
+        (1) if `client_options.api_endpoint` if provided, use the provided one.
+        (2) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is "always", use the
+        default mTLS endpoint; if the environment variabel is "never", use the default API
+        endpoint; otherwise if client cert source exists, use the default mTLS endpoint, otherwise
+        use the default API endpoint.
+
+        More details can be found at https://google.aip.dev/auth/4114.
+
+        Args:
+            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+                client. Only the `api_endpoint` and `client_cert_source` properties may be used
+                in this method.
+
+        Returns:
+            Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
+                client cert source to use.
+
+        Raises:
+            google.auth.exceptions.MutualTLSChannelError: If any errors happen.
+        """
+        if client_options is None:
+            client_options = client_options_lib.ClientOptions()
+        use_client_cert = os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false")
+        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
+        if use_client_cert not in ("true", "false"):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        if use_mtls_endpoint not in ("auto", "never", "always"):
+            raise MutualTLSChannelError(
+                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
+            )
+
+        # Figure out the client cert source to use.
+        client_cert_source = None
+        if use_client_cert == "true":
+            if client_options.client_cert_source:
+                client_cert_source = client_options.client_cert_source
+            elif mtls.has_default_client_cert_source():
+                client_cert_source = mtls.default_client_cert_source()
+
+        # Figure out which api endpoint to use.
+        if client_options.api_endpoint is not None:
+            api_endpoint = client_options.api_endpoint
+        elif use_mtls_endpoint == "always" or (
+            use_mtls_endpoint == "auto" and client_cert_source
+        ):
+            api_endpoint = cls.DEFAULT_MTLS_ENDPOINT
+        else:
+            api_endpoint = cls.DEFAULT_ENDPOINT
+
+        return api_endpoint, client_cert_source
+
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, SecurityCenterTransport, None] = None,
         client_options: Optional[client_options_lib.ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
@@ -359,76 +426,50 @@
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
 
-        # Create SSL credentials for mutual TLS if needed.
-        if os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") not in (
-            "true",
-            "false",
-        ):
-            raise ValueError(
-                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
-            )
-        use_client_cert = (
-            os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") == "true"
+        api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
+            client_options
         )
 
-        client_cert_source_func = None
-        is_mtls = False
-        if use_client_cert:
-            if client_options.client_cert_source:
-                is_mtls = True
-                client_cert_source_func = client_options.client_cert_source
-            else:
-                is_mtls = mtls.has_default_client_cert_source()
-                if is_mtls:
-                    client_cert_source_func = mtls.default_client_cert_source()
-                else:
-                    client_cert_source_func = None
-
-        # Figure out which api endpoint to use.
-        if client_options.api_endpoint is not None:
-            api_endpoint = client_options.api_endpoint
-        else:
-            use_mtls_env = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
-            if use_mtls_env == "never":
-                api_endpoint = self.DEFAULT_ENDPOINT
-            elif use_mtls_env == "always":
-                api_endpoint = self.DEFAULT_MTLS_ENDPOINT
-            elif use_mtls_env == "auto":
-                if is_mtls:
-                    api_endpoint = self.DEFAULT_MTLS_ENDPOINT
-                else:
-                    api_endpoint = self.DEFAULT_ENDPOINT
-            else:
-                raise MutualTLSChannelError(
-                    "Unsupported GOOGLE_API_USE_MTLS_ENDPOINT value. Accepted "
-                    "values: never, auto, always"
-                )
+        api_key_value = getattr(client_options, "api_key", None)
+        if api_key_value and credentials:
+            raise ValueError(
+                "client_options.api_key and credentials are mutually exclusive"
+            )
 
         # Save or instantiate the transport.
         # Ordinarily, we provide the transport, but allowing a custom transport
         # instance provides an extensibility point for unusual situations.
         if isinstance(transport, SecurityCenterTransport):
             # transport is a SecurityCenterTransport instance.
-            if credentials or client_options.credentials_file:
+            if credentials or client_options.credentials_file or api_key_value:
                 raise ValueError(
                     "When providing a transport instance, "
                     "provide its credentials directly."
                 )
             if client_options.scopes:
                 raise ValueError(
                     "When providing a transport instance, provide its scopes "
                     "directly."
                 )
             self._transport = transport
         else:
+            import google.auth._default  # type: ignore
+
+            if api_key_value and hasattr(
+                google.auth._default, "get_api_key_credentials"
+            ):
+                credentials = google.auth._default.get_api_key_credentials(
+                    api_key_value
+                )
+
             Transport = type(self).get_transport_class(transport)
             self._transport = Transport(
                 credentials=credentials,
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
@@ -445,14 +486,33 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Creates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_create_source():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.CreateSourceRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                response = client.create_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.CreateSourceRequest, dict]):
                 The request object. Request message for creating a
                 source.
             parent (str):
                 Required. Resource name of the new source's parent. Its
                 format should be "organizations/[organization_id]".
@@ -481,15 +541,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -533,14 +593,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates a finding. The corresponding source must
         exist for finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_create_finding():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.CreateFindingRequest(
+                    parent="parent_value",
+                    finding_id="finding_id_value",
+                )
+
+                # Make the request
+                response = client.create_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.CreateFindingRequest, dict]):
                 The request object. Request message for creating a
                 finding.
             parent (str):
                 Required. Resource name of the new finding's parent. Its
                 format should be
@@ -583,15 +664,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, finding_id, finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -635,14 +716,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_get_iam_policy():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.get_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
@@ -714,15 +815,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -762,14 +863,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> organization_settings.OrganizationSettings:
         r"""Gets the settings for an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_get_organization_settings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GetOrganizationSettingsRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GetOrganizationSettingsRequest, dict]):
                 The request object. Request message for getting
                 organization settings.
             name (str):
                 Required. Name of the organization to get organization
                 settings for. Its format is
@@ -788,15 +908,15 @@
             google.cloud.securitycenter_v1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -839,14 +959,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> source.Source:
         r"""Gets a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_get_source():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GetSourceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GetSourceRequest, dict]):
                 The request object. Request message for getting a
                 source.
             name (str):
                 Required. Relative resource name of the source. Its
                 format is
@@ -868,15 +1007,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -915,14 +1054,36 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.GroupAssetsPager:
         r"""Filters an organization's assets and  groups them by
         their specified properties.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_group_assets():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GroupAssetsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GroupAssetsRequest, dict]):
                 The request object. Request message for grouping by
                 assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -981,14 +1142,36 @@
         r"""Filters an organization or source's findings and groups them by
         their specified properties.
 
         To group across all sources provide a ``-`` as the source id.
         Example:
         /v1beta1/organizations/{organization_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_group_findings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.GroupFindingsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.GroupFindingsRequest, dict]):
                 The request object. Request message for grouping by
                 findings.
             parent (str):
                 Required. Name of the source to groupBy. Its format is
                 "organizations/[organization_id]/sources/[source_id]".
@@ -1027,15 +1210,15 @@
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, group_by])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1081,14 +1264,34 @@
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAssetsPager:
         r"""Lists an organization's assets.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_list_assets():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.ListAssetsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.ListAssetsRequest, dict]):
                 The request object. Request message for listing assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -1142,14 +1345,35 @@
     ) -> pagers.ListFindingsPager:
         r"""Lists an organization or source's findings.
 
         To list across all sources provide a ``-`` as the source id.
         Example:
         /v1beta1/organizations/{organization_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_list_findings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.ListFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.ListFindingsRequest, dict]):
                 The request object. Request message for listing
                 findings.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1202,14 +1426,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListSourcesPager:
         r"""Lists all sources belonging to an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_list_sources():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.ListSourcesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_sources(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.ListSourcesRequest, dict]):
                 The request object. Request message for listing sources.
             parent (str):
                 Required. Resource name of the parent of sources to
                 list. Its format should be
                 "organizations/[organization_id]".
@@ -1228,15 +1472,15 @@
                 Response message for listing sources.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1286,14 +1530,38 @@
         r"""Runs asset discovery. The discovery is tracked with a
         long-running operation.
 
         This API can only be called with limited frequency for an
         organization. If it is called too frequently the caller will
         receive a TOO_MANY_REQUESTS error.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_run_asset_discovery():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.RunAssetDiscoveryRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.run_asset_discovery(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.RunAssetDiscoveryRequest, dict]):
                 The request object. Request message for running asset
                 discovery for an organization.
             parent (str):
                 Required. Name of the organization to run asset
                 discovery for. Its format is
@@ -1324,15 +1592,15 @@
                       }
 
                    The JSON representation for Empty is empty JSON
                    object {}.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1381,14 +1649,34 @@
         start_time: timestamp_pb2.Timestamp = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_set_finding_state():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.SetFindingStateRequest(
+                    name="name_value",
+                    state="INACTIVE",
+                )
+
+                # Make the request
+                response = client.set_finding_state(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.SetFindingStateRequest, dict]):
                 The request object. Request message for updating a
                 finding's state.
             name (str):
                 Required. The relative resource name of the finding.
                 See:
@@ -1429,15 +1717,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, state, start_time])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1481,14 +1769,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_set_iam_policy():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.SetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.set_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
@@ -1560,15 +1868,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1608,14 +1916,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Returns the permissions that a caller has on the
         specified source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_test_iam_permissions():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.TestIamPermissionsRequest(
+                    resource="resource_value",
+                    permissions=['permissions_value_1', 'permissions_value_2'],
+                )
+
+                # Make the request
+                response = client.test_iam_permissions(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
@@ -1641,15 +1970,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.iam_policy_pb2.TestIamPermissionsResponse:
                 Response message for TestIamPermissions method.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource, permissions])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1690,14 +2019,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates or updates a finding. The corresponding
         source must exist for a finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_finding():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateFindingRequest(
+                )
+
+                # Make the request
+                response = client.update_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateFindingRequest, dict]):
                 The request object. Request message for updating or
                 creating a finding.
             finding (google.cloud.securitycenter_v1beta1.types.Finding):
                 Required. The finding resource to update or create if it
                 does not already exist. parent, security_marks, and
@@ -1726,15 +2074,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1777,14 +2125,32 @@
         organization_settings: gcs_organization_settings.OrganizationSettings = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_organization_settings.OrganizationSettings:
         r"""Updates an organization's settings.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_organization_settings():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateOrganizationSettingsRequest(
+                )
+
+                # Make the request
+                response = client.update_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateOrganizationSettingsRequest, dict]):
                 The request object. Request message for updating an
                 organization's settings.
             organization_settings (google.cloud.securitycenter_v1beta1.types.OrganizationSettings):
                 Required. The organization settings
                 resource to update.
@@ -1802,15 +2168,15 @@
             google.cloud.securitycenter_v1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([organization_settings])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1855,14 +2221,32 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Updates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_source():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateSourceRequest(
+                )
+
+                # Make the request
+                response = client.update_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateSourceRequest, dict]):
                 The request object. Request message for updating a
                 source.
             source (google.cloud.securitycenter_v1beta1.types.Source):
                 Required. The source resource to
                 update.
@@ -1883,15 +2267,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1932,14 +2316,32 @@
         security_marks: gcs_security_marks.SecurityMarks = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_security_marks.SecurityMarks:
         r"""Updates security marks.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1beta1
+
+            def sample_update_security_marks():
+                # Create a client
+                client = securitycenter_v1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1beta1.UpdateSecurityMarksRequest(
+                )
+
+                # Make the request
+                response = client.update_security_marks(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1beta1.types.UpdateSecurityMarksRequest, dict]):
                 The request object. Request message for updating a
                 SecurityMarks resource.
             security_marks (google.cloud.securitycenter_v1beta1.types.SecurityMarks):
                 Required. The security marks resource
                 to update.
@@ -1962,15 +2364,15 @@
                 Center organization -- they can be
                 modified and viewed by all users who
                 have proper permissions on the
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([security_marks])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/pagers.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/pagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/base.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -170,16 +170,19 @@
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
+                # use the credentials which are saved
                 credentials=self._credentials,
-                credentials_file=credentials_file,
+                # Set ``credentials_file`` to ``None`` here as
+                # the credentials that we saved earlier should be used.
+                credentials_file=None,
                 scopes=self._scopes,
                 ssl_credentials=self._ssl_channel_credentials,
                 quota_project_id=quota_project_id,
                 options=[
                     ("grpc.max_send_message_length", -1),
                     ("grpc.max_receive_message_length", -1),
                 ],
@@ -244,15 +247,15 @@
     @property
     def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
-        # Sanity check: Only create a new client if we do not already have one.
+        # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
             self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc_asyncio.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/services/security_center/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -215,16 +215,19 @@
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
+                # use the credentials which are saved
                 credentials=self._credentials,
-                credentials_file=credentials_file,
+                # Set ``credentials_file`` to ``None`` here as
+                # the credentials that we saved earlier should be used.
+                credentials_file=None,
                 scopes=self._scopes,
                 ssl_credentials=self._ssl_channel_credentials,
                 quota_project_id=quota_project_id,
                 options=[
                     ("grpc.max_send_message_length", -1),
                     ("grpc.max_receive_message_length", -1),
                 ],
@@ -246,15 +249,15 @@
     @property
     def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
-        # Sanity check: Only create a new client if we do not already have one.
+        # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
             self._operations_client = operations_v1.OperationsAsyncClient(
                 self.grpc_channel
             )
 
         # Return the client from cache.
         return self._operations_client
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/asset.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/finding.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/organization_settings.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/organization_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/run_asset_discovery_response.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/run_asset_discovery_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/security_marks.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/security_marks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/securitycenter_service.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/securitycenter_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1beta1/types/source.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1beta1/types/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/gapic_metadata.json` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/async_client.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/async_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Sequence, Tuple, Type, Union
+from typing import Dict, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -148,14 +148,50 @@
         Returns:
             SecurityCenterAsyncClient: The constructed client.
         """
         return SecurityCenterClient.from_service_account_file.__func__(SecurityCenterAsyncClient, filename, *args, **kwargs)  # type: ignore
 
     from_service_account_json = from_service_account_file
 
+    @classmethod
+    def get_mtls_endpoint_and_cert_source(
+        cls, client_options: Optional[ClientOptions] = None
+    ):
+        """Return the API endpoint and client cert source for mutual TLS.
+
+        The client cert source is determined in the following order:
+        (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
+        client cert source is None.
+        (2) if `client_options.client_cert_source` is provided, use the provided one; if the
+        default client cert source exists, use the default one; otherwise the client cert
+        source is None.
+
+        The API endpoint is determined in the following order:
+        (1) if `client_options.api_endpoint` if provided, use the provided one.
+        (2) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is "always", use the
+        default mTLS endpoint; if the environment variabel is "never", use the default API
+        endpoint; otherwise if client cert source exists, use the default mTLS endpoint, otherwise
+        use the default API endpoint.
+
+        More details can be found at https://google.aip.dev/auth/4114.
+
+        Args:
+            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+                client. Only the `api_endpoint` and `client_cert_source` properties may be used
+                in this method.
+
+        Returns:
+            Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
+                client cert source to use.
+
+        Raises:
+            google.auth.exceptions.MutualTLSChannelError: If any errors happen.
+        """
+        return SecurityCenterClient.get_mtls_endpoint_and_cert_source(client_options)  # type: ignore
+
     @property
     def transport(self) -> SecurityCenterTransport:
         """Returns the transport used by the client instance.
 
         Returns:
             SecurityCenterTransport: The transport used by the client instance.
         """
@@ -220,14 +256,33 @@
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Creates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_create_source():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.CreateSourceRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                response = client.create_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateSourceRequest, dict]):
                 The request object. Request message for creating a
                 source.
             parent (:class:`str`):
                 Required. Resource name of the new source's parent. Its
                 format should be "organizations/[organization_id]".
@@ -256,15 +311,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -308,14 +363,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates a finding. The corresponding source must
         exist for finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_create_finding():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.CreateFindingRequest(
+                    parent="parent_value",
+                    finding_id="finding_id_value",
+                )
+
+                # Make the request
+                response = client.create_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateFindingRequest, dict]):
                 The request object. Request message for creating a
                 finding.
             parent (:class:`str`):
                 Required. Resource name of the new finding's parent. Its
                 format should be
@@ -355,15 +431,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, finding_id, finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -410,14 +486,34 @@
         notification_config: gcs_notification_config.NotificationConfig = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Creates a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_create_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.CreateNotificationConfigRequest(
+                    parent="parent_value",
+                    config_id="config_id_value",
+                )
+
+                # Make the request
+                response = client.create_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateNotificationConfigRequest, dict]):
                 The request object. Request message for creating a
                 notification config.
             parent (:class:`str`):
                 Required. Resource name of the new notification config's
                 parent. Its format is "organizations/[organization_id]".
@@ -458,15 +554,15 @@
                 Command Center resource that contains
                 the configuration to send notifications
                 for create/update events of findings,
                 assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, config_id, notification_config])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -511,14 +607,30 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_delete_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.DeleteNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_notification_config(request=request)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.DeleteNotificationConfigRequest, dict]):
                 The request object. Request message for deleting a
                 notification config.
             name (:class:`str`):
                 Required. Name of the notification config to delete. Its
                 format is
@@ -530,15 +642,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -577,14 +689,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_iam_policy():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.get_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
@@ -656,15 +788,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -715,14 +847,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification_config.NotificationConfig:
         r"""Gets a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.GetNotificationConfigRequest, dict]):
                 The request object. Request message for getting a
                 notification config.
             name (:class:`str`):
                 Required. Name of the notification config to get. Its
                 format is
@@ -745,15 +896,15 @@
                 Command Center resource that contains
                 the configuration to send notifications
                 for create/update events of findings,
                 assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -804,14 +955,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> organization_settings.OrganizationSettings:
         r"""Gets the settings for an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_organization_settings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetOrganizationSettingsRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.GetOrganizationSettingsRequest, dict]):
                 The request object. Request message for getting
                 organization settings.
             name (:class:`str`):
                 Required. Name of the organization to get organization
                 settings for. Its format is
@@ -830,15 +1000,15 @@
             google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -887,14 +1057,33 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> source.Source:
         r"""Gets a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_get_source():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GetSourceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.GetSourceRequest, dict]):
                 The request object. Request message for getting a
                 source.
             name (:class:`str`):
                 Required. Relative resource name of the source. Its
                 format is
@@ -916,15 +1105,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -973,14 +1162,36 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.GroupAssetsAsyncPager:
         r"""Filters an organization's assets and  groups them by
         their specified properties.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_group_assets():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GroupAssetsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.GroupAssetsRequest, dict]):
                 The request object. Request message for grouping by
                 assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1049,14 +1260,36 @@
         their specified properties.
 
         To group across all sources provide a ``-`` as the source id.
         Example: /v1/organizations/{organization_id}/sources/-/findings,
         /v1/folders/{folder_id}/sources/-/findings,
         /v1/projects/{project_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_group_findings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.GroupFindingsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.GroupFindingsRequest, dict]):
                 The request object. Request message for grouping by
                 findings.
             parent (:class:`str`):
                 Required. Name of the source to groupBy. Its format is
                 "organizations/[organization_id]/sources/[source_id]",
@@ -1104,15 +1337,15 @@
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, group_by])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1169,14 +1402,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAssetsAsyncPager:
         r"""Lists an organization's assets.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_assets():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListAssetsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.ListAssetsRequest, dict]):
                 The request object. Request message for listing assets.
             parent (:class:`str`):
                 Required. Name of the organization assets should belong
                 to. Its format is "organizations/[organization_id],
                 folders/[folder_id], or projects/[project_id]".
@@ -1195,15 +1448,15 @@
                 Response message for listing assets.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1262,14 +1515,35 @@
     ) -> pagers.ListFindingsAsyncPager:
         r"""Lists an organization or source's findings.
 
         To list across all sources provide a ``-`` as the source id.
         Example:
         /v1p1beta1/organizations/{organization_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_findings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.ListFindingsRequest, dict]):
                 The request object. Request message for listing
                 findings.
             parent (:class:`str`):
                 Required. Name of the source the findings belong to. Its
                 format is
@@ -1296,15 +1570,15 @@
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1361,14 +1635,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationConfigsAsyncPager:
         r"""Lists notification configs.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_notification_configs():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListNotificationConfigsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_notification_configs(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.ListNotificationConfigsRequest, dict]):
                 The request object. Request message for listing
                 notification configs.
             parent (:class:`str`):
                 Required. Name of the organization to list notification
                 configs. Its format is
@@ -1389,15 +1683,15 @@
                 notification configs.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1452,14 +1746,34 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListSourcesAsyncPager:
         r"""Lists all sources belonging to an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_list_sources():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.ListSourcesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_sources(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.ListSourcesRequest, dict]):
                 The request object. Request message for listing sources.
             parent (:class:`str`):
                 Required. Resource name of the parent of sources to
                 list. Its format should be
                 "organizations/[organization_id], folders/[folder_id],
@@ -1479,15 +1793,15 @@
                 Response message for listing sources.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1547,14 +1861,38 @@
         r"""Runs asset discovery. The discovery is tracked with a
         long-running operation.
 
         This API can only be called with limited frequency for an
         organization. If it is called too frequently the caller will
         receive a TOO_MANY_REQUESTS error.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_run_asset_discovery():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.RunAssetDiscoveryRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.run_asset_discovery(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.RunAssetDiscoveryRequest, dict]):
                 The request object. Request message for running asset
                 discovery for an organization.
             parent (:class:`str`):
                 Required. Name of the organization to run asset
                 discovery for. Its format is
@@ -1575,15 +1913,15 @@
 
                 The result type for the operation will be
                 :class:`google.cloud.securitycenter_v1p1beta1.types.RunAssetDiscoveryResponse`
                 Response of asset discovery run
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1632,14 +1970,34 @@
         start_time: timestamp_pb2.Timestamp = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_set_finding_state():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.SetFindingStateRequest(
+                    name="name_value",
+                    state="INACTIVE",
+                )
+
+                # Make the request
+                response = client.set_finding_state(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.SetFindingStateRequest, dict]):
                 The request object. Request message for updating a
                 finding's state.
             name (:class:`str`):
                 Required. The relative resource name of the finding.
                 See:
@@ -1680,15 +2038,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, state, start_time])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1732,14 +2090,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_set_iam_policy():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.SetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.set_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
@@ -1811,15 +2189,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1860,14 +2238,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Returns the permissions that a caller has on the
         specified source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_test_iam_permissions():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.TestIamPermissionsRequest(
+                    resource="resource_value",
+                    permissions=['permissions_value_1', 'permissions_value_2'],
+                )
+
+                # Make the request
+                response = client.test_iam_permissions(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
@@ -1893,15 +2292,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.iam_policy_pb2.TestIamPermissionsResponse:
                 Response message for TestIamPermissions method.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource, permissions])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1954,14 +2353,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates or updates a finding. The corresponding
         source must exist for a finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_finding():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateFindingRequest(
+                )
+
+                # Make the request
+                response = client.update_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateFindingRequest, dict]):
                 The request object. Request message for updating or
                 creating a finding.
             finding (:class:`google.cloud.securitycenter_v1p1beta1.types.Finding`):
                 Required. The finding resource to update or create if it
                 does not already exist. parent, security_marks, and
@@ -2004,15 +2422,15 @@
                 analysis, policy testing, and
                 enforcement. For example, an XSS
                 vulnerability in an App Engine
                 application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([finding, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2059,14 +2477,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Updates a notification config. The following update fields are
         allowed: description, pubsub_topic, streaming_config.filter
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_notification_config():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateNotificationConfigRequest(
+                )
+
+                # Make the request
+                response = client.update_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateNotificationConfigRequest, dict]):
                 The request object. Request message for updating a
                 notification config.
             notification_config (:class:`google.cloud.securitycenter_v1p1beta1.types.NotificationConfig`):
                 Required. The notification config to
                 update.
@@ -2097,15 +2534,15 @@
                 Command Center resource that contains
                 the configuration to send notifications
                 for create/update events of findings,
                 assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([notification_config, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2150,14 +2587,32 @@
         organization_settings: gcs_organization_settings.OrganizationSettings = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_organization_settings.OrganizationSettings:
         r"""Updates an organization's settings.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_organization_settings():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateOrganizationSettingsRequest(
+                )
+
+                # Make the request
+                response = client.update_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateOrganizationSettingsRequest, dict]):
                 The request object. Request message for updating an
                 organization's settings.
             organization_settings (:class:`google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings`):
                 Required. The organization settings
                 resource to update.
@@ -2175,15 +2630,15 @@
             google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([organization_settings])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2225,14 +2680,32 @@
         update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Updates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_source():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateSourceRequest(
+                )
+
+                # Make the request
+                response = client.update_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateSourceRequest, dict]):
                 The request object. Request message for updating a
                 source.
             source (:class:`google.cloud.securitycenter_v1p1beta1.types.Source`):
                 Required. The source resource to
                 update.
@@ -2262,15 +2735,15 @@
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
                 monitor, etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([source, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2314,14 +2787,32 @@
         update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_security_marks.SecurityMarks:
         r"""Updates security marks.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1p1beta1
+
+            def sample_update_security_marks():
+                # Create a client
+                client = securitycenter_v1p1beta1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1p1beta1.UpdateSecurityMarksRequest(
+                )
+
+                # Make the request
+                response = client.update_security_marks(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateSecurityMarksRequest, dict]):
                 The request object. Request message for updating a
                 SecurityMarks resource.
             security_marks (:class:`google.cloud.securitycenter_v1p1beta1.types.SecurityMarks`):
                 Required. The security marks resource
                 to update.
@@ -2356,15 +2847,15 @@
                 Center organization -- they can be
                 modified and viewed by all users who
                 have proper permissions on the
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([security_marks, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/client.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1/services/security_center/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,33 +32,37 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
-from google.cloud.securitycenter_v1p1beta1.services.security_center import pagers
-from google.cloud.securitycenter_v1p1beta1.types import finding
-from google.cloud.securitycenter_v1p1beta1.types import finding as gcs_finding
-from google.cloud.securitycenter_v1p1beta1.types import notification_config
-from google.cloud.securitycenter_v1p1beta1.types import (
+from google.cloud.securitycenter_v1.services.security_center import pagers
+from google.cloud.securitycenter_v1.types import access
+from google.cloud.securitycenter_v1.types import external_system as gcs_external_system
+from google.cloud.securitycenter_v1.types import finding
+from google.cloud.securitycenter_v1.types import finding as gcs_finding
+from google.cloud.securitycenter_v1.types import indicator
+from google.cloud.securitycenter_v1.types import mute_config
+from google.cloud.securitycenter_v1.types import mute_config as gcs_mute_config
+from google.cloud.securitycenter_v1.types import notification_config
+from google.cloud.securitycenter_v1.types import (
     notification_config as gcs_notification_config,
 )
-from google.cloud.securitycenter_v1p1beta1.types import organization_settings
-from google.cloud.securitycenter_v1p1beta1.types import (
+from google.cloud.securitycenter_v1.types import organization_settings
+from google.cloud.securitycenter_v1.types import (
     organization_settings as gcs_organization_settings,
 )
-from google.cloud.securitycenter_v1p1beta1.types import run_asset_discovery_response
-from google.cloud.securitycenter_v1p1beta1.types import security_marks
-from google.cloud.securitycenter_v1p1beta1.types import (
-    security_marks as gcs_security_marks,
-)
-from google.cloud.securitycenter_v1p1beta1.types import securitycenter_service
-from google.cloud.securitycenter_v1p1beta1.types import source
-from google.cloud.securitycenter_v1p1beta1.types import source as gcs_source
+from google.cloud.securitycenter_v1.types import run_asset_discovery_response
+from google.cloud.securitycenter_v1.types import security_marks
+from google.cloud.securitycenter_v1.types import security_marks as gcs_security_marks
+from google.cloud.securitycenter_v1.types import securitycenter_service
+from google.cloud.securitycenter_v1.types import source
+from google.cloud.securitycenter_v1.types import source as gcs_source
+from google.cloud.securitycenter_v1.types import vulnerability
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import SecurityCenterTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import SecurityCenterGrpcTransport
@@ -95,15 +99,15 @@
 
         # No transport is requested; return the default (that is, the first one
         # in the dictionary).
         return next(iter(cls._transport_registry.values()))
 
 
 class SecurityCenterClient(metaclass=SecurityCenterClientMeta):
-    """V1p1Beta1 APIs for Security Center service."""
+    """V1 APIs for Security Center service."""
 
     @staticmethod
     def _get_default_mtls_endpoint(api_endpoint):
         """Converts api endpoint to mTLS endpoint.
 
         Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
         "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
@@ -195,14 +199,35 @@
         """Parses a asset path into its component segments."""
         m = re.match(
             r"^organizations/(?P<organization>.+?)/assets/(?P<asset>.+?)$", path
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def external_system_path(
+        organization: str, source: str, finding: str, externalsystem: str,
+    ) -> str:
+        """Returns a fully-qualified external_system string."""
+        return "organizations/{organization}/sources/{source}/findings/{finding}/externalSystems/{externalsystem}".format(
+            organization=organization,
+            source=source,
+            finding=finding,
+            externalsystem=externalsystem,
+        )
+
+    @staticmethod
+    def parse_external_system_path(path: str) -> Dict[str, str]:
+        """Parses a external_system path into its component segments."""
+        m = re.match(
+            r"^organizations/(?P<organization>.+?)/sources/(?P<source>.+?)/findings/(?P<finding>.+?)/externalSystems/(?P<externalsystem>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def finding_path(organization: str, source: str, finding: str,) -> str:
         """Returns a fully-qualified finding string."""
         return "organizations/{organization}/sources/{source}/findings/{finding}".format(
             organization=organization, source=source, finding=finding,
         )
 
     @staticmethod
@@ -211,14 +236,30 @@
         m = re.match(
             r"^organizations/(?P<organization>.+?)/sources/(?P<source>.+?)/findings/(?P<finding>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def mute_config_path(organization: str, mute_config: str,) -> str:
+        """Returns a fully-qualified mute_config string."""
+        return "organizations/{organization}/muteConfigs/{mute_config}".format(
+            organization=organization, mute_config=mute_config,
+        )
+
+    @staticmethod
+    def parse_mute_config_path(path: str) -> Dict[str, str]:
+        """Parses a mute_config path into its component segments."""
+        m = re.match(
+            r"^organizations/(?P<organization>.+?)/muteConfigs/(?P<mute_config>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def notification_config_path(organization: str, notification_config: str,) -> str:
         """Returns a fully-qualified notification_config string."""
         return "organizations/{organization}/notificationConfigs/{notification_config}".format(
             organization=organization, notification_config=notification_config,
         )
 
     @staticmethod
@@ -342,14 +383,81 @@
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
 
+    @classmethod
+    def get_mtls_endpoint_and_cert_source(
+        cls, client_options: Optional[client_options_lib.ClientOptions] = None
+    ):
+        """Return the API endpoint and client cert source for mutual TLS.
+
+        The client cert source is determined in the following order:
+        (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
+        client cert source is None.
+        (2) if `client_options.client_cert_source` is provided, use the provided one; if the
+        default client cert source exists, use the default one; otherwise the client cert
+        source is None.
+
+        The API endpoint is determined in the following order:
+        (1) if `client_options.api_endpoint` if provided, use the provided one.
+        (2) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is "always", use the
+        default mTLS endpoint; if the environment variabel is "never", use the default API
+        endpoint; otherwise if client cert source exists, use the default mTLS endpoint, otherwise
+        use the default API endpoint.
+
+        More details can be found at https://google.aip.dev/auth/4114.
+
+        Args:
+            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+                client. Only the `api_endpoint` and `client_cert_source` properties may be used
+                in this method.
+
+        Returns:
+            Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
+                client cert source to use.
+
+        Raises:
+            google.auth.exceptions.MutualTLSChannelError: If any errors happen.
+        """
+        if client_options is None:
+            client_options = client_options_lib.ClientOptions()
+        use_client_cert = os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false")
+        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
+        if use_client_cert not in ("true", "false"):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        if use_mtls_endpoint not in ("auto", "never", "always"):
+            raise MutualTLSChannelError(
+                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
+            )
+
+        # Figure out the client cert source to use.
+        client_cert_source = None
+        if use_client_cert == "true":
+            if client_options.client_cert_source:
+                client_cert_source = client_options.client_cert_source
+            elif mtls.has_default_client_cert_source():
+                client_cert_source = mtls.default_client_cert_source()
+
+        # Figure out which api endpoint to use.
+        if client_options.api_endpoint is not None:
+            api_endpoint = client_options.api_endpoint
+        elif use_mtls_endpoint == "always" or (
+            use_mtls_endpoint == "auto" and client_cert_source
+        ):
+            api_endpoint = cls.DEFAULT_MTLS_ENDPOINT
+        else:
+            api_endpoint = cls.DEFAULT_ENDPOINT
+
+        return api_endpoint, client_cert_source
+
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, SecurityCenterTransport, None] = None,
         client_options: Optional[client_options_lib.ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
@@ -392,137 +500,248 @@
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
 
-        # Create SSL credentials for mutual TLS if needed.
-        if os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") not in (
-            "true",
-            "false",
-        ):
-            raise ValueError(
-                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
-            )
-        use_client_cert = (
-            os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false") == "true"
+        api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
+            client_options
         )
 
-        client_cert_source_func = None
-        is_mtls = False
-        if use_client_cert:
-            if client_options.client_cert_source:
-                is_mtls = True
-                client_cert_source_func = client_options.client_cert_source
-            else:
-                is_mtls = mtls.has_default_client_cert_source()
-                if is_mtls:
-                    client_cert_source_func = mtls.default_client_cert_source()
-                else:
-                    client_cert_source_func = None
-
-        # Figure out which api endpoint to use.
-        if client_options.api_endpoint is not None:
-            api_endpoint = client_options.api_endpoint
-        else:
-            use_mtls_env = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
-            if use_mtls_env == "never":
-                api_endpoint = self.DEFAULT_ENDPOINT
-            elif use_mtls_env == "always":
-                api_endpoint = self.DEFAULT_MTLS_ENDPOINT
-            elif use_mtls_env == "auto":
-                if is_mtls:
-                    api_endpoint = self.DEFAULT_MTLS_ENDPOINT
-                else:
-                    api_endpoint = self.DEFAULT_ENDPOINT
-            else:
-                raise MutualTLSChannelError(
-                    "Unsupported GOOGLE_API_USE_MTLS_ENDPOINT value. Accepted "
-                    "values: never, auto, always"
-                )
+        api_key_value = getattr(client_options, "api_key", None)
+        if api_key_value and credentials:
+            raise ValueError(
+                "client_options.api_key and credentials are mutually exclusive"
+            )
 
         # Save or instantiate the transport.
         # Ordinarily, we provide the transport, but allowing a custom transport
         # instance provides an extensibility point for unusual situations.
         if isinstance(transport, SecurityCenterTransport):
             # transport is a SecurityCenterTransport instance.
-            if credentials or client_options.credentials_file:
+            if credentials or client_options.credentials_file or api_key_value:
                 raise ValueError(
                     "When providing a transport instance, "
                     "provide its credentials directly."
                 )
             if client_options.scopes:
                 raise ValueError(
                     "When providing a transport instance, provide its scopes "
                     "directly."
                 )
             self._transport = transport
         else:
+            import google.auth._default  # type: ignore
+
+            if api_key_value and hasattr(
+                google.auth._default, "get_api_key_credentials"
+            ):
+                credentials = google.auth._default.get_api_key_credentials(
+                    api_key_value
+                )
+
             Transport = type(self).get_transport_class(transport)
             self._transport = Transport(
                 credentials=credentials,
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
                 always_use_jwt_access=True,
             )
 
+    def bulk_mute_findings(
+        self,
+        request: Union[securitycenter_service.BulkMuteFindingsRequest, dict] = None,
+        *,
+        parent: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Kicks off an LRO to bulk mute findings for a parent
+        based on a filter. The parent can be either an
+        organization, folder or project. The findings matched by
+        the filter will be muted after the LRO is done.
+
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_bulk_mute_findings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.BulkMuteFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.bulk_mute_findings(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.BulkMuteFindingsRequest, dict]):
+                The request object. Request message for bulk findings
+                update.
+                Note:
+                1. If multiple bulk update requests match the same
+                resource, the order in which they get executed is not
+                defined.
+                2. Once a bulk operation is started, there is no way to
+                stop it.
+            parent (str):
+                Required. The parent, at which bulk action needs to be
+                applied. Its format is
+                "organizations/[organization_id]",
+                "folders/[folder_id]", "projects/[project_id]".
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.securitycenter_v1.types.BulkMuteFindingsResponse`
+                The response to a BulkMute request. Contains the LRO
+                information.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.BulkMuteFindingsRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.BulkMuteFindingsRequest):
+            request = securitycenter_service.BulkMuteFindingsRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.bulk_mute_findings]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            securitycenter_service.BulkMuteFindingsResponse,
+            metadata_type=empty_pb2.Empty,
+        )
+
+        # Done; return the response.
+        return response
+
     def create_source(
         self,
         request: Union[securitycenter_service.CreateSourceRequest, dict] = None,
         *,
         parent: str = None,
         source: gcs_source.Source = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Creates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_source():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.CreateSourceRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                response = client.create_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateSourceRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.CreateSourceRequest, dict]):
                 The request object. Request message for creating a
                 source.
             parent (str):
                 Required. Resource name of the new source's parent. Its
                 format should be "organizations/[organization_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            source (google.cloud.securitycenter_v1p1beta1.types.Source):
+            source (google.cloud.securitycenter_v1.types.Source):
                 Required. The Source being created, only the
                 display_name and description will be used. All other
                 fields will be ignored.
 
                 This corresponds to the ``source`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.Source:
+            google.cloud.securitycenter_v1.types.Source:
                 Security Command Center finding
                 source. A finding source is an entity or
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
-                monitor, etc.
+                monitor, and other tools.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -566,62 +785,86 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates a finding. The corresponding source must
         exist for finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_finding():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.CreateFindingRequest(
+                    parent="parent_value",
+                    finding_id="finding_id_value",
+                )
+
+                # Make the request
+                response = client.create_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateFindingRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.CreateFindingRequest, dict]):
                 The request object. Request message for creating a
                 finding.
             parent (str):
                 Required. Resource name of the new finding's parent. Its
                 format should be
                 "organizations/[organization_id]/sources/[source_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             finding_id (str):
                 Required. Unique identifier provided
                 by the client within the parent scope.
+                It must be alphanumeric and less than or
+                equal to 32 characters and greater than
+                0 characters in length.
 
                 This corresponds to the ``finding_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            finding (google.cloud.securitycenter_v1p1beta1.types.Finding):
+            finding (google.cloud.securitycenter_v1.types.Finding):
                 Required. The Finding being created. The name and
                 security_marks will be ignored as they are both output
                 only fields on this resource.
 
                 This corresponds to the ``finding`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.Finding:
+            google.cloud.securitycenter_v1.types.Finding:
                 Security Command Center finding.
                 A finding is a record of assessment data
-                (security, risk, health or privacy)
-                ingested into Security Command Center
-                for presentation, notification,
+                like security, risk, health, or privacy,
+                that is ingested into Security Command
+                Center for presentation, notification,
                 analysis, policy testing, and
-                enforcement. For example, an XSS
-                vulnerability in an App Engine
-                application is a finding.
+                enforcement. For example, a cross-site
+                scripting (XSS) vulnerability in an App
+                Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, finding_id, finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -653,14 +896,135 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def create_mute_config(
+        self,
+        request: Union[securitycenter_service.CreateMuteConfigRequest, dict] = None,
+        *,
+        parent: str = None,
+        mute_config: gcs_mute_config.MuteConfig = None,
+        mute_config_id: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> gcs_mute_config.MuteConfig:
+        r"""Creates a mute config.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                mute_config = securitycenter_v1.MuteConfig()
+                mute_config.filter = "filter_value"
+
+                request = securitycenter_v1.CreateMuteConfigRequest(
+                    parent="parent_value",
+                    mute_config=mute_config,
+                    mute_config_id="mute_config_id_value",
+                )
+
+                # Make the request
+                response = client.create_mute_config(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.CreateMuteConfigRequest, dict]):
+                The request object. Request message for creating a mute
+                config.
+            parent (str):
+                Required. Resource name of the new mute configs's
+                parent. Its format is "organizations/[organization_id]",
+                "folders/[folder_id]", or "projects/[project_id]".
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            mute_config (google.cloud.securitycenter_v1.types.MuteConfig):
+                Required. The mute config being
+                created.
+
+                This corresponds to the ``mute_config`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            mute_config_id (str):
+                Required. Unique identifier provided
+                by the client within the parent scope.
+                It must consist of lower case letters,
+                numbers, and hyphen, with the first
+                character a letter, the last a letter or
+                a number, and a 63 character maximum.
+
+                This corresponds to the ``mute_config_id`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycenter_v1.types.MuteConfig:
+                A mute config is a Cloud SCC resource
+                that contains the configuration to mute
+                create/update events of findings.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent, mute_config, mute_config_id])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.CreateMuteConfigRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.CreateMuteConfigRequest):
+            request = securitycenter_service.CreateMuteConfigRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+            if mute_config is not None:
+                request.mute_config = mute_config
+            if mute_config_id is not None:
+                request.mute_config_id = mute_config_id
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.create_mute_config]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # Done; return the response.
+        return response
+
     def create_notification_config(
         self,
         request: Union[
             securitycenter_service.CreateNotificationConfigRequest, dict
         ] = None,
         *,
         parent: str = None,
@@ -668,36 +1032,57 @@
         notification_config: gcs_notification_config.NotificationConfig = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Creates a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_create_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.CreateNotificationConfigRequest(
+                    parent="parent_value",
+                    config_id="config_id_value",
+                )
+
+                # Make the request
+                response = client.create_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.CreateNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.CreateNotificationConfigRequest, dict]):
                 The request object. Request message for creating a
                 notification config.
             parent (str):
                 Required. Resource name of the new notification config's
                 parent. Its format is "organizations/[organization_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             config_id (str):
-                Required. Unique identifier provided
-                by the client within the parent scope.
-                It must be between 1 and 128 characters,
-                and contains alphanumeric characters,
+                Required.
+                Unique identifier provided by the client
+                within the parent scope. It must be
+                between 1 and 128 characters, and
+                contains alphanumeric characters,
                 underscores or hyphens only.
 
                 This corresponds to the ``config_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            notification_config (google.cloud.securitycenter_v1p1beta1.types.NotificationConfig):
+            notification_config (google.cloud.securitycenter_v1.types.NotificationConfig):
                 Required. The notification config
                 being created. The name and the service
                 account will be ignored as they are both
                 output only fields on this resource.
 
                 This corresponds to the ``notification_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -705,26 +1090,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.NotificationConfig:
-                Security Command Center notification
-                configs.
-                A notification config is a Security
-                Command Center resource that contains
-                the configuration to send notifications
-                for create/update events of findings,
-                assets and etc.
+            google.cloud.securitycenter_v1.types.NotificationConfig:
+                Cloud Security Command Center (Cloud
+                SCC) notification configs.
+                A notification config is a Cloud SCC
+                resource that contains the configuration
+                to send notifications for create/update
+                events of findings, assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, config_id, notification_config])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -760,29 +1144,127 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def delete_mute_config(
+        self,
+        request: Union[securitycenter_service.DeleteMuteConfigRequest, dict] = None,
+        *,
+        name: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Deletes an existing mute config.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_delete_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.DeleteMuteConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_mute_config(request=request)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.DeleteMuteConfigRequest, dict]):
+                The request object. Request message for deleting a mute
+                config.
+            name (str):
+                Required. Name of the mute config to delete. Its format
+                is organizations/{organization}/muteConfigs/{config_id},
+                folders/{folder}/muteConfigs/{config_id}, or
+                projects/{project}/muteConfigs/{config_id}
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.DeleteMuteConfigRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.DeleteMuteConfigRequest):
+            request = securitycenter_service.DeleteMuteConfigRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.delete_mute_config]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        rpc(
+            request, retry=retry, timeout=timeout, metadata=metadata,
+        )
+
     def delete_notification_config(
         self,
         request: Union[
             securitycenter_service.DeleteNotificationConfigRequest, dict
         ] = None,
         *,
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_delete_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.DeleteNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_notification_config(request=request)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.DeleteNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.DeleteNotificationConfigRequest, dict]):
                 The request object. Request message for deleting a
                 notification config.
             name (str):
                 Required. Name of the notification config to delete. Its
                 format is
                 "organizations/[organization_id]/notificationConfigs/[config_id]".
 
@@ -792,15 +1274,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -843,14 +1325,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Gets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_iam_policy():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.get_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
                 The request object. Request message for `GetIamPolicy`
                 method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
@@ -922,15 +1424,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -957,29 +1459,142 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def get_mute_config(
+        self,
+        request: Union[securitycenter_service.GetMuteConfigRequest, dict] = None,
+        *,
+        name: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> mute_config.MuteConfig:
+        r"""Gets a mute config.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetMuteConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_mute_config(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.GetMuteConfigRequest, dict]):
+                The request object. Request message for retrieving a
+                mute config.
+            name (str):
+                Required. Name of the mute config to retrieve. Its
+                format is
+                organizations/{organization}/muteConfigs/{config_id},
+                folders/{folder}/muteConfigs/{config_id}, or
+                projects/{project}/muteConfigs/{config_id}
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycenter_v1.types.MuteConfig:
+                A mute config is a Cloud SCC resource
+                that contains the configuration to mute
+                create/update events of findings.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.GetMuteConfigRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.GetMuteConfigRequest):
+            request = securitycenter_service.GetMuteConfigRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.get_mute_config]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # Done; return the response.
+        return response
+
     def get_notification_config(
         self,
         request: Union[
             securitycenter_service.GetNotificationConfigRequest, dict
         ] = None,
         *,
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification_config.NotificationConfig:
         r"""Gets a notification config.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetNotificationConfigRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.GetNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.GetNotificationConfigRequest, dict]):
                 The request object. Request message for getting a
                 notification config.
             name (str):
                 Required. Name of the notification config to get. Its
                 format is
                 "organizations/[organization_id]/notificationConfigs/[config_id]".
 
@@ -989,26 +1604,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.NotificationConfig:
-                Security Command Center notification
-                configs.
-                A notification config is a Security
-                Command Center resource that contains
-                the configuration to send notifications
-                for create/update events of findings,
-                assets and etc.
+            google.cloud.securitycenter_v1.types.NotificationConfig:
+                Cloud Security Command Center (Cloud
+                SCC) notification configs.
+                A notification config is a Cloud SCC
+                resource that contains the configuration
+                to send notifications for create/update
+                events of findings, assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1049,16 +1663,35 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> organization_settings.OrganizationSettings:
         r"""Gets the settings for an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_organization_settings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetOrganizationSettingsRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.GetOrganizationSettingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.GetOrganizationSettingsRequest, dict]):
                 The request object. Request message for getting
                 organization settings.
             name (str):
                 Required. Name of the organization to get organization
                 settings for. Its format is
                 "organizations/[organization_id]/organizationSettings".
 
@@ -1068,22 +1701,22 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings:
+            google.cloud.securitycenter_v1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1126,16 +1759,35 @@
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> source.Source:
         r"""Gets a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_get_source():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GetSourceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.GetSourceRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.GetSourceRequest, dict]):
                 The request object. Request message for getting a
                 source.
             name (str):
                 Required. Relative resource name of the source. Its
                 format is
                 "organizations/[organization_id]/source/[source_id]".
 
@@ -1145,25 +1797,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.Source:
+            google.cloud.securitycenter_v1.types.Source:
                 Security Command Center finding
                 source. A finding source is an entity or
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
-                monitor, etc.
+                monitor, and other tools.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1202,26 +1854,48 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.GroupAssetsPager:
         r"""Filters an organization's assets and  groups them by
         their specified properties.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_group_assets():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GroupAssetsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.GroupAssetsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.GroupAssetsRequest, dict]):
                 The request object. Request message for grouping by
                 assets.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.GroupAssetsPager:
+            google.cloud.securitycenter_v1.services.security_center.pagers.GroupAssetsPager:
                 Response message for grouping by
                 assets.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1269,16 +1943,38 @@
         their specified properties.
 
         To group across all sources provide a ``-`` as the source id.
         Example: /v1/organizations/{organization_id}/sources/-/findings,
         /v1/folders/{folder_id}/sources/-/findings,
         /v1/projects/{project_id}/sources/-/findings
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_group_findings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.GroupFindingsRequest(
+                    parent="parent_value",
+                    group_by="group_by_value",
+                )
+
+                # Make the request
+                page_result = client.group_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.GroupFindingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.GroupFindingsRequest, dict]):
                 The request object. Request message for grouping by
                 findings.
             parent (str):
                 Required. Name of the source to groupBy. Its format is
                 "organizations/[organization_id]/sources/[source_id]",
                 folders/[folder_id]/sources/[source_id], or
                 projects/[project_id]/sources/[source_id]. To groupBy
@@ -1315,24 +2011,24 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.GroupFindingsPager:
+            google.cloud.securitycenter_v1.services.security_center.pagers.GroupFindingsPager:
                 Response message for group by
                 findings.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, group_by])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1372,66 +2068,64 @@
         # Done; return the response.
         return response
 
     def list_assets(
         self,
         request: Union[securitycenter_service.ListAssetsRequest, dict] = None,
         *,
-        parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAssetsPager:
         r"""Lists an organization's assets.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_assets():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListAssetsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_assets(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListAssetsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.ListAssetsRequest, dict]):
                 The request object. Request message for listing assets.
-            parent (str):
-                Required. Name of the organization assets should belong
-                to. Its format is "organizations/[organization_id],
-                folders/[folder_id], or projects/[project_id]".
-
-                This corresponds to the ``parent`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListAssetsPager:
+            google.cloud.securitycenter_v1.services.security_center.pagers.ListAssetsPager:
                 Response message for listing assets.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([parent])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
         # Minor optimization to avoid making a copy if the user passes
         # in a securitycenter_service.ListAssetsRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.ListAssetsRequest):
             request = securitycenter_service.ListAssetsRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.list_assets]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -1451,95 +2145,190 @@
         # Done; return the response.
         return response
 
     def list_findings(
         self,
         request: Union[securitycenter_service.ListFindingsRequest, dict] = None,
         *,
-        parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFindingsPager:
         r"""Lists an organization or source's findings.
 
         To list across all sources provide a ``-`` as the source id.
-        Example:
-        /v1p1beta1/organizations/{organization_id}/sources/-/findings
+        Example: /v1/organizations/{organization_id}/sources/-/findings
+
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_findings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListFindingsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_findings(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
 
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListFindingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.ListFindingsRequest, dict]):
                 The request object. Request message for listing
                 findings.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycenter_v1.services.security_center.pagers.ListFindingsPager:
+                Response message for listing
+                findings.
+                Iterating over this object will yield
+                results and resolve additional pages
+                automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.ListFindingsRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.ListFindingsRequest):
+            request = securitycenter_service.ListFindingsRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.list_findings]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__iter__` convenience method.
+        response = pagers.ListFindingsPager(
+            method=rpc, request=request, response=response, metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_mute_configs(
+        self,
+        request: Union[securitycenter_service.ListMuteConfigsRequest, dict] = None,
+        *,
+        parent: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListMuteConfigsPager:
+        r"""Lists mute configs.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_mute_configs():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListMuteConfigsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_mute_configs(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.ListMuteConfigsRequest, dict]):
+                The request object. Request message for listing  mute
+                configs at a given scope e.g. organization, folder or
+                project.
             parent (str):
-                Required. Name of the source the findings belong to. Its
-                format is
-                "organizations/[organization_id]/sources/[source_id],
-                folders/[folder_id]/sources/[source_id], or
-                projects/[project_id]/sources/[source_id]". To list
-                across all sources provide a source_id of ``-``. For
-                example: organizations/{organization_id}/sources/-,
-                folders/{folder_id}/sources/- or
-                projects/{projects_id}/sources/-
+                Required. The parent, which owns the collection of mute
+                configs. Its format is
+                "organizations/[organization_id]",
+                "folders/[folder_id]", "projects/[project_id]".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListFindingsPager:
-                Response message for listing
-                findings.
+            google.cloud.securitycenter_v1.services.security_center.pagers.ListMuteConfigsPager:
+                Response message for listing mute
+                configs.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
-        # in a securitycenter_service.ListFindingsRequest.
+        # in a securitycenter_service.ListMuteConfigsRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
-        if not isinstance(request, securitycenter_service.ListFindingsRequest):
-            request = securitycenter_service.ListFindingsRequest(request)
+        if not isinstance(request, securitycenter_service.ListMuteConfigsRequest):
+            request = securitycenter_service.ListMuteConfigsRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.list_findings]
+        rpc = self._transport._wrapped_methods[self._transport.list_mute_configs]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
-        response = pagers.ListFindingsPager(
+        response = pagers.ListMuteConfigsPager(
             method=rpc, request=request, response=response, metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def list_notification_configs(
@@ -1551,16 +2340,36 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationConfigsPager:
         r"""Lists notification configs.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_notification_configs():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListNotificationConfigsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_notification_configs(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListNotificationConfigsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.ListNotificationConfigsRequest, dict]):
                 The request object. Request message for listing
                 notification configs.
             parent (str):
                 Required. Name of the organization to list notification
                 configs. Its format is
                 "organizations/[organization_id]".
 
@@ -1570,24 +2379,24 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListNotificationConfigsPager:
+            google.cloud.securitycenter_v1.services.security_center.pagers.ListNotificationConfigsPager:
                 Response message for listing
                 notification configs.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1636,16 +2445,36 @@
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListSourcesPager:
         r"""Lists all sources belonging to an organization.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_list_sources():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.ListSourcesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_sources(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.ListSourcesRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.ListSourcesRequest, dict]):
                 The request object. Request message for listing sources.
             parent (str):
                 Required. Resource name of the parent of sources to
                 list. Its format should be
                 "organizations/[organization_id], folders/[folder_id],
                 or projects/[project_id]".
 
@@ -1655,23 +2484,23 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.services.security_center.pagers.ListSourcesPager:
+            google.cloud.securitycenter_v1.services.security_center.pagers.ListSourcesPager:
                 Response message for listing sources.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1721,16 +2550,40 @@
         r"""Runs asset discovery. The discovery is tracked with a
         long-running operation.
 
         This API can only be called with limited frequency for an
         organization. If it is called too frequently the caller will
         receive a TOO_MANY_REQUESTS error.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_run_asset_discovery():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.RunAssetDiscoveryRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                operation = client.run_asset_discovery(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.RunAssetDiscoveryRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.RunAssetDiscoveryRequest, dict]):
                 The request object. Request message for running asset
                 discovery for an organization.
             parent (str):
                 Required. Name of the organization to run asset
                 discovery for. Its format is
                 "organizations/[organization_id]".
 
@@ -1744,20 +2597,20 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.securitycenter_v1p1beta1.types.RunAssetDiscoveryResponse`
+                :class:`google.cloud.securitycenter_v1.types.RunAssetDiscoveryResponse`
                 Response of asset discovery run
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1806,29 +2659,49 @@
         start_time: timestamp_pb2.Timestamp = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> finding.Finding:
         r"""Updates the state of a finding.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_set_finding_state():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.SetFindingStateRequest(
+                    name="name_value",
+                    state="INACTIVE",
+                )
+
+                # Make the request
+                response = client.set_finding_state(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.SetFindingStateRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.SetFindingStateRequest, dict]):
                 The request object. Request message for updating a
                 finding's state.
             name (str):
                 Required. The relative resource name of the finding.
                 See:
                 https://cloud.google.com/apis/design/resource_names#relative_resource_name
                 Example:
                 "organizations/{organization_id}/sources/{source_id}/finding/{finding_id}".
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            state (google.cloud.securitycenter_v1p1beta1.types.Finding.State):
+            state (google.cloud.securitycenter_v1.types.Finding.State):
                 Required. The desired State of the
                 finding.
 
                 This corresponds to the ``state`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             start_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -1841,28 +2714,28 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.Finding:
+            google.cloud.securitycenter_v1.types.Finding:
                 Security Command Center finding.
                 A finding is a record of assessment data
-                (security, risk, health or privacy)
-                ingested into Security Command Center
-                for presentation, notification,
+                like security, risk, health, or privacy,
+                that is ingested into Security Command
+                Center for presentation, notification,
                 analysis, policy testing, and
-                enforcement. For example, an XSS
-                vulnerability in an App Engine
-                application is a finding.
+                enforcement. For example, a cross-site
+                scripting (XSS) vulnerability in an App
+                Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, state, start_time])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -1894,26 +2767,159 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def set_mute(
+        self,
+        request: Union[securitycenter_service.SetMuteRequest, dict] = None,
+        *,
+        name: str = None,
+        mute: finding.Finding.Mute = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> finding.Finding:
+        r"""Updates the mute state of a finding.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_set_mute():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.SetMuteRequest(
+                    name="name_value",
+                    mute="UNDEFINED",
+                )
+
+                # Make the request
+                response = client.set_mute(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.SetMuteRequest, dict]):
+                The request object. Request message for updating a
+                finding's mute status.
+            name (str):
+                Required. The relative resource name of the finding.
+                See:
+                https://cloud.google.com/apis/design/resource_names#relative_resource_name
+                Example:
+                "organizations/{organization_id}/sources/{source_id}/finding/{finding_id}",
+                "folders/{folder_id}/sources/{source_id}/finding/{finding_id}",
+                "projects/{project_id}/sources/{source_id}/finding/{finding_id}".
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            mute (google.cloud.securitycenter_v1.types.Finding.Mute):
+                Required. The desired state of the
+                Mute.
+
+                This corresponds to the ``mute`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycenter_v1.types.Finding:
+                Security Command Center finding.
+                A finding is a record of assessment data
+                like security, risk, health, or privacy,
+                that is ingested into Security Command
+                Center for presentation, notification,
+                analysis, policy testing, and
+                enforcement. For example, a cross-site
+                scripting (XSS) vulnerability in an App
+                Engine application is a finding.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name, mute])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.SetMuteRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.SetMuteRequest):
+            request = securitycenter_service.SetMuteRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+            if mute is not None:
+                request.mute = mute
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.set_mute]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # Done; return the response.
+        return response
+
     def set_iam_policy(
         self,
         request: Union[iam_policy_pb2.SetIamPolicyRequest, dict] = None,
         *,
         resource: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy_pb2.Policy:
         r"""Sets the access control policy on the specified
         Source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_set_iam_policy():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.SetIamPolicyRequest(
+                    resource="resource_value",
+                )
+
+                # Make the request
+                response = client.set_iam_policy(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
                 The request object. Request message for `SetIamPolicy`
                 method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
@@ -1985,15 +2991,15 @@
 
                    For a description of IAM and its features, see the
                    [IAM developer's
                    guide](\ https://cloud.google.com/iam/docs).
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2033,14 +3039,35 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> iam_policy_pb2.TestIamPermissionsResponse:
         r"""Returns the permissions that a caller has on the
         specified source.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_test_iam_permissions():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.TestIamPermissionsRequest(
+                    resource="resource_value",
+                    permissions=['permissions_value_1', 'permissions_value_2'],
+                )
+
+                # Make the request
+                response = client.test_iam_permissions(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
                 The request object. Request message for
                 `TestIamPermissions` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
@@ -2066,15 +3093,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.iam_policy_pb2.TestIamPermissionsResponse:
                 Response message for TestIamPermissions method.
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource, permissions])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2103,80 +3130,187 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def update_external_system(
+        self,
+        request: Union[securitycenter_service.UpdateExternalSystemRequest, dict] = None,
+        *,
+        external_system: gcs_external_system.ExternalSystem = None,
+        update_mask: field_mask_pb2.FieldMask = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> gcs_external_system.ExternalSystem:
+        r"""Updates external system. This is for a given finding.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_external_system():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateExternalSystemRequest(
+                )
+
+                # Make the request
+                response = client.update_external_system(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.UpdateExternalSystemRequest, dict]):
+                The request object. Request message for updating a
+                ExternalSystem resource.
+            external_system (google.cloud.securitycenter_v1.types.ExternalSystem):
+                Required. The external system
+                resource to update.
+
+                This corresponds to the ``external_system`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                The FieldMask to use when updating
+                the external system resource.
+                If empty all mutable fields will be
+                updated.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycenter_v1.types.ExternalSystem:
+                Representation of third party
+                SIEM/SOAR fields within SCC.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([external_system, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.UpdateExternalSystemRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.UpdateExternalSystemRequest):
+            request = securitycenter_service.UpdateExternalSystemRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if external_system is not None:
+                request.external_system = external_system
+            if update_mask is not None:
+                request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.update_external_system]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("external_system.name", request.external_system.name),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # Done; return the response.
+        return response
+
     def update_finding(
         self,
         request: Union[securitycenter_service.UpdateFindingRequest, dict] = None,
         *,
         finding: gcs_finding.Finding = None,
-        update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_finding.Finding:
         r"""Creates or updates a finding. The corresponding
         source must exist for a finding creation to succeed.
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_finding():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateFindingRequest(
+                )
+
+                # Make the request
+                response = client.update_finding(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateFindingRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.UpdateFindingRequest, dict]):
                 The request object. Request message for updating or
                 creating a finding.
-            finding (google.cloud.securitycenter_v1p1beta1.types.Finding):
+            finding (google.cloud.securitycenter_v1.types.Finding):
                 Required. The finding resource to update or create if it
                 does not already exist. parent, security_marks, and
                 update_time will be ignored.
 
                 In the case of creation, the finding id portion of the
                 name must be alphanumeric and less than or equal to 32
                 characters and greater than 0 characters in length.
 
                 This corresponds to the ``finding`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
-                The FieldMask to use when updating the finding resource.
-                This field should not be specified when creating a
-                finding.
-
-                When updating a finding, an empty mask is treated as
-                updating all mutable fields and replacing
-                source_properties. Individual source_properties can be
-                added/updated by using "source_properties." in the field
-                mask.
-
-                This corresponds to the ``update_mask`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.Finding:
+            google.cloud.securitycenter_v1.types.Finding:
                 Security Command Center finding.
                 A finding is a record of assessment data
-                (security, risk, health or privacy)
-                ingested into Security Command Center
-                for presentation, notification,
+                like security, risk, health, or privacy,
+                that is ingested into Security Command
+                Center for presentation, notification,
                 analysis, policy testing, and
-                enforcement. For example, an XSS
-                vulnerability in an App Engine
-                application is a finding.
+                enforcement. For example, a cross-site
+                scripting (XSS) vulnerability in an App
+                Engine application is a finding.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([finding, update_mask])
+        has_flattened_params = any([finding])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
@@ -2185,16 +3319,14 @@
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.UpdateFindingRequest):
             request = securitycenter_service.UpdateFindingRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if finding is not None:
                 request.finding = finding
-            if update_mask is not None:
-                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_finding]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -2206,14 +3338,121 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def update_mute_config(
+        self,
+        request: Union[securitycenter_service.UpdateMuteConfigRequest, dict] = None,
+        *,
+        mute_config: gcs_mute_config.MuteConfig = None,
+        update_mask: field_mask_pb2.FieldMask = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> gcs_mute_config.MuteConfig:
+        r"""Updates a mute config.
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_mute_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                mute_config = securitycenter_v1.MuteConfig()
+                mute_config.filter = "filter_value"
+
+                request = securitycenter_v1.UpdateMuteConfigRequest(
+                    mute_config=mute_config,
+                )
+
+                # Make the request
+                response = client.update_mute_config(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycenter_v1.types.UpdateMuteConfigRequest, dict]):
+                The request object. Request message for updating a mute
+                config.
+            mute_config (google.cloud.securitycenter_v1.types.MuteConfig):
+                Required. The mute config being
+                updated.
+
+                This corresponds to the ``mute_config`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                The list of fields to be updated.
+                If empty all mutable fields will be
+                updated.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycenter_v1.types.MuteConfig:
+                A mute config is a Cloud SCC resource
+                that contains the configuration to mute
+                create/update events of findings.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([mute_config, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a securitycenter_service.UpdateMuteConfigRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, securitycenter_service.UpdateMuteConfigRequest):
+            request = securitycenter_service.UpdateMuteConfigRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if mute_config is not None:
+                request.mute_config = mute_config
+            if update_mask is not None:
+                request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.update_mute_config]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("mute_config.name", request.mute_config.name),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+
+        # Done; return the response.
+        return response
+
     def update_notification_config(
         self,
         request: Union[
             securitycenter_service.UpdateNotificationConfigRequest, dict
         ] = None,
         *,
         notification_config: gcs_notification_config.NotificationConfig = None,
@@ -2221,19 +3460,38 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_notification_config.NotificationConfig:
         r"""Updates a notification config. The following update fields are
         allowed: description, pubsub_topic, streaming_config.filter
 
+
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_notification_config():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateNotificationConfigRequest(
+                )
+
+                # Make the request
+                response = client.update_notification_config(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateNotificationConfigRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.UpdateNotificationConfigRequest, dict]):
                 The request object. Request message for updating a
                 notification config.
-            notification_config (google.cloud.securitycenter_v1p1beta1.types.NotificationConfig):
+            notification_config (google.cloud.securitycenter_v1.types.NotificationConfig):
                 Required. The notification config to
                 update.
 
                 This corresponds to the ``notification_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
@@ -2248,26 +3506,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.NotificationConfig:
-                Security Command Center notification
-                configs.
-                A notification config is a Security
-                Command Center resource that contains
-                the configuration to send notifications
-                for create/update events of findings,
-                assets and etc.
+            google.cloud.securitycenter_v1.types.NotificationConfig:
+                Cloud Security Command Center (Cloud
+                SCC) notification configs.
+                A notification config is a Cloud SCC
+                resource that contains the configuration
+                to send notifications for create/update
+                events of findings, assets and etc.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([notification_config, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2316,40 +3573,58 @@
         organization_settings: gcs_organization_settings.OrganizationSettings = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_organization_settings.OrganizationSettings:
         r"""Updates an organization's settings.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_organization_settings():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateOrganizationSettingsRequest(
+                )
+
+                # Make the request
+                response = client.update_organization_settings(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateOrganizationSettingsRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.UpdateOrganizationSettingsRequest, dict]):
                 The request object. Request message for updating an
                 organization's settings.
-            organization_settings (google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings):
+            organization_settings (google.cloud.securitycenter_v1.types.OrganizationSettings):
                 Required. The organization settings
                 resource to update.
 
                 This corresponds to the ``organization_settings`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.OrganizationSettings:
+            google.cloud.securitycenter_v1.types.OrganizationSettings:
                 User specified settings that are
                 attached to the Security Command Center
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([organization_settings])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
@@ -2388,61 +3663,69 @@
         return response
 
     def update_source(
         self,
         request: Union[securitycenter_service.UpdateSourceRequest, dict] = None,
         *,
         source: gcs_source.Source = None,
-        update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_source.Source:
         r"""Updates a source.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_source():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateSourceRequest(
+                )
+
+                # Make the request
+                response = client.update_source(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateSourceRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.UpdateSourceRequest, dict]):
                 The request object. Request message for updating a
                 source.
-            source (google.cloud.securitycenter_v1p1beta1.types.Source):
+            source (google.cloud.securitycenter_v1.types.Source):
                 Required. The source resource to
                 update.
 
                 This corresponds to the ``source`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
-                The FieldMask to use when updating
-                the source resource.
-                If empty all mutable fields will be
-                updated.
-
-                This corresponds to the ``update_mask`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.Source:
+            google.cloud.securitycenter_v1.types.Source:
                 Security Command Center finding
                 source. A finding source is an entity or
                 a mechanism that can produce a finding.
                 A source is like a container of findings
                 that come from the same scanner, logger,
-                monitor, etc.
+                monitor, and other tools.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([source, update_mask])
+        has_flattened_params = any([source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
@@ -2451,16 +3734,14 @@
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.UpdateSourceRequest):
             request = securitycenter_service.UpdateSourceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if source is not None:
                 request.source = source
-            if update_mask is not None:
-                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_source]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -2477,66 +3758,71 @@
         return response
 
     def update_security_marks(
         self,
         request: Union[securitycenter_service.UpdateSecurityMarksRequest, dict] = None,
         *,
         security_marks: gcs_security_marks.SecurityMarks = None,
-        update_mask: field_mask_pb2.FieldMask = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcs_security_marks.SecurityMarks:
         r"""Updates security marks.
 
+        .. code-block:: python
+
+            from google.cloud import securitycenter_v1
+
+            def sample_update_security_marks():
+                # Create a client
+                client = securitycenter_v1.SecurityCenterClient()
+
+                # Initialize request argument(s)
+                request = securitycenter_v1.UpdateSecurityMarksRequest(
+                )
+
+                # Make the request
+                response = client.update_security_marks(request=request)
+
+                # Handle the response
+                print(response)
+
         Args:
-            request (Union[google.cloud.securitycenter_v1p1beta1.types.UpdateSecurityMarksRequest, dict]):
+            request (Union[google.cloud.securitycenter_v1.types.UpdateSecurityMarksRequest, dict]):
                 The request object. Request message for updating a
                 SecurityMarks resource.
-            security_marks (google.cloud.securitycenter_v1p1beta1.types.SecurityMarks):
+            security_marks (google.cloud.securitycenter_v1.types.SecurityMarks):
                 Required. The security marks resource
                 to update.
 
                 This corresponds to the ``security_marks`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
-                The FieldMask to use when updating the security marks
-                resource.
-
-                The field mask must not contain duplicate fields. If
-                empty or set to "marks", all marks will be replaced.
-                Individual marks can be updated using
-                "marks.<mark_key>".
-
-                This corresponds to the ``update_mask`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.securitycenter_v1p1beta1.types.SecurityMarks:
+            google.cloud.securitycenter_v1.types.SecurityMarks:
                 User specified security marks that
                 are attached to the parent Security
                 Command Center resource. Security marks
                 are scoped within a Security Command
                 Center organization -- they can be
                 modified and viewed by all users who
                 have proper permissions on the
                 organization.
 
         """
         # Create or coerce a protobuf request object.
-        # Sanity check: If we got a request object, we should *not* have
+        # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([security_marks, update_mask])
+        has_flattened_params = any([security_marks])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
         # Minor optimization to avoid making a copy if the user passes
@@ -2545,16 +3831,14 @@
         # there are no flattened fields.
         if not isinstance(request, securitycenter_service.UpdateSecurityMarksRequest):
             request = securitycenter_service.UpdateSecurityMarksRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if security_marks is not None:
                 request.security_marks = security_marks
-            if update_mask is not None:
-                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_security_marks]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/pagers.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/base.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -175,16 +175,19 @@
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
+                # use the credentials which are saved
                 credentials=self._credentials,
-                credentials_file=credentials_file,
+                # Set ``credentials_file`` to ``None`` here as
+                # the credentials that we saved earlier should be used.
+                credentials_file=None,
                 scopes=self._scopes,
                 ssl_credentials=self._ssl_channel_credentials,
                 quota_project_id=quota_project_id,
                 options=[
                     ("grpc.max_send_message_length", -1),
                     ("grpc.max_receive_message_length", -1),
                 ],
@@ -249,15 +252,15 @@
     @property
     def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
-        # Sanity check: Only create a new client if we do not already have one.
+        # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
             self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc_asyncio.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/services/security_center/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -220,16 +220,19 @@
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
+                # use the credentials which are saved
                 credentials=self._credentials,
-                credentials_file=credentials_file,
+                # Set ``credentials_file`` to ``None`` here as
+                # the credentials that we saved earlier should be used.
+                credentials_file=None,
                 scopes=self._scopes,
                 ssl_credentials=self._ssl_channel_credentials,
                 quota_project_id=quota_project_id,
                 options=[
                     ("grpc.max_send_message_length", -1),
                     ("grpc.max_receive_message_length", -1),
                 ],
@@ -251,15 +254,15 @@
     @property
     def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
-        # Sanity check: Only create a new client if we do not already have one.
+        # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
             self._operations_client = operations_v1.OperationsAsyncClient(
                 self.grpc_channel
             )
 
         # Return the client from cache.
         return self._operations_client
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/__init__.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/asset.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/finding.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/folder.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/notification_config.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/notification_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/notification_message.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/notification_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/organization_settings.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/organization_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/resource.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/run_asset_discovery_response.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/run_asset_discovery_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/security_marks.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/security_marks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/securitycenter_service.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/securitycenter_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google/cloud/securitycenter_v1p1beta1/types/source.py` & `google-cloud-securitycenter-1.9.0/google/cloud/securitycenter_v1p1beta1/types/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/PKG-INFO` & `google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-securitycenter
-Version: 1.8.0
+Version: 1.9.0
 Summary: Cloud Security Command Center API client library
 Home-page: https://github.com/googleapis/python-securitycenter
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-securitycenter-1.8.0/google_cloud_securitycenter.egg-info/SOURCES.txt` & `google-cloud-securitycenter-1.9.0/google_cloud_securitycenter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 google/cloud/securitycenter_v1/services/security_center/client.py
 google/cloud/securitycenter_v1/services/security_center/pagers.py
 google/cloud/securitycenter_v1/services/security_center/transports/__init__.py
 google/cloud/securitycenter_v1/services/security_center/transports/base.py
 google/cloud/securitycenter_v1/services/security_center/transports/grpc.py
 google/cloud/securitycenter_v1/services/security_center/transports/grpc_asyncio.py
 google/cloud/securitycenter_v1/types/__init__.py
+google/cloud/securitycenter_v1/types/access.py
 google/cloud/securitycenter_v1/types/asset.py
 google/cloud/securitycenter_v1/types/external_system.py
 google/cloud/securitycenter_v1/types/finding.py
 google/cloud/securitycenter_v1/types/folder.py
 google/cloud/securitycenter_v1/types/indicator.py
 google/cloud/securitycenter_v1/types/mute_config.py
 google/cloud/securitycenter_v1/types/notification_config.py
```

### Comparing `google-cloud-securitycenter-1.8.0/scripts/fixup_securitycenter_v1_keywords.py` & `google-cloud-securitycenter-1.9.0/scripts/fixup_securitycenter_v1_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/scripts/fixup_securitycenter_v1beta1_keywords.py` & `google-cloud-securitycenter-1.9.0/scripts/fixup_securitycenter_v1beta1_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/scripts/fixup_securitycenter_v1p1beta1_keywords.py` & `google-cloud-securitycenter-1.9.0/scripts/fixup_securitycenter_v1p1beta1_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/setup.py` & `google-cloud-securitycenter-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-securitycenter"
 description = "Cloud Security Command Center API client library"
-version = "1.8.0"
+version = "1.9.0"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.28.0, <3.0.0dev",
     "grpc-google-iam-v1 >= 0.12.3, < 0.13dev",
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/__init__.py` & `google-cloud-securitycenter-1.9.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/__init__.py` & `google-cloud-securitycenter-1.9.0/tests/unit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/__init__.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1/__init__.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1/test_security_center.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1/test_security_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,25 +25,27 @@
 
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import future
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
+from google.api_core import operation
 from google.api_core import operation_async  # type: ignore
 from google.api_core import operations_v1
 from google.api_core import path_template
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.securitycenter_v1.services.security_center import (
     SecurityCenterAsyncClient,
 )
 from google.cloud.securitycenter_v1.services.security_center import SecurityCenterClient
 from google.cloud.securitycenter_v1.services.security_center import pagers
 from google.cloud.securitycenter_v1.services.security_center import transports
+from google.cloud.securitycenter_v1.types import access
 from google.cloud.securitycenter_v1.types import external_system
 from google.cloud.securitycenter_v1.types import external_system as gcs_external_system
 from google.cloud.securitycenter_v1.types import finding
 from google.cloud.securitycenter_v1.types import finding as gcs_finding
 from google.cloud.securitycenter_v1.types import indicator
 from google.cloud.securitycenter_v1.types import mute_config
 from google.cloud.securitycenter_v1.types import mute_config as gcs_mute_config
@@ -427,14 +429,95 @@
                     quota_project_id=None,
                     client_info=transports.base.DEFAULT_CLIENT_INFO,
                     always_use_jwt_access=True,
                 )
 
 
 @pytest.mark.parametrize(
+    "client_class", [SecurityCenterClient, SecurityCenterAsyncClient]
+)
+@mock.patch.object(
+    SecurityCenterClient,
+    "DEFAULT_ENDPOINT",
+    modify_default_endpoint(SecurityCenterClient),
+)
+@mock.patch.object(
+    SecurityCenterAsyncClient,
+    "DEFAULT_ENDPOINT",
+    modify_default_endpoint(SecurityCenterAsyncClient),
+)
+def test_security_center_client_get_mtls_endpoint_and_cert_source(client_class):
+    mock_client_cert_source = mock.Mock()
+
+    # Test the case GOOGLE_API_USE_CLIENT_CERTIFICATE is "true".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        mock_api_endpoint = "foo"
+        options = client_options.ClientOptions(
+            client_cert_source=mock_client_cert_source, api_endpoint=mock_api_endpoint
+        )
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source(
+            options
+        )
+        assert api_endpoint == mock_api_endpoint
+        assert cert_source == mock_client_cert_source
+
+    # Test the case GOOGLE_API_USE_CLIENT_CERTIFICATE is "false".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "false"}):
+        mock_client_cert_source = mock.Mock()
+        mock_api_endpoint = "foo"
+        options = client_options.ClientOptions(
+            client_cert_source=mock_client_cert_source, api_endpoint=mock_api_endpoint
+        )
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source(
+            options
+        )
+        assert api_endpoint == mock_api_endpoint
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "never".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "never"}):
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+        assert api_endpoint == client_class.DEFAULT_ENDPOINT
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "always".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "always"}):
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+        assert api_endpoint == client_class.DEFAULT_MTLS_ENDPOINT
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "auto" and default cert doesn't exist.
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        with mock.patch(
+            "google.auth.transport.mtls.has_default_client_cert_source",
+            return_value=False,
+        ):
+            api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+            assert api_endpoint == client_class.DEFAULT_ENDPOINT
+            assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "auto" and default cert exists.
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        with mock.patch(
+            "google.auth.transport.mtls.has_default_client_cert_source",
+            return_value=True,
+        ):
+            with mock.patch(
+                "google.auth.transport.mtls.default_client_cert_source",
+                return_value=mock_client_cert_source,
+            ):
+                (
+                    api_endpoint,
+                    cert_source,
+                ) = client_class.get_mtls_endpoint_and_cert_source()
+                assert api_endpoint == client_class.DEFAULT_MTLS_ENDPOINT
+                assert cert_source == mock_client_cert_source
+
+
+@pytest.mark.parametrize(
     "client_class,transport_class,transport_name",
     [
         (SecurityCenterClient, transports.SecurityCenterGrpcTransport, "grpc"),
         (
             SecurityCenterAsyncClient,
             transports.SecurityCenterGrpcAsyncIOTransport,
             "grpc_asyncio",
@@ -458,29 +541,36 @@
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
         )
 
 
 @pytest.mark.parametrize(
-    "client_class,transport_class,transport_name",
+    "client_class,transport_class,transport_name,grpc_helpers",
     [
-        (SecurityCenterClient, transports.SecurityCenterGrpcTransport, "grpc"),
+        (
+            SecurityCenterClient,
+            transports.SecurityCenterGrpcTransport,
+            "grpc",
+            grpc_helpers,
+        ),
         (
             SecurityCenterAsyncClient,
             transports.SecurityCenterGrpcAsyncIOTransport,
             "grpc_asyncio",
+            grpc_helpers_async,
         ),
     ],
 )
 def test_security_center_client_client_options_credentials_file(
-    client_class, transport_class, transport_name
+    client_class, transport_class, transport_name, grpc_helpers
 ):
     # Check the case credentials file is provided.
     options = client_options.ClientOptions(credentials_file="credentials.json")
+
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
@@ -509,14 +599,80 @@
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
         )
 
 
 @pytest.mark.parametrize(
+    "client_class,transport_class,transport_name,grpc_helpers",
+    [
+        (
+            SecurityCenterClient,
+            transports.SecurityCenterGrpcTransport,
+            "grpc",
+            grpc_helpers,
+        ),
+        (
+            SecurityCenterAsyncClient,
+            transports.SecurityCenterGrpcAsyncIOTransport,
+            "grpc_asyncio",
+            grpc_helpers_async,
+        ),
+    ],
+)
+def test_security_center_client_create_channel_credentials_file(
+    client_class, transport_class, transport_name, grpc_helpers
+):
+    # Check the case credentials file is provided.
+    options = client_options.ClientOptions(credentials_file="credentials.json")
+
+    with mock.patch.object(transport_class, "__init__") as patched:
+        patched.return_value = None
+        client = client_class(client_options=options, transport=transport_name)
+        patched.assert_called_once_with(
+            credentials=None,
+            credentials_file="credentials.json",
+            host=client.DEFAULT_ENDPOINT,
+            scopes=None,
+            client_cert_source_for_mtls=None,
+            quota_project_id=None,
+            client_info=transports.base.DEFAULT_CLIENT_INFO,
+            always_use_jwt_access=True,
+        )
+
+    # test that the credentials from file are saved and used as the credentials.
+    with mock.patch.object(
+        google.auth, "load_credentials_from_file", autospec=True
+    ) as load_creds, mock.patch.object(
+        google.auth, "default", autospec=True
+    ) as adc, mock.patch.object(
+        grpc_helpers, "create_channel"
+    ) as create_channel:
+        creds = ga_credentials.AnonymousCredentials()
+        file_creds = ga_credentials.AnonymousCredentials()
+        load_creds.return_value = (file_creds, None)
+        adc.return_value = (creds, None)
+        client = client_class(client_options=options, transport=transport_name)
+        create_channel.assert_called_with(
+            "securitycenter.googleapis.com:443",
+            credentials=file_creds,
+            credentials_file=None,
+            quota_project_id=None,
+            default_scopes=("https://www.googleapis.com/auth/cloud-platform",),
+            scopes=None,
+            default_host="securitycenter.googleapis.com",
+            ssl_credentials=None,
+            options=[
+                ("grpc.max_send_message_length", -1),
+                ("grpc.max_receive_message_length", -1),
+            ],
+        )
+
+
+@pytest.mark.parametrize(
     "request_type", [securitycenter_service.BulkMuteFindingsRequest, dict,]
 )
 def test_bulk_mute_findings(request_type, transport: str = "grpc"):
     client = SecurityCenterClient(
         credentials=ga_credentials.AnonymousCredentials(), transport=transport,
     )
 
@@ -8727,14 +8883,31 @@
     )
     with pytest.raises(ValueError):
         client = SecurityCenterClient(
             client_options={"credentials_file": "credentials.json"},
             transport=transport,
         )
 
+    # It is an error to provide an api_key and a transport instance.
+    transport = transports.SecurityCenterGrpcTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    options = client_options.ClientOptions()
+    options.api_key = "api_key"
+    with pytest.raises(ValueError):
+        client = SecurityCenterClient(client_options=options, transport=transport,)
+
+    # It is an error to provide an api_key and a credential.
+    options = mock.Mock()
+    options.api_key = "api_key"
+    with pytest.raises(ValueError):
+        client = SecurityCenterClient(
+            client_options=options, credentials=ga_credentials.AnonymousCredentials()
+        )
+
     # It is an error to provide scopes and a transport instance.
     transport = transports.SecurityCenterGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = SecurityCenterClient(
             client_options={"scopes": ["1", "2"]}, transport=transport,
@@ -9530,7 +9703,37 @@
         )
         # Test client calls underlying transport.
         with mock.patch.object(type(client.transport), "close") as close:
             close.assert_not_called()
             with client:
                 pass
             close.assert_called()
+
+
+@pytest.mark.parametrize(
+    "client_class,transport_class",
+    [
+        (SecurityCenterClient, transports.SecurityCenterGrpcTransport),
+        (SecurityCenterAsyncClient, transports.SecurityCenterGrpcAsyncIOTransport),
+    ],
+)
+def test_api_key_credentials(client_class, transport_class):
+    with mock.patch.object(
+        google.auth._default, "get_api_key_credentials", create=True
+    ) as get_api_key_credentials:
+        mock_cred = mock.Mock()
+        get_api_key_credentials.return_value = mock_cred
+        options = client_options.ClientOptions()
+        options.api_key = "api_key"
+        with mock.patch.object(transport_class, "__init__") as patched:
+            patched.return_value = None
+            client = client_class(client_options=options)
+            patched.assert_called_once_with(
+                credentials=mock_cred,
+                credentials_file=None,
+                host=client.DEFAULT_ENDPOINT,
+                scopes=None,
+                client_cert_source_for_mtls=None,
+                quota_project_id=None,
+                client_info=transports.base.DEFAULT_CLIENT_INFO,
+                always_use_jwt_access=True,
+            )
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1beta1/__init__.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1beta1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1beta1/test_security_center.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1beta1/test_security_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,14 +25,15 @@
 
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import future
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
+from google.api_core import operation
 from google.api_core import operation_async  # type: ignore
 from google.api_core import operations_v1
 from google.api_core import path_template
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.securitycenter_v1beta1.services.security_center import (
     SecurityCenterAsyncClient,
@@ -420,14 +421,95 @@
                     quota_project_id=None,
                     client_info=transports.base.DEFAULT_CLIENT_INFO,
                     always_use_jwt_access=True,
                 )
 
 
 @pytest.mark.parametrize(
+    "client_class", [SecurityCenterClient, SecurityCenterAsyncClient]
+)
+@mock.patch.object(
+    SecurityCenterClient,
+    "DEFAULT_ENDPOINT",
+    modify_default_endpoint(SecurityCenterClient),
+)
+@mock.patch.object(
+    SecurityCenterAsyncClient,
+    "DEFAULT_ENDPOINT",
+    modify_default_endpoint(SecurityCenterAsyncClient),
+)
+def test_security_center_client_get_mtls_endpoint_and_cert_source(client_class):
+    mock_client_cert_source = mock.Mock()
+
+    # Test the case GOOGLE_API_USE_CLIENT_CERTIFICATE is "true".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        mock_api_endpoint = "foo"
+        options = client_options.ClientOptions(
+            client_cert_source=mock_client_cert_source, api_endpoint=mock_api_endpoint
+        )
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source(
+            options
+        )
+        assert api_endpoint == mock_api_endpoint
+        assert cert_source == mock_client_cert_source
+
+    # Test the case GOOGLE_API_USE_CLIENT_CERTIFICATE is "false".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "false"}):
+        mock_client_cert_source = mock.Mock()
+        mock_api_endpoint = "foo"
+        options = client_options.ClientOptions(
+            client_cert_source=mock_client_cert_source, api_endpoint=mock_api_endpoint
+        )
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source(
+            options
+        )
+        assert api_endpoint == mock_api_endpoint
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "never".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "never"}):
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+        assert api_endpoint == client_class.DEFAULT_ENDPOINT
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "always".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "always"}):
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+        assert api_endpoint == client_class.DEFAULT_MTLS_ENDPOINT
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "auto" and default cert doesn't exist.
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        with mock.patch(
+            "google.auth.transport.mtls.has_default_client_cert_source",
+            return_value=False,
+        ):
+            api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+            assert api_endpoint == client_class.DEFAULT_ENDPOINT
+            assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "auto" and default cert exists.
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        with mock.patch(
+            "google.auth.transport.mtls.has_default_client_cert_source",
+            return_value=True,
+        ):
+            with mock.patch(
+                "google.auth.transport.mtls.default_client_cert_source",
+                return_value=mock_client_cert_source,
+            ):
+                (
+                    api_endpoint,
+                    cert_source,
+                ) = client_class.get_mtls_endpoint_and_cert_source()
+                assert api_endpoint == client_class.DEFAULT_MTLS_ENDPOINT
+                assert cert_source == mock_client_cert_source
+
+
+@pytest.mark.parametrize(
     "client_class,transport_class,transport_name",
     [
         (SecurityCenterClient, transports.SecurityCenterGrpcTransport, "grpc"),
         (
             SecurityCenterAsyncClient,
             transports.SecurityCenterGrpcAsyncIOTransport,
             "grpc_asyncio",
@@ -451,29 +533,36 @@
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
         )
 
 
 @pytest.mark.parametrize(
-    "client_class,transport_class,transport_name",
+    "client_class,transport_class,transport_name,grpc_helpers",
     [
-        (SecurityCenterClient, transports.SecurityCenterGrpcTransport, "grpc"),
+        (
+            SecurityCenterClient,
+            transports.SecurityCenterGrpcTransport,
+            "grpc",
+            grpc_helpers,
+        ),
         (
             SecurityCenterAsyncClient,
             transports.SecurityCenterGrpcAsyncIOTransport,
             "grpc_asyncio",
+            grpc_helpers_async,
         ),
     ],
 )
 def test_security_center_client_client_options_credentials_file(
-    client_class, transport_class, transport_name
+    client_class, transport_class, transport_name, grpc_helpers
 ):
     # Check the case credentials file is provided.
     options = client_options.ClientOptions(credentials_file="credentials.json")
+
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
@@ -502,14 +591,80 @@
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
         )
 
 
 @pytest.mark.parametrize(
+    "client_class,transport_class,transport_name,grpc_helpers",
+    [
+        (
+            SecurityCenterClient,
+            transports.SecurityCenterGrpcTransport,
+            "grpc",
+            grpc_helpers,
+        ),
+        (
+            SecurityCenterAsyncClient,
+            transports.SecurityCenterGrpcAsyncIOTransport,
+            "grpc_asyncio",
+            grpc_helpers_async,
+        ),
+    ],
+)
+def test_security_center_client_create_channel_credentials_file(
+    client_class, transport_class, transport_name, grpc_helpers
+):
+    # Check the case credentials file is provided.
+    options = client_options.ClientOptions(credentials_file="credentials.json")
+
+    with mock.patch.object(transport_class, "__init__") as patched:
+        patched.return_value = None
+        client = client_class(client_options=options, transport=transport_name)
+        patched.assert_called_once_with(
+            credentials=None,
+            credentials_file="credentials.json",
+            host=client.DEFAULT_ENDPOINT,
+            scopes=None,
+            client_cert_source_for_mtls=None,
+            quota_project_id=None,
+            client_info=transports.base.DEFAULT_CLIENT_INFO,
+            always_use_jwt_access=True,
+        )
+
+    # test that the credentials from file are saved and used as the credentials.
+    with mock.patch.object(
+        google.auth, "load_credentials_from_file", autospec=True
+    ) as load_creds, mock.patch.object(
+        google.auth, "default", autospec=True
+    ) as adc, mock.patch.object(
+        grpc_helpers, "create_channel"
+    ) as create_channel:
+        creds = ga_credentials.AnonymousCredentials()
+        file_creds = ga_credentials.AnonymousCredentials()
+        load_creds.return_value = (file_creds, None)
+        adc.return_value = (creds, None)
+        client = client_class(client_options=options, transport=transport_name)
+        create_channel.assert_called_with(
+            "securitycenter.googleapis.com:443",
+            credentials=file_creds,
+            credentials_file=None,
+            quota_project_id=None,
+            default_scopes=("https://www.googleapis.com/auth/cloud-platform",),
+            scopes=None,
+            default_host="securitycenter.googleapis.com",
+            ssl_credentials=None,
+            options=[
+                ("grpc.max_send_message_length", -1),
+                ("grpc.max_receive_message_length", -1),
+            ],
+        )
+
+
+@pytest.mark.parametrize(
     "request_type", [securitycenter_service.CreateSourceRequest, dict,]
 )
 def test_create_source(request_type, transport: str = "grpc"):
     client = SecurityCenterClient(
         credentials=ga_credentials.AnonymousCredentials(), transport=transport,
     )
 
@@ -5138,14 +5293,31 @@
     )
     with pytest.raises(ValueError):
         client = SecurityCenterClient(
             client_options={"credentials_file": "credentials.json"},
             transport=transport,
         )
 
+    # It is an error to provide an api_key and a transport instance.
+    transport = transports.SecurityCenterGrpcTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    options = client_options.ClientOptions()
+    options.api_key = "api_key"
+    with pytest.raises(ValueError):
+        client = SecurityCenterClient(client_options=options, transport=transport,)
+
+    # It is an error to provide an api_key and a credential.
+    options = mock.Mock()
+    options.api_key = "api_key"
+    with pytest.raises(ValueError):
+        client = SecurityCenterClient(
+            client_options=options, credentials=ga_credentials.AnonymousCredentials()
+        )
+
     # It is an error to provide scopes and a transport instance.
     transport = transports.SecurityCenterGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = SecurityCenterClient(
             client_options={"scopes": ["1", "2"]}, transport=transport,
@@ -5831,7 +6003,37 @@
         )
         # Test client calls underlying transport.
         with mock.patch.object(type(client.transport), "close") as close:
             close.assert_not_called()
             with client:
                 pass
             close.assert_called()
+
+
+@pytest.mark.parametrize(
+    "client_class,transport_class",
+    [
+        (SecurityCenterClient, transports.SecurityCenterGrpcTransport),
+        (SecurityCenterAsyncClient, transports.SecurityCenterGrpcAsyncIOTransport),
+    ],
+)
+def test_api_key_credentials(client_class, transport_class):
+    with mock.patch.object(
+        google.auth._default, "get_api_key_credentials", create=True
+    ) as get_api_key_credentials:
+        mock_cred = mock.Mock()
+        get_api_key_credentials.return_value = mock_cred
+        options = client_options.ClientOptions()
+        options.api_key = "api_key"
+        with mock.patch.object(transport_class, "__init__") as patched:
+            patched.return_value = None
+            client = client_class(client_options=options)
+            patched.assert_called_once_with(
+                credentials=mock_cred,
+                credentials_file=None,
+                host=client.DEFAULT_ENDPOINT,
+                scopes=None,
+                client_cert_source_for_mtls=None,
+                quota_project_id=None,
+                client_info=transports.base.DEFAULT_CLIENT_INFO,
+                always_use_jwt_access=True,
+            )
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1p1beta1/__init__.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1p1beta1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-securitycenter-1.8.0/tests/unit/gapic/securitycenter_v1p1beta1/test_security_center.py` & `google-cloud-securitycenter-1.9.0/tests/unit/gapic/securitycenter_v1p1beta1/test_security_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,14 +25,15 @@
 
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import future
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
+from google.api_core import operation
 from google.api_core import operation_async  # type: ignore
 from google.api_core import operations_v1
 from google.api_core import path_template
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.securitycenter_v1p1beta1.services.security_center import (
     SecurityCenterAsyncClient,
@@ -425,14 +426,95 @@
                     quota_project_id=None,
                     client_info=transports.base.DEFAULT_CLIENT_INFO,
                     always_use_jwt_access=True,
                 )
 
 
 @pytest.mark.parametrize(
+    "client_class", [SecurityCenterClient, SecurityCenterAsyncClient]
+)
+@mock.patch.object(
+    SecurityCenterClient,
+    "DEFAULT_ENDPOINT",
+    modify_default_endpoint(SecurityCenterClient),
+)
+@mock.patch.object(
+    SecurityCenterAsyncClient,
+    "DEFAULT_ENDPOINT",
+    modify_default_endpoint(SecurityCenterAsyncClient),
+)
+def test_security_center_client_get_mtls_endpoint_and_cert_source(client_class):
+    mock_client_cert_source = mock.Mock()
+
+    # Test the case GOOGLE_API_USE_CLIENT_CERTIFICATE is "true".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        mock_api_endpoint = "foo"
+        options = client_options.ClientOptions(
+            client_cert_source=mock_client_cert_source, api_endpoint=mock_api_endpoint
+        )
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source(
+            options
+        )
+        assert api_endpoint == mock_api_endpoint
+        assert cert_source == mock_client_cert_source
+
+    # Test the case GOOGLE_API_USE_CLIENT_CERTIFICATE is "false".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "false"}):
+        mock_client_cert_source = mock.Mock()
+        mock_api_endpoint = "foo"
+        options = client_options.ClientOptions(
+            client_cert_source=mock_client_cert_source, api_endpoint=mock_api_endpoint
+        )
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source(
+            options
+        )
+        assert api_endpoint == mock_api_endpoint
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "never".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "never"}):
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+        assert api_endpoint == client_class.DEFAULT_ENDPOINT
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "always".
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "always"}):
+        api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+        assert api_endpoint == client_class.DEFAULT_MTLS_ENDPOINT
+        assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "auto" and default cert doesn't exist.
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        with mock.patch(
+            "google.auth.transport.mtls.has_default_client_cert_source",
+            return_value=False,
+        ):
+            api_endpoint, cert_source = client_class.get_mtls_endpoint_and_cert_source()
+            assert api_endpoint == client_class.DEFAULT_ENDPOINT
+            assert cert_source is None
+
+    # Test the case GOOGLE_API_USE_MTLS_ENDPOINT is "auto" and default cert exists.
+    with mock.patch.dict(os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": "true"}):
+        with mock.patch(
+            "google.auth.transport.mtls.has_default_client_cert_source",
+            return_value=True,
+        ):
+            with mock.patch(
+                "google.auth.transport.mtls.default_client_cert_source",
+                return_value=mock_client_cert_source,
+            ):
+                (
+                    api_endpoint,
+                    cert_source,
+                ) = client_class.get_mtls_endpoint_and_cert_source()
+                assert api_endpoint == client_class.DEFAULT_MTLS_ENDPOINT
+                assert cert_source == mock_client_cert_source
+
+
+@pytest.mark.parametrize(
     "client_class,transport_class,transport_name",
     [
         (SecurityCenterClient, transports.SecurityCenterGrpcTransport, "grpc"),
         (
             SecurityCenterAsyncClient,
             transports.SecurityCenterGrpcAsyncIOTransport,
             "grpc_asyncio",
@@ -456,29 +538,36 @@
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
         )
 
 
 @pytest.mark.parametrize(
-    "client_class,transport_class,transport_name",
+    "client_class,transport_class,transport_name,grpc_helpers",
     [
-        (SecurityCenterClient, transports.SecurityCenterGrpcTransport, "grpc"),
+        (
+            SecurityCenterClient,
+            transports.SecurityCenterGrpcTransport,
+            "grpc",
+            grpc_helpers,
+        ),
         (
             SecurityCenterAsyncClient,
             transports.SecurityCenterGrpcAsyncIOTransport,
             "grpc_asyncio",
+            grpc_helpers_async,
         ),
     ],
 )
 def test_security_center_client_client_options_credentials_file(
-    client_class, transport_class, transport_name
+    client_class, transport_class, transport_name, grpc_helpers
 ):
     # Check the case credentials file is provided.
     options = client_options.ClientOptions(credentials_file="credentials.json")
+
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
@@ -507,14 +596,80 @@
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
         )
 
 
 @pytest.mark.parametrize(
+    "client_class,transport_class,transport_name,grpc_helpers",
+    [
+        (
+            SecurityCenterClient,
+            transports.SecurityCenterGrpcTransport,
+            "grpc",
+            grpc_helpers,
+        ),
+        (
+            SecurityCenterAsyncClient,
+            transports.SecurityCenterGrpcAsyncIOTransport,
+            "grpc_asyncio",
+            grpc_helpers_async,
+        ),
+    ],
+)
+def test_security_center_client_create_channel_credentials_file(
+    client_class, transport_class, transport_name, grpc_helpers
+):
+    # Check the case credentials file is provided.
+    options = client_options.ClientOptions(credentials_file="credentials.json")
+
+    with mock.patch.object(transport_class, "__init__") as patched:
+        patched.return_value = None
+        client = client_class(client_options=options, transport=transport_name)
+        patched.assert_called_once_with(
+            credentials=None,
+            credentials_file="credentials.json",
+            host=client.DEFAULT_ENDPOINT,
+            scopes=None,
+            client_cert_source_for_mtls=None,
+            quota_project_id=None,
+            client_info=transports.base.DEFAULT_CLIENT_INFO,
+            always_use_jwt_access=True,
+        )
+
+    # test that the credentials from file are saved and used as the credentials.
+    with mock.patch.object(
+        google.auth, "load_credentials_from_file", autospec=True
+    ) as load_creds, mock.patch.object(
+        google.auth, "default", autospec=True
+    ) as adc, mock.patch.object(
+        grpc_helpers, "create_channel"
+    ) as create_channel:
+        creds = ga_credentials.AnonymousCredentials()
+        file_creds = ga_credentials.AnonymousCredentials()
+        load_creds.return_value = (file_creds, None)
+        adc.return_value = (creds, None)
+        client = client_class(client_options=options, transport=transport_name)
+        create_channel.assert_called_with(
+            "securitycenter.googleapis.com:443",
+            credentials=file_creds,
+            credentials_file=None,
+            quota_project_id=None,
+            default_scopes=("https://www.googleapis.com/auth/cloud-platform",),
+            scopes=None,
+            default_host="securitycenter.googleapis.com",
+            ssl_credentials=None,
+            options=[
+                ("grpc.max_send_message_length", -1),
+                ("grpc.max_receive_message_length", -1),
+            ],
+        )
+
+
+@pytest.mark.parametrize(
     "request_type", [securitycenter_service.CreateSourceRequest, dict,]
 )
 def test_create_source(request_type, transport: str = "grpc"):
     client = SecurityCenterClient(
         credentials=ga_credentials.AnonymousCredentials(), transport=transport,
     )
 
@@ -6832,14 +6987,31 @@
     )
     with pytest.raises(ValueError):
         client = SecurityCenterClient(
             client_options={"credentials_file": "credentials.json"},
             transport=transport,
         )
 
+    # It is an error to provide an api_key and a transport instance.
+    transport = transports.SecurityCenterGrpcTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    options = client_options.ClientOptions()
+    options.api_key = "api_key"
+    with pytest.raises(ValueError):
+        client = SecurityCenterClient(client_options=options, transport=transport,)
+
+    # It is an error to provide an api_key and a credential.
+    options = mock.Mock()
+    options.api_key = "api_key"
+    with pytest.raises(ValueError):
+        client = SecurityCenterClient(
+            client_options=options, credentials=ga_credentials.AnonymousCredentials()
+        )
+
     # It is an error to provide scopes and a transport instance.
     transport = transports.SecurityCenterGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = SecurityCenterClient(
             client_options={"scopes": ["1", "2"]}, transport=transport,
@@ -7574,7 +7746,37 @@
         )
         # Test client calls underlying transport.
         with mock.patch.object(type(client.transport), "close") as close:
             close.assert_not_called()
             with client:
                 pass
             close.assert_called()
+
+
+@pytest.mark.parametrize(
+    "client_class,transport_class",
+    [
+        (SecurityCenterClient, transports.SecurityCenterGrpcTransport),
+        (SecurityCenterAsyncClient, transports.SecurityCenterGrpcAsyncIOTransport),
+    ],
+)
+def test_api_key_credentials(client_class, transport_class):
+    with mock.patch.object(
+        google.auth._default, "get_api_key_credentials", create=True
+    ) as get_api_key_credentials:
+        mock_cred = mock.Mock()
+        get_api_key_credentials.return_value = mock_cred
+        options = client_options.ClientOptions()
+        options.api_key = "api_key"
+        with mock.patch.object(transport_class, "__init__") as patched:
+            patched.return_value = None
+            client = client_class(client_options=options)
+            patched.assert_called_once_with(
+                credentials=mock_cred,
+                credentials_file=None,
+                host=client.DEFAULT_ENDPOINT,
+                scopes=None,
+                client_cert_source_for_mtls=None,
+                quota_project_id=None,
+                client_info=transports.base.DEFAULT_CLIENT_INFO,
+                always_use_jwt_access=True,
+            )
```

