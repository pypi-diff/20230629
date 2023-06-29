# Comparing `tmp/folio_migration_tools-1.8.0rc8.tar.gz` & `tmp/folio_migration_tools-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folio_migration_tools-1.8.0rc8.tar", max compression
+gzip compressed data, was "folio_migration_tools-1.8.1.tar", max compression
```

## Comparing `folio_migration_tools-1.8.0rc8.tar` & `folio_migration_tools-1.8.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.0rc8/LICENSE
--rw-r--r--   0        0        0     4193 2023-03-21 14:28:28.887645 folio_migration_tools-1.8.0rc8/README.md
--rw-r--r--   0        0        0     1748 2023-05-15 11:37:25.726916 folio_migration_tools-1.8.0rc8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/__init__.py
--rw-r--r--   0        0        0     5322 2023-05-15 11:23:50.124863 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/__main__.py
--rw-r--r--   0        0        0    14007 2023-05-15 11:23:50.267365 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/circulation_helper.py
--rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/colors.py
--rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_dict.py
--rw-r--r--   0        0        0     2488 2023-05-15 11:23:50.020165 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_exceptions.py
--rw-r--r--   0        0        0     1678 2023-03-06 22:17:01.812068 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/extradata_writer.py
--rw-r--r--   0        0        0     6573 2023-03-06 22:17:01.812324 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/folder_structure.py
--rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/helper.py
--rw-r--r--   0        0        0     7089 2023-03-06 22:17:01.812878 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/holdings_helper.py
--rw-r--r--   0        0        0     2636 2023-04-18 23:46:20.197850 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/library_configuration.py
--rw-r--r--   0        0        0    19557 2023-05-15 11:23:50.020857 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapper_base.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/__init__.py
--rw-r--r--   0        0        0     8117 2023-04-19 02:19:29.600062 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
--rw-r--r--   0        0        0     6423 2023-04-19 02:19:29.616368 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
--rw-r--r--   0        0        0    10080 2023-05-03 19:02:35.234989 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
--rw-r--r--   0        0        0    13432 2023-05-15 11:23:50.021671 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
--rw-r--r--   0        0        0    37969 2023-05-15 11:23:50.022160 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
--rw-r--r--   0        0        0     3456 2023-05-15 11:23:50.022533 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
--rw-r--r--   0        0        0    16822 2023-05-15 11:23:50.080287 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
--rw-r--r--   0        0        0    14644 2023-05-15 11:23:50.103757 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
--rw-r--r--   0        0        0     8855 2023-05-03 19:02:35.238368 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
--rw-r--r--   0        0        0     7683 2023-04-19 02:19:29.634576 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/__init__.py
--rw-r--r--   0        0        0    34047 2023-04-18 23:46:20.215442 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/conditions.py
--rw-r--r--   0        0        0    11297 2023-03-06 22:17:01.817193 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
--rw-r--r--   0        0        0     9386 2023-05-15 11:23:50.081780 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
--rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
--rw-r--r--   0        0        0    10697 2023-05-15 11:23:50.218672 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
--rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
--rw-r--r--   0        0        0     5850 2023-03-27 22:22:56.116126 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
--rw-r--r--   0        0        0    34454 2023-04-17 23:01:11.524015 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
--rw-r--r--   0        0        0    25845 2023-04-17 23:01:11.525499 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
--rw-r--r--   0        0        0    17417 2023-04-17 23:01:11.530990 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
--rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_report.py
--rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-17 23:01:11.544786 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/authority_transformer.py
--rw-r--r--   0        0        0    28090 2023-05-15 11:23:50.202973 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/batch_poster.py
--rw-r--r--   0        0        0     7360 2023-04-19 02:19:29.638089 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/bibs_transformer.py
--rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/courses_migrator.py
--rw-r--r--   0        0        0    19445 2023-05-15 11:23:50.252409 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
--rw-r--r--   0        0        0     9602 2023-04-19 02:19:29.644858 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
--rw-r--r--   0        0        0    14990 2023-04-17 23:01:11.562933 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/items_transformer.py
--rw-r--r--   0        0        0    32162 2023-05-15 11:23:50.083455 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/loans_migrator.py
--rw-r--r--   0        0        0     7325 2023-05-15 11:23:50.028181 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
--rw-r--r--   0        0        0    13448 2023-05-15 11:23:50.029279 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/migration_task_base.py
--rw-r--r--   0        0        0    11392 2023-05-15 11:23:50.030013 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/orders_transformer.py
--rw-r--r--   0        0        0    14832 2023-05-15 11:23:50.030305 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/organization_transformer.py
--rw-r--r--   0        0        0    12990 2023-03-06 22:17:01.823855 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/requests_migrator.py
--rw-r--r--   0        0        0     8868 2023-05-15 11:23:50.084036 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/reserves_migrator.py
--rw-r--r--   0        0        0     9919 2023-05-15 11:23:50.032346 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/user_transformer.py
--rw-r--r--   0        0        0    16086 2023-05-15 11:23:50.033320 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/report_blurbs.py
--rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/task_configuration.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/test_infrastructure/__init__.py
--rw-r--r--   0        0        0     9150 2023-05-15 11:23:50.033592 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/test_infrastructure/mocked_classes.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/__init__.py
--rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_loan.py
--rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_request.py
--rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_reserve.py
--rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/transaction_result.py
--rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc8/setup.py
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.1/LICENSE
+-rw-r--r--   0        0        0     4193 2023-06-08 16:57:16.396521 folio_migration_tools-1.8.1/README.md
+-rw-r--r--   0        0        0     1742 2023-06-29 09:10:46.119130 folio_migration_tools-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.1/src/folio_migration_tools/__init__.py
+-rw-r--r--   0        0        0     5322 2023-06-08 16:57:16.409747 folio_migration_tools-1.8.1/src/folio_migration_tools/__main__.py
+-rw-r--r--   0        0        0    14007 2023-06-08 16:57:16.410871 folio_migration_tools-1.8.1/src/folio_migration_tools/circulation_helper.py
+-rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.1/src/folio_migration_tools/colors.py
+-rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.1/src/folio_migration_tools/custom_dict.py
+-rw-r--r--   0        0        0     2488 2023-06-08 16:57:16.411473 folio_migration_tools-1.8.1/src/folio_migration_tools/custom_exceptions.py
+-rw-r--r--   0        0        0     1678 2023-06-08 16:57:16.411848 folio_migration_tools-1.8.1/src/folio_migration_tools/extradata_writer.py
+-rw-r--r--   0        0        0     6573 2023-06-08 16:57:16.412056 folio_migration_tools-1.8.1/src/folio_migration_tools/folder_structure.py
+-rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.1/src/folio_migration_tools/helper.py
+-rw-r--r--   0        0        0     7478 2023-06-12 05:09:55.289424 folio_migration_tools-1.8.1/src/folio_migration_tools/holdings_helper.py
+-rw-r--r--   0        0        0     2636 2023-06-08 16:57:16.413411 folio_migration_tools-1.8.1/src/folio_migration_tools/library_configuration.py
+-rw-r--r--   0        0        0    19557 2023-06-08 16:57:16.414408 folio_migration_tools-1.8.1/src/folio_migration_tools/mapper_base.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/__init__.py
+-rw-r--r--   0        0        0     8117 2023-06-08 16:57:16.415441 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
+-rw-r--r--   0        0        0     6918 2023-06-12 05:09:55.289906 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
+-rw-r--r--   0        0        0    10495 2023-06-12 05:09:55.290349 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
+-rw-r--r--   0        0        0    13432 2023-06-08 16:57:16.417193 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
+-rw-r--r--   0        0        0    37969 2023-06-08 16:57:16.417837 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
+-rw-r--r--   0        0        0     3456 2023-06-22 06:35:48.233117 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
+-rw-r--r--   0        0        0    16822 2023-06-08 16:57:16.418987 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
+-rw-r--r--   0        0        0    14644 2023-06-08 16:57:16.419725 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
+-rw-r--r--   0        0        0     8855 2023-06-08 16:57:16.420433 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
+-rw-r--r--   0        0        0     7683 2023-06-08 16:57:16.421066 folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/__init__.py
+-rw-r--r--   0        0        0    34332 2023-06-29 08:51:14.839405 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/conditions.py
+-rw-r--r--   0        0        0    11619 2023-06-12 05:09:55.290715 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
+-rw-r--r--   0        0        0     9459 2023-06-29 08:51:14.840095 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
+-rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
+-rw-r--r--   0        0        0    10746 2023-06-12 05:09:55.291351 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
+-rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
+-rw-r--r--   0        0        0     5850 2023-06-08 16:57:16.424901 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
+-rw-r--r--   0        0        0    34817 2023-06-29 08:51:14.840839 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
+-rw-r--r--   0        0        0    25845 2023-06-08 16:57:16.426204 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
+-rw-r--r--   0        0        0    17591 2023-06-29 08:51:14.841479 folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
+-rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_report.py
+-rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/__init__.py
+-rw-r--r--   0        0        0     4231 2023-06-08 16:57:16.428070 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/authority_transformer.py
+-rw-r--r--   0        0        0    28090 2023-06-08 16:57:16.429041 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/batch_poster.py
+-rw-r--r--   0        0        0     7360 2023-06-08 16:57:16.430011 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/bibs_transformer.py
+-rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/courses_migrator.py
+-rw-r--r--   0        0        0    19445 2023-06-08 16:57:16.430863 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
+-rw-r--r--   0        0        0     9602 2023-06-08 16:57:16.431740 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
+-rw-r--r--   0        0        0    15071 2023-06-12 05:09:55.292928 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/items_transformer.py
+-rw-r--r--   0        0        0    32942 2023-06-29 08:51:14.842251 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/loans_migrator.py
+-rw-r--r--   0        0        0     7325 2023-06-08 16:57:16.434313 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
+-rw-r--r--   0        0        0    13448 2023-06-08 16:57:16.435049 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/migration_task_base.py
+-rw-r--r--   0        0        0    11392 2023-06-08 16:57:16.435218 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/orders_transformer.py
+-rw-r--r--   0        0        0    14832 2023-06-08 16:57:16.435485 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/organization_transformer.py
+-rw-r--r--   0        0        0    12990 2023-06-08 16:57:16.436019 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/requests_migrator.py
+-rw-r--r--   0        0        0     8868 2023-06-08 16:57:16.436883 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/reserves_migrator.py
+-rw-r--r--   0        0        0     9919 2023-06-08 16:57:16.437685 folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/user_transformer.py
+-rw-r--r--   0        0        0    16086 2023-06-08 16:57:16.438557 folio_migration_tools-1.8.1/src/folio_migration_tools/report_blurbs.py
+-rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.1/src/folio_migration_tools/task_configuration.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.1/src/folio_migration_tools/test_infrastructure/__init__.py
+-rw-r--r--   0        0        0     9150 2023-06-08 16:57:16.438864 folio_migration_tools-1.8.1/src/folio_migration_tools/test_infrastructure/mocked_classes.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/__init__.py
+-rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/legacy_loan.py
+-rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/legacy_request.py
+-rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/legacy_reserve.py
+-rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/transaction_result.py
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.1/setup.py
+-rw-r--r--   0        0        0     5441 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.1/PKG-INFO
```

### Comparing `folio_migration_tools-1.8.0rc8/LICENSE` & `folio_migration_tools-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/README.md` & `folio_migration_tools-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/pyproject.toml` & `folio_migration_tools-1.8.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "folio_migration_tools"
-version = "1.8.0rc8"
+version = "1.8.1"
 description =  "A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP"
 authors = ["Theodor Tolstoy <github.teddes@tolstoy.se>", "Lisa Sjögren", "Brooks Travis"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/FOLIO-FSE/folio_migration_tools"
 repository = "https://github.com/FOLIO-FSE/folio_migration_tools"
 keywords = ["FOLIO", "ILS", "LSP", "Library Systems", "MARC21", "Library data"]
@@ -29,20 +29,20 @@
 
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-folioclient = "^0.50.0rc1"
+folioclient = "^0.50.0"
 pyhumps = "^3.7.3"
 defusedxml = "^0.7.1"
 python-dateutil = "^2.8.2"
 folio-uuid = "^0.2.8"
-pymarc = "^4.2.1"
+pymarc = "^5.0.0"
 pydantic = "^1.10.2"
 argparse-prompt = "^0.0.5"
 deepdiff = "^6.2.3"
 pyaml = "^21.10.1"
 httpx = "^0.23.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/__main__.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/circulation_helper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/circulation_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_dict.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/custom_dict.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/custom_exceptions.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/extradata_writer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/extradata_writer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/folder_structure.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/folder_structure.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/helper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/holdings_helper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/holdings_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         extend_list("holdingsStatements", holdings_record, incoming_holdings, True)
         extend_list("holdingsStatementsForSupplements", holdings_record, incoming_holdings, True)
         extend_list("notes", holdings_record, incoming_holdings)
         holdings_record["notes"] = dedupe(holdings_record.get("notes", []))
         extend_list("formerIds", holdings_record, incoming_holdings)
         extend_list("electronicAccess", holdings_record, incoming_holdings)
         HoldingsHelper.remove_empty_holdings_statements(holdings_record)
+        merge_boolean("discoverySuppress", holdings_record, incoming_holdings)
         return holdings_record
 
     @staticmethod
     def remove_empty_holdings_statements(holdings_record: dict):
         keys = [
             "holdingsStatements",
             "holdingsStatementsForIndexes",
@@ -162,7 +163,17 @@
             temp.append(f)
     if temp:
         holdings_record[prop_name] = temp
 
 
 def dedupe(list_of_dicts):
     return [dict(t) for t in {tuple(d.items()) for d in list_of_dicts}]
+
+
+def merge_boolean(prop_name: str, holdings_record: dict, incoming_holdings: dict):
+    if (
+        holdings_record.get(prop_name, False) is True
+        and incoming_holdings.get(prop_name, False) is True
+    ):
+        holdings_record[prop_name] = True
+    else:
+        holdings_record[prop_name] = False
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/library_configuration.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/library_configuration.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapper_base.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 
 from folio_uuid.folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
 
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
+from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
 from folio_migration_tools.mapping_file_transformation.ref_data_mapping import (
     RefDataMapping,
 )
@@ -51,14 +52,24 @@
                 "/call-number-types",
                 "callNumberTypes",
                 call_number_type_map,
                 "name",
                 Blurbs.CallNumberTypeMapping,
             )
 
+    def perform_additional_mappings(self, folio_rec, file_def):
+        self.handle_suppression(folio_rec, file_def)
+
+    def handle_suppression(self, folio_record, file_def: FileDefinition):
+        folio_record["discoverySuppress"] = file_def.discovery_suppressed
+        self.migration_report.add(
+            Blurbs.Suppression,
+            f'Suppressed from discovery = {folio_record["discoverySuppress"]}',
+        )
+
     def get_prop(self, legacy_item, folio_prop_name, index_or_id, schema_default_value):
         if folio_prop_name == "permanentLocationId":
             return self.get_location_id(legacy_item, index_or_id, folio_prop_name)
         elif folio_prop_name == "callNumberTypeId":
             return self.get_call_number_type_id(legacy_item, folio_prop_name, index_or_id)
         elif folio_prop_name.startswith("statisticalCodeIds"):
             return self.get_statistical_code(legacy_item, folio_prop_name, index_or_id)
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/item_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/item_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from folio_uuid.folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.helper import Helper
+from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
 from folio_migration_tools.mapping_file_transformation.ref_data_mapping import (
     RefDataMapping,
 )
@@ -110,16 +111,23 @@
             "/locations",
             "locations",
             location_map,
             "code",
             Blurbs.LocationMapping,
         )
 
