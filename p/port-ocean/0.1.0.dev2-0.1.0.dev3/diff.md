# Comparing `tmp/port_ocean-0.1.0.dev2.tar.gz` & `tmp/port_ocean-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev2.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0.dev3.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev2.tar` & `port_ocean-0.1.0.dev3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     3218 2023-06-28 11:41:00.486335 port_ocean-0.1.0.dev2/README.md
--rw-r--r--   0        0        0      440 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     3385 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       54 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0      598 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0      751 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      406 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0     1091 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/example.config.yaml
--rw-r--r--   0        0        0      392 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0      640 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/project.toml
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1334 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      766 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0    10983 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0      593 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2592 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/config/base.py
--rw-r--r--   0        0        0     1035 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3811 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     1896 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/context/event.py
--rw-r--r--   0        0        0     3995 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/base.py
--rw-r--r--   0        0        0      300 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0      685 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     2516 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      452 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1426 2023-06-28 11:41:00.518336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      909 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1173 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/get_required_entities.py
--rw-r--r--   0        0        0     1043 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     4677 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1495 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     3589 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      687 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2393 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     7018 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      448 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/base.py
--rw-r--r--   0        0        0     2616 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/factory.py
--rw-r--r--   0        0        0      817 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/http.py
--rw-r--r--   0        0        0     3229 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/kafka.py
--rw-r--r--   0        0        0      909 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/settings.py
--rw-r--r--   0        0        0     1957 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/core/utils.py
--rw-r--r--   0        0        0      166 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/errors.py
--rw-r--r--   0        0        0      534 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/logging.py
--rw-r--r--   0        0        0     2064 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4421 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/port_ocean.py
--rw-r--r--   0        0        0      563 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/port_ocean/types.py
--rw-r--r--   0        0        0     1845 2023-06-28 11:41:00.522336 port_ocean-0.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     3218 2023-06-29 12:30:35.401267 port_ocean-0.1.0.dev3/README.md
+-rw-r--r--   0        0        0      440 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     3385 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       54 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0      598 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1718 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      406 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0      392 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1184 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1334 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      766 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0    10983 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0      593 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2592 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1035 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     3825 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     1896 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4017 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/base.py
+-rw-r--r--   0        0        0      300 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/__init__.py
+-rw-r--r--   0        0        0      690 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/base.py
+-rw-r--r--   0        0        0     2521 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/jq_manipulation.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1432 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/base.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/__init__.py
+-rw-r--r--   0        0        0     1173 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/get_required_entities.py
+-rw-r--r--   0        0        0     1043 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     4656 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/transport.py
+-rw-r--r--   0        0        0     1495 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     3593 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2393 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0     7023 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/models.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/__init__.py
+-rw-r--r--   0        0        0      448 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/base.py
+-rw-r--r--   0        0        0     2616 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/factory.py
+-rw-r--r--   0        0        0      817 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/http.py
+-rw-r--r--   0        0        0     3229 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/kafka.py
+-rw-r--r--   0        0        0      909 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/settings.py
+-rw-r--r--   0        0        0      563 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/types.py
+-rw-r--r--   0        0        0     1957 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/utils.py
+-rw-r--r--   0        0        0      166 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/errors.py
+-rw-r--r--   0        0        0      534 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2064 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4269 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/port_ocean.py
+-rw-r--r--   0        0        0     1938 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev3/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev2/README.md` & `port_ocean-0.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/cli/commands.py` & `port_ocean-0.1.0.dev3/port_ocean/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 # ruff: noqa: E501
 
 import os
 
 import click
 from cookiecutter.main import cookiecutter  # type: ignore
-from rich import print
-from rich.console import Console
-
 from port_ocean.cli.download_git_folder import download_folder
 from port_ocean.cli.list_integrations import list_git_folders
