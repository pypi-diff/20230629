# Comparing `tmp/jtech-1.0.5.tar.gz` & `tmp/jtech-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtech-1.0.5.tar", max compression
+gzip compressed data, was "jtech-1.0.6.tar", max compression
```

## Comparing `jtech-1.0.5.tar` & `jtech-1.0.6.tar`

### file list

```diff
@@ -1,98 +1,146 @@
--rw-r--r--   0        0        0        0 2023-06-19 12:53:20.183574 jtech-1.0.5/jtech/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-26 16:33:22.667880 jtech-1.0.5/jtech/__main__.py
--rw-r--r--   0        0        0        0 2023-06-19 12:57:41.640049 jtech-1.0.5/jtech/architecture/__init__.py
--rw-r--r--   0        0        0     5946 2023-06-26 15:01:17.570284 jtech-1.0.5/jtech/architecture/clean_architecture_generator.py
--rw-r--r--   0        0        0        0 2023-06-19 12:58:05.011675 jtech-1.0.5/jtech/clean_generators/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-20 16:24:08.670365 jtech-1.0.5/jtech/clean_generators/clean_adapter_generator.py
--rw-r--r--   0        0        0      866 2023-06-20 17:33:31.654651 jtech-1.0.5/jtech/clean_generators/clean_api_error_generator.py
--rw-r--r--   0        0        0      879 2023-06-20 17:37:47.222366 jtech-1.0.5/jtech/clean_generators/clean_api_sub_error_generator.py
--rw-r--r--   0        0        0      907 2023-06-20 17:39:21.310839 jtech-1.0.5/jtech/clean_generators/clean_api_validation_error_generator.py
--rw-r--r--   0        0        0     1200 2023-06-20 16:24:08.713367 jtech-1.0.5/jtech/clean_generators/clean_config_generator.py
--rw-r--r--   0        0        0     1277 2023-06-20 16:24:08.730367 jtech-1.0.5/jtech/clean_generators/clean_controller_generator.py
--rw-r--r--   0        0        0     1158 2023-06-20 16:24:08.675366 jtech-1.0.5/jtech/clean_generators/clean_domain_generator.py
--rw-r--r--   0        0        0     1911 2023-06-23 18:48:38.519153 jtech-1.0.5/jtech/clean_generators/clean_entity_generator.py
--rw-r--r--   0        0        0      835 2023-06-20 17:41:06.462602 jtech-1.0.5/jtech/clean_generators/clean_gen_id_generator.py
--rw-r--r--   0        0        0     8065 2023-06-23 13:37:46.794747 jtech-1.0.5/jtech/clean_generators/clean_generator.py
--rw-r--r--   0        0        0      916 2023-06-20 17:36:09.141789 jtech-1.0.5/jtech/clean_generators/clean_global_handler_generator.py
--rw-r--r--   0        0        0     1307 2023-06-20 16:24:08.736367 jtech-1.0.5/jtech/clean_generators/clean_input_gateway_generator.py
--rw-r--r--   0        0        0      834 2023-06-20 17:42:13.571365 jtech-1.0.5/jtech/clean_generators/clean_jsons_generator.py
--rw-r--r--   0        0        0      874 2023-06-20 17:30:35.029010 jtech-1.0.5/jtech/clean_generators/clean_kafka_generator.py
--rw-r--r--   0        0        0      905 2023-06-20 17:43:54.808025 jtech-1.0.5/jtech/clean_generators/clean_openapi_generator.py
--rw-r--r--   0        0        0     1314 2023-06-20 16:24:08.692366 jtech-1.0.5/jtech/clean_generators/clean_output_gateway_generator.py
--rw-r--r--   0        0        0      899 2023-06-20 17:46:21.255873 jtech-1.0.5/jtech/clean_generators/clean_ready_event_listener_generator.py
--rw-r--r--   0        0        0      873 2023-06-20 17:47:43.993047 jtech-1.0.5/jtech/clean_generators/clean_redis_generator.py
--rw-r--r--   0        0        0     1394 2023-06-20 16:25:42.838850 jtech-1.0.5/jtech/clean_generators/clean_repository_default_generator.py
--rw-r--r--   0        0        0     1296 2023-06-20 16:24:08.719367 jtech-1.0.5/jtech/clean_generators/clean_repository_jpa_template.py
--rw-r--r--   0        0        0     1263 2023-06-20 16:24:08.708366 jtech-1.0.5/jtech/clean_generators/clean_repository_mongo_template.py
--rw-r--r--   0        0        0     1112 2023-06-20 16:24:08.697366 jtech-1.0.5/jtech/clean_generators/clean_request_template.py
--rw-r--r--   0        0        0     1175 2023-06-20 16:24:08.703366 jtech-1.0.5/jtech/clean_generators/clean_response_template.py
--rw-r--r--   0        0        0     1176 2023-06-20 16:24:08.687366 jtech-1.0.5/jtech/clean_generators/clean_usecase_template.py
--rw-r--r--   0        0        0        0 2023-06-19 12:58:17.065998 jtech-1.0.5/jtech/cqrs_generators/__init__.py
--rw-r--r--   0        0        0     1213 2023-06-19 15:27:17.587214 jtech-1.0.5/jtech/cqrs_generators/cars_controller_template.py
--rw-r--r--   0        0        0     1100 2023-06-20 16:04:27.456358 jtech-1.0.5/jtech/cqrs_generators/cqrs_aggregator_template.py
--rw-r--r--   0        0        0     1025 2023-06-19 15:31:21.389627 jtech-1.0.5/jtech/cqrs_generators/cqrs_generator.py
--rw-r--r--   0        0        0        0 2023-06-19 15:34:07.706004 jtech-1.0.5/jtech/creators/__init__.py
--rw-r--r--   0        0        0      271 2023-06-14 15:39:52.623663 jtech-1.0.5/jtech/creators/gradle_properties_creator.py
--rw-r--r--   0        0        0      709 2023-06-14 15:43:22.480067 jtech-1.0.5/jtech/creators/readme_creator.py
--rw-r--r--   0        0        0        0 2023-06-23 19:00:13.758726 jtech-1.0.5/jtech/docker_compose/__init__.py
--rw-r--r--   0        0        0     8152 2023-06-26 13:29:59.849326 jtech-1.0.5/jtech/docker_compose/generate_docker_compose.py
--rw-r--r--   0        0        0        0 2023-06-19 16:37:48.899891 jtech-1.0.5/jtech/manipulate/__init__.py
--rw-r--r--   0        0        0     7631 2023-06-23 19:08:33.286070 jtech-1.0.5/jtech/manipulate/application_yml_manipulator.py
--rw-r--r--   0        0        0     4034 2023-06-20 17:15:07.065746 jtech-1.0.5/jtech/manipulate/build_gradle_manipulator.py
--rw-r--r--   0        0        0     2717 2023-06-20 19:28:16.842650 jtech-1.0.5/jtech/manipulate/java_class_manipulator.py
--rw-r--r--   0        0        0      976 2023-06-23 19:08:14.046556 jtech-1.0.5/jtech/manipulate/yaml_manipulator.py
--rw-r--r--   0        0        0        0 2023-06-26 13:36:17.584000 jtech-1.0.5/jtech/mockserver/__init__.py
--rw-r--r--   0        0        0      586 2023-06-26 15:24:47.248281 jtech-1.0.5/jtech/mockserver/mockserver.py
--rw-r--r--   0        0        0        0 2023-06-23 14:19:25.872787 jtech-1.0.5/jtech/project/__init__.py
--rw-r--r--   0        0        0     6671 2023-06-26 13:29:11.648247 jtech-1.0.5/jtech/project/create_project.py
--rw-r--r--   0        0        0      540 2023-06-23 16:17:26.834452 jtech-1.0.5/jtech/resources/banner/banner.txt
--rw-r--r--   0        0        0     1695 2023-06-20 18:41:45.182305 jtech-1.0.5/jtech/resources/dependencies/dependencies.json
--rw-r--r--   0        0        0     2170 2023-06-26 14:52:11.058124 jtech-1.0.5/jtech/resources/mock/http.tar.gz
--rw-r--r--   0        0        0     1699 2023-06-26 14:52:21.954146 jtech-1.0.5/jtech/resources/mock/mqtt.tar.gz
--rw-r--r--   0        0        0     1096 2023-06-15 15:47:48.302121 jtech-1.0.5/jtech/resources/tpl/clean_adapter.tpl
--rw-r--r--   0        0        0     2176 2023-06-20 16:45:02.296425 jtech-1.0.5/jtech/resources/tpl/clean_api_error.tpl
--rw-r--r--   0        0        0      585 2023-06-20 16:46:15.081344 jtech-1.0.5/jtech/resources/tpl/clean_api_sub_error.tpl
--rw-r--r--   0        0        0     1206 2023-06-20 16:47:28.810287 jtech-1.0.5/jtech/resources/tpl/clean_api_validation_error.tpl
--rw-r--r--   0        0        0     1042 2023-06-15 15:47:25.965530 jtech-1.0.5/jtech/resources/tpl/clean_config.tpl
--rw-r--r--   0        0        0     1517 2023-06-20 16:00:46.105564 jtech-1.0.5/jtech/resources/tpl/clean_controller.tpl
--rw-r--r--   0        0        0     1528 2023-06-23 12:50:38.457021 jtech-1.0.5/jtech/resources/tpl/clean_domain.tpl
--rw-r--r--   0        0        0      899 2023-06-23 13:22:13.689725 jtech-1.0.5/jtech/resources/tpl/clean_entity.tpl
--rw-r--r--   0        0        0      794 2023-06-20 17:40:23.718478 jtech-1.0.5/jtech/resources/tpl/clean_gen_id.tpl
--rw-r--r--   0        0        0     2375 2023-06-20 16:43:30.448004 jtech-1.0.5/jtech/resources/tpl/clean_global_handler.tpl
--rw-r--r--   0        0        0      697 2023-06-15 15:48:21.222993 jtech-1.0.5/jtech/resources/tpl/clean_input_gateway.tpl
--rw-r--r--   0        0        0     1020 2023-06-23 12:26:52.913732 jtech-1.0.5/jtech/resources/tpl/clean_jpa_entity2.tpl
--rw-r--r--   0        0        0     1026 2023-06-22 17:05:47.475660 jtech-1.0.5/jtech/resources/tpl/clean_jpa_entity3.tpl
--rw-r--r--   0        0        0     4654 2023-06-20 16:34:17.510426 jtech-1.0.5/jtech/resources/tpl/clean_jsons.tpl
--rw-r--r--   0        0        0     1171 2023-06-20 16:42:13.632980 jtech-1.0.5/jtech/resources/tpl/clean_kafka.tpl
--rw-r--r--   0        0        0     1107 2023-06-23 13:20:23.008763 jtech-1.0.5/jtech/resources/tpl/clean_mongo_entity.tpl
--rw-r--r--   0        0        0     2490 2023-06-20 17:43:39.504623 jtech-1.0.5/jtech/resources/tpl/clean_openapi.tpl
--rw-r--r--   0        0        0      701 2023-06-15 15:48:32.462291 jtech-1.0.5/jtech/resources/tpl/clean_output_gateway.tpl
--rw-r--r--   0        0        0     1542 2023-06-22 16:26:15.375485 jtech-1.0.5/jtech/resources/tpl/clean_ready_listener.tpl
--rw-r--r--   0        0        0     3582 2023-06-20 16:38:23.431913 jtech-1.0.5/jtech/resources/tpl/clean_redis.tpl
--rw-r--r--   0        0        0      758 2023-06-15 15:48:41.589532 jtech-1.0.5/jtech/resources/tpl/clean_repository_default.tpl
--rw-r--r--   0        0        0      856 2023-06-23 13:09:29.436274 jtech-1.0.5/jtech/resources/tpl/clean_repository_jpa.tpl
--rw-r--r--   0        0        0      860 2023-06-23 13:10:31.845943 jtech-1.0.5/jtech/resources/tpl/clean_repository_mongo.tpl
--rw-r--r--   0        0        0      974 2023-06-15 15:49:11.150315 jtech-1.0.5/jtech/resources/tpl/clean_request.tpl
--rw-r--r--   0        0        0     1952 2023-06-15 15:49:19.726542 jtech-1.0.5/jtech/resources/tpl/clean_response.tpl
--rw-r--r--   0        0        0     1276 2023-06-15 15:49:29.709807 jtech-1.0.5/jtech/resources/tpl/clean_usecase.tpl
--rw-r--r--   0        0        0      728 2023-06-15 19:19:22.686251 jtech-1.0.5/jtech/resources/tpl/cqrs_aggregate.tpl
--rw-r--r--   0        0        0     1003 2023-06-15 19:20:29.776027 jtech-1.0.5/jtech/resources/tpl/cqrs_aggregate_impl.tpl
--rw-r--r--   0        0        0     1424 2023-06-15 19:23:06.152169 jtech-1.0.5/jtech/resources/tpl/cqrs_cmd_controller.tpl
--rw-r--r--   0        0        0     1056 2023-06-15 18:52:17.712070 jtech-1.0.5/jtech/resources/tpl/cqrs_entity.tpl
--rw-r--r--   0        0        0     1348 2023-06-15 19:01:31.065875 jtech-1.0.5/jtech/resources/tpl/cqrs_qry_controller.tpl
--rw-r--r--   0        0        0        0 2023-06-19 13:04:59.491638 jtech-1.0.5/jtech/template_processor/__init__.py
--rw-r--r--   0        0        0      924 2023-06-23 14:11:12.824566 jtech-1.0.5/jtech/template_processor/template_processor.py
--rw-r--r--   0        0        0        0 2023-06-19 16:37:32.717465 jtech-1.0.5/jtech/utils/__init__.py
--rw-r--r--   0        0        0      287 2023-06-20 19:39:52.159935 jtech-1.0.5/jtech/utils/file_remove.py
--rw-r--r--   0        0        0      708 2023-06-26 13:29:05.616237 jtech-1.0.5/jtech/utils/param_configuration.py
--rw-r--r--   0        0        0      521 2023-06-26 15:18:33.671487 jtech-1.0.5/jtech/utils/tar_gz_extractor.py
--rw-r--r--   0        0        0        0 2023-06-19 16:35:55.615903 jtech-1.0.5/jtech/webclient/__init__.py
--rw-r--r--   0        0        0     1119 2023-06-19 17:10:17.936011 jtech-1.0.5/jtech/webclient/spring_boot_client.py
--rw-r--r--   0        0        0        0 2023-06-19 12:59:40.314234 jtech-1.0.5/jtech/wizards/__init__.py
--rw-r--r--   0        0        0      575 2023-06-19 16:15:08.306931 jtech-1.0.5/jtech/wizards/architecture_choice_wizard.py
--rw-r--r--   0        0        0     1248 2023-06-19 16:29:10.214206 jtech-1.0.5/jtech/wizards/checkbox_wizard.py
--rw-r--r--   0        0        0     1825 2023-06-23 16:39:20.028880 jtech-1.0.5/jtech/wizards/metadata_wizard.py
--rw-r--r--   0        0        0      741 2023-06-19 16:32:07.309879 jtech-1.0.5/jtech/wizards/project.py
--rw-r--r--   0        0        0      570 2023-06-20 16:16:32.641378 jtech-1.0.5/jtech/wizards/samples_choice_wizard.py
--rw-r--r--   0        0        0      659 2023-06-27 17:13:31.244165 jtech-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 jtech-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 12:53:20.183574 jtech-1.0.6/jtech/__init__.py
+-rw-r--r--   0        0        0     3002 2023-06-29 16:57:55.303758 jtech-1.0.6/jtech/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:57:41.640049 jtech-1.0.6/jtech/architecture/__init__.py
+-rw-r--r--   0        0        0     6415 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/architecture/clean_architecture_generator.py
+-rw-r--r--   0        0        0     5740 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/architecture/cqrs_architecture_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:58:05.011675 jtech-1.0.6/jtech/clean_generators/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-20 16:24:08.670365 jtech-1.0.6/jtech/clean_generators/clean_adapter_generator.py
+-rw-r--r--   0        0        0      866 2023-06-20 17:33:31.654651 jtech-1.0.6/jtech/clean_generators/clean_api_error_generator.py
+-rw-r--r--   0        0        0      879 2023-06-20 17:37:47.222366 jtech-1.0.6/jtech/clean_generators/clean_api_sub_error_generator.py
+-rw-r--r--   0        0        0      907 2023-06-20 17:39:21.310839 jtech-1.0.6/jtech/clean_generators/clean_api_validation_error_generator.py
+-rw-r--r--   0        0        0     1200 2023-06-20 16:24:08.713367 jtech-1.0.6/jtech/clean_generators/clean_config_generator.py
+-rw-r--r--   0        0        0     1277 2023-06-20 16:24:08.730367 jtech-1.0.6/jtech/clean_generators/clean_controller_generator.py
+-rw-r--r--   0        0        0     1158 2023-06-20 16:24:08.675366 jtech-1.0.6/jtech/clean_generators/clean_domain_generator.py
+-rw-r--r--   0        0        0     1911 2023-06-23 18:48:38.519153 jtech-1.0.6/jtech/clean_generators/clean_entity_generator.py
+-rw-r--r--   0        0        0      835 2023-06-20 17:41:06.462602 jtech-1.0.6/jtech/clean_generators/clean_gen_id_generator.py
+-rw-r--r--   0        0        0     7961 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_generator.py
+-rw-r--r--   0        0        0      916 2023-06-20 17:36:09.141789 jtech-1.0.6/jtech/clean_generators/clean_global_handler_generator.py
+-rw-r--r--   0        0        0     1307 2023-06-20 16:24:08.736367 jtech-1.0.6/jtech/clean_generators/clean_input_gateway_generator.py
+-rw-r--r--   0        0        0      834 2023-06-20 17:42:13.571365 jtech-1.0.6/jtech/clean_generators/clean_jsons_generator.py
+-rw-r--r--   0        0        0      874 2023-06-20 17:30:35.029010 jtech-1.0.6/jtech/clean_generators/clean_kafka_generator.py
+-rw-r--r--   0        0        0      905 2023-06-20 17:43:54.808025 jtech-1.0.6/jtech/clean_generators/clean_openapi_generator.py
+-rw-r--r--   0        0        0     1314 2023-06-20 16:24:08.692366 jtech-1.0.6/jtech/clean_generators/clean_output_gateway_generator.py
+-rw-r--r--   0        0        0      899 2023-06-20 17:46:21.255873 jtech-1.0.6/jtech/clean_generators/clean_ready_event_listener_generator.py
+-rw-r--r--   0        0        0      873 2023-06-20 17:47:43.993047 jtech-1.0.6/jtech/clean_generators/clean_redis_generator.py
+-rw-r--r--   0        0        0     1394 2023-06-20 16:25:42.838850 jtech-1.0.6/jtech/clean_generators/clean_repository_default_generator.py
+-rw-r--r--   0        0        0     1296 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_repository_jpa_generator.py
+-rw-r--r--   0        0        0     1263 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_repository_mongo_generator.py
+-rw-r--r--   0        0        0     1112 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_request_generator.py
+-rw-r--r--   0        0        0     1175 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_response_generator.py
+-rw-r--r--   0        0        0     1176 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_usecase_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:58:17.065998 jtech-1.0.6/jtech/cqrs_generators/__init__.py
+-rw-r--r--   0        0        0     1082 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_aggregator_generator.py
+-rw-r--r--   0        0        0      740 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_api_error_generator.py
+-rw-r--r--   0        0        0      750 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_api_sub_error_generator.py
+-rw-r--r--   0        0        0      771 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_api_validation_error_generator.py
+-rw-r--r--   0        0        0      991 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_command_generator.py
+-rw-r--r--   0        0        0     1038 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_controller_generator.py
+-rw-r--r--   0        0        0     1460 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_entity_generator.py
+-rw-r--r--   0        0        0     1016 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_find_by_id_query_generator.py
+-rw-r--r--   0        0        0      793 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_gen_id_generator.py
+-rw-r--r--   0        0        0     5741 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_generator.py
+-rw-r--r--   0        0        0      762 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_global_handler_generator.py
+-rw-r--r--   0        0        0      951 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_http_utils_generator.py
+-rw-r--r--   0        0        0      782 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_jsons_generator.py
+-rw-r--r--   0        0        0      732 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_kafka_generator.py
+-rw-r--r--   0        0        0      740 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_openapi_generator.py
+-rw-r--r--   0        0        0      732 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_redis_generator.py
+-rw-r--r--   0        0        0     1026 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_default_generator.py
+-rw-r--r--   0        0        0     1170 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_jpa_generator.py
+-rw-r--r--   0        0        0     1164 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_mongo_generator.py
+-rw-r--r--   0        0        0      999 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_request_generator.py
+-rw-r--r--   0        0        0     1003 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_response_generator.py
+-rw-r--r--   0        0        0     1576 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_service_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 15:34:07.706004 jtech-1.0.6/jtech/creators/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-14 15:39:52.623663 jtech-1.0.6/jtech/creators/gradle_properties_creator.py
+-rw-r--r--   0        0        0      709 2023-06-14 15:43:22.480067 jtech-1.0.6/jtech/creators/readme_creator.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:00:13.758726 jtech-1.0.6/jtech/docker_compose/__init__.py
+-rw-r--r--   0        0        0     8152 2023-06-26 13:29:59.849326 jtech-1.0.6/jtech/docker_compose/generate_docker_compose.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:37:48.899891 jtech-1.0.6/jtech/manipulate/__init__.py
+-rw-r--r--   0        0        0     7631 2023-06-23 19:08:33.286070 jtech-1.0.6/jtech/manipulate/application_yml_manipulator.py
+-rw-r--r--   0        0        0     4034 2023-06-20 17:15:07.065746 jtech-1.0.6/jtech/manipulate/build_gradle_manipulator.py
+-rw-r--r--   0        0        0     2717 2023-06-20 19:28:16.842650 jtech-1.0.6/jtech/manipulate/java_class_manipulator.py
+-rw-r--r--   0        0        0      976 2023-06-23 19:08:14.046556 jtech-1.0.6/jtech/manipulate/yaml_manipulator.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:26:58.305867 jtech-1.0.6/jtech/mockserver/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-27 17:26:58.305867 jtech-1.0.6/jtech/mockserver/mockserver.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:19:25.872787 jtech-1.0.6/jtech/project/__init__.py
+-rw-r--r--   0        0        0     7241 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/project/create_project.py
+-rw-r--r--   0        0        0      540 2023-06-23 16:17:26.834452 jtech-1.0.6/jtech/resources/banner/banner.txt
+-rw-r--r--   0        0        0     1695 2023-06-20 18:41:45.182305 jtech-1.0.6/jtech/resources/dependencies/dependencies.json
+-rw-r--r--   0        0        0     2170 2023-06-26 14:52:11.058124 jtech-1.0.6/jtech/resources/mock/http.tar.gz
+-rw-r--r--   0        0        0     1699 2023-06-26 14:52:21.954146 jtech-1.0.6/jtech/resources/mock/mqtt.tar.gz
+-rw-r--r--   0        0        0     1096 2023-06-15 15:47:48.302121 jtech-1.0.6/jtech/resources/tpl/clean_adapter.tpl
+-rw-r--r--   0        0        0     2176 2023-06-20 16:45:02.296425 jtech-1.0.6/jtech/resources/tpl/clean_api_error.tpl
+-rw-r--r--   0        0        0      585 2023-06-20 16:46:15.081344 jtech-1.0.6/jtech/resources/tpl/clean_api_sub_error.tpl
+-rw-r--r--   0        0        0     1206 2023-06-20 16:47:28.810287 jtech-1.0.6/jtech/resources/tpl/clean_api_validation_error.tpl
+-rw-r--r--   0        0        0     1042 2023-06-15 15:47:25.965530 jtech-1.0.6/jtech/resources/tpl/clean_config.tpl
+-rw-r--r--   0        0        0     1517 2023-06-20 16:00:46.105564 jtech-1.0.6/jtech/resources/tpl/clean_controller.tpl
+-rw-r--r--   0        0        0     1528 2023-06-23 12:50:38.457021 jtech-1.0.6/jtech/resources/tpl/clean_domain.tpl
+-rw-r--r--   0        0        0      899 2023-06-23 13:22:13.689725 jtech-1.0.6/jtech/resources/tpl/clean_entity.tpl
+-rw-r--r--   0        0        0      794 2023-06-20 17:40:23.718478 jtech-1.0.6/jtech/resources/tpl/clean_gen_id.tpl
+-rw-r--r--   0        0        0     2375 2023-06-20 16:43:30.448004 jtech-1.0.6/jtech/resources/tpl/clean_global_handler.tpl
+-rw-r--r--   0        0        0      697 2023-06-15 15:48:21.222993 jtech-1.0.6/jtech/resources/tpl/clean_input_gateway.tpl
+-rw-r--r--   0        0        0     1020 2023-06-23 12:26:52.913732 jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity2.tpl
+-rw-r--r--   0        0        0     1026 2023-06-22 17:05:47.475660 jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity3.tpl
+-rw-r--r--   0        0        0     4654 2023-06-20 16:34:17.510426 jtech-1.0.6/jtech/resources/tpl/clean_jsons.tpl
+-rw-r--r--   0        0        0     1171 2023-06-20 16:42:13.632980 jtech-1.0.6/jtech/resources/tpl/clean_kafka.tpl
+-rw-r--r--   0        0        0     1107 2023-06-23 13:20:23.008763 jtech-1.0.6/jtech/resources/tpl/clean_mongo_entity.tpl
+-rw-r--r--   0        0        0     2490 2023-06-20 17:43:39.504623 jtech-1.0.6/jtech/resources/tpl/clean_openapi.tpl
+-rw-r--r--   0        0        0      701 2023-06-15 15:48:32.462291 jtech-1.0.6/jtech/resources/tpl/clean_output_gateway.tpl
+-rw-r--r--   0        0        0     1542 2023-06-22 16:26:15.375485 jtech-1.0.6/jtech/resources/tpl/clean_ready_listener.tpl
+-rw-r--r--   0        0        0     3582 2023-06-20 16:38:23.431913 jtech-1.0.6/jtech/resources/tpl/clean_redis.tpl
+-rw-r--r--   0        0        0      758 2023-06-15 15:48:41.589532 jtech-1.0.6/jtech/resources/tpl/clean_repository_default.tpl
+-rw-r--r--   0        0        0      856 2023-06-23 13:09:29.436274 jtech-1.0.6/jtech/resources/tpl/clean_repository_jpa.tpl
+-rw-r--r--   0        0        0      860 2023-06-23 13:10:31.845943 jtech-1.0.6/jtech/resources/tpl/clean_repository_mongo.tpl
+-rw-r--r--   0        0        0      974 2023-06-15 15:49:11.150315 jtech-1.0.6/jtech/resources/tpl/clean_request.tpl
+-rw-r--r--   0        0        0     1952 2023-06-15 15:49:19.726542 jtech-1.0.6/jtech/resources/tpl/clean_response.tpl
+-rw-r--r--   0        0        0     1276 2023-06-15 15:49:29.709807 jtech-1.0.6/jtech/resources/tpl/clean_usecase.tpl
+-rw-r--r--   0        0        0      941 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate.tpl
+-rw-r--r--   0        0        0     1616 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate_impl.tpl
+-rw-r--r--   0        0        0     2169 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_api_error.tpl
+-rw-r--r--   0        0        0      578 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_api_sub_error.tpl
+-rw-r--r--   0        0        0     1199 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_api_validation_error.tpl
+-rw-r--r--   0        0        0     1760 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_controller_command.tpl
+-rw-r--r--   0        0        0     1536 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_controller_query.tpl
+-rw-r--r--   0        0        0     1355 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_create_command.tpl
+-rw-r--r--   0        0        0      795 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_default_entity.tpl
+-rw-r--r--   0        0        0     1055 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_entity_jpa_2.tpl
+-rw-r--r--   0        0        0      997 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_entity_jpa_3.tpl
+-rw-r--r--   0        0        0     1060 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_entity_mongo.tpl
+-rw-r--r--   0        0        0      598 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_find_by_id_query.tpl
+-rw-r--r--   0        0        0      780 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_gen_id.tpl
+-rw-r--r--   0        0        0     2352 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_global_handler.tpl
+-rw-r--r--   0        0        0      884 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_http_utils.tpl
+-rw-r--r--   0        0        0     4644 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_jsons.tpl
+-rw-r--r--   0        0        0     1158 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_kafka.tpl
+-rw-r--r--   0        0        0     2474 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_openapi.tpl
+-rw-r--r--   0        0        0     3569 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_redis.tpl
+-rw-r--r--   0        0        0      745 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_repository_default.tpl
+-rw-r--r--   0        0        0      811 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_repository_jpa.tpl
+-rw-r--r--   0        0        0      815 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_repository_mongo.tpl
+-rw-r--r--   0        0        0     1019 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_request.tpl
+-rw-r--r--   0        0        0     1323 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_response.tpl
+-rw-r--r--   0        0        0      803 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_command.tpl
+-rw-r--r--   0        0        0     1260 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_command_impl.tpl
+-rw-r--r--   0        0        0      771 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_query.tpl
+-rw-r--r--   0        0        0     1306 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_query_impl.tpl
+-rw-r--r--   0        0        0        0 2023-06-19 13:04:59.491638 jtech-1.0.6/jtech/template_processor/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-28 14:38:39.932374 jtech-1.0.6/jtech/template_processor/template_processor.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:37:32.717465 jtech-1.0.6/jtech/utils/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/convert.py
+-rw-r--r--   0        0        0     1630 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/dir_constants.py
+-rw-r--r--   0        0        0      287 2023-06-20 19:39:52.159935 jtech-1.0.6/jtech/utils/file_remove.py
+-rw-r--r--   0        0        0      504 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/generator.py
+-rw-r--r--   0        0        0      688 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/param_configuration.py
+-rw-r--r--   0        0        0      521 2023-06-26 15:18:33.671487 jtech-1.0.6/jtech/utils/tar_gz_extractor.py
+-rw-r--r--   0        0        0     2180 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/tpl_constants.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:35:55.615903 jtech-1.0.6/jtech/webclient/__init__.py
+-rw-r--r--   0        0        0     1119 2023-06-19 17:10:17.936011 jtech-1.0.6/jtech/webclient/spring_boot_client.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:59:40.314234 jtech-1.0.6/jtech/wizards/__init__.py
+-rw-r--r--   0        0        0      575 2023-06-19 16:15:08.306931 jtech-1.0.6/jtech/wizards/architecture_choice_wizard.py
+-rw-r--r--   0        0        0     1248 2023-06-19 16:29:10.214206 jtech-1.0.6/jtech/wizards/checkbox_wizard.py
+-rw-r--r--   0        0        0     1825 2023-06-23 16:39:20.028880 jtech-1.0.6/jtech/wizards/metadata_wizard.py
+-rw-r--r--   0        0        0      741 2023-06-19 16:32:07.309879 jtech-1.0.6/jtech/wizards/project.py
+-rw-r--r--   0        0        0      570 2023-06-20 16:16:32.641378 jtech-1.0.6/jtech/wizards/samples_choice_wizard.py
+-rw-r--r--   0        0        0      659 2023-06-29 16:34:03.317942 jtech-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 jtech-1.0.6/PKG-INFO
```

### Comparing `jtech-1.0.5/jtech/__main__.py` & `jtech-1.0.6/jtech/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 import argparse
-
+import requests
+import subprocess
+from pkg_resources import parse_version
 import colorama
 import pkg_resources
 import textwrap3
 import platform
 
 from jtech.project.create_project import CreateProject
 
 
 def read_banner():
     banner_path = pkg_resources.resource_filename('jtech', 'resources/banner/banner.txt')
     with open(banner_path, 'r') as file:
         banner = file.read()
     return banner
 