-    def perform_additional_mappings(self):
-        raise NotImplementedError()
+    def perform_additional_mappings(self, folio_rec, file_def):
+        self.handle_suppression(folio_rec, file_def)
+
+    def handle_suppression(self, folio_record, file_def: FileDefinition):
+        folio_record["discoverySuppress"] = file_def.discovery_suppressed
+        self.migration_report.add(
+            Blurbs.Suppression,
+            f'Suppressed from discovery = {folio_record["discoverySuppress"]}',
+        )
 
     def setup_status_mapping(self, item_statuses_map):
         statuses = self.item_schema["properties"]["status"]["properties"]["name"]["enum"]
         for mapping in item_statuses_map:
             if "folio_name" not in mapping:
                 logging.critical("folio_name is not a column in the status mapping file")
                 sys.exit(1)
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/order_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/order_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/mapping_file_transformation/user_mapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/mapping_file_transformation/user_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/conditions.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,23 @@
         self.mapper.migration_report.add(Blurbs.HoldingsTypeMapping, "Condition in rules hit")
         return ""
 
     def condition_concat_subfields_by_name(
         self, legacy_id, value, parameter, marc_field: field.Field
     ):
         subfields_to_concat = parameter.get("subfieldsToConcat", [])
-        concat_string = " ".join(marc_field.get_subfields(*subfields_to_concat))
+        subfields_to_stop_concat = parameter.get("subfieldsToStopConcat", [])
+        concat_subfields = []
+        subfields = marc_field.subfields
+        for t in subfields:
+            if t[0] in subfields_to_stop_concat:
+                break
+            elif t[0] in subfields_to_concat:
+                concat_subfields.append(t[1])
+        concat_string = " ".join(concat_subfields)
         return f"{value} {concat_string}"
 
     def condition_get_value_if_subfield_is_empty(
         self, legacy_id, value, parameter, marc_field: field.Field
     ):
         if value.strip():
             return value.strip()
