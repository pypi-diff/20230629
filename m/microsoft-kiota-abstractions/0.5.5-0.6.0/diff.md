# Comparing `tmp/microsoft_kiota_abstractions-0.5.5.tar.gz` & `tmp/microsoft_kiota_abstractions-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_abstractions-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_abstractions-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_abstractions-0.5.5.tar` & `microsoft_kiota_abstractions-0.6.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
--rw-r--r--   0        0        0       82 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1927 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/workflows/build.yml
--rw-r--r--   0        0        0     2538 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1097 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1799 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.gitignore
--rw-r--r--   0        0        0    15931 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.pylintrc
--rw-r--r--   0        0        0     1197 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/LICENSE
--rw-r--r--   0        0        0     2512 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/README.md
--rw-r--r--   0        0        0     2757 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/__init__.py
--rw-r--r--   0        0        0       23 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/_version.py
--rw-r--r--   0        0        0     3566 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/api_client_builder.py
--rw-r--r--   0        0        0      399 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/api_error.py
--rw-r--r--   0        0        0      346 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/__init__.py
--rw-r--r--   0        0        0      836 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/access_token_provider.py
--rw-r--r--   0        0        0     2120 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/allowed_hosts_validator.py
--rw-r--r--   0        0        0      607 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/anonymous_authentication_provider.py
--rw-r--r--   0        0        0      473 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/authentication_provider.py
--rw-r--r--   0        0        0     1231 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
--rw-r--r--   0        0        0     1252 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_builder.py
--rw-r--r--   0        0        0      667 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_configuration.py
--rw-r--r--   0        0        0      372 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/default_query_parameters.py
--rw-r--r--   0        0        0      453 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/get_path_parameters.py
--rw-r--r--   0        0        0      529 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/method.py
--rw-r--r--   0        0        0      938 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/native_response_handler.py
--rw-r--r--   0        0        0     5164 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_adapter.py
--rw-r--r--   0        0        0     9048 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_information.py
--rw-r--r--   0        0        0      312 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_option.py
--rw-r--r--   0        0        0      965 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/response_handler.py
--rw-r--r--   0        0        0      679 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/__init__.py
--rw-r--r--   0        0        0      374 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/additional_data_holder.py
--rw-r--r--   0        0        0     1006 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable.py
--rw-r--r--   0        0        0      642 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable_factory.py
--rw-r--r--   0        0        0     5793 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node.py
--rw-r--r--   0        0        0      903 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory.py
--rw-r--r--   0        0        0     1972 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory_registry.py
--rw-r--r--   0        0        0      949 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_helper.py
--rw-r--r--   0        0        0     2424 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_proxy_factory.py
--rw-r--r--   0        0        0     9768 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer.py
--rw-r--r--   0        0        0      898 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory.py
--rw-r--r--   0        0        0     2025 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory_registry.py
--rw-r--r--   0        0        0     3132 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0      529 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/__init__.py
--rw-r--r--   0        0        0      398 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backed_model.py
--rw-r--r--   0        0        0     3892 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store.py
--rw-r--r--   0        0        0      424 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_factory.py
--rw-r--r--   0        0        0      237 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_factory_singleton.py
--rw-r--r--   0        0        0     1166 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_parse_node_factory.py
--rw-r--r--   0        0        0     1809 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0     4488 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/in_memory_backing_store.py
--rw-r--r--   0        0        0      380 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/in_memory_backing_store_factory.py
--rw-r--r--   0        0        0      899 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/utils.py
--rw-r--r--   0        0        0     1268 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1130 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/authentication/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/authentication/test_base_bearer_token_authentication.py
--rw-r--r--   0        0        0      831 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/conftest.py
--rw-r--r--   0        0        0     5109 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/test_request_information.py
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1987 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2538 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1097 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.gitignore
+-rw-r--r--   0        0        0    15931 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/.pylintrc
+-rw-r--r--   0        0        0     1281 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/LICENSE
+-rw-r--r--   0        0        0      335 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/Makefile
+-rw-r--r--   0        0        0     2512 2023-06-29 11:29:17.966215 microsoft_kiota_abstractions-0.6.0/README.md
+-rw-r--r--   0        0        0     2757 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/_version.py
+-rw-r--r--   0        0        0     3566 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/api_client_builder.py
+-rw-r--r--   0        0        0      399 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/api_error.py
+-rw-r--r--   0        0        0      673 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/__init__.py
+-rw-r--r--   0        0        0      836 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/access_token_provider.py
+-rw-r--r--   0        0        0     2120 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/allowed_hosts_validator.py
+-rw-r--r--   0        0        0      607 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/anonymous_authentication_provider.py
+-rw-r--r--   0        0        0     2341 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/api_key_authentication_provider.py
+-rw-r--r--   0        0        0      473 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/authentication_provider.py
+-rw-r--r--   0        0        0     1231 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
+-rw-r--r--   0        0        0     1252 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_builder.py
+-rw-r--r--   0        0        0      667 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_configuration.py
+-rw-r--r--   0        0        0      372 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/default_query_parameters.py
+-rw-r--r--   0        0        0      453 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/get_path_parameters.py
+-rw-r--r--   0        0        0      529 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/method.py
+-rw-r--r--   0        0        0      938 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/native_response_handler.py
+-rw-r--r--   0        0        0     5164 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_adapter.py
+-rw-r--r--   0        0        0     9048 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_information.py
+-rw-r--r--   0        0        0      312 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_option.py
+-rw-r--r--   0        0        0      965 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/response_handler.py
+-rw-r--r--   0        0        0      679 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/__init__.py
+-rw-r--r--   0        0        0      374 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/additional_data_holder.py
+-rw-r--r--   0        0        0     1006 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable.py
+-rw-r--r--   0        0        0      642 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable_factory.py
+-rw-r--r--   0        0        0     5793 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node.py
+-rw-r--r--   0        0        0      903 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory.py
+-rw-r--r--   0        0        0     1972 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory_registry.py
+-rw-r--r--   0        0        0      949 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_helper.py
+-rw-r--r--   0        0        0     2424 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_proxy_factory.py
+-rw-r--r--   0        0        0     9768 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer.py
+-rw-r--r--   0        0        0      898 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory.py
+-rw-r--r--   0        0        0     2025 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py
+-rw-r--r--   0        0        0     3132 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0      529 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/__init__.py
+-rw-r--r--   0        0        0      398 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backed_model.py
+-rw-r--r--   0        0        0     3892 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store.py
+-rw-r--r--   0        0        0      424 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_factory.py
+-rw-r--r--   0        0        0      237 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_factory_singleton.py
+-rw-r--r--   0        0        0     1166 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_parse_node_factory.py
+-rw-r--r--   0        0        0     1809 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0     4488 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/in_memory_backing_store.py
+-rw-r--r--   0        0        0      380 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/in_memory_backing_store_factory.py
+-rw-r--r--   0        0        0      899 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/kiota_abstractions/utils.py
+-rw-r--r--   0        0        0     1268 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1130 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/authentication/__init__.py
+-rw-r--r--   0        0        0     2340 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/authentication/test_api_key_authentication_provider.py
+-rw-r--r--   0        0        0     1041 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/authentication/test_base_bearer_token_authentication.py
+-rw-r--r--   0        0        0      831 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     5109 2023-06-29 11:29:17.970214 microsoft_kiota_abstractions-0.6.0/tests/test_request_information.py
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.6.0/PKG-INFO
```

### Comparing `microsoft_kiota_abstractions-0.5.5/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_abstractions-0.6.0/.github/workflows/auto-merge-dependabot.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.5.1
+        uses: dependabot/fetch-metadata@v1.6.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_abstractions-0.5.5/.github/workflows/build.yml` & `microsoft_kiota_abstractions-0.6.0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
           isort kiota_abstractions
       - name: Lint with Pylint
         run: |
           pylint kiota_abstractions --disable=W --rcfile=.pylintrc
       - name: Static type checking with Mypy
         run: |
           mypy kiota_abstractions