+def check_update(current_version):
+    package_name = "jtech"
+    response = requests.get(f"https://pypi.org/pypi/{package_name}/json")
+    data = response.json()
+    latest_version = data["info"]["version"]
+
+    if parse_version(latest_version) > parse_version(current_version):
+        print(f"Uma nova versão ({latest_version}) está disponível. Deseja atualizar? (y/n)")
+        choice = input()
+
+        if choice.lower() == "y":
+            subprocess.run(["pip", "install", "--upgrade", package_name])
+            print("Atualização realizada com sucesso!")
+    else:
+        print("Você já está usando a versão mais recente.")
+
 
 def get_linux_distribution():
     with open('/etc/os-release', 'r') as f:
         lines = f.readlines()
 
     dist_info = {}
     for line in lines:
@@ -71,14 +89,15 @@
         if vargs.project_name:
             project.create(vargs.project_name)
         else:
             project.create()
 
     elif vargs.version:
         print_info_system(version)
+        check_update(version)
 
     else:
         parser.print_help()
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jtech-1.0.5/jtech/architecture/clean_architecture_generator.py` & `jtech-1.0.6/jtech/architecture/clean_architecture_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,89 +3,112 @@
 from jtech.clean_generators.clean_generator import CleanArchitectureGenerator
 from jtech.docker_compose.generate_docker_compose import GenerateDockerCompose
 from jtech.manipulate.application_yml_manipulator import ApplicationYmlManipulator
 from jtech.manipulate.java_class_manipulator import JavaFileManipulator
 from jtech.mockserver.mockserver import GenerateMockServer
 from jtech.utils.file_remove import RemoveFile
 
