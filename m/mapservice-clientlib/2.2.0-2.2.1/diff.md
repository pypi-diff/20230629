# Comparing `tmp/mapservice-clientlib-2.2.0.tar.gz` & `tmp/mapservice_clientlib-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapservice-clientlib-2.2.0.tar", max compression
+gzip compressed data, was "mapservice_clientlib-2.2.1.tar", max compression
```

## Comparing `mapservice-clientlib-2.2.0.tar` & `mapservice_clientlib-2.2.1.tar`

### file list

```diff
@@ -1,98 +1,97 @@
--rw-r--r--   0        0        0     1507 2021-08-28 01:05:02.414811 mapservice-clientlib-2.2.0/LICENSE
--rw-r--r--   0        0        0     5888 2022-10-04 20:59:57.908195 mapservice-clientlib-2.2.0/README.md
--rw-r--r--   0        0        0       22 2022-10-04 21:20:12.123104 mapservice-clientlib-2.2.0/clients/__init__.py
--rw-r--r--   0        0        0    43285 2022-10-04 20:59:57.908695 mapservice-clientlib-2.2.0/clients/arcgis.py
--rw-r--r--   0        0        0     3461 2022-10-04 20:59:57.909012 mapservice-clientlib-2.2.0/clients/exceptions.py
--rw-r--r--   0        0        0        0 2021-08-28 01:05:02.415973 mapservice-clientlib-2.2.0/clients/query/__init__.py
--rw-r--r--   0        0        0      627 2021-08-28 01:05:02.416084 mapservice-clientlib-2.2.0/clients/query/actions.py
--rw-r--r--   0        0        0     3345 2021-08-28 01:05:02.416226 mapservice-clientlib-2.2.0/clients/query/arcgis.py
--rw-r--r--   0        0        0     8904 2021-08-28 01:05:02.416382 mapservice-clientlib-2.2.0/clients/query/fields.py
--rw-r--r--   0        0        0      301 2021-08-28 01:05:02.416516 mapservice-clientlib-2.2.0/clients/query/serializers.py
--rw-r--r--   0        0        0    13704 2022-10-04 20:59:57.909323 mapservice-clientlib-2.2.0/clients/resources.py
--rw-r--r--   0        0        0    17414 2022-10-04 20:59:57.909664 mapservice-clientlib-2.2.0/clients/sciencebase.py
--rw-r--r--   0        0        0      479 2021-08-28 01:05:02.417373 mapservice-clientlib-2.2.0/clients/tests/__init__.py
--rw-r--r--   0        0        0    56256 2021-08-28 01:05:02.417746 mapservice-clientlib-2.2.0/clients/tests/arcgis_tests.py
--rw-r--r--   0        0        0    12665 2021-08-28 01:05:02.417954 mapservice-clientlib-2.2.0/clients/tests/conversion_tests.py
--rw-r--r--   0        0        0      107 2021-08-28 01:05:02.418248 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/config-error.json
--rw-r--r--   0        0        0       18 2021-08-28 01:05:02.418386 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/empty-error.json
--rw-r--r--   0        0        0      884 2021-08-28 01:05:02.418544 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/error.html
--rw-r--r--   0        0        0       64 2021-08-28 01:05:02.418685 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-layer-ids.json
--rw-r--r--   0        0        0     3283 2021-08-28 01:05:02.418818 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-layer-version-error.json
--rw-r--r--   0        0        0     5479 2021-08-28 01:05:02.418969 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-layer.json
--rw-r--r--   0        0        0     2064 2021-08-28 01:05:02.419133 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-version-error.json
--rw-r--r--   0        0        0     2304 2021-08-28 01:05:02.419294 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature.json
--rw-r--r--   0        0        0      105 2021-08-28 01:05:02.419447 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/generic-error.json
--rw-r--r--   0        0        0      181 2021-08-28 01:05:02.419588 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/geometry.json
--rw-r--r--   0        0        0     2336 2021-08-28 01:05:02.419761 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/image-version-error.json
--rw-r--r--   0        0        0     6313 2021-08-28 01:05:02.419934 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/image.json
--rw-r--r--   0        0        0     1565 2021-08-28 01:05:02.420084 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-layer-version-error.json
--rw-r--r--   0        0        0     5291 2021-08-28 01:05:02.420249 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-layer.json
--rw-r--r--   0        0        0     6165 2021-08-28 01:05:02.420425 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-layers.json
--rw-r--r--   0        0        0     4000 2021-08-28 01:05:02.420579 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-legend.json
--rw-r--r--   0        0        0     1749 2021-08-28 01:05:02.420729 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-version-error.json
--rw-r--r--   0        0        0     5173 2021-08-28 01:05:02.420900 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map.json
--rw-r--r--   0        0        0     1464 2021-08-28 01:05:02.421155 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/no-feature-layer.json
--rw-r--r--   0        0        0       19 2021-08-28 01:05:02.421329 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/no-map-layers-layers.json
--rw-r--r--   0        0        0     1249 2021-08-28 01:05:02.421477 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/no-map-layers.json
--rw-r--r--   0        0        0      112 2021-08-28 01:05:02.421614 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/not-found.json
--rw-r--r--   0        0        0      155 2021-08-28 01:05:02.421825 mapservice-clientlib-2.2.0/clients/tests/data/arcgis/token-required.json
--rw-r--r--   0        0        0     1905 2021-08-28 01:05:02.422052 mapservice-clientlib-2.2.0/clients/tests/data/resources/test-client-bulk-keys.json
--rw-r--r--   0        0        0     1721 2021-08-28 01:05:02.422190 mapservice-clientlib-2.2.0/clients/tests/data/resources/test-client-bulk.json
--rw-r--r--   0        0        0      728 2021-08-28 01:05:02.422358 mapservice-clientlib-2.2.0/clients/tests/data/resources/test-client.json
--rw-r--r--   0        0        0      260 2021-08-28 01:05:02.422588 mapservice-clientlib-2.2.0/clients/tests/data/resources/test-invalid-json.html
--rw-r--r--   0        0        0       45 2021-08-28 01:05:02.422749 mapservice-clientlib-2.2.0/clients/tests/data/resources/test-invalid-max.json
--rw-r--r--   0        0        0       44 2021-08-28 01:05:02.422895 mapservice-clientlib-2.2.0/clients/tests/data/resources/test-invalid-min.json
--rw-r--r--   0        0        0     8726 2021-08-28 01:05:02.423165 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-item.json
--rw-r--r--   0        0        0     1394 2021-08-28 01:05:02.423326 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service-layer.json
--rw-r--r--   0        0        0     7957 2021-08-28 01:05:02.423486 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service-layers.json
--rw-r--r--   0        0        0     3230 2021-08-28 01:05:02.423632 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service-legend.json
--rw-r--r--   0        0        0     4644 2021-08-28 01:05:02.423780 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service.json
--rw-r--r--   0        0        0       76 2021-08-28 01:05:02.423940 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/deprecated.json
--rw-r--r--   0        0        0        3 2021-08-28 01:05:02.424156 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/empty-error.json
--rw-r--r--   0        0        0     3586 2021-08-28 01:05:02.424412 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/footprint.json
--rw-r--r--   0        0        0       60 2021-08-28 01:05:02.424551 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/message-error.json
--rw-r--r--   0        0        0      126 2021-08-28 01:05:02.424697 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/messages-error.json
--rw-r--r--   0        0        0     6424 2021-08-28 01:05:02.424909 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/missing-fields.json
--rw-r--r--   0        0        0      167 2021-08-28 01:05:02.425065 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/unpublished.json
--rw-r--r--   0        0        0    17722 2021-08-28 01:05:02.425227 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/wms-item.json
--rw-r--r--   0        0        0     9259 2021-08-28 01:05:02.425404 mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/wms-service.xml
--rw-r--r--   0        0        0      384 2021-08-28 01:05:02.425587 mapservice-clientlib-2.2.0/clients/tests/data/test.html
--rw-r--r--   0        0        0      583 2021-08-28 01:05:02.425721 mapservice-clientlib-2.2.0/clients/tests/data/test.jpeg
--rw-r--r--   0        0        0      110 2021-08-28 01:05:02.425915 mapservice-clientlib-2.2.0/clients/tests/data/test.png
--rw-r--r--   0        0        0     1079 2021-08-28 01:05:02.426169 mapservice-clientlib-2.2.0/clients/tests/data/thredds/invalid-iso-catalog.xml
--rw-r--r--   0        0        0     1079 2021-08-28 01:05:02.426338 mapservice-clientlib-2.2.0/clients/tests/data/thredds/invalid-wms-catalog.xml
--rw-r--r--   0        0        0      483 2021-08-28 01:05:02.426526 mapservice-clientlib-2.2.0/clients/tests/data/thredds/missing-dataset.xml
--rw-r--r--   0        0        0     1404 2021-08-28 01:05:02.426719 mapservice-clientlib-2.2.0/clients/tests/data/thredds/multiple-datasets.xml
--rw-r--r--   0        0        0     1092 2021-08-28 01:05:02.426863 mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-catalog.xml
--rw-r--r--   0        0        0      462 2021-08-28 01:05:02.427099 mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-layer.json
--rw-r--r--   0        0        0      381 2021-08-28 01:05:02.427261 mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-layers.json
--rw-r--r--   0        0        0   304926 2021-08-28 01:05:02.428147 mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-metadata.xml
--rw-r--r--   0        0        0     5709 2021-08-28 01:05:02.428430 mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-wms.xml
--rw-r--r--   0        0        0    10129 2021-08-28 01:05:02.428674 mapservice-clientlib-2.2.0/clients/tests/data/wms/demo-wms-max.xml
--rw-r--r--   0        0        0     8815 2021-08-28 01:05:02.428844 mapservice-clientlib-2.2.0/clients/tests/data/wms/demo-wms-min.xml
--rw-r--r--   0        0        0      464 2021-08-28 01:05:02.429030 mapservice-clientlib-2.2.0/clients/tests/data/wms/invalid-ncwms-layer.json
--rw-r--r--   0        0        0     4919 2021-08-28 01:05:02.429395 mapservice-clientlib-2.2.0/clients/tests/data/wms/invalid-wms-layer-extent.xml
--rw-r--r--   0        0        0     4539 2021-08-28 01:05:02.429643 mapservice-clientlib-2.2.0/clients/tests/data/wms/missing-wms-layer-extent.xml
--rw-r--r--   0        0        0     4313 2021-08-28 01:05:02.429846 mapservice-clientlib-2.2.0/clients/tests/data/wms/missing-wms-layers.xml
--rw-r--r--   0        0        0    29640 2021-08-28 01:05:02.430035 mapservice-clientlib-2.2.0/clients/tests/data/wms/ncwms-layer.json
--rw-r--r--   0        0        0    18693 2021-08-28 01:05:02.430250 mapservice-clientlib-2.2.0/clients/tests/data/wms/ncwms-max.xml
--rw-r--r--   0        0        0    19263 2021-08-28 01:05:02.430518 mapservice-clientlib-2.2.0/clients/tests/data/wms/ncwms-min.xml
--rw-r--r--   0        0        0      385 2021-08-28 01:05:02.430689 mapservice-clientlib-2.2.0/clients/tests/data/wms/service-exception.xml
--rw-r--r--   0        0        0     9155 2021-08-28 01:05:02.430842 mapservice-clientlib-2.2.0/clients/tests/data/wms/version-error.xml
--rw-r--r--   0        0        0    34519 2022-10-04 20:59:57.910044 mapservice-clientlib-2.2.0/clients/tests/geometry_tests.py
--rw-r--r--   0        0        0    16319 2021-08-28 01:05:02.431349 mapservice-clientlib-2.2.0/clients/tests/images_tests.py
--rw-r--r--   0        0        0    13551 2021-08-28 01:05:02.431576 mapservice-clientlib-2.2.0/clients/tests/query_tests.py
--rw-r--r--   0        0        0    14059 2021-08-28 01:05:02.431866 mapservice-clientlib-2.2.0/clients/tests/resource_tests.py
--rw-r--r--   0        0        0    33476 2022-10-04 20:59:57.910428 mapservice-clientlib-2.2.0/clients/tests/sciencebase_tests.py
--rw-r--r--   0        0        0    14900 2022-10-04 20:59:57.910747 mapservice-clientlib-2.2.0/clients/tests/thredds_tests.py
--rw-r--r--   0        0        0     9389 2021-08-28 01:05:02.432573 mapservice-clientlib-2.2.0/clients/tests/utils.py
--rw-r--r--   0        0        0    27699 2022-10-04 20:59:57.911089 mapservice-clientlib-2.2.0/clients/tests/wms_tests.py
--rw-r--r--   0        0        0    19907 2022-10-04 20:59:57.911547 mapservice-clientlib-2.2.0/clients/thredds.py
--rw-r--r--   0        0        0      329 2021-08-28 01:05:02.433346 mapservice-clientlib-2.2.0/clients/utils/__init__.py
--rw-r--r--   0        0        0     5124 2021-08-28 01:05:02.433711 mapservice-clientlib-2.2.0/clients/utils/conversion.py
--rw-r--r--   0        0        0    23397 2021-08-28 01:05:02.434166 mapservice-clientlib-2.2.0/clients/utils/geometry.py
--rw-r--r--   0        0        0     5358 2021-08-28 01:05:02.434478 mapservice-clientlib-2.2.0/clients/utils/images.py
--rw-r--r--   0        0        0    31226 2022-10-04 20:59:57.911964 mapservice-clientlib-2.2.0/clients/wms.py
--rw-r--r--   0        0        0      934 2022-10-04 21:19:58.578344 mapservice-clientlib-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     7273 1970-01-01 00:00:00.000000 mapservice-clientlib-2.2.0/setup.py
--rw-r--r--   0        0        0     7026 1970-01-01 00:00:00.000000 mapservice-clientlib-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1507 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/LICENSE
+-rw-r--r--   0        0        0     5830 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/__init__.py
+-rw-r--r--   0        0        0    43285 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/arcgis.py
+-rw-r--r--   0        0        0     3461 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/query/__init__.py
+-rw-r--r--   0        0        0      627 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/query/actions.py
+-rw-r--r--   0        0        0     3345 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/query/arcgis.py
+-rw-r--r--   0        0        0     8904 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/query/fields.py
+-rw-r--r--   0        0        0      301 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/query/serializers.py
+-rw-r--r--   0        0        0    13704 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/resources.py
+-rw-r--r--   0        0        0    17414 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/sciencebase.py
+-rw-r--r--   0        0        0      479 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/__init__.py
+-rw-r--r--   0        0        0    56256 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/arcgis_tests.py
+-rw-r--r--   0        0        0    12665 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/conversion_tests.py
+-rw-r--r--   0        0        0      107 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/config-error.json
+-rw-r--r--   0        0        0       18 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/empty-error.json
+-rw-r--r--   0        0        0      884 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/error.html
+-rw-r--r--   0        0        0       64 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-layer-ids.json
+-rw-r--r--   0        0        0     3283 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-layer-version-error.json
+-rw-r--r--   0        0        0     5479 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-layer.json
+-rw-r--r--   0        0        0     2064 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-version-error.json
+-rw-r--r--   0        0        0     2304 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature.json
+-rw-r--r--   0        0        0      105 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/generic-error.json
+-rw-r--r--   0        0        0      181 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/geometry.json
+-rw-r--r--   0        0        0     2336 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/image-version-error.json
+-rw-r--r--   0        0        0     6313 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/image.json
+-rw-r--r--   0        0        0     1565 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-layer-version-error.json
+-rw-r--r--   0        0        0     5291 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-layer.json
+-rw-r--r--   0        0        0     6165 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-layers.json
+-rw-r--r--   0        0        0     4000 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-legend.json
+-rw-r--r--   0        0        0     1749 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-version-error.json
+-rw-r--r--   0        0        0     5173 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map.json
+-rw-r--r--   0        0        0     1464 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/no-feature-layer.json
+-rw-r--r--   0        0        0       19 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/no-map-layers-layers.json
+-rw-r--r--   0        0        0     1249 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/no-map-layers.json
+-rw-r--r--   0        0        0      112 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/not-found.json
+-rw-r--r--   0        0        0      155 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/arcgis/token-required.json
+-rw-r--r--   0        0        0     1905 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/resources/test-client-bulk-keys.json
+-rw-r--r--   0        0        0     1721 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/resources/test-client-bulk.json
+-rw-r--r--   0        0        0      728 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/resources/test-client.json
+-rw-r--r--   0        0        0      260 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/resources/test-invalid-json.html
+-rw-r--r--   0        0        0       45 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/resources/test-invalid-max.json
+-rw-r--r--   0        0        0       44 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/resources/test-invalid-min.json
+-rw-r--r--   0        0        0     8726 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-item.json
+-rw-r--r--   0        0        0     1394 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service-layer.json
+-rw-r--r--   0        0        0     7957 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service-layers.json
+-rw-r--r--   0        0        0     3230 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service-legend.json
+-rw-r--r--   0        0        0     4644 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service.json
+-rw-r--r--   0        0        0       76 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/deprecated.json
+-rw-r--r--   0        0        0        3 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/empty-error.json
+-rw-r--r--   0        0        0     3586 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/footprint.json
+-rw-r--r--   0        0        0       60 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/message-error.json
+-rw-r--r--   0        0        0      126 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/messages-error.json
+-rw-r--r--   0        0        0     6424 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/missing-fields.json
+-rw-r--r--   0        0        0      167 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/unpublished.json
+-rw-r--r--   0        0        0    17722 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/wms-item.json
+-rw-r--r--   0        0        0     9259 2023-06-29 17:18:08.876129 mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/wms-service.xml
+-rw-r--r--   0        0        0      384 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/test.html
+-rw-r--r--   0        0        0      583 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/test.jpeg
+-rw-r--r--   0        0        0      110 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/test.png
+-rw-r--r--   0        0        0     1079 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/invalid-iso-catalog.xml
+-rw-r--r--   0        0        0     1079 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/invalid-wms-catalog.xml
+-rw-r--r--   0        0        0      483 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/missing-dataset.xml
+-rw-r--r--   0        0        0     1404 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/multiple-datasets.xml
+-rw-r--r--   0        0        0     1092 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-catalog.xml
+-rw-r--r--   0        0        0      462 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-layer.json
+-rw-r--r--   0        0        0      381 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-layers.json
+-rw-r--r--   0        0        0   304926 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-metadata.xml
+-rw-r--r--   0        0        0     5709 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-wms.xml
+-rw-r--r--   0        0        0    10129 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/demo-wms-max.xml
+-rw-r--r--   0        0        0     8815 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/demo-wms-min.xml
+-rw-r--r--   0        0        0      464 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/invalid-ncwms-layer.json
+-rw-r--r--   0        0        0     4919 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/invalid-wms-layer-extent.xml
+-rw-r--r--   0        0        0     4539 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/missing-wms-layer-extent.xml
+-rw-r--r--   0        0        0     4313 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/missing-wms-layers.xml
+-rw-r--r--   0        0        0    29640 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/ncwms-layer.json
+-rw-r--r--   0        0        0    18693 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/ncwms-max.xml
+-rw-r--r--   0        0        0    19263 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/ncwms-min.xml
+-rw-r--r--   0        0        0      385 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/service-exception.xml
+-rw-r--r--   0        0        0     9155 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/data/wms/version-error.xml
+-rw-r--r--   0        0        0    34519 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/geometry_tests.py
+-rw-r--r--   0        0        0    16319 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/images_tests.py
+-rw-r--r--   0        0        0    13551 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/query_tests.py
+-rw-r--r--   0        0        0    14059 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/resource_tests.py
+-rw-r--r--   0        0        0    33476 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/sciencebase_tests.py
+-rw-r--r--   0        0        0    14900 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/thredds_tests.py
+-rw-r--r--   0        0        0     9389 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/utils.py
+-rw-r--r--   0        0        0    27699 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/tests/wms_tests.py
+-rw-r--r--   0        0        0    19907 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/thredds.py
+-rw-r--r--   0        0        0      329 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/utils/__init__.py
+-rw-r--r--   0        0        0     5124 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/utils/conversion.py
+-rw-r--r--   0        0        0    23397 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/utils/geometry.py
+-rw-r--r--   0        0        0     5358 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/utils/images.py
+-rw-r--r--   0        0        0    31226 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/clients/wms.py
+-rw-r--r--   0        0        0      934 2023-06-29 17:18:08.880129 mapservice_clientlib-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7012 1970-01-01 00:00:00.000000 mapservice_clientlib-2.2.1/PKG-INFO
```

### Comparing `mapservice-clientlib-2.2.0/LICENSE` & `mapservice_clientlib-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/README.md` & `mapservice_clientlib-2.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # mapservice-clientlib
 