+      - name: Run the tests
+        run: |
+          pytest
 
   publish:
     name: Publish distribution to PyPI
     if: ${{ github.ref == 'refs/heads/main' }}
     runs-on: ubuntu-latest
     environment: pypi_prod
     needs: [build]
```

### Comparing `microsoft_kiota_abstractions-0.5.5/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_abstractions-0.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_abstractions-0.6.0/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/.github/workflows/publish.yml` & `microsoft_kiota_abstractions-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/.gitignore` & `microsoft_kiota_abstractions-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/.pylintrc` & `microsoft_kiota_abstractions-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/CHANGELOG.md` & `microsoft_kiota_abstractions-0.6.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.6.0] - 2023-06-27
+
+### Added
+- API key authentication provider.
+
+### Changed
+
 ## [0.5.5] - 2023-06-26
 
 ### Added
 
 ### Changed
 
 - Changed BaseRequesBuilder class to be instantiable.
```

### Comparing `microsoft_kiota_abstractions-0.5.5/LICENSE` & `microsoft_kiota_abstractions-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/README.md` & `microsoft_kiota_abstractions-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/SECURITY.md` & `microsoft_kiota_abstractions-0.6.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/SUPPORT.md` & `microsoft_kiota_abstractions-0.6.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/api_client_builder.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/access_token_provider.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/access_token_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/allowed_hosts_validator.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/allowed_hosts_validator.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/anonymous_authentication_provider.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/anonymous_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_builder.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_configuration.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/base_request_configuration.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/method.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/method.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/native_response_handler.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/native_response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_adapter.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_information.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/response_handler.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/__init__.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parsable_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory_registry.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_helper.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_helper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_proxy_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/parse_node_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory_registry.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/__init__.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_parse_node_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/in_memory_backing_store.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/store/in_memory_backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/utils.py` & `microsoft_kiota_abstractions-0.6.0/kiota_abstractions/utils.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/pyproject.toml` & `microsoft_kiota_abstractions-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/requirements-dev.txt` & `microsoft_kiota_abstractions-0.6.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/tests/authentication/test_base_bearer_token_authentication.py` & `microsoft_kiota_abstractions-0.6.0/tests/authentication/test_base_bearer_token_authentication.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/tests/conftest.py` & `microsoft_kiota_abstractions-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/tests/test_request_information.py` & `microsoft_kiota_abstractions-0.6.0/tests/test_request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.5/PKG-INFO` & `microsoft_kiota_abstractions-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-abstractions
-Version: 0.5.5
+Version: 0.6.0
 Summary: Core abstractions for kiota generated libraries in Python
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