+import jtech.utils.dir_constants as const
+
 
 class CleanArchitectureStructureCreator:
     """
     Generate clean architecture structure and sample files.
 
     :param param: DTO with all parameters.
     """
 
     def __init__(self, param):
         self.param = param
 
     def create_structure(self):
         """Create folder structure."""
-        main_dir = os.path.join(self.param.base_dir, "src/main/java")
-        resources_dir = os.path.join(self.param.base_dir, "src/main/resources")
-        package_dir = self.param.package_name.replace(".", "/")
-        project_dir = os.path.join(main_dir, package_dir)
-        composer_dir = os.path.join(self.param.base_dir, "composer")
-        mockserver_dir = os.path.join(self.param.base_dir, "mockserver")
-
-        # Create folders
-        os.makedirs(project_dir, exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "application/core/domains"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "application/core/usecases"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "application/ports/input"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "application/ports/output"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "adapters/input/controllers"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "adapters/input/handlers"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "adapters/input/protocols"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "adapters/output/repositories/entities"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "config/infra/swagger"), exist_ok=True)
+        composer_dir, mockserver_dir, project_dir, resources_dir = self.generate_base_folder()
+        self.generate_subfolders(project_dir)
+        self.generate_docker_and_mockserver(composer_dir, mockserver_dir)
+        project = self.generate_sample_files(project_dir)
+        self.remove_application_properties(resources_dir)
+        self.create_yaml(resources_dir, project, self.param.package)
+        self.generate_docker_compose(composer_dir)
+        self.generate_mockserver(mockserver_dir)
 