+from rich import print
+from rich.console import Console
 
 
 def print_logo() -> None:
     ascii_art = """
 =====================================================================================
           ::::::::       ::::::::       ::::::::::           :::        ::::    ::: 
         :+:    :+:     :+:    :+:      :+:                :+: :+:      :+:+:   :+:  
@@ -63,15 +62,15 @@
     console.print(
         "\n🌊 Ahoy, Captain! Your project has set sail into the vast ocean of possibilities!",
         style="bold",
     )
     console.print("Here are your next steps: \n", style="bold")
     console.print(
         "⚓️ Install necessary packages: Run [bold][blue]make install[/blue][/bold] to install all required packages for your project.\n"
-        f"▶️ [bold][blue]cd {path}/{name} && make install && . venv/bin/activate[/blue][/bold]\n"
+        f"▶️ [bold][blue]cd {path}/{name} && make install && . .venv/bin/activate[/blue][/bold]\n"
     )
     console.print(
         "⚓️ Set sail with [blue]Ocean[/blue]: Run [bold][blue]ocean sail[/blue] <path_to_integration>[/bold] to run the project using Ocean.\n"
         f"▶️ [bold][blue]ocean sail {path}/{name}[/blue][/bold] \n"
     )
     console.print(
         "⚓️ Smooth sailing with [blue]Make[/blue]: Alternatively, you can run [bold][blue]make run[/blue][/bold] to launch your project using Make. \n"
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile` & `port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0.dev3/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0.dev3/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/clients/port/client.py` & `port_ocean-0.1.0.dev3/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/clients/port/types.py` & `port_ocean-0.1.0.dev3/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/config/base.py` & `port_ocean-0.1.0.dev3/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/config/integration.py` & `port_ocean-0.1.0.dev3/port_ocean/config/integration.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0.dev3/port_ocean/consumers/kafka_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from pydantic import BaseModel
 
 from port_ocean.consumers.base_consumer import BaseConsumer
 
 
 class KafkaConsumerConfig(BaseModel):
     brokers: str
-    username: str | None
-    password: str | None
+    username: str | None = None
+    password: str | None = None
     security_protocol: str
     authentication_mechanism: str
     kafka_security_enabled: bool
 
 
 class KafkaConsumer(BaseConsumer):
     def __init__(
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/context/event.py` & `port_ocean-0.1.0.dev3/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/context/ocean.py` & `port_ocean-0.1.0.dev3/port_ocean/context/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 from fastapi import APIRouter
 from werkzeug.local import LocalProxy, LocalStack
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.core.models import Entity
+from port_ocean.core.types import (
+    RESYNC_EVENT_LISTENER,
+    START_EVENT_LISTENER,
+    RawEntityDiff,
+)
 from port_ocean.errors import PortOceanContextNotFoundError
-from port_ocean.types import RESYNC_EVENT_LISTENER, START_EVENT_LISTENER, RawEntityDiff
 
 if TYPE_CHECKING:
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.port_ocean import Ocean
 
 
 @dataclass
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/manipulation/base.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 from dataclasses import dataclass, field
 
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
-from port_ocean.types import RawEntityDiff, EntityDiff
+from port_ocean.core.types import RawEntityDiff, EntityDiff
 
 
 @dataclass
 class EntityPortDiff:
     deleted: list[Entity] = field(default_factory=list)
     modified: list[Entity] = field(default_factory=list)
     created: list[Entity] = field(default_factory=list)
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/manipulation/jq_manipulation.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/jq_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any
 
 import pyjq as jq  # type: ignore
 
 from port_ocean.core.handlers.manipulation.base import BaseManipulation
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
-from port_ocean.types import RawEntityDiff, EntityDiff
+from port_ocean.core.types import RawEntityDiff, EntityDiff
 
 
 class JQManipulation(BaseManipulation):
     @lru_cache
     def _compile(self, pattern: str) -> Any:
         return jq.compile(pattern)
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Optional
 
-from pydantic import BaseModel, Field
-
 from port_ocean.clients.port.types import RequestOptions
+from pydantic import BaseModel, Field
 
 
 class EntityMapping(BaseModel):
     identifier: str
-    title: str
+    title: str | None
     blueprint: str
     properties: dict[str, str] = Field(default_factory=dict)
     relations: dict[str, str] = Field(default_factory=dict)
 
 
 class PortResourceConfig(BaseModel):
     class MappingsConfig(BaseModel):
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/base.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.models import Entity
-from port_ocean.types import EntityDiff
+from port_ocean.core.types import EntityDiff
 
 
 class BaseTransport(BaseWithContext):
     DEFAULT_USER_AGENT_TYPE = UserAgentType.exporter
 
     @abstractmethod
     async def update_diff(
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/get_required_entities.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/get_required_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/transport.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import asyncio
 from itertools import chain
 
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.context.event import event
-from port_ocean.core.handlers.manipulation.base import (
-    EntityPortDiff,
-)
+from port_ocean.core.handlers.manipulation.base import EntityPortDiff
 from port_ocean.core.handlers.transport.base import BaseTransport
 from port_ocean.core.handlers.transport.port.order_by_entities_dependencies import (
     order_by_entities_dependencies,
 )
 from port_ocean.core.handlers.transport.port.validate_entity_relations import (
     validate_entity_relations,
 )
 from port_ocean.core.models import Entity
-from port_ocean.core.utils import (
-    is_same_entity,
-    get_unique,
-    get_port_diff,
-)
-from port_ocean.types import EntityDiff
+from port_ocean.core.types import EntityDiff
+from port_ocean.core.utils import is_same_entity, get_unique, get_port_diff
 
 
 class HttpPortTransport(BaseTransport):
     async def _validate_delete_dependent_entities(self, entities: list[Entity]) -> None:
         logger.info("Validated deleted entities")
         if not event.port_app_config.delete_dependent_entities:
             deps = await asyncio.gather(
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0.dev3/port_ocean/core/integrations/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 from typing import (
     Any,
 )
 
 from loguru import logger
-
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.context.event import (
     event_context,
     TriggerType,
 )
 from port_ocean.context.ocean import PortOceanContext
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
@@ -34,15 +33,15 @@
     async def _sync_new_in_batches(
         self, resource_config: ResourceConfig, user_agent_type: UserAgentType
     ) -> list[Entity]:
         resource, results = await self._get_resource_raw_results(resource_config)
 
         tasks = []
 
-        batch_size = self.context.config.batch_work_size or len(results)
+        batch_size = self.context.config.batch_work_size or len(results) or 1
         for batch in [
             results[i : i + batch_size] for i in range(0, len(results), batch_size)
         ]:
             tasks.append(self._register_resource_raw(resource, batch, user_agent_type))
         entities = await asyncio.gather(*tasks)
         return sum(entities, [])
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 
-from port_ocean.types import (
+from port_ocean.core.types import (
     IntegrationEventsCallbacks,
     START_EVENT_LISTENER,
     RESYNC_EVENT_LISTENER,
 )
 
 
 class EventsMixin:
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.events import EventsMixin
 from port_ocean.core.integrations.mixins.handler import HandlerMixin
 from port_ocean.core.models import Entity
+from port_ocean.core.types import RawEntityDiff, EntityDiff
 from port_ocean.core.utils import validate_result, zip_and_sum
-from port_ocean.types import RawEntityDiff, EntityDiff
 
 
 class SyncMixin(HandlerMixin, EventsMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
         EventsMixin.__init__(self)
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/models.py` & `port_ocean-0.1.0.dev3/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/factory.py` & `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/http.py` & `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/http.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/kafka.py` & `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/kafka.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/trigger_channel/settings.py` & `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/core/utils.py` & `port_ocean-0.1.0.dev3/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/logging.py` & `port_ocean-0.1.0.dev3/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/middlewares.py` & `port_ocean-0.1.0.dev3/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/port_ocean/port_ocean.py` & `port_ocean-0.1.0.dev3/port_ocean/port_ocean.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from inspect import getmembers, isclass
 from types import ModuleType
 from typing import Type, Callable
 
 import uvicorn
 from fastapi import FastAPI, APIRouter
 from loguru import logger
-from starlette.types import Scope, Receive, Send
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.context.ocean import (
     PortOceanContext,
     ocean,
     initialize_port_ocean_context,
 )
 from port_ocean.core.integrations.base import BaseIntegration
-from pydantic import BaseSettings
-
 from port_ocean.middlewares import request_handler
+from pydantic import BaseSettings
+from starlette.types import Scope, Receive, Send
 
 
 def _get_base_integration_class_from_module(
     module: ModuleType,
 ) -> Type[BaseIntegration]:
     for name, obj in getmembers(module):
         if (
@@ -43,18 +42,14 @@
         raise Exception(f"Failed to load integration from path: {file_path}")
 
     module = module_from_spec(spec)
 
     try:
         spec.loader.exec_module(module)
     except Exception as e:
-        logger.error(
-            f"Failed to load integration with error: {e}, "
-            f"please validate the integration type exists"
-        )
         raise e
 
     return module
 
 
 def _include_target_channel_router(app: FastAPI, _ocean: PortOceanContext) -> None:
     target_channel_router = APIRouter()
```

### Comparing `port_ocean-0.1.0.dev2/port_ocean/types.py` & `port_ocean-0.1.0.dev3/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev2/pyproject.toml` & `port_ocean-0.1.0.dev3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.dev2"
+version = "0.1.0.dev3"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
     { include = "port_ocean", from = "." }
 ]
 
@@ -47,15 +47,17 @@
 types-requests = "^2.31.0.1"
 types-pyyaml = "^6.0.12.10"
 ruff = "^0.0.272"
 
 
 [tool.mypy]
 exclude = [
-    'port_ocean/cli/cookiecutter'
+    'port_ocean/cli/cookiecutter',
+    'venv',
+    'integrations'
 ]
 plugins = [
     "pydantic.mypy"
 ]
 
 follow_imports = "silent"
 warn_redundant_casts = true
@@ -67,14 +69,15 @@
 # for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
 
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
 ignore = ["E501"]
+exclude = ['venv', 'integrations']
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
@@ -86,9 +89,11 @@
 /(
   \scripts
   \.toml
   |\.sh
   |\.git
   |\.ini
   |Dockerfile
+  |\.venv
+  |integrations
 )/
 '''
```

### Comparing `port_ocean-0.1.0.dev2/PKG-INFO` & `port_ocean-0.1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
```

