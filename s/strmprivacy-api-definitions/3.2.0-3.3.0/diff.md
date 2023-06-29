# Comparing `tmp/strmprivacy-api-definitions-3.2.0.tar.gz` & `tmp/strmprivacy-api-definitions-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strmprivacy-api-definitions-3.2.0.tar", last modified: Wed Jun 28 12:26:12 2023, max compression
+gzip compressed data, was "strmprivacy-api-definitions-3.3.0.tar", last modified: Thu Jun 29 07:57:55 2023, max compression
```

## Comparing `strmprivacy-api-definitions-3.2.0.tar` & `strmprivacy-api-definitions-3.3.0.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.436246 strmprivacy-api-definitions-3.2.0/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-28 12:26:12.435246 strmprivacy-api-definitions-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 12:26:12.436246 strmprivacy-api-definitions-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-28 12:25:34.000000 strmprivacy-api-definitions-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.288233 strmprivacy-api-definitions-3.2.0/strmprivacy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.288233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.289233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.289233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12198 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/v1/account_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16789 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.290233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.292233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3261 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.293233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.293233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5030 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.294233 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.295234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5338 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.295234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.296234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7665 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10858 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.297234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.298234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/v1/cli_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.298234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.299234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3987 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6740 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.299234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.300234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8979 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.301234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.302234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7497 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.302234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.303234 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5978 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.307235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.308235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22863 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28488 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.308235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.309235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9865 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.309235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.310235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81835 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.310235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12632 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.311235 strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.331237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15658 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20098 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.331237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.332237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.332237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.334237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7909 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6958 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10345 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.334237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.338237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6199 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9342 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.339237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.339237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.339237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.340237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5369 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8964 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.341237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.341237 strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.344238 strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.362239 strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.363239 strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.364240 strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10605 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13648 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.365240 strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.366240 strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.367240 strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.375240 strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9075 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.375240 strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.376241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.376241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.377241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.377241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.382241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7409 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.383241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.384241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7458 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14509 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.384241 strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.392242 strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.392242 strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.399242 strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    17973 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.400243 strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.403243 strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5254 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.405243 strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.409243 strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.409243 strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.415244 strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:26:11.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4644 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4831 2023-06-28 12:24:56.000000 strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:26:12.435246 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-28 12:26:12.000000 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7436 2023-06-28 12:26:12.000000 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 12:26:12.000000 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 12:26:12.000000 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-28 12:26:12.000000 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-28 12:26:12.000000 strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.408593 strmprivacy-api-definitions-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-29 07:57:55.407593 strmprivacy-api-definitions-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:57:55.408593 strmprivacy-api-definitions-3.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-29 07:57:30.000000 strmprivacy-api-definitions-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.373589 strmprivacy-api-definitions-3.3.0/strmprivacy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.373589 strmprivacy-api-definitions-3.3.0/strmprivacy/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.374590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.374590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12198 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.375589 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.377590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.377590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.377590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.378590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.378590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.379590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.379590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10858 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.379590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.380590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.380590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.381590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.381590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.382590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8979 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.382590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.383590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.383590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.384590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.384590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.384590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22863 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.385590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.385590 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9865 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.386591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.386591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81835 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.387591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12632 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.387591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.388591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15658 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20098 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.388591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.389591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.389591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.391591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6958 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10345 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.391591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.392591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6199 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.392591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.392591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.393591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.393591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8964 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.394591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.394591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.394591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.395591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.395591 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.396592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10605 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13648 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.396592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.397592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.397592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.398592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.398592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.399592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.399592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.399592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.400592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.400592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.401592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.401592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.402592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.402592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.402592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.403592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17973 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.403592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.404592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.404592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.405592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.405592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.406592 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:57:54.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-06-29 07:56:56.000000 strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:57:55.407593 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-29 07:57:55.000000 strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/top_level.txt
```

### Comparing `strmprivacy-api-definitions-3.2.0/PKG-INFO` & `strmprivacy-api-definitions-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.2.0
+Version: 3.3.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.2.0/setup.py` & `strmprivacy-api-definitions-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/v1/account_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/v1/audit_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/v1/cli_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/v1/comments_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1/entities_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/v1/handles_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/entities_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installations_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/paging/v1/paging_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/paging/v1/paging_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/v1/policies_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from strmprivacy.api.entities.v1alpha import entities_v1alpha_pb2 as strmprivacy_dot_api_dot_entities_dot_v1alpha_dot_entities__v1alpha__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAstrmprivacy/api/project_plans/v1alpha/project_plans_v1alpha.proto\x12%strmprivacy.api.project_plans.v1alpha\x1a\x1fgoogle/api/field_behavior.proto\x1a\x37strmprivacy/api/entities/v1alpha/entities_v1alpha.proto\x1a\x17validate/validate.proto\":\n\x17ListProjectPlansRequest\x12\x1f\n\x0bis_template\x18\x01 \x01(\x08R\nisTemplate\"n\n\x18ListProjectPlansResponse\x12R\n\rproject_plans\x18\x01 \x03(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanR\x0cprojectPlans\"@\n\x15GetProjectPlanRequest\x12\'\n\nproject_id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"o\n\x16GetProjectPlanResponse\x12U\n\x0cproject_plan\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanB\x03\xe0\x41\x02R\x0bprojectPlan\"q\n\x18UpsertProjectPlanRequest\x12U\n\x0cproject_plan\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanB\x03\xe0\x41\x02R\x0bprojectPlan\"r\n\x19UpsertProjectPlanResponse\x12U\n\x0cproject_plan\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanB\x03\xe0\x41\x02R\x0bprojectPlan2\xd4\x03\n\x13ProjectPlansService\x12\x93\x01\n\x10ListProjectPlans\x12>.strmprivacy.api.project_plans.v1alpha.ListProjectPlansRequest\x1a?.strmprivacy.api.project_plans.v1alpha.ListProjectPlansResponse\x12\x8d\x01\n\x0eGetProjectPlan\x12<.strmprivacy.api.project_plans.v1alpha.GetProjectPlanRequest\x1a=.strmprivacy.api.project_plans.v1alpha.GetProjectPlanResponse\x12\x96\x01\n\x11UpsertProjectPlan\x12?.strmprivacy.api.project_plans.v1alpha.UpsertProjectPlanRequest\x1a@.strmprivacy.api.project_plans.v1alpha.UpsertProjectPlanResponseB\x82\x01\n(io.strmprivacy.api.project_plans.v1alphaP\x01ZTgithub.com/strmprivacy/api-definitions-go/v2/api/project_plans/v1alpha;project_plansb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAstrmprivacy/api/project_plans/v1alpha/project_plans_v1alpha.proto\x12%strmprivacy.api.project_plans.v1alpha\x1a\x1fgoogle/api/field_behavior.proto\x1a\x37strmprivacy/api/entities/v1alpha/entities_v1alpha.proto\x1a\x17validate/validate.proto\"p\n\x17ListProjectPlansRequest\x12\x1f\n\x0bis_template\x18\x01 \x01(\x08R\nisTemplate\x12\x34\n\x16include_dummy_template\x18\x02 \x01(\x08R\x14includeDummyTemplate\"n\n\x18ListProjectPlansResponse\x12R\n\rproject_plans\x18\x01 \x03(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanR\x0cprojectPlans\"@\n\x15GetProjectPlanRequest\x12\'\n\nproject_id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"o\n\x16GetProjectPlanResponse\x12U\n\x0cproject_plan\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanB\x03\xe0\x41\x02R\x0bprojectPlan\"q\n\x18UpsertProjectPlanRequest\x12U\n\x0cproject_plan\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanB\x03\xe0\x41\x02R\x0bprojectPlan\"r\n\x19UpsertProjectPlanResponse\x12U\n\x0cproject_plan\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1alpha.ProjectPlanB\x03\xe0\x41\x02R\x0bprojectPlan2\xd4\x03\n\x13ProjectPlansService\x12\x93\x01\n\x10ListProjectPlans\x12>.strmprivacy.api.project_plans.v1alpha.ListProjectPlansRequest\x1a?.strmprivacy.api.project_plans.v1alpha.ListProjectPlansResponse\x12\x8d\x01\n\x0eGetProjectPlan\x12<.strmprivacy.api.project_plans.v1alpha.GetProjectPlanRequest\x1a=.strmprivacy.api.project_plans.v1alpha.GetProjectPlanResponse\x12\x96\x01\n\x11UpsertProjectPlan\x12?.strmprivacy.api.project_plans.v1alpha.UpsertProjectPlanRequest\x1a@.strmprivacy.api.project_plans.v1alpha.UpsertProjectPlanResponseB\x82\x01\n(io.strmprivacy.api.project_plans.v1alphaP\x01ZTgithub.com/strmprivacy/api-definitions-go/v2/api/project_plans/v1alpha;project_plansb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'strmprivacy.api.project_plans.v1alpha.project_plans_v1alpha_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n(io.strmprivacy.api.project_plans.v1alphaP\001ZTgithub.com/strmprivacy/api-definitions-go/v2/api/project_plans/v1alpha;project_plans'
@@ -29,21 +29,21 @@
   _GETPROJECTPLANRESPONSE.fields_by_name['project_plan']._options = None
   _GETPROJECTPLANRESPONSE.fields_by_name['project_plan']._serialized_options = b'\340A\002'
   _UPSERTPROJECTPLANREQUEST.fields_by_name['project_plan']._options = None
   _UPSERTPROJECTPLANREQUEST.fields_by_name['project_plan']._serialized_options = b'\340A\002'
   _UPSERTPROJECTPLANRESPONSE.fields_by_name['project_plan']._options = None
   _UPSERTPROJECTPLANRESPONSE.fields_by_name['project_plan']._serialized_options = b'\340A\002'
   _LISTPROJECTPLANSREQUEST._serialized_start=223