-        if self.param.kafka:
-            os.makedirs(os.path.join(project_dir, "config/infra/kafka"), exist_ok=True)
-        if self.param.redis:
-            os.makedirs(os.path.join(project_dir, "config/infra/redis"), exist_ok=True)
+    def generate_mockserver(self, mockserver_dir):
+        """Generate mockserver folder and add mockeserver"""
+        mockserver = GenerateMockServer(path=mockserver_dir, param=self.param)
+        mockserver.generate()
 
-        os.makedirs(os.path.join(project_dir, "config/infra/utils"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "config/infra/exceptions"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "config/infra/handlers"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "config/infra/listeners"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "config/usecases"), exist_ok=True)
-        os.makedirs(os.path.join(project_dir, "config/infra"), exist_ok=True)
+    def generate_docker_compose(self, composer_dir):
+        docker_compose = GenerateDockerCompose(path=os.path.join(composer_dir, 'docker-compose.yml'), param=self.param)
+        docker_compose.generate()
 
-        os.makedirs(composer_dir, exist_ok=True)
-        os.makedirs(mockserver_dir, exist_ok=True)
+    def remove_application_properties(self, resources_dir):
+        application_properties = RemoveFile(os.path.join(resources_dir, "application.properties"))
+        application_properties.remove()
 