@@ -643,15 +651,15 @@
     ):
         for subfield in marc_field.get_subfields("4", "e"):
             normalized_subfield = re.sub(r"[^A-Za-z0-9 ]+", "", subfield.strip())
             for cont_type in self.folio.contributor_types:
                 if normalized_subfield in [cont_type["code"], cont_type["name"]]:
                     return cont_type["name"]
         try:
-            marc_field.get_subfields("j", "e")[0]
+            return value
         except IndexError as ee:
             return ""
 
     def condition_set_alternative_title_type_id(self, legacy_id, value, parameter, marc_field):
         try:
             t = self.get_ref_data_tuple_by_name(
                 self.folio.alt_title_types, "alt_title_types", parameter["name"]
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,28 +146,37 @@
             legacy_ids (List[str]): List of legacy ids in record
 
         Raises:
             TransformationFieldMappingError: _description_
             TransformationFieldMappingError: _description_
         """
         for f in marc_record.get_fields(field_textual):
-            if "a" not in f and "z" not in f and "x" not in f:
+            codes = [sf.code for sf in f.subfields]
+            if "a" not in codes and "z" not in codes and "x" not in codes:
                 raise TransformationFieldMappingError(
                     legacy_ids,
                     f"{field_textual} subfields a, x, and z missing from field",
                     f,
                 )
-            if not (f["a"] or f["z"] or f["x"]):
+            if not (
+                len(f.get_subfields("a")) == 0
+                or len(f.get_subfields("z")) == 0
+                or len(f.get_subfields("x")) == 0
+            ):
                 raise TransformationFieldMappingError(
                     legacy_ids,
                     f"{field_textual} a,x and z are all empty",
                     f,
                 )
             return_dict["statements"].append(
-                {"statement": (f["a"] or ""), "note": (f["z"] or ""), "staffNote": (f["x"] or "")}
+                {
+                    "statement": "".join(f.get_subfields("a")),
+                    "note": "".join(f.get_subfields("z")),
+                    "staffNote": "".join(f.get_subfields("x")),
+                }
             )
             return_dict["migration_report"].append(
                 ("Holdings statements", f"From {field_textual}")
             )
 
     @staticmethod
     def get_break_indicator(field: Field):
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Set
 
 import httpx
 from folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
 from pymarc import Field
 from pymarc import Record
+from pymarc import Subfield
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import HridHandling
 from folio_migration_tools.migration_report import MigrationReport
 from folio_migration_tools.report_blurbs import Blurbs
 
@@ -26,19 +27,19 @@
         self.unique_001s: Set[str] = set()
         self.deactivate035_from001: bool = deactivate035_from001
         self.hrid_path = "/hrid-settings-storage/hrid-settings"
         self.folio_client: FolioClient = folio_client
         self.handling: HridHandling = handling
         self.migration_report: MigrationReport = migration_report
         self.hrid_settings = self.folio_client.folio_get_single_object(self.hrid_path)
-        self.instance_hrid_prefix = self.hrid_settings["instances"]["prefix"]
+        self.instance_hrid_prefix = self.hrid_settings["instances"].get("prefix", "")
         self.instance_hrid_counter = self.hrid_settings["instances"]["startNumber"]
-        self.holdings_hrid_prefix = self.hrid_settings["holdings"]["prefix"]
+        self.holdings_hrid_prefix = self.hrid_settings["holdings"].get("prefix", "")
         self.holdings_hrid_counter = self.hrid_settings["holdings"]["startNumber"]
-        self.items_hrid_prefix = self.hrid_settings["items"]["prefix"]
+        self.items_hrid_prefix = self.hrid_settings["items"].get("prefix", "")
         self.items_hrid_counter = self.hrid_settings["items"]["startNumber"]
         self.common_retain_leading_zeroes: bool = self.hrid_settings["commonRetainLeadingZeroes"]
         logging.info(f"HRID handling is set to: '{self.handling}'")
 
     def handle_hrid(
         self,
         namespace: FOLIONamespaces,
@@ -119,15 +120,15 @@
             if deactivate035_from001:
                 migration_report.add(Blurbs.HridHandling, "035 generation from 001 turned off")
             else:
                 str_035 = f"({f_003}){f_001}" if f_003 else f"{f_001}"
                 new_035 = Field(
                     tag="035",
                     indicators=[" ", " "],
-                    subfields=["a", str_035],
+                    subfields=[Subfield(code="a", value=str_035)],
                 )
                 marc_record.add_ordered_field(new_035)
                 migration_report.add(Blurbs.HridHandling, "Added 035 from 001")
             if remove_001:
                 marc_record.remove_fields("001")
 
         except Exception:
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import traceback
 from typing import List
 
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from pymarc import Field
 from pymarc import Record
+from pymarc import Subfield
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.folder_structure import FolderStructure
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import HridHandling
@@ -141,15 +142,15 @@
             marc_record.remove_fields("004")
             marc_record.add_ordered_field(new_004)
             for former_id in legacy_ids:
                 if self.mapper.task_configuration.hrid_handling == HridHandling.default:
                     new_035 = Field(
                         tag="035",
                         indicators=[" ", " "],
-                        subfields=["a", former_id],
+                        subfields=[Subfield(code="a", value=former_id)],
                     )
                     marc_record.add_ordered_field(new_035)
         self.mapper.save_source_record(
             self.srs_records_file,
             self.object_type,
             self.mapper.folio_client,
             marc_record,
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from dateutil.parser import parse
 from folio_uuid.folio_uuid import FOLIONamespaces
 from folio_uuid.folio_uuid import FolioUUID
 from folioclient import FolioClient
 from pymarc import Field
 from pymarc import Leader
 from pymarc import Record
+from pymarc import Subfield
 
 from folio_migration_tools.custom_exceptions import TransformationFieldMappingError
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
@@ -175,24 +176,24 @@
         legacy_id,
         mapping,
         marc_field,
     ):
         stripped_conds = mapping["rules"][0]["conditions"][0]["type"].split(",")
         condition_types = list(map(str.strip, stripped_conds))
         parameter = mapping["rules"][0]["conditions"][0].get("parameter", {})
-        if mapping.get("applyRulesOnConcatenatedData", ""):
+        if mapping.get("applyRulesOnConcatenatedData", ""):  # TODO: implement subfieldDelimiter
             value = " ".join(marc_field.get_subfields(*mapping["subfield"]))
             return self.apply_rule(legacy_id, value, condition_types, marc_field, parameter)
         elif mapping.get("subfield", []):
             subfields = marc_field.get_subfields(*mapping["subfield"])
             x = [
                 self.apply_rule(legacy_id, x, condition_types, marc_field, parameter)
                 for x in subfields
             ]
-            return " ".join(set(x))
+            return " ".join(dict.fromkeys(x))  # Create an ordered set of unique values before join
         else:
             value1 = marc_field.format_field() if marc_field else ""
             return self.apply_rule(legacy_id, value1, condition_types, marc_field, parameter)
 
     def process_marc_field(
         self,
         folio_record: dict,
@@ -265,14 +266,16 @@
         self.report_bad_tags(marc_field, bad_tags, legacy_ids)
         mapped = marc_field.tag in self.mappings
         if marc_field.tag in ignored_subsequent_fields:
             mapped = False
         self.report_legacy_mapping(marc_field.tag, True, mapped)
 
     def report_source_and_links(self, marc_field: Field):
+        if marc_field.is_control_field():
+            return
         for subfield_2 in marc_field.get_subfields("2"):
             self.migration_report.add(
                 Blurbs.AuthoritySources, f"Source of heading or term: {subfield_2.split(' ')[0]}"
             )
         for subfield_0 in marc_field.get_subfields("0"):
             code = ""
             if "(" in subfield_0 and ")" in subfield_0:
@@ -626,20 +629,21 @@
             _type_: _description_
         """
         unique_subfields: list = []
         repeated_subfields: list = []
         results = []
         for sf, sf_vals in marc_field.subfields_as_dict().items():
             if len(sf_vals) == 1:
-                unique_subfields.extend([sf, sf_vals[0]])
+                unique_subfields.append(Subfield(code=sf, value=sf_vals[0]))
             else:
-                repeated_subfields.extend([sf, sf_val] for sf_val in sf_vals)
+                repeated_subfields.extend([Subfield(code=sf, value=sf_val) for sf_val in sf_vals])
         if any(repeated_subfields):
             for repeated_subfield in repeated_subfields:
-                new_subfields = [repeated_subfield[0], repeated_subfield[1], *unique_subfields]
+                new_subfields = [repeated_subfield]
+                new_subfields.extend(unique_subfields)
                 temp_field = Field(
                     tag=marc_field.tag,
                     indicators=marc_field.indicators,
                     subfields=new_subfields,
                 )
                 results.append(temp_field)
         else:
@@ -660,15 +664,15 @@
             marc_field (Field): _description_
 
         Returns:
             _type_: _description_
         """
         new_subfields = []
         for sf, sf_vals in marc_field.subfields_as_dict().items():
-            new_subfields.extend([sf, sf_vals[0]])
+            new_subfields.extend([Subfield(code=sf, value=sf_vals[0])])
         return Field(
             tag=marc_field.tag,
             indicators=marc_field.indicators,
             subfields=new_subfields,
         )
 
     @staticmethod
@@ -694,15 +698,18 @@
         """
         srs_id = RulesMapperBase.create_srs_id(record_type, folio_client.okapi_url, legacy_ids[-1])
 
         marc_record.add_ordered_field(
             Field(
                 tag="999",
                 indicators=["f", "f"],
-                subfields=["i", folio_record["id"], "s", srs_id],
+                subfields=[
+                    Subfield(code="i", value=folio_record["id"]),
+                    Subfield(code="s", value=srs_id),
+                ],
             )
         )
         # Since they all should be UTF encoded, make the leader align.
         try:
             temp_leader = Leader(marc_record.leader)
             temp_leader[9] = "a"
             marc_record.leader = temp_leader
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from folio_migration_tools.custom_exceptions import TransformationFieldMappingError
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.holdings_helper import HoldingsHelper
 from folio_migration_tools.library_configuration import FileDefinition
+from folio_migration_tools.library_configuration import HridHandling
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.marc_rules_transformation.conditions import Conditions
 from folio_migration_tools.marc_rules_transformation.holdings_statementsparser import (
     HoldingsStatementsParser,
 )
 from folio_migration_tools.marc_rules_transformation.rules_mapper_base import (
     RulesMapperBase,
@@ -249,15 +250,18 @@
             TransformationRecordFailedError: _description_
         """
         self.set_holdings_type(marc_record, folio_holding, legacy_ids)
         self.set_default_call_number_type_if_empty(folio_holding)
         self.pick_first_location_if_many(folio_holding, legacy_ids)
         self.parse_coded_holdings_statements(marc_record, folio_holding, legacy_ids)
         HoldingsHelper.handle_notes(folio_holding)
-        if self.task_configuration.create_source_records:
+        if (
+            self.task_configuration.create_source_records
+            or self.task_configuration.hrid_handling == HridHandling.preserve001
+        ):
             self.hrid_handler.handle_hrid(
                 FOLIONamespaces.holdings, folio_holding, marc_record, legacy_ids
             )
         else:
             del folio_holding["hrid"]
         if not folio_holding.get("instanceId", ""):
             raise TransformationRecordFailedError(
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_report.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_report.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/authority_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/authority_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/batch_poster.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/batch_poster.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/bibs_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/bibs_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/courses_migrator.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/courses_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/items_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/items_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,15 @@
                         logging.info("First legacy record:")
                         logging.info(json.dumps(record, indent=4))
                         self.mapper.verify_legacy_record(record, idx)
                     folio_rec, legacy_id = self.mapper.do_map(
                         record, f"row {idx}", FOLIONamespaces.items
                     )
 
+                    self.mapper.perform_additional_mappings(folio_rec, file_def)
                     self.handle_circiulation_notes(folio_rec, self.folio_client.current_user)
                     self.handle_notes(folio_rec)
                     if folio_rec["holdingsRecordId"] in self.mapper.boundwith_relationship_map:
                         for idx, instance_id in enumerate(
                             self.mapper.boundwith_relationship_map.get(
                                 folio_rec["holdingsRecordId"]
                             )
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/loans_migrator.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/loans_migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import httpx
 from dateutil import parser as du_parser
 from folio_uuid.folio_namespaces import FOLIONamespaces
 
 from folio_migration_tools.circulation_helper import CirculationHelper
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
+from folio_migration_tools.library_configuration import FolioRelease
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
 from folio_migration_tools.migration_report import MigrationReport
 from folio_migration_tools.migration_tasks.migration_task_base import MigrationTaskBase
 from folio_migration_tools.report_blurbs import Blurbs
@@ -125,29 +126,44 @@
                 "previously migrated objects"
             )
             self.valid_legacy_loans = self.semi_valid_legacy_loans
         logging.info("Starting row number is %s", task_configuration.starting_row)
         logging.info("Init completed")
 
     def check_smtp_config(self):
-        okapi_config_base_path = "/configurations/entries"
-        okapi_config_query = "(module=={}%20and%20configName=={}%20and%20code=={})"
-        okapi_config_limit = 1000
-        okapi_config_module = "SMTP_SERVER"
-        okapi_config_name = "smtp"
-        okapi_config_code = "EMAIL_SMTP_HOST_DISABLED"
-        smtp_config_path = (
-            okapi_config_base_path
-            + "?"
-            + str(okapi_config_limit)
-            + "&query="
-            + okapi_config_query.format(okapi_config_module, okapi_config_name, okapi_config_code)
-        )
+        if self.library_configuration.folio_release.lower() == FolioRelease.morning_glory:
+            logging.warn("DEPRECATED: Morning Glory support will be removed in a future release!")
+            okapi_config_base_path = "/configurations/entries"
+            okapi_config_query = "(module=={}%20and%20configName=={}%20and%20code=={})"
+            okapi_config_limit = 1000
+            okapi_config_module = "SMTP_SERVER"
+            okapi_config_name = "smtp"
+            okapi_config_code = "EMAIL_SMTP_HOST_DISABLED"
+            smtp_config_path = (
+                okapi_config_base_path
+                + "?"
+                + str(okapi_config_limit)
+                + "&query="
+                + okapi_config_query.format(
+                    okapi_config_module, okapi_config_name, okapi_config_code
+                )
+            )
+            smtp_config_disabled = self.folio_client.folio_get_single_object(smtp_config_path)[
+                "configs"
+            ]
+        else:
+            try:
+                smtp_config = self.folio_client.folio_get_single_object("/smtp-configuration")[
+                    "smtpConfigurations"
+                ][0]
+                smtp_config_disabled = "disabled" in smtp_config["host"].lower()
+            except IndexError:
+                smtp_config_disabled = True
         print_smtp_warning()
-        if not self.folio_client.folio_get_single_object(smtp_config_path)["configs"]:
+        if not smtp_config_disabled:
             logging.warn("SMTP connection not disabled...")
             for i in range(10, 0, -1):
                 sys.stdout.write("Pausing for {:02d} seconds. Press Ctrl+C to exit...\r".format(i))
                 time.sleep(1)
         else:
             logging.info("SMTP connection is disabled...")
```

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/migration_task_base.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/migration_task_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/orders_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/orders_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/organization_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/organization_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/requests_migrator.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/requests_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/reserves_migrator.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/reserves_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/migration_tasks/user_transformer.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/migration_tasks/user_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/report_blurbs.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/report_blurbs.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/test_infrastructure/mocked_classes.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/test_infrastructure/mocked_classes.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_loan.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/legacy_loan.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_request.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/legacy_request.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/legacy_reserve.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/legacy_reserve.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/src/folio_migration_tools/transaction_migration/transaction_result.py` & `folio_migration_tools-1.8.1/src/folio_migration_tools/transaction_migration/transaction_result.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc8/setup.py` & `folio_migration_tools-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 {'': ['*']}
 
 install_requires = \
 ['argparse-prompt>=0.0.5,<0.0.6',
  'deepdiff>=6.2.3,<7.0.0',
  'defusedxml>=0.7.1,<0.8.0',
  'folio-uuid>=0.2.8,<0.3.0',
- 'folioclient>=0.50.0rc1,<0.51.0',
+ 'folioclient>=0.50.0,<0.51.0',
  'httpx>=0.23.3,<0.24.0',
  'pyaml>=21.10.1,<22.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pyhumps>=3.7.3,<4.0.0',
- 'pymarc>=4.2.1,<5.0.0',
+ 'pymarc>=5.0.0,<6.0.0',
  'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'folio-migration-tools',
-    'version': '1.8.0rc8',
+    'version': '1.8.1',
     'description': 'A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP',
     'long_description': '# FOLIO Migration Tools\n![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)\n\nA toolkit that enables you to migrate data over from a legacy ILS system into [FOLIO LSP](https://www.folio.org/)\n\n# What is it good for?\nFOLIO Migration tools enables you to migrate libraries with the most common ILS:s over to FOLIO without data losses or any major data transformation tasks. \nThe tools transforms and loads the data providing you and the library with good actionable logs and data cleaning task lists together with the migrated data.\n\n## What data does it cover?\nFOLIO Migration Tools currently covers the following data sets:\n* Catalog (Inventory and SRS in FOLIO terminology)\n* Circulation transactions (Open loans and requests)\n* Users/Patrons (In FOLIO, these share the same app/database)\n* Courses and Reserves (Course reserves)\n* Organizations (Vendor records)\n* Orders (limited support)\n\n### What additional functionality is on the roadmap?\nThis is the loose roadmap, in order of most likely implementations first\n* ERM-related objects\n* Financial records\n\n### Can I use the tools for ongoing imports and integrations?\nThe tools are primarliy maintained for performing initial data migrations. We recommend that you use native FOLIO functionality for ongoing loads where possible. \nIn theory, these tools can be used for ongoing patron loads from systems like Banner, Workday, or PeopleSoft. But we recommend you to weigh your options carefully before going down this path. \n\n# Contributing\nWant to contribute? Read the [CONTRIBUTING.MD](https://github.com/FOLIO-FSE/folio_migration_tools/blob/main/CONTRIBUTING.md)\n\n# Found an issue?\nReport it on the [Github Issue tracker](https://github.com/FOLIO-FSE/folio_migration_tools/issues)\n\nThe scripts requires a FOLIO tenant with reference data properly set up. The script will throw messages telling what reference data is missing.\n# Installing\nMake sure you are running Python 3.9 or above. \n## 1. Using pip and venv\n### 2.1. Create and activate a [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)   \n```   \npython -m venv ./.venv     # Creates a virtual env in the current folder\nsource .venv/bin/activate  # Activates the venv    \n```\n### 2. Install using pip: \n```\npython -m pip install folio_migration_tools\n```\n### 3. Test the installation by showing the help pages \n```   \npython -m folio_migration_tools -h\n```    \n\n## 2. Using pipenv\n### 1. Run\n```   \npipenv install folio-migration-tools\n```   \n### 2. Test the installation by showing the help pages\n```  \npipenv run python3 -m folio_migration_tools -h\n```  \n\n# FOLIO migration process\nThis repo plays the main part in a process using a collection of tools. The process itself is documented in more detail, including example configuration files, at [this template repository](https://github.com/FOLIO-FSE/migration_repo_template)\nIn order to perform migrations according to this process, you need the following:\n* An Installation of [FOLIO Migration Tools](https://pypi.org/project/folio-migration-tools/). Installation instructions above.\n* A clone, or a separate repo created from [migration_repo_template](https://github.com/FOLIO-FSE/migration_repo_template)\n* Access to the [Data mapping file creator](https://data-mapping-file-creator.folio.ebsco.com/data_mapping_creation) web tool\n* A FOLIO tenant running the latest or the second latest version of FOLIO\n\n\n\n# Running the scripts\nFor information on syntax, what files are needed and produced by the toolkit, refer to the documentation and example files in the [template repository](https://github.com/FOLIO-FSE/migration_repo_template). We are building out the docs section in this repository as well:[Documentation](https://folio-migration-tools.readthedocs.io/en/latest/)\n¨\n',
     'author': 'Theodor Tolstoy',
     'author_email': 'github.teddes@tolstoy.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FOLIO-FSE/folio_migration_tools',
```

### Comparing `folio_migration_tools-1.8.0rc8/PKG-INFO` & `folio_migration_tools-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folio-migration-tools
-Version: 1.8.0rc8
+Version: 1.8.1
 Summary: A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP
 Home-page: https://github.com/FOLIO-FSE/folio_migration_tools
 License: MIT
 Keywords: FOLIO,ILS,LSP,Library Systems,MARC21,Library data
 Author: Theodor Tolstoy
 Author-email: github.teddes@tolstoy.se
 Requires-Python: >=3.9,<4.0
@@ -14,20 +14,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: argparse-prompt (>=0.0.5,<0.0.6)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: folio-uuid (>=0.2.8,<0.3.0)
-Requires-Dist: folioclient (>=0.50.0rc1,<0.51.0)
+Requires-Dist: folioclient (>=0.50.0,<0.51.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: pyaml (>=21.10.1,<22.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.3,<4.0.0)
-Requires-Dist: pymarc (>=4.2.1,<5.0.0)
+Requires-Dist: pymarc (>=5.0.0,<6.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/FOLIO-FSE/folio_migration_tools
 Description-Content-Type: text/markdown
 
 # FOLIO Migration Tools
 ![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)
```