-[![Build Status](https://api.travis-ci.com/consbio/mapservice-clientlib.png?branch=main)](https://app.travis-ci.com/github/consbio/mapservice-clientlib)
+![Published](https://github.com/consbio/mapservice-clientlib/actions/workflows/publish.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/consbio/mapservice-clientlib/badge.svg?branch=main)](https://coveralls.io/github/consbio/mapservice-clientlib?branch=main)
 
-
 A library to make web service calls to map service REST APIs easier. Currently supported:
 
-* ArcGIS (version 10.1 and greater)
-* THREDDS
-* WMS / NcWMS (versions 1.1.1 and 1.3.0)
-* ScienceBase
+- ArcGIS (version 10.1 and greater)
+- THREDDS
+- WMS / NcWMS (versions 1.1.1 and 1.3.0)
+- ScienceBase
 
 Each leverages the [restle](https://github.com/consbio/restle) library to represent queried map service data as Python objects.
 Each also provides some default functionality for rendering projected map service data as images, which may be overridden per class as needed.
 
 Beyond this are some utilities for working with images (PIL) and extents (mostly Geographic, Web Mercator and other proj4 compatible projections).
 
 ## Installation
 
 Install with `pip install mapservice-clientlib`.
 
-
 ## Usage
 
 Below are some examples of each supported map service web API standard:
 
-
 ### ArcGIS Resources
 
 ArcGIS Map, Feature and Image services may be queried.
 
 ```python
 from clients.arcgis import MapServerResource, ArcGISSecureResource
 from clients.arcgis import FeatureLayerResource, FeatureServerResource, ImageServerResource
@@ -68,15 +65,14 @@
     spatial_reference={'wkid': 4326}
 )
 geometry_url = 'http://tasks.arcgisonline.com/arcgis/rest/services/Geometry/GeometryServer'
 client = GeometryServiceClient(geometry_url)
 extent = client.project_extent(old_extent, {'wkid': 3857}).limit_to_global_extent()
 ```
 
-
 ### WMS
 
 WMS services may be queried, with support for NcWMS
 
 ```python
 from clients.wms import WMSResource
 
@@ -95,15 +91,14 @@
     style_ids=[...],
     time_range="<wms_time_val>",
     params={...},  # Additional image params
     image_format="png"
 )
 ```
 
-
 ### THREDDS
 
 THREDDS resources may be queried, with metadata from related WMS endpoint:
 
 ```python
 from clients.thredds import ThreddsResource
 
@@ -122,15 +117,14 @@
     style_ids=[...],
     time_range="<wms_time_val>",
     params={...},  # Additional image params
     image_format="png"
 )
 ```
 
-
 ### ScienceBase
 
 Public and private ScienceBase items may be queried:
 
 ```python
 from clients.sciencebase import ScienceBaseResource, ScienceBaseSession
 
@@ -175,15 +169,14 @@
         "username": "arcgis_user",
         "password": "arcgis_pass"
     }
 )
 client.service_client.full_extent  # ArcGISResource.full_extent
 ```
 
-
 ### Extent Utilities
 
 Extent objects have a number of useful methods. Here are some examples that support projection:
 
 ```python
 from clients.utils.geometry import Extent
```

### Comparing `mapservice-clientlib-2.2.0/clients/arcgis.py` & `mapservice_clientlib-2.2.1/clients/arcgis.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/exceptions.py` & `mapservice_clientlib-2.2.1/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/query/actions.py` & `mapservice_clientlib-2.2.1/clients/query/actions.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/query/arcgis.py` & `mapservice_clientlib-2.2.1/clients/query/arcgis.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/query/fields.py` & `mapservice_clientlib-2.2.1/clients/query/fields.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/resources.py` & `mapservice_clientlib-2.2.1/clients/resources.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/sciencebase.py` & `mapservice_clientlib-2.2.1/clients/sciencebase.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/arcgis_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/arcgis_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/conversion_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/conversion_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/error.html` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/error.html`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-layer-version-error.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-layer-version-error.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-layer.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-layer.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature-version-error.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature-version-error.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/feature.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/feature.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/image-version-error.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/image-version-error.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/image.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/image.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-layer-version-error.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-layer-version-error.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-layer.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-layer.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-layers.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-layers.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-legend.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-legend.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map-version-error.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map-version-error.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/map.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/map.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/no-feature-layer.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/no-feature-layer.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/arcgis/no-map-layers.json` & `mapservice_clientlib-2.2.1/clients/tests/data/arcgis/no-map-layers.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/resources/test-client-bulk-keys.json` & `mapservice_clientlib-2.2.1/clients/tests/data/resources/test-client-bulk-keys.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/resources/test-client-bulk.json` & `mapservice_clientlib-2.2.1/clients/tests/data/resources/test-client-bulk.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/resources/test-client.json` & `mapservice_clientlib-2.2.1/clients/tests/data/resources/test-client.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-item.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-item.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service-layer.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service-layer.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service-layers.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service-layers.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service-legend.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service-legend.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/arcgis-service.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/arcgis-service.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/footprint.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/footprint.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/missing-fields.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/missing-fields.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/wms-item.json` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/wms-item.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/sciencebase/wms-service.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/sciencebase/wms-service.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/test.jpeg` & `mapservice_clientlib-2.2.1/clients/tests/data/test.jpeg`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/thredds/invalid-iso-catalog.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/thredds/invalid-iso-catalog.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/thredds/invalid-wms-catalog.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/thredds/invalid-wms-catalog.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/thredds/multiple-datasets.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/thredds/multiple-datasets.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-catalog.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-catalog.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-metadata.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-metadata.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/thredds/thredds-wms.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/thredds/thredds-wms.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/demo-wms-max.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/demo-wms-max.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/demo-wms-min.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/demo-wms-min.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/invalid-wms-layer-extent.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/invalid-wms-layer-extent.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/missing-wms-layer-extent.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/missing-wms-layer-extent.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/missing-wms-layers.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/missing-wms-layers.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/ncwms-layer.json` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/ncwms-layer.json`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/ncwms-max.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/ncwms-max.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/ncwms-min.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/ncwms-min.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/data/wms/version-error.xml` & `mapservice_clientlib-2.2.1/clients/tests/data/wms/version-error.xml`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/geometry_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/geometry_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/images_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/images_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/query_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/query_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/resource_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/resource_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/sciencebase_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/sciencebase_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/thredds_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/thredds_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/utils.py` & `mapservice_clientlib-2.2.1/clients/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/tests/wms_tests.py` & `mapservice_clientlib-2.2.1/clients/tests/wms_tests.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/thredds.py` & `mapservice_clientlib-2.2.1/clients/thredds.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/utils/conversion.py` & `mapservice_clientlib-2.2.1/clients/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/utils/geometry.py` & `mapservice_clientlib-2.2.1/clients/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/utils/images.py` & `mapservice_clientlib-2.2.1/clients/utils/images.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/clients/wms.py` & `mapservice_clientlib-2.2.1/clients/wms.py`

 * *Files identical despite different names*

### Comparing `mapservice-clientlib-2.2.0/pyproject.toml` & `mapservice_clientlib-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mapservice-clientlib"
-version = "2.2.0"
+version = "2.2.1"
 description = "Library to query mapservices including ArcGIS, THREDDS, WMS and ScienceBase"
 authors = ["dharvey-consbio <dani.harvey@consbio.org>"]
 keywords = ["arcgis", "thredds", "ncwms", "wms", "sciencebase", "geospatial", "gis", "mapservice", "map service", "clients", "mapservice_clientlib"]
 readme = "README.md"
 homepage = "https://github.com/consbio/mapservice-clientlib/"
 repository = "https://github.com/consbio/mapservice-clientlib/"
 license = "BSD"
```

### Comparing `mapservice-clientlib-2.2.0/setup.py` & `mapservice_clientlib-2.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,224 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mapservice-clientlib
+Version: 2.2.1
+Summary: Library to query mapservices including ArcGIS, THREDDS, WMS and ScienceBase
+Home-page: https://github.com/consbio/mapservice-clientlib/
+License: BSD
+Keywords: arcgis,thredds,ncwms,wms,sciencebase,geospatial,gis,mapservice,map service,clients,mapservice_clientlib
+Author: dharvey-consbio
+Author-email: dani.harvey@consbio.org
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (==7.2.*)
+Requires-Dist: gis-metadata-parser (>=2.0,<3.0)
+Requires-Dist: parserutils (>=2.0.1,<3.0.0)
+Requires-Dist: pyproj (>=3.2.1,<4.0.0)
+Requires-Dist: python-ags (>=0.3.2,<0.4.0)
+Requires-Dist: restle (>=0.5.1,<0.6.0)
+Requires-Dist: sciencebasepy (>=2.0.4,<3.0.0)
+Project-URL: Repository, https://github.com/consbio/mapservice-clientlib/
+Description-Content-Type: text/markdown
+
+# mapservice-clientlib
+
+![Published](https://github.com/consbio/mapservice-clientlib/actions/workflows/publish.yml/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/consbio/mapservice-clientlib/badge.svg?branch=main)](https://coveralls.io/github/consbio/mapservice-clientlib?branch=main)
+
+A library to make web service calls to map service REST APIs easier. Currently supported:
+
+- ArcGIS (version 10.1 and greater)
+- THREDDS
+- WMS / NcWMS (versions 1.1.1 and 1.3.0)
+- ScienceBase
+
+Each leverages the [restle](https://github.com/consbio/restle) library to represent queried map service data as Python objects.
+Each also provides some default functionality for rendering projected map service data as images, which may be overridden per class as needed.
+
+Beyond this are some utilities for working with images (PIL) and extents (mostly Geographic, Web Mercator and other proj4 compatible projections).
+
+## Installation
+
+Install with `pip install mapservice-clientlib`.
+
+## Usage
+
+Below are some examples of each supported map service web API standard:
+
+### ArcGIS Resources
+
+ArcGIS Map, Feature and Image services may be queried.
+
+```python
+from clients.arcgis import MapServerResource, ArcGISSecureResource
+from clients.arcgis import FeatureLayerResource, FeatureServerResource, ImageServerResource
+from clients.utils.geometry import Extent
+
+
+# Query the feature service, or an individual layer (lazy=False: query executed right away)
+client = FeatureServerResource.get(service_url, lazy=False)
+layer = FeatureLayerResource.get(service_url + "/0", lazy=False)
+
+# Query an image service lazily (default behavior: executes query on property reference)
+client = ImageServerResource.get(service_url, lazy=True)
+client.extent  # Query executes here
+
+# Query a map service and generate an image
+arcgis_image = MapServerResource.get(service_url).get_image(
+    extent, width=400, height=200,
+    layers="show:0",
+    layer_defs="<arcgis_layer_defs>",
+    time="<arcgis_time_val>",
+    custom_renderers={}  # Renderer JSON
+)
+
+# Query a secure map service (generates token from URL and credentials)
+client = MapServerResource.get(service_url, username="user", password="pass")
+
+# Query a secure map service with existing token
+token_obj = ArcGISSecureResource.generate_token(
+    service_url, "user", "pass",  duration=15
+)
+client = MapServerResource.get(service_url, token=token_obj.token)
+
+# Reproject an ArcGIS extent to Web Mercator
+old_extent = Extent(
+    {'xmin': -180.0000, 'xmax': 180.0000, 'ymin': -90.0000, 'ymax': 90.0000},
+    spatial_reference={'wkid': 4326}
+)
+geometry_url = 'http://tasks.arcgisonline.com/arcgis/rest/services/Geometry/GeometryServer'
+client = GeometryServiceClient(geometry_url)
+extent = client.project_extent(old_extent, {'wkid': 3857}).limit_to_global_extent()
+```
+
+### WMS
+
+WMS services may be queried, with support for NcWMS
+
+```python
+from clients.wms import WMSResource
+
+
+# Query a secure WMS service
+client = WMSResource.get(
+    url=wms_url, token="token", token_id="josso", version="1.3.0", spatial_ref="EPSG:3857"
+)
+
+# Query a public WMS service and generate an image (supports NcWMS as well)
+wms_image = WMSResource.get(
+    wms_url
+).get_image(
+    extent, width=400, height=200,
+    layer_ids=[...],
+    style_ids=[...],
+    time_range="<wms_time_val>",
+    params={...},  # Additional image params
+    image_format="png"
+)
+```
+
+### THREDDS
+
+THREDDS resources may be queried, with metadata from related WMS endpoint:
+
+```python
+from clients.thredds import ThreddsResource
+
+
+client = ThreddsResource.get(url)
+
+# See gis-metadata-parser for more
+metadata = client._metadata_parser
+metadata.data_credits
+metadata.use_constraints
+
+# Makes a WMS image request
+thredds_image = client.get_image(
+    extent, width, height,
+    layer_ids=[...],
+    style_ids=[...],
+    time_range="<wms_time_val>",
+    params={...},  # Additional image params
+    image_format="png"
+)
+```
+
+### ScienceBase
+
+Public and private ScienceBase items may be queried:
+
+```python
+from clients.sciencebase import ScienceBaseResource, ScienceBaseSession
+
+
+# Query a public ScienceBase item
+client = ScienceBaseResource.get(service_url, lazy=False)
+client.summary
+
+# Query a private WMS-backed ScienceBase item
+
+sb_session = ScienceBaseSession(
+    josso_session_id="token",
+    username="sciencebase_user"
+)
+sb_session.login("sciencebase_user", "pass")
+
+client = ScienceBaseResource.get(
+    url=service_url,
+    lazy=False,
+    session=sb_session,
+    # Same token for WMS as for base item
+    token=sb_session._jossosessionid
+)
+client.service_client.full_extent  # WMSResource.full_extent
+
+# Query a private ArcGIS-backed ScienceBase item
+
+sb_session = ScienceBaseSession(
+    josso_session_id="token",
+    username="sciencebase_user"
+)
+sb_session.login("sciencebase_user", "pass")
+
+client = ScienceBaseResource.get(
+    url=service_url,
+    lazy=False,
+    session=sb_session,
+    token=sb_session._jossosessionid,
+    # Separate credentials for ArcGIS service
+    arcgis_credentials={
+        # Or just use "token": "existing_token"
+        "username": "arcgis_user",
+        "password": "arcgis_pass"
+    }
+)
+client.service_client.full_extent  # ArcGISResource.full_extent
+```
+
+### Extent Utilities
+
+Extent objects have a number of useful methods. Here are some examples that support projection:
+
+```python
+from clients.utils.geometry import Extent
+
+
+extent_from_dict = Extent({
+    "xmin": -180.0, "ymin": -90.0, "xmax": 180.0, "ymax": 90.0,
+    "spatial_reference": {"wkid": 4326}
+})
+web_mercator_extent = extent_from_dict.project_to_web_mercator()
+
+extent_from_list = Extent(
+    # In order of xmin, ymin, xmax, ymax
+    [-20037508.342789244, -20037471.205137067, 20037508.342789244, 20037471.20513706],
+    spatial_reference="EPSG:3857"
+)
+geographic_extent = extent_from_dict.project_to_geographic()
+```
 
-packages = \
-['clients', 'clients.query', 'clients.tests', 'clients.utils']
-
-package_data = \
-{'': ['*'],
- 'clients.tests': ['data/*',
-                   'data/arcgis/*',
-                   'data/resources/*',
-                   'data/sciencebase/*',
-                   'data/thredds/*',
-                   'data/wms/*']}
-
-install_requires = \
-['Pillow>=7.2.0,<7.3.0',
- 'gis-metadata-parser>=2.0,<3.0',
- 'parserutils>=2.0.1,<3.0.0',
- 'pyproj>=3.2.1,<4.0.0',
- 'python-ags>=0.3.2,<0.4.0',
- 'restle>=0.5.1,<0.6.0',
- 'sciencebasepy>=2.0.4,<3.0.0']
-
-setup_kwargs = {
-    'name': 'mapservice-clientlib',
-    'version': '2.2.0',
-    'description': 'Library to query mapservices including ArcGIS, THREDDS, WMS and ScienceBase',
-    'long_description': '# mapservice-clientlib\n\n[![Build Status](https://api.travis-ci.com/consbio/mapservice-clientlib.png?branch=main)](https://app.travis-ci.com/github/consbio/mapservice-clientlib)\n[![Coverage Status](https://coveralls.io/repos/github/consbio/mapservice-clientlib/badge.svg?branch=main)](https://coveralls.io/github/consbio/mapservice-clientlib?branch=main)\n\n\nA library to make web service calls to map service REST APIs easier. Currently supported:\n\n* ArcGIS (version 10.1 and greater)\n* THREDDS\n* WMS / NcWMS (versions 1.1.1 and 1.3.0)\n* ScienceBase\n\nEach leverages the [restle](https://github.com/consbio/restle) library to represent queried map service data as Python objects.\nEach also provides some default functionality for rendering projected map service data as images, which may be overridden per class as needed.\n\nBeyond this are some utilities for working with images (PIL) and extents (mostly Geographic, Web Mercator and other proj4 compatible projections).\n\n## Installation\n\nInstall with `pip install mapservice-clientlib`.\n\n\n## Usage\n\nBelow are some examples of each supported map service web API standard:\n\n\n### ArcGIS Resources\n\nArcGIS Map, Feature and Image services may be queried.\n\n```python\nfrom clients.arcgis import MapServerResource, ArcGISSecureResource\nfrom clients.arcgis import FeatureLayerResource, FeatureServerResource, ImageServerResource\nfrom clients.utils.geometry import Extent\n\n\n# Query the feature service, or an individual layer (lazy=False: query executed right away)\nclient = FeatureServerResource.get(service_url, lazy=False)\nlayer = FeatureLayerResource.get(service_url + "/0", lazy=False)\n\n# Query an image service lazily (default behavior: executes query on property reference)\nclient = ImageServerResource.get(service_url, lazy=True)\nclient.extent  # Query executes here\n\n# Query a map service and generate an image\narcgis_image = MapServerResource.get(service_url).get_image(\n    extent, width=400, height=200,\n    layers="show:0",\n    layer_defs="<arcgis_layer_defs>",\n    time="<arcgis_time_val>",\n    custom_renderers={}  # Renderer JSON\n)\n\n# Query a secure map service (generates token from URL and credentials)\nclient = MapServerResource.get(service_url, username="user", password="pass")\n\n# Query a secure map service with existing token\ntoken_obj = ArcGISSecureResource.generate_token(\n    service_url, "user", "pass",  duration=15\n)\nclient = MapServerResource.get(service_url, token=token_obj.token)\n\n# Reproject an ArcGIS extent to Web Mercator\nold_extent = Extent(\n    {\'xmin\': -180.0000, \'xmax\': 180.0000, \'ymin\': -90.0000, \'ymax\': 90.0000},\n    spatial_reference={\'wkid\': 4326}\n)\ngeometry_url = \'http://tasks.arcgisonline.com/arcgis/rest/services/Geometry/GeometryServer\'\nclient = GeometryServiceClient(geometry_url)\nextent = client.project_extent(old_extent, {\'wkid\': 3857}).limit_to_global_extent()\n```\n\n\n### WMS\n\nWMS services may be queried, with support for NcWMS\n\n```python\nfrom clients.wms import WMSResource\n\n\n# Query a secure WMS service\nclient = WMSResource.get(\n    url=wms_url, token="token", token_id="josso", version="1.3.0", spatial_ref="EPSG:3857"\n)\n\n# Query a public WMS service and generate an image (supports NcWMS as well)\nwms_image = WMSResource.get(\n    wms_url\n).get_image(\n    extent, width=400, height=200,\n    layer_ids=[...],\n    style_ids=[...],\n    time_range="<wms_time_val>",\n    params={...},  # Additional image params\n    image_format="png"\n)\n```\n\n\n### THREDDS\n\nTHREDDS resources may be queried, with metadata from related WMS endpoint:\n\n```python\nfrom clients.thredds import ThreddsResource\n\n\nclient = ThreddsResource.get(url)\n\n# See gis-metadata-parser for more\nmetadata = client._metadata_parser\nmetadata.data_credits\nmetadata.use_constraints\n\n# Makes a WMS image request\nthredds_image = client.get_image(\n    extent, width, height,\n    layer_ids=[...],\n    style_ids=[...],\n    time_range="<wms_time_val>",\n    params={...},  # Additional image params\n    image_format="png"\n)\n```\n\n\n### ScienceBase\n\nPublic and private ScienceBase items may be queried:\n\n```python\nfrom clients.sciencebase import ScienceBaseResource, ScienceBaseSession\n\n\n# Query a public ScienceBase item\nclient = ScienceBaseResource.get(service_url, lazy=False)\nclient.summary\n\n# Query a private WMS-backed ScienceBase item\n\nsb_session = ScienceBaseSession(\n    josso_session_id="token",\n    username="sciencebase_user"\n)\nsb_session.login("sciencebase_user", "pass")\n\nclient = ScienceBaseResource.get(\n    url=service_url,\n    lazy=False,\n    session=sb_session,\n    # Same token for WMS as for base item\n    token=sb_session._jossosessionid\n)\nclient.service_client.full_extent  # WMSResource.full_extent\n\n# Query a private ArcGIS-backed ScienceBase item\n\nsb_session = ScienceBaseSession(\n    josso_session_id="token",\n    username="sciencebase_user"\n)\nsb_session.login("sciencebase_user", "pass")\n\nclient = ScienceBaseResource.get(\n    url=service_url,\n    lazy=False,\n    session=sb_session,\n    token=sb_session._jossosessionid,\n    # Separate credentials for ArcGIS service\n    arcgis_credentials={\n        # Or just use "token": "existing_token"\n        "username": "arcgis_user",\n        "password": "arcgis_pass"\n    }\n)\nclient.service_client.full_extent  # ArcGISResource.full_extent\n```\n\n\n### Extent Utilities\n\nExtent objects have a number of useful methods. Here are some examples that support projection:\n\n```python\nfrom clients.utils.geometry import Extent\n\n\nextent_from_dict = Extent({\n    "xmin": -180.0, "ymin": -90.0, "xmax": 180.0, "ymax": 90.0,\n    "spatial_reference": {"wkid": 4326}\n})\nweb_mercator_extent = extent_from_dict.project_to_web_mercator()\n\nextent_from_list = Extent(\n    # In order of xmin, ymin, xmax, ymax\n    [-20037508.342789244, -20037471.205137067, 20037508.342789244, 20037471.20513706],\n    spatial_reference="EPSG:3857"\n)\ngeographic_extent = extent_from_dict.project_to_geographic()\n```\n',
-    'author': 'dharvey-consbio',
-    'author_email': 'dani.harvey@consbio.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/consbio/mapservice-clientlib/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