-        names = self.param.project_name.split("-")
+    def generate_sample_files(self, project_dir):
+        names = self.param.project.split("-")
         real_name = names[-1]
         cap_name = real_name[0].upper() + real_name[1:]
         if self.param.samples:
             self.generate_samples(project_name=real_name, cap_name=cap_name, project_dir=project_dir)
+        return real_name
 
-        application_properties = RemoveFile(os.path.join(resources_dir, "application.properties"))
-        application_properties.remove()
+    def generate_docker_and_mockserver(self, composer_dir, mockserver_dir):
+        os.makedirs(composer_dir, exist_ok=True)
+        os.makedirs(mockserver_dir, exist_ok=True)
 
-        self.create_yaml(os.path.join(resources_dir, "application.yml"), real_name, self.param.package_name)
+    def generate_subfolders(self, project_dir):
+        """Create subfolders for project"""
+        os.makedirs(project_dir, exist_ok=True)
+        subfolders = [
+            const.CLEAN_DOMAINS,
+            const.CLEAN_USECASE,
+            const.CLEAN_PORT_INPUT,
+            const.CLEAN_PORT_OUTPUT,
+            const.CLEAN_ADAPTERS_INPUT_CONTROLLERS,
+            const.CLEAN_ADAPTERS_INPUT_HANDLERS,
+            const.CLEAN_ADAPTERS_INPUT_PROTOCOLS,
+            const.CLEAN_ADAPTERS_OUTPUT_ENTITIES,
+            const.CLEAN_CONFIG_INFRA_SWAGGER,
+            const.CLEAN_CONFIG_INFRA_UTILS,
+            const.CLEAN_CONFIG_INFRA_EXCEPTIONS,
+            const.CLEAN_CONFIG_INFRA_HANDLERS,
+            const.CLEAN_CONFIG_INFRA_LISTENERS,
+            const.CLEAN_CONFIG_USECASES,
+        ]
 
-        docker_compose = GenerateDockerCompose(path=os.path.join(composer_dir, 'docker-compose.yml'), param=self.param)
-        docker_compose.generate()
+        for subfolder in subfolders:
+            os.makedirs(os.path.join(project_dir), subfolder)
 
-        mockserver = GenerateMockServer(path=mockserver_dir, param=self.param)
-        mockserver.generate()
+        if self.param.kafka:
+            os.makedirs(os.path.join(project_dir, const.CLEAN_CONFIG_INFRA_KAFKA), exist_ok=True)
+        if self.param.redis:
+            os.makedirs(os.path.join(project_dir, const.CLEAN_CONFIG_INFRA_REDIS), exist_ok=True)
+
+    def generate_base_folder(self):
+        main_dir = os.path.join(self.param.base_dir, "src/main/java")
+        resources_dir = os.path.join(self.param.base_dir, "src/main/resources")
+        package_dir = self.param.package.replace(".", "/")
+        project_dir = os.path.join(main_dir, package_dir)
+        composer_dir = os.path.join(self.param.base_dir, "composer")
+        mockserver_dir = os.path.join(self.param.base_dir, "mockserver")
+        return composer_dir, mockserver_dir, project_dir, resources_dir
 
-    def create_yaml(self, file, project, package):
+    def create_yaml(self, resources_dir, project, package):
+        file = os.path.join(resources_dir, "application.yml")
         application = ApplicationYmlManipulator(file)
         application.generate_header(project, package)
 
         if self.param.kafka:
             application.generate_kafka_configuration()
 
         if self.param.redis:
             application.generate_redis_configuration()
 
-        if self.param.jpa:
+        if self.param.is_jpa:
             application.generate_jpa_configuration()
 
         if self.param.mongo:
             application.generate_mongodb_configuration(project)
 
         if self.param.zipkin:
             application.generate_zipkin_configuration()
@@ -101,27 +124,27 @@
         generator = CleanArchitectureGenerator(project_name, cap_name, project_dir, self.param)
         generator.all()
 
         manipulator = JavaFileManipulator(os.path.join(project_dir, "Start" + cap_name + ".java"))
 
         if self.param.redis & self.param.kafka:
             imports = [
-                self.param.package_name + ".config.infra.kafka.KafkaConfiguration",
-                self.param.package_name + ".config.infra.redis.RedisConfiguration",
+                self.param.package + ".config.infra.kafka.KafkaConfiguration",
+                self.param.package + ".config.infra.redis.RedisConfiguration",
                 "org.springframework.context.annotation.Import"
             ]
             manipulator.add_import_to_class(["RedisConfiguration.class", "KafkaConfiguration.class"])
             manipulator.add_imports(imports)
         elif self.param.redis:
             imports = [
-                self.param.package_name + ".config.infra.redis.RedisConfiguration",
+                self.param.package + ".config.infra.redis.RedisConfiguration",
                 "org.springframework.context.annotation.Import"
             ]
             manipulator.add_import_to_class("RedisConfiguration.class")
             manipulator.add_imports(imports)
         elif self.param.kafka:
             imports = [
-                self.param.package_name + ".config.infra.kafka.KafkaConfiguration",
+                self.param.package + ".config.infra.kafka.KafkaConfiguration",
                 "org.springframework.context.annotation.Import"
             ]
             manipulator.add_import_to_class("KafkaConfiguration.class")
             manipulator.add_imports(imports)