-  _LISTPROJECTPLANSREQUEST._serialized_end=281
-  _LISTPROJECTPLANSRESPONSE._serialized_start=283
-  _LISTPROJECTPLANSRESPONSE._serialized_end=393
-  _GETPROJECTPLANREQUEST._serialized_start=395
-  _GETPROJECTPLANREQUEST._serialized_end=459
-  _GETPROJECTPLANRESPONSE._serialized_start=461
-  _GETPROJECTPLANRESPONSE._serialized_end=572
-  _UPSERTPROJECTPLANREQUEST._serialized_start=574
-  _UPSERTPROJECTPLANREQUEST._serialized_end=687
-  _UPSERTPROJECTPLANRESPONSE._serialized_start=689
-  _UPSERTPROJECTPLANRESPONSE._serialized_end=803
-  _PROJECTPLANSSERVICE._serialized_start=806
-  _PROJECTPLANSSERVICE._serialized_end=1274
+  _LISTPROJECTPLANSREQUEST._serialized_end=335
+  _LISTPROJECTPLANSRESPONSE._serialized_start=337
+  _LISTPROJECTPLANSRESPONSE._serialized_end=447
+  _GETPROJECTPLANREQUEST._serialized_start=449
+  _GETPROJECTPLANREQUEST._serialized_end=513
+  _GETPROJECTPLANRESPONSE._serialized_start=515
+  _GETPROJECTPLANRESPONSE._serialized_end=626
+  _UPSERTPROJECTPLANREQUEST._serialized_start=628
+  _UPSERTPROJECTPLANREQUEST._serialized_end=741
+  _UPSERTPROJECTPLANRESPONSE._serialized_start=743
+  _UPSERTPROJECTPLANRESPONSE._serialized_end=857
+  _PROJECTPLANSSERVICE._serialized_start=860
+  _PROJECTPLANSSERVICE._serialized_end=1328
 # @@protoc_insertion_point(module_scope)
```

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/v1/projects_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/v1/streams_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/v1/usage_v1_pb2.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.3.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/PKG-INFO` & `strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.2.0
+Version: 3.3.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.2.0/strmprivacy_api_definitions.egg-info/SOURCES.txt` & `strmprivacy-api-definitions-3.3.0/strmprivacy_api_definitions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