```

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_adapter_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_adapter_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_api_error_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_api_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_api_sub_error_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_api_sub_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_api_validation_error_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_api_validation_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_config_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_config_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_controller_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_controller_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_domain_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_domain_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_entity_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_entity_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_gen_id_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_gen_id_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 from jtech.clean_generators.clean_jsons_generator import CleanJsonsGenerator
 from jtech.clean_generators.clean_kafka_generator import CleanKafkaGenerator
 from jtech.clean_generators.clean_openapi_generator import CleanOpenApiGenerator
 from jtech.clean_generators.clean_output_gateway_generator import CleanOutputGatewayGenerator
 from jtech.clean_generators.clean_ready_event_listener_generator import CleanReadyEventListenerGenerator
 from jtech.clean_generators.clean_redis_generator import CleanRedisGenerator
 from jtech.clean_generators.clean_repository_default_generator import CleanRepositoryDefaultGenerator
-from jtech.clean_generators.clean_repository_jpa_template import CleanRepositoryJpaGenerator
-from jtech.clean_generators.clean_repository_mongo_template import CleanRepositoryMongoGenerator
-from jtech.clean_generators.clean_request_template import CleanRequestGenerator
-from jtech.clean_generators.clean_response_template import CleanResponseGenerator
-from jtech.clean_generators.clean_usecase_template import CleanUseCaseGenerator
+from jtech.clean_generators.clean_repository_jpa_generator import CleanRepositoryJpaGenerator
+from jtech.clean_generators.clean_repository_mongo_generator import CleanRepositoryMongoGenerator
+from jtech.clean_generators.clean_request_generator import CleanRequestGenerator
+from jtech.clean_generators.clean_response_generator import CleanResponseGenerator
+from jtech.clean_generators.clean_usecase_generator import CleanUseCaseGenerator
 
 
 class CleanArchitectureGenerator:
     """
     Class for Generate all Java Classes
 
     :param project: Project name for use in lowercase.
@@ -37,125 +37,125 @@
         self.project = project
         self.capitalize = capitalize
         self.path = path
         self.param = param
 
     def gen_adapter(self):
         """Generate Adapter"""
-        adapter = CleanAdapterGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        adapter = CleanAdapterGenerator(self.param.package, self.project, self.capitalize, self.path)
         adapter.generate()
 
     def gen_config(self):
         """Generate UseCase Configuration"""
-        config = CleanConfigGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        config = CleanConfigGenerator(self.param.package, self.project, self.capitalize, self.path)
         config.generate()
 
     def gen_controller(self):
         """Generate Create Controller"""
-        controller = CleanControllerGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        controller = CleanControllerGenerator(self.param.package, self.project, self.capitalize, self.path)
         controller.generate()
 
     def gen_domain(self):
         """Generate Domain"""
-        domain = CleanDomainGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        domain = CleanDomainGenerator(self.param.package, self.project, self.capitalize, self.path)
         domain.generate()
 
     def gen_entity(self):
         """Generate JPA or MongoDB Entity"""
-        entity = CleanEntityGenerator(self.param.package_name, self.project, self.capitalize, self.path,
-                                      self.param.spring_version, self.param.jpa, self.param.mongo)
+        entity = CleanEntityGenerator(self.param.package, self.project, self.capitalize, self.path,
+                                      self.param.spring_version, self.param.is_jpa, self.param.mongo)
         entity.generate()
 
     def gen_input_gateway(self):
         """Generate Create Input Gateway Interface"""
-        gateway = CleanInputGatewayGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        gateway = CleanInputGatewayGenerator(self.param.package, self.project, self.capitalize, self.path)
         gateway.generate()
 
     def gen_output_gateway(self):
         """Generate Create Output Gateway Interface"""
-        gateway = CleanOutputGatewayGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        gateway = CleanOutputGatewayGenerator(self.param.package, self.project, self.capitalize, self.path)
         gateway.generate()
 
     def gen_repository(self):
         """Generate JPA or MongoDB repository"""
-        if self.param.jpa:
-            repository = CleanRepositoryJpaGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        if self.param.is_jpa:
+            repository = CleanRepositoryJpaGenerator(self.param.package, self.project, self.capitalize, self.path)
             repository.generate()
         elif self.param.mongo:
-            repository = CleanRepositoryMongoGenerator(self.param.package_name, self.project, self.capitalize,
+            repository = CleanRepositoryMongoGenerator(self.param.package, self.project, self.capitalize,
                                                        self.path)
             repository.generate()
         else:
-            repository = CleanRepositoryDefaultGenerator(self.param.package_name, self.project, self.capitalize,
+            repository = CleanRepositoryDefaultGenerator(self.param.package, self.project, self.capitalize,
                                                          self.path)
             repository.generate()
 
     def gen_request(self):
         """Generate Request Protocol"""
-        request = CleanRequestGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        request = CleanRequestGenerator(self.param.package, self.project, self.capitalize, self.path)
         request.generate()
 
     def gen_response(self):
         """Generate Response Protocol"""
-        response = CleanResponseGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        response = CleanResponseGenerator(self.param.package, self.project, self.capitalize, self.path)
         response.generate()
 
     def gen_usecase(self):
         """Generate UseCase"""
-        usecase = CleanUseCaseGenerator(self.param.package_name, self.project, self.capitalize, self.path)
+        usecase = CleanUseCaseGenerator(self.param.package, self.project, self.capitalize, self.path)
         usecase.generate()
 
     def gen_kafka_configuration(self):
         """Generate kafka Configuration if necessary"""
-        kafka = CleanKafkaGenerator(self.param.package_name, self.path)
+        kafka = CleanKafkaGenerator(self.param.package, self.path)
         kafka.generate()
 
     def gen_genid(self):
         """Generate GenId Utility class"""
-        genid = CleanGenIdGenerator(self.param.package_name, self.path)
+        genid = CleanGenIdGenerator(self.param.package, self.path)
         genid.generate()
 
     def gen_api_error(self):
         """Generate API Error"""
-        api_error = CleanApiErrorGenerator(self.param.package_name, self.path)
+        api_error = CleanApiErrorGenerator(self.param.package, self.path)
         api_error.generate()
 
     def gen_api_sub_error(self):
         """Generate API Sub Error Interface"""
-        api_error = CleanApiSubErrorGenerator(self.param.package_name, self.path)
+        api_error = CleanApiSubErrorGenerator(self.param.package, self.path)
         api_error.generate()
 
     def gen_api_validation_error(self):
         """Generate API Validation Error"""
-        api_error = CleanApiValidationErrorGenerator(self.param.package_name, self.path)
+        api_error = CleanApiValidationErrorGenerator(self.param.package, self.path)
         api_error.generate()
 
     def gen_global_exception_handler(self):
         """Generate Global Exception Error Handler"""
-        command = CleanGlobalExceptionHandlerGenerator(self.param.package_name, self.path)
+        command = CleanGlobalExceptionHandlerGenerator(self.param.package, self.path)
         command.generate()
 
     def gen_jsons(self):
         """Generate JSON Parser utility"""
-        command = CleanJsonsGenerator(self.param.package_name, self.path)
+        command = CleanJsonsGenerator(self.param.package, self.path)
         command.generate()
 
     def gen_openapi(self):
         """Generate configuration OpenAPI"""
-        command = CleanOpenApiGenerator(self.param.package_name, self.path)
+        command = CleanOpenApiGenerator(self.param.package, self.path)
         command.generate()
 
     def gen_redis_configuration(self):
         """Generate Redis Configuration if necessary"""
-        command = CleanRedisGenerator(self.param.package_name, self.path)
+        command = CleanRedisGenerator(self.param.package, self.path)
         command.generate()
 
     def gen_ready_event_listener(self):
         """Generate Ready Event Listener for Spring Boot"""
-        command = CleanReadyEventListenerGenerator(self.param.package_name, self.path)
+        command = CleanReadyEventListenerGenerator(self.param.package, self.path)
         command.generate()
 
     def all(self):
         """Generate All methods above"""
         self.gen_adapter()
         self.gen_config()
         self.gen_controller()
```

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_global_handler_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_global_handler_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_input_gateway_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_input_gateway_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_jsons_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_jsons_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_kafka_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_kafka_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_openapi_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_openapi_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_output_gateway_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_output_gateway_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_ready_event_listener_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_ready_event_listener_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_redis_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_redis_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_repository_default_generator.py` & `jtech-1.0.6/jtech/clean_generators/clean_repository_default_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_repository_jpa_template.py` & `jtech-1.0.6/jtech/clean_generators/clean_repository_jpa_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_repository_mongo_template.py` & `jtech-1.0.6/jtech/clean_generators/clean_repository_mongo_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_request_template.py` & `jtech-1.0.6/jtech/clean_generators/clean_request_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_response_template.py` & `jtech-1.0.6/jtech/clean_generators/clean_response_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/clean_generators/clean_usecase_template.py` & `jtech-1.0.6/jtech/clean_generators/clean_usecase_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/cqrs_generators/cars_controller_template.py` & `jtech-1.0.6/jtech/cqrs_generators/cqrs_controller_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import os
 import getpass
 
-from jtech.template_processor.template_processor import TemplateProcessor
+from jtech.utils.generator import Generator
+import jtech.utils.tpl_constants as tpl
+import jtech.utils.dir_constants as source
 
 
 class CqrsControllerGenerator:
     def __init__(self, package, project_name, cap_name, project_dir):
         self.package_name = package
         self.project_name = project_name
         self.cap_name = cap_name
         self.project_dir = project_dir
 
     def generate(self):
         target_filename_create = "Create" + self.cap_name + "Controller.java"
         target_filename_find = "Find" + self.cap_name + "ByIdController.java"
-        cmd_controller = TemplateProcessor("./tpl/cqrs_cmd_controller.tpl",
-                                           os.path.join(self.project_dir, "controllers/commands"))
-        qry_controller = TemplateProcessor("./tpl/cqrs_qry_controller.tpl",
-                                           os.path.join(self.project_dir, "controllers/queries"))
         data = {
             "package": self.package_name,
             "className": self.cap_name,
             "project": self.project_name,
             "username": getpass.getuser()
         }
-        cmd_controller.process_template(data, target_filename_create)
-        qry_controller.process_template(data, target_filename_find)
+        generator = Generator(self.project_dir, data)
+        generator.exec(tpl.CQRS_CONTROLLER_COMMAND, source.CQRS_CONTROLLERS_COMMANDS, target_filename_create)
+        generator.exec(tpl.CQRS_CONTROLLER_QUERY, source.CQRS_CONTROLLERS_QUERIES, target_filename_find)
```

### Comparing `jtech-1.0.5/jtech/creators/readme_creator.py` & `jtech-1.0.6/jtech/creators/readme_creator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/docker_compose/generate_docker_compose.py` & `jtech-1.0.6/jtech/docker_compose/generate_docker_compose.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/manipulate/application_yml_manipulator.py` & `jtech-1.0.6/jtech/manipulate/application_yml_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/manipulate/build_gradle_manipulator.py` & `jtech-1.0.6/jtech/manipulate/build_gradle_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/manipulate/java_class_manipulator.py` & `jtech-1.0.6/jtech/manipulate/java_class_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/manipulate/yaml_manipulator.py` & `jtech-1.0.6/jtech/manipulate/yaml_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/mockserver/mockserver.py` & `jtech-1.0.6/jtech/mockserver/mockserver.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/project/create_project.py` & `jtech-1.0.6/jtech/project/create_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from jtech.architecture.clean_architecture_generator import CleanArchitectureStructureCreator
+from jtech.architecture.cqrs_architecture_generator import CqrsArchitectureStructureCreator
 from jtech.creators.gradle_properties_creator import GradlePropertiesCreator
 from jtech.creators.readme_creator import ReadmeCreator
 from jtech.manipulate.build_gradle_manipulator import BuildGradleManipulator
 from jtech.utils.file_remove import RemoveFile
 from jtech.utils.param_configuration import ParamConfiguration
 from jtech.utils.tar_gz_extractor import TarGzExtractor
 from jtech.webclient.spring_boot_client import SpringBootWebClient
@@ -24,28 +25,30 @@
         # Load Metadata from user
         metadata = ProjectMetadataWizard(project_name)
         metadata.run()
         # Select default dependencies
         choice_dependencies = CheckboxWizard(options)
         selected_dependencies = choice_dependencies.run()
         # Select default architecture
-        choice_architecture = ArchitectureChoiceWizard(["Clean", "CQRS", "Default"])
+        choice_architecture = ArchitectureChoiceWizard(["CQRS", "Clean", "Default"])
         selected_architecture = choice_architecture.run()
         # Choice generate with samples or not
         choice_with_samples = SampleChoiceWizard(["yes", "no"])
         sample_selected = choice_with_samples.run()
         # Create Project DTO
         project = self.make_project_class(metadata, selected_dependencies)
         # Download default project from Spring Start
         filename = self.download_default_project(project)
         # Extract downloaded project em exclude own zip file
         self.extract_default_project_and_delete_zip(filename)
         # Create folder, files and configurations by architecture
         if selected_architecture == "Clean":
             self.create_clean_architecture(project, sample_selected, selected_dependencies)
+        elif selected_architecture == "CQRS":
+            self.create_cqrs_architecture(project, sample_selected, selected_dependencies)
         # Add libs, plugins and others
         self.manipulate_build_gradle(project, selected_dependencies)
         # Create gradle.properties file
         self.create_gradle_properties(project)
         # Remove files unnecessary
         self.remove_unnecessary_files(project)
 
@@ -84,14 +87,20 @@
 
     def create_clean_architecture(self, project, sample_selected, selected_dependencies):
         """Create Clean Architecture Structure"""
         param = self.extract_parameters(project, sample_selected, selected_dependencies)
         clean_architecture = CleanArchitectureStructureCreator(param)
         clean_architecture.create_structure()
 
+    def create_cqrs_architecture(self, project, sample_selected, selected_dependencies):
+        """Create CQRS Architecture Structure"""
+        param = self.extract_parameters(project, sample_selected, selected_dependencies)
+        cqrs_architecture = CqrsArchitectureStructureCreator(param)
+        cqrs_architecture.create_structure()
+
     def extract_parameters(self, project, sample_selected, selected_dependencies):
         """Create ParamConfiguration DTO"""
         has_jpa = "data-jpa" in selected_dependencies
         has_mongo = "data-mongodb" in selected_dependencies
         has_redis = "data-redis" in selected_dependencies
         has_kafka = "kafka" in selected_dependencies
         has_eureka_client = "cloud-eureka" in selected_dependencies
```

### Comparing `jtech-1.0.5/jtech/resources/banner/banner.txt` & `jtech-1.0.6/jtech/resources/banner/banner.txt`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/dependencies/dependencies.json` & `jtech-1.0.6/jtech/resources/dependencies/dependencies.json`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/mock/http.tar.gz` & `jtech-1.0.6/jtech/resources/mock/http.tar.gz`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/mock/mqtt.tar.gz` & `jtech-1.0.6/jtech/resources/mock/mqtt.tar.gz`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_adapter.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_adapter.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_api_error.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_api_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_api_sub_error.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_api_sub_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_api_validation_error.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_api_validation_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_config.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_config.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_controller.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_controller.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_domain.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_domain.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_entity.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_gen_id.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_gen_id.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_global_handler.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_global_handler.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_input_gateway.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_input_gateway.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_jpa_entity2.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity2.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_jpa_entity3.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity3.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_jsons.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_jsons.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_kafka.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_kafka.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_mongo_entity.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_mongo_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_openapi.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_openapi.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_output_gateway.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_output_gateway.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_ready_listener.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_ready_listener.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_redis.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_redis.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_repository_default.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_repository_default.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_repository_jpa.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_repository_jpa.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_repository_mongo.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_repository_mongo.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_request.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_request.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_response.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_response.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/clean_usecase.tpl` & `jtech-1.0.6/jtech/resources/tpl/clean_usecase.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/resources/tpl/cqrs_aggregate.tpl` & `jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate.tpl`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,23 @@
  *  ("Confidential Information"). You shall not disclose such Confidential
  *  Information and shall use it only in accordance with the terms of the
  *  license agreement you entered into with J-Tech.
  *
  */
 package {{ package }}.aggregate;
 
-import {{ package }}.services.commands.command.*;
+import {{ package }}.entities.{{ className }}Entity;
+import {{ package }}.services.commands.command.Create{{ className }}Command;
+import {{ package }}.services.queries.query.Find{{ className }}ByIdQuery;
 
-import java.util.List;
 import java.util.Optional;
 
 /**
  * {{ className }}Aggregate
  *
- *  user {{ username }}
+ *  @author {{ username }}
  */
 public interface {{ className }}Aggregate {
-    Optional<{{ className }}Entity> create({{ className }}Command command);
+    Optional<{{ className }}Entity> create(Create{{ className }}Command command);
+
+    {{ className }}Entity findById(Find{{ className }}ByIdQuery query);
 }
```

### Comparing `jtech-1.0.5/jtech/resources/tpl/cqrs_aggregate_impl.tpl` & `jtech-1.0.6/jtech/resources/tpl/cqrs_service_command_impl.tpl`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 /*
- *  @(#){{ className }}AggregateImpl.java
- *
- *  Copyright (c) J-Tech Solucoes em Informatica.
- *  All Rights Reserved.
- *
- *  This software is the confidential and proprietary information of J-Tech.
- *  ("Confidential Information"). You shall not disclose such Confidential
- *  Information and shall use it only in accordance with the terms of the
- *  license agreement you entered into with J-Tech.
- *
- */
-package {{ package }}.aggregate.impl;
+*  @(#)Create{{ className }}ServiceImpl.java
+*
+*  Copyright (c) J-Tech Solucoes em Informatica.
+*  All Rights Reserved.
+*
+*  This software is the confidential and proprietary information of J-Tech.
+*  ("Confidential Information"). You shall not disclose such Confidential
+*  Information and shall use it only in accordance with the terms of the
+*  license agreement you entered into with J-Tech.
+*
+*/
+package {{ package }}.services.commands.impl;
 
-import {{ package }}.aggregate.{{ className }}Aggregate;
+import {{ package }}.entities.{{ className }}Entity;
+import {{ package }}.repositories.{{ className }}Repository;
+import {{ package }}.services.commands.Create{{ className }}Service;
+import {{ package }}.services.commands.command.Create{{ className }}Command;
 import lombok.RequiredArgsConstructor;
 import org.springframework.stereotype.Service;
 
+import java.util.Optional;
 /**
- * {{ className }}AggregateImpl
- *
- *  user {{ username }}
- */
+* class Create{{ className }}ServiceImpl
+*
+* @author {{ username }}
+**/
 @Service
 @RequiredArgsConstructor
-public class {{ className }}AggregateImpl implements {{ className }}Aggregate {
+public class Create{{ className }}ServiceImpl implements Create{{ className }}Service {
 
-    private final Create{{ className }}Service createService;
+    private final {{ className }}Repository repository;
 
     @Override
-    public Optional<{{ className }}Entity> create({{ className }}Command command) {
-        return createService.create(command.toEntity());
+    public Optional<{{ className }}Entity> create(Create{{ className }}Command command) {
+        return Optional.of(repository.save(command.toEntity()));
     }
-
 }
+
+
```

### Comparing `jtech-1.0.5/jtech/resources/tpl/cqrs_cmd_controller.tpl` & `jtech-1.0.6/jtech/resources/tpl/cqrs_controller_query.tpl`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 
 /*
-*  @(#) Create{{className}}Controller.java
+*  @(#) Find{{className}}ByIdController.java
 *
 *  Copyright (c) J-Tech Solucoes em Informatica.
 *  All Rights Reserved.
 *
 *  This software is the confidential and proprietary information of J-Tech.
 *  ("Confidential Information"). You shall not disclose such Confidential
 *  Information and shall use it only in accordance with the terms of the
 *  license agreement you entered into with J-Tech.
 *
 */
-package {{ package }}.controllers.commands;
+package {{ package }}.controllers.queries;
 
+import {{ package }}.aggregate.{{ className }}Aggregate;
+import {{ package }}.protocols.{{ className }}Response;
+import {{ package }}.services.queries.query.Find{{ className }}ByIdQuery;
 import lombok.RequiredArgsConstructor;
 import org.springframework.http.ResponseEntity;
-import org.springframework.web.bind.annotation.PostMapping;
-import org.springframework.web.bind.annotation.RequestBody;
+import org.springframework.web.bind.annotation.GetMapping;
+import org.springframework.web.bind.annotation.PathVariable;
 import org.springframework.web.bind.annotation.RequestMapping;
 import org.springframework.web.bind.annotation.RestController;
-import {{ package }}.aggregate.*;
-import {{ package }}.protocols.*;
 
-import static {{ package }}.entities.{{ className }}.of;
+import java.util.UUID;
 
 /**
-* class Create{{ className }}Controller
+* class Find{{ className }}ByIdController
 * 
-* user {{ username }}
+* @author {{ username }}
 */
 @RestController
-@RequestMapping("/api/v1/{{ project }}s")
+@RequestMapping("/v1/{{ project }}s")
 @RequiredArgsConstructor
-public class Create{{ className }}Controller {
+public class Find{{ className }}ByIdController {
 
     private final {{ className }}Aggregate aggregate;
 
-    @PostMapping
-    public ResponseEntity<{{ className }}Response> create(@RequestBody {{ className }}Request request) {
-        var response = aggregate.create(of(request));
-        return ResponseEntity.ok({{ className }}Response.of(response));
-     }
- }
+
+    @GetMapping("/{id}")
+    public ResponseEntity<{{ className }}Response> findById(@PathVariable String id) {
+        return ResponseEntity.ok({{ className }}Response.of(this.aggregate
+                .findById(new Find{{ className }}ByIdQuery(UUID.fromString(id)))));
+
+    }
+}
```

### Comparing `jtech-1.0.5/jtech/resources/tpl/cqrs_entity.tpl` & `jtech-1.0.6/jtech/resources/tpl/cqrs_default_entity.tpl`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,27 @@
  *
  */
 package {{ package }}.entities;
 
 import lombok.AllArgsConstructor;
 import lombok.Builder;
 import lombok.Data;
-import lombok.NoArgsConstructor;
-import org.springframework.beans.BeanUtils;
+
+import java.io.Serializable;
+import java.util.UUID;
 
 /**
 * class {{ className  }}Entity 
 * 
-* user {{ username  }} 
+* @author {{ username  }}
 */
 @Data
 @Builder
-@NoArgsConstructor
 @AllArgsConstructor
-public class {{ className }}Entity {
+public class {{ className }}Entity implements Serializable {
 
-    //@NotEmpty(message = "ID not generated")
     //@Id
-    private String id;
+    private UUID id;
 
     //Others parameters...
 
-    public static {{ className }} of({{ className }}Request request) {
-        var entity = new {{ className }}();
-        BeanUtils.copyProperties(request, entity);
-        return entity;
-    }
-
 }
```

### Comparing `jtech-1.0.5/jtech/template_processor/template_processor.py` & `jtech-1.0.6/jtech/template_processor/template_processor.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/utils/param_configuration.py` & `jtech-1.0.6/jtech/utils/param_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class ParamConfiguration:
-    def __init__(self, base_dir, spring_version, project_name, package, jpa=False, mongo=False, samples=True,
+    def __init__(self, base_dir, spring_version, project, package, jpa=False, mongo=False, samples=True,
                  redis=False, kafka=False, eureka_client=False,
                  config_server=False, zipkin=False, rabbitmq=False):
         self.base_dir = base_dir
-        self.project_name = project_name
-        self.package_name = package
+        self.project = project
+        self.package = package
         self.jpa = jpa
         self.mongo = mongo
         self.samples = samples
         self.redis = redis
         self.kafka = kafka
         self.config_server = config_server
         self.zipkin = zipkin
```

### Comparing `jtech-1.0.5/jtech/utils/tar_gz_extractor.py` & `jtech-1.0.6/jtech/utils/tar_gz_extractor.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/webclient/spring_boot_client.py` & `jtech-1.0.6/jtech/webclient/spring_boot_client.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/wizards/architecture_choice_wizard.py` & `jtech-1.0.6/jtech/wizards/architecture_choice_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/wizards/checkbox_wizard.py` & `jtech-1.0.6/jtech/wizards/checkbox_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/wizards/metadata_wizard.py` & `jtech-1.0.6/jtech/wizards/metadata_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/wizards/project.py` & `jtech-1.0.6/jtech/wizards/project.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/jtech/wizards/samples_choice_wizard.py` & `jtech-1.0.6/jtech/wizards/samples_choice_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.5/pyproject.toml` & `jtech-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "jtech"
-version = "1.0.5"
+version = "1.0.6"
 description = "Jtech Project CLI"
 authors = ["Angelo Vicente Filho <angelo.vicente@veolia.com>"]
 
 [tool.poetry.scripts]
 jtech = "jtech.__main__:main"
 
 [tool.poetry.dependencies]
```

### Comparing `jtech-1.0.5/PKG-INFO` & `jtech-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtech
-Version: 1.0.5
+Version: 1.0.6
 Summary: Jtech Project CLI
 Author: Angelo Vicente Filho
 Author-email: angelo.vicente@veolia.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

