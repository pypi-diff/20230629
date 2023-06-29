# Comparing `tmp/datarobot_bosun-9.1.1rc1-py3-none-any.whl.zip` & `tmp/datarobot_bosun-9.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,74 +1,74 @@
-Zip file size: 125605 bytes, number of entries: 72
--rw-r--r--  2.0 unx      583 b- defN 23-May-18 21:10 bosun/model_connector/__init__.py
--rw-rw-r--  2.0 unx      399 b- defN 23-May-18 21:10 bosun/model_connector/config_external.json
--rw-r--r--  2.0 unx     1507 b- defN 23-May-18 21:10 bosun/model_connector/constants.py
--rw-r--r--  2.0 unx     1395 b- defN 23-May-18 21:10 bosun/model_connector/file_uri_fetcher.py
--rw-r--r--  2.0 unx     7190 b- defN 23-May-18 21:10 bosun/model_connector/mc_bosun.py
--rw-r--r--  2.0 unx     5269 b- defN 23-May-18 21:10 bosun/model_connector/mc_runner.py
--rw-r--r--  2.0 unx     5433 b- defN 23-May-18 21:10 bosun/model_connector/model_connector_base.py
--rw-r--r--  2.0 unx     2334 b- defN 23-May-18 21:10 bosun/model_connector/s3_uri_fetcher.py
--rw-r--r--  2.0 unx      894 b- defN 23-May-18 21:10 bosun/model_connector/uri_fetcher_base.py
--rw-r--r--  2.0 unx      583 b- defN 23-May-18 21:10 bosun/plugin/__init__.py
--rw-r--r--  2.0 unx     2260 b- defN 23-May-18 21:10 bosun/plugin/action_status.py
--rw-r--r--  2.0 unx     6147 b- defN 23-May-18 21:10 bosun/plugin/bosun_plugin_base.py
--rw-r--r--  2.0 unx    11466 b- defN 23-May-18 21:10 bosun/plugin/bosun_test_plugin.py
--rw-r--r--  2.0 unx     2833 b- defN 23-May-18 21:10 bosun/plugin/constants.py
--rw-r--r--  2.0 unx     3354 b- defN 23-May-18 21:10 bosun/plugin/deployment_info.py
--rw-r--r--  2.0 unx     1047 b- defN 23-May-18 21:10 bosun/plugin/exceptions.py
--rw-r--r--  2.0 unx     2493 b- defN 23-May-18 21:10 bosun/plugin/pe_info.py
--rw-r--r--  2.0 unx    16799 b- defN 23-May-18 21:10 bosun/plugin/plugin_runner.py
--rw-r--r--  2.0 unx      640 b- defN 23-May-18 21:10 bosun/plugin/azureml/__init__.py
--rw-r--r--  2.0 unx    12218 b- defN 23-May-18 21:10 bosun/plugin/azureml/azureml_plugin.py
--rw-r--r--  2.0 unx     3313 b- defN 23-May-18 21:10 bosun/plugin/azureml/azureml_status_reporter.py
--rw-r--r--  2.0 unx     1516 b- defN 23-May-18 21:10 bosun/plugin/azureml/template_renderer.py
--rw-r--r--  2.0 unx    18410 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/base_endpoint_client.py
--rw-r--r--  2.0 unx     6743 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/batch_endpoint_client.py
--rw-r--r--  2.0 unx    17972 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/online_endpoint_client.py
--rw-r--r--  2.0 unx     1394 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/scoring_snippets.py
--rw-r--r--  2.0 unx      583 b- defN 23-May-18 21:10 bosun/plugin/azureml/config/__init__.py
--rw-r--r--  2.0 unx    11520 b- defN 23-May-18 21:10 bosun/plugin/azureml/config/azureml_client_config.py
--rw-r--r--  2.0 unx     3420 b- defN 23-May-18 21:10 bosun/plugin/azureml/config/config_keys.py
--rw-r--r--  2.0 unx     3767 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/batch_score.py
--rw-r--r--  2.0 unx     9634 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/common.py
--rw-rw-r--  2.0 unx      697 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/conda.yml
--rw-r--r--  2.0 unx     5452 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/online_score.py
--rw-rw-r--  2.0 unx      963 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/scoring_script_builder.py.j2
--rw-r--r--  2.0 unx      702 b- defN 23-May-18 21:10 bosun/plugin/config_samples/__init__.py
--rw-r--r--  2.0 unx      757 b- defN 23-May-18 21:10 bosun/plugin/docker/__init__.py
--rw-r--r--  2.0 unx    14934 b- defN 23-May-18 21:10 bosun/plugin/docker/docker_helper.py
--rw-r--r--  2.0 unx    23290 b- defN 23-May-18 21:10 bosun/plugin/docker/docker_plugin.py
--rw-r--r--  2.0 unx     5419 b- defN 23-May-18 21:10 bosun/plugin/docker/docker_plugin_config.py
--rw-r--r--  2.0 unx     7897 b- defN 23-May-18 21:10 bosun/plugin/docker/mlops_monitoring.py
--rw-r--r--  2.0 unx      646 b- defN 23-May-18 21:10 bosun/plugin/filesystem/__init__.py
--rw-r--r--  2.0 unx    14021 b- defN 23-May-18 21:10 bosun/plugin/filesystem/filesystem_plugin.py
--rw-r--r--  2.0 unx      646 b- defN 23-May-18 21:10 bosun/plugin/k8s/__init__.py
--rw-r--r--  2.0 unx    37071 b- defN 23-May-18 21:10 bosun/plugin/k8s/client.py
--rw-r--r--  2.0 unx    20247 b- defN 23-May-18 21:10 bosun/plugin/k8s/config.py
--rw-r--r--  2.0 unx    28225 b- defN 23-May-18 21:10 bosun/plugin/k8s/kubernetes_plugin.py
--rw-r--r--  2.0 unx     9170 b- defN 23-May-18 21:10 bosun/plugin/k8s/manifests.py
--rw-rw-r--  2.0 unx      303 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2
--rw-rw-r--  2.0 unx     2263 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/_helpers.j2
--rw-rw-r--  2.0 unx     4603 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2
--rw-rw-r--  2.0 unx     1393 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/image-builder.yaml.j2
--rw-rw-r--  2.0 unx      356 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2
--rw-rw-r--  2.0 unx     1106 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources.yaml.j2
--rw-rw-r--  2.0 unx     4929 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2
--rw-rw-r--  2.0 unx      119 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2
--rw-rw-r--  2.0 unx      842 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2
--rw-rw-r--  2.0 unx     1253 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2
--rw-rw-r--  2.0 unx      484 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2
--rw-rw-r--  2.0 unx      547 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/service.yaml.j2
--rw-r--r--  2.0 unx      630 b- defN 23-May-18 21:10 bosun/plugin/s3/__init__.py
--rw-r--r--  2.0 unx    11175 b- defN 23-May-18 21:10 bosun/plugin/s3/s3_plugin.py
--rw-r--r--  2.0 unx     2705 b- defN 23-May-18 21:10 bosun/plugin/s3/s3_plugin_config.py
--rw-r--r--  2.0 unx      644 b- defN 23-May-18 21:10 bosun/plugin/snowflake/__init__.py
--rw-r--r--  2.0 unx    10034 b- defN 23-May-18 21:10 bosun/plugin/snowflake/snowflake_plugin.py
--rw-r--r--  2.0 unx     5491 b- defN 23-May-18 21:10 bosun/plugin/snowflake/snowflake_plugin_config.py
--rwxr-xr-x  2.0 unx      671 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner
--rwxr-xr-x  2.0 unx      676 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.data/scripts/mcrunner
--rwxr-xr-x  2.0 unx      671 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner
--rw-r--r--  2.0 unx     4471 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6972 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/RECORD
-72 files, 395689 bytes uncompressed, 114239 bytes compressed:  71.1%
+Zip file size: 127328 bytes, number of entries: 72
+-rw-r--r--  2.0 unx      583 b- defN 23-Jun-29 21:29 bosun/model_connector/__init__.py
+-rw-rw-r--  2.0 unx      399 b- defN 23-Jun-29 21:29 bosun/model_connector/config_external.json
+-rw-r--r--  2.0 unx     1507 b- defN 23-Jun-29 21:29 bosun/model_connector/constants.py
+-rw-r--r--  2.0 unx     1395 b- defN 23-Jun-29 21:29 bosun/model_connector/file_uri_fetcher.py
+-rw-r--r--  2.0 unx     7190 b- defN 23-Jun-29 21:29 bosun/model_connector/mc_bosun.py
+-rw-r--r--  2.0 unx     5269 b- defN 23-Jun-29 21:29 bosun/model_connector/mc_runner.py
+-rw-r--r--  2.0 unx     5433 b- defN 23-Jun-29 21:29 bosun/model_connector/model_connector_base.py
+-rw-r--r--  2.0 unx     2334 b- defN 23-Jun-29 21:29 bosun/model_connector/s3_uri_fetcher.py
+-rw-r--r--  2.0 unx      894 b- defN 23-Jun-29 21:29 bosun/model_connector/uri_fetcher_base.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jun-29 21:29 bosun/plugin/__init__.py
+-rw-r--r--  2.0 unx     2260 b- defN 23-Jun-29 21:29 bosun/plugin/action_status.py
+-rw-r--r--  2.0 unx     6240 b- defN 23-Jun-29 21:29 bosun/plugin/bosun_plugin_base.py
+-rw-r--r--  2.0 unx    11492 b- defN 23-Jun-29 21:29 bosun/plugin/bosun_test_plugin.py
+-rw-r--r--  2.0 unx     2833 b- defN 23-Jun-29 21:29 bosun/plugin/constants.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-Jun-29 21:29 bosun/plugin/deployment_info.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Jun-29 21:29 bosun/plugin/exceptions.py
+-rw-r--r--  2.0 unx     2493 b- defN 23-Jun-29 21:29 bosun/plugin/pe_info.py
+-rw-r--r--  2.0 unx    16892 b- defN 23-Jun-29 21:29 bosun/plugin/plugin_runner.py
+-rw-r--r--  2.0 unx      640 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/__init__.py
+-rw-r--r--  2.0 unx    12219 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/azureml_plugin.py
+-rw-r--r--  2.0 unx     3313 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/azureml_status_reporter.py
+-rw-r--r--  2.0 unx     1516 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/template_renderer.py
+-rw-r--r--  2.0 unx    20318 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/client/base_endpoint_client.py
+-rw-r--r--  2.0 unx     6797 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/client/batch_endpoint_client.py
+-rw-r--r--  2.0 unx    17972 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/client/online_endpoint_client.py
+-rw-r--r--  2.0 unx     1394 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/client/scoring_snippets.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/config/__init__.py
+-rw-r--r--  2.0 unx    11520 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/config/azureml_client_config.py
+-rw-r--r--  2.0 unx     3420 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/config/config_keys.py
+-rw-r--r--  2.0 unx     4719 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/templates/batch_score.py
+-rw-r--r--  2.0 unx    11617 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/templates/common.py
+-rw-rw-r--  2.0 unx      697 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/templates/conda.yml
+-rw-r--r--  2.0 unx     6394 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/templates/online_score.py
+-rw-rw-r--  2.0 unx      963 b- defN 23-Jun-29 21:29 bosun/plugin/azureml/templates/scoring_script_builder.py.j2
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-29 21:29 bosun/plugin/config_samples/__init__.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Jun-29 21:29 bosun/plugin/docker/__init__.py
+-rw-r--r--  2.0 unx    14934 b- defN 23-Jun-29 21:29 bosun/plugin/docker/docker_helper.py
+-rw-r--r--  2.0 unx    23367 b- defN 23-Jun-29 21:29 bosun/plugin/docker/docker_plugin.py
+-rw-r--r--  2.0 unx     5419 b- defN 23-Jun-29 21:29 bosun/plugin/docker/docker_plugin_config.py
+-rw-r--r--  2.0 unx     7897 b- defN 23-Jun-29 21:29 bosun/plugin/docker/mlops_monitoring.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-29 21:29 bosun/plugin/filesystem/__init__.py
+-rw-r--r--  2.0 unx    14022 b- defN 23-Jun-29 21:29 bosun/plugin/filesystem/filesystem_plugin.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/__init__.py
+-rw-r--r--  2.0 unx    37071 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/client.py
+-rw-r--r--  2.0 unx    20270 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/config.py
+-rw-r--r--  2.0 unx    28225 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/kubernetes_plugin.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/manifests.py
+-rw-rw-r--  2.0 unx      303 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2
+-rw-rw-r--  2.0 unx     2263 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/_helpers.j2
+-rw-rw-r--  2.0 unx     4603 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2
+-rw-rw-r--  2.0 unx     1393 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/image-builder.yaml.j2
+-rw-rw-r--  2.0 unx      356 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2
+-rw-rw-r--  2.0 unx     1106 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources.yaml.j2
+-rw-rw-r--  2.0 unx     4929 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2
+-rw-rw-r--  2.0 unx      119 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2
+-rw-rw-r--  2.0 unx      842 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2
+-rw-rw-r--  2.0 unx     1253 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2
+-rw-rw-r--  2.0 unx      484 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2
+-rw-rw-r--  2.0 unx      547 b- defN 23-Jun-29 21:29 bosun/plugin/k8s/templates/model-resources/service.yaml.j2
+-rw-r--r--  2.0 unx      630 b- defN 23-Jun-29 21:29 bosun/plugin/s3/__init__.py
+-rw-r--r--  2.0 unx    11176 b- defN 23-Jun-29 21:29 bosun/plugin/s3/s3_plugin.py
+-rw-r--r--  2.0 unx     2705 b- defN 23-Jun-29 21:29 bosun/plugin/s3/s3_plugin_config.py
+-rw-r--r--  2.0 unx      644 b- defN 23-Jun-29 21:29 bosun/plugin/snowflake/__init__.py
+-rw-r--r--  2.0 unx    10035 b- defN 23-Jun-29 21:29 bosun/plugin/snowflake/snowflake_plugin.py
+-rw-r--r--  2.0 unx     5491 b- defN 23-Jun-29 21:29 bosun/plugin/snowflake/snowflake_plugin_config.py
+-rwxr-xr-x  2.0 unx      671 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.data/scripts/bosun-plugin-runner
+-rwxr-xr-x  2.0 unx      676 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.data/scripts/mcrunner
+-rwxr-xr-x  2.0 unx      671 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.data/scripts/plugin-runner
+-rw-r--r--  2.0 unx     4547 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6952 b- defN 23-Jun-29 21:38 datarobot_bosun-9.1.3.dist-info/RECORD
+72 files, 402291 bytes uncompressed, 116004 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -189,29 +189,29 @@
 
 Filename: bosun/plugin/snowflake/snowflake_plugin.py
 Comment: 
 
 Filename: bosun/plugin/snowflake/snowflake_plugin_config.py
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner
+Filename: datarobot_bosun-9.1.3.data/scripts/bosun-plugin-runner
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.data/scripts/mcrunner
+Filename: datarobot_bosun-9.1.3.data/scripts/mcrunner
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner
+Filename: datarobot_bosun-9.1.3.data/scripts/plugin-runner
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.dist-info/METADATA
+Filename: datarobot_bosun-9.1.3.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.dist-info/WHEEL
+Filename: datarobot_bosun-9.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.dist-info/top_level.txt
+Filename: datarobot_bosun-9.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_bosun-9.1.1rc1.dist-info/RECORD
+Filename: datarobot_bosun-9.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosun/plugin/bosun_plugin_base.py

```diff
@@ -18,14 +18,15 @@
 from abc import abstractmethod
 from typing import Optional
 
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.constants import BosunPluginActions
 from bosun.plugin.constants import BosunPluginConfigConstants
+from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
 from bosun.plugin.pe_info import PEInfo
 
 
 class BosunPluginBase(ABC):
     def __init__(
         self,
@@ -127,15 +128,17 @@
                 raise Exception(f"Action is not supported: {action}")
             if not isinstance(action_status, ActionStatusInfo):
                 raise Exception(f"Action {action} provide - did not return ActionStatusInfo object")
         except Exception as e:
             msg = f"Exception occurred while running action {action} : error {e}"
             self._logger.error(msg)
             traceback.print_exc()
-            action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
+            action_status = ActionStatusInfo(
+                ActionStatus.ERROR, msg=msg, state=DeploymentState.ERROR
+            )
 
         action_end = time.time()
         action_status.set_duration(round(action_end - action_start, 4))
         action_status.write_to_file(status_file=status_file)
 
         return action_status
```

## bosun/plugin/bosun_test_plugin.py

```diff
@@ -236,20 +236,20 @@
                 content["status_timestamp"] = datetime.datetime.utcnow().isoformat()
                 deployment_file.seek(0)
                 deployment_file.write(yaml.safe_dump(content))
                 deployment_file.truncate()
                 action_status = ActionStatusInfo(
                     ActionStatus.OK,
                     msg="Deployment health looks good",
-                    state="ready",
+                    state=DeploymentState.READY,
                     data={ActionDataFields.CURRENT_MODEL_ID: content["model_id"]},
                 )
         else:
             action_status = ActionStatusInfo(
-                ActionStatus.ERROR, msg="Deployment not found", state="errored"
+                ActionStatus.ERROR, msg="Deployment not found", state=DeploymentState.ERROR
             )
         self._logger.info("done deployment_status")
         return action_status
 
     def deployment_list(self):
         """
         Get the list of running deployments
```

## bosun/plugin/deployment_info.py

```diff
@@ -38,14 +38,16 @@
                 "modelExecutionType": And(str, len),
                 Optional("keyValueConfig", default={}): dict,
                 Optional("name"): str,
                 Optional("description"): Or(None, str),
                 Optional("modelArtifact"): Or(None, And(str, len, Use(Path))),
                 Optional("modelFormat"): Or(None, str),
                 Optional("newModelId"): And(str, len),
+                Optional("featureTypes"): Or(None, And(str, len, Use(Path))),
+                Optional("settings"): Or(None, And(str, len, Use(Path))),
                 Optional("isPredictionExplanationsSupported"): Or(None, bool),
             },
             ignore_extra_keys=True,
         )
 
         self._deployment_info = schema.validate(deployment_info)
 
@@ -95,9 +97,17 @@
         return self._deployment_info["keyValueConfig"]
 
     @property
     def new_model_id(self) -> Nullable[str]:
         return self._deployment_info.get("newModelId")
 
     @property
+    def feature_types_path(self) -> Nullable[Path]:
+        return self._deployment_info.get("featureTypes")
+
+    @property
+    def settings_path(self) -> Nullable[Path]:
+        return self._deployment_info.get("settings")
+
+    @property
     def is_prediction_explanations_supported(self) -> bool:
         return self._deployment_info.get("isPredictionExplanationsSupported", False)
```

## bosun/plugin/plugin_runner.py

```diff
@@ -27,14 +27,15 @@
 
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import BosunPluginActions
 from bosun.plugin.constants import BosunPluginConfigConstants
 from bosun.plugin.constants import DeploymentInfoConfigConstants
+from bosun.plugin.constants import DeploymentState
 from bosun.plugin.constants import PeInfoConfigConstants
 
 # TODO: add ability for plugin to generate private config file template
 # TODO: add ability for plugin to generate plugin description
 # TODO: A test to verify gen-config option
 # TODO: change bosun python package to datarobot-bosun (bosun is already used on pip).
 # TODO: pass pe_info config to pe_status
@@ -312,15 +313,17 @@
                 plugin_module, plugin_config, self._private_config_file, pe_info, deployment_info
             )
         except Exception as e:
             msg = "Exception occurred while loading plugin object for action {}: error {}".format(
                 self._action, e
             )
             logger.exception(msg)
-            action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
+            action_status = ActionStatusInfo(
+                ActionStatus.ERROR, msg=msg, state=DeploymentState.ERROR
+            )
 
             action_status.write_to_file(status_file=self._status_file)
             return action_status
 
         return pbe.run_action(self._action, deployment_info, status_file=self._status_file)
```

## bosun/plugin/azureml/azureml_plugin.py

```diff
@@ -68,15 +68,15 @@
             if len(datarobot_model_deployments) > 0
             else "No deployments found"
         )
 
         self._logger.info(status_msg)
 
         deployments_map = {
-            deployment_id: ActionStatusInfo(ActionStatus.OK, state=deployment_state).__dict__
+            deployment_id: ActionStatusInfo(ActionStatus.OK, state=deployment_state).to_dict()
             for deployment_id, deployment_state in datarobot_model_deployments.items()
         }
 
         return ActionStatusInfo(ActionStatus.OK, msg=status_msg, data=deployments_map)
 
     def deployment_start(
         self,
```

## bosun/plugin/azureml/client/base_endpoint_client.py

```diff
@@ -5,14 +5,15 @@
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
+import json
 import logging
 from abc import ABC
 from abc import abstractmethod
 from datetime import datetime
 from datetime import timezone
 from functools import cached_property
 from pathlib import Path
@@ -39,14 +40,15 @@
 from bosun.plugin.azureml.config.azureml_client_config import EndpointType
 from bosun.plugin.azureml.config.config_keys import Constants
 from bosun.plugin.azureml.config.config_keys import Key
 from bosun.plugin.azureml.config.config_keys import ProvisioningState
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
 from bosun.plugin.pe_info import PEInfo
+from datarobot.mlops.common.aggregation_util import convert_feature_format
 
 
 class BaseEndpointClient(ABC):
     _EXTERNAL_TO_INTERNAL_STATE_MAP = {
         ProvisioningState.FAILED.value: DeploymentState.ERROR,
         ProvisioningState.SUCCEEDED.value: DeploymentState.READY,
         ProvisioningState.DELETING.value: DeploymentState.SHUTTING_DOWN,
@@ -144,14 +146,32 @@
                 description="DataRobot environment containing MLOPS library and wrappers to run "
                 "scoring model.",
                 conda_file=Path(AZURE_TEMPLATE_DIR) / "conda.yml",
                 tags=self.prediction_environment_tags,
             )
             return self._client.environments.create_or_update(env_docker_image)
 
+    def copy_feature_types(self, workdir):
+        """
+        Copies feature_types into the same directory as scoring code wrapper, so
+        feature_types can be loaded before inference is started.
+        """
+        source_path = self.deployment.feature_types_path
+        assert source_path
+        target_path = Path(workdir) / "feature_types.json"
+
+        with open(source_path, "r") as source_file:
+            data = json.load(source_file)
+        # MLOps monitoring library requires all feature data to be in a different format from what
+        # the public API outputs.
+        feature_types = [convert_feature_format(f) for f in data["data"]]
+
+        with open(target_path, "w") as target_file:
+            json.dump(feature_types, target_file)
+
     def register_model(self, model_path):
         model_tags = {Key.DATAROBOT_MODEL_ID.value: self.datarobot_model_id}
         model_tags.update(self.prediction_environment_tags)
 
         model = Model(
             name=self.datarobot_model_name,
             path=model_path,
@@ -323,18 +343,37 @@
             # Our scoring script doesn't need Flask 1.x compatibility and just adds complexity
             "AML_FLASK_ONE_COMPATIBILITY": "False",
         }
         if self.config.is_monitoring_enabled:
             bootstrap_server = (
                 f"{self.config[Key.AZURE_EVENTHUBS_NAMESPACE]}.servicebus.windows.net:9093"
             )
+            association_id_column = None
+            association_id_allow_missing = None
+            if self.deployment and self.deployment.settings_path:
+                with open(self.deployment.settings_path) as settings_file:
+                    deployment_settings = json.load(settings_file)
+                    association_id = deployment_settings.get("associationId")
+                    if association_id:
+                        association_id_column = association_id["columnNames"]
+                        association_id_allow_missing = not association_id[
+                            "requiredInPredictionRequests"
+                        ]
+
+                if association_id_column:
+                    # composite association IDs are not supported
+                    assert len(association_id_column) == 1
+                    association_id_column = association_id_column[0]
+
             base_vars.update(
                 {
                     "MLOPS_DEPLOYMENT_ID": self.datarobot_deployment_id,
                     "MLOPS_MODEL_ID": self.datarobot_model_id,
+                    "MLOPS_ASSOCIATION_ID_COLUMN": association_id_column,
+                    "MLOPS_ASSOCIATION_ID_ALLOW_MISSING_VALUES": association_id_allow_missing,
                     "MLOPS_SPOOLER_TYPE": "KAFKA",
                     "MLOPS_KAFKA_BOOTSTRAP_SERVERS": bootstrap_server,
                     "MLOPS_KAFKA_TOPIC_NAME": self.config[Key.AZURE_EVENTHUBS_INSTANCE],
                     # We are using a managed identity to authenticate with EventHubs, so we need to
                     # set the client_id of the user defined identity and turn on OAuth:
                     #   https://github.com/Azure/azure-sdk-for-python/blob/azure-identity_1.12.0/sdk/identity/azure-identity/azure/identity/_credentials/managed_identity.py#L70-L72
                     "MLOPS_KAFKA_SASL_MECHANISM": "OAUTHBEARER",
```

## bosun/plugin/azureml/client/batch_endpoint_client.py

```diff
@@ -60,14 +60,15 @@
         }
         deployment_tags.update(self.prediction_environment_tags)
         with tempfile.TemporaryDirectory() as scoring_code_dir, open(
             Path(scoring_code_dir) / scoring_script_name, "w"
         ) as scoring_code_file:
             scoring_code_file.write(self.get_scoring_snippet(model_filename))
             scoring_code_file.flush()
+            self.copy_feature_types(scoring_code_dir)
 
             deployment = BatchDeployment(
                 name=deployment_name or self.deployment_name,
                 endpoint_name=self.endpoint_name,
                 model=model,
                 code_configuration=CodeConfiguration(
                     code=str(scoring_code_dir), scoring_script=scoring_script_name
```

## bosun/plugin/azureml/templates/batch_score.py

```diff
@@ -5,14 +5,15 @@
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
+import http.client as http_codes
 import logging
 import os
 import time
 from pathlib import Path
 
 import pandas as pd
 
@@ -25,47 +26,61 @@
 
     # TODO: [AGENT-4189] to work around jpype issues, we can't start the JVM until
     # we are in the worker process (after the fork). For now just do some simple
     # sanity checks.
     if not MODEL_PATH.exists():
         raise RuntimeError(f"Model JAR is not present: {MODEL_PATH}")
 
+    # Sanity check to make sure we can load the feature types but we will actually use them
+    # after we fork.
+    read_feature_types()  # noqa: F821
+
 
 def run(mini_batch):
     start_time = time.monotonic_ns()
     model, model_id = load_model(MODEL_PATH)  # noqa: F821
-    # AGENT-4338: calculate feature_types (e.g. FeatureDescriptors) for the model to support
-    # stats agg
-    mlops_sdk = get_mlops(model_id=model_id)  # noqa: F821
+    feature_types = read_feature_types()  # noqa: F821
+    mlops_sdk = get_mlops(model_id=model_id, feature_types=feature_types)  # noqa: F821
 
     # TODO: not sure how to pass params at runtime so just use the defaults for now.
     params = GenericModelParams()  # noqa: F821
     return make_prediction(model, mini_batch, params, mlops_sdk, start_time)
 
 
 def make_prediction(model, scoring_batches, params, mlops_sdk, start_time) -> pd.DataFrame:
+    # Delay importing this exception until we know jpype has been loaded
+    from java.lang import Exception as JavaException
+
     incoming = []
     results = []
     for iteration, file_path in enumerate(scoring_batches, start=1):
         try:
             df = pd.read_csv(file_path, dtype=model.features)
-        except Exception:
+        except Exception as err:
             logging.exception("#%s: error while loading inference data: %s", iteration, file_path)
+            msg = f"#{iteration}: error while loading inference data: {file_path}: {err}"
+            report_prediction_server_error_via_tracking_agent(  # noqa: F821
+                mlops_sdk, msg, http_codes.BAD_REQUEST
+            )
             continue
 
         try:
             logging.info("Scoring batch #%s", iteration)
             predictions: pd.DataFrame = model.predict(df, **params.dict())
-        except Exception:
+        except (Exception, JavaException) as err:
             # Log the error but continue so we can correctly support the `error_threshold`
             # the user has configured. The AzureML platform does this by monitoring the
             # the gap between mini-batch input count and returns. 'Batch inferencing' scenario
             # should return a list, dataframe, or tuple with the successful items to try to meet
             # this threshold.
             logging.exception("#%s: error while scoring: %s", iteration, df)
+            msg = f"#{iteration}: error while scoring: {df}: {err}"
+            report_prediction_server_error_via_tracking_agent(  # noqa: F821
+                mlops_sdk, msg, http_codes.UNPROCESSABLE_ENTITY
+            )
             predictions = pd.DataFrame()
         if predictions.empty:
             logging.warning("Empty results, batch #%s", iteration)
             # TODO: add logic to fillna prediction data so it will line up with feature data and
             # we can at least send that but for now just skip the batch entirely.
             continue
 
@@ -74,17 +89,19 @@
         results.append(predictions)
     combined_predictions = pd.concat(results) if results else pd.DataFrame()
     combined_scoring_data = pd.concat(incoming) if incoming else pd.DataFrame()
 
     report_service_health_via_tracking_agent(  # noqa: F821
         mlops_sdk, start_time, combined_predictions
     )
-    report_predictions_data_via_tracking_agent(  # noqa: F821
-        mlops_sdk,
-        model,
-        combined_predictions,
-        combined_scoring_data,
-        params,
-        # AGENT-4338: Uncomment when MLOps init is done
-        # max_unaggregated_rows=MAX_RAW_ROWS,
-    )
+    # If the combined scoring data is empty then that means this run completely failed so
+    # no need to attempt to report any prediction data back to MLOps.
+    if not combined_scoring_data.empty:
+        report_predictions_data_via_tracking_agent(  # noqa: F821
+            mlops_sdk,
+            model,
+            combined_predictions,
+            combined_scoring_data,
+            params,
+            max_unaggregated_rows=MAX_RAW_ROWS,
+        )
     return combined_predictions
```

## bosun/plugin/azureml/templates/common.py

```diff
@@ -5,19 +5,21 @@
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
+import json
 import logging
 import os
 import shutil
 import time
 from datetime import datetime
+from enum import Enum
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 from datarobot_predict.scoring_code import ModelType
 from datarobot_predict.scoring_code import ScoringCodeModel
@@ -71,14 +73,44 @@
                 return TimeSeriesType(int(v))
             else:
                 return TimeSeriesType[v.upper()]
         else:
             return TimeSeriesType(v)
 
 
+class ErrorCodes(Enum):
+    # Copied from datarobot/DataRobot/blob/master/predictions_api/constants.py#L66
+
+    # The error code is returned when a requested passthrough column has the same
+    # name as one of the output column names in the tabular format (i.e. CSV). For
+    # instance: POSITIVE_CLASS or FORECAST_POINT.
+    PASSTHROUGH_COLUMNS_CONFLICT = "passthrough_columns_conflict"
+
+    # The error code is returned when a request passthrough column could not be
+    # found in the scoring dataset.
+    PASSTHROUGH_COLUMN_DOES_NOT_EXIST = "passthrough_column_does_not_exist"
+
+    # The error code is returned when one or more features required for predictions
+    # are missing from the scoring dataset.
+    MISSING_COLUMNS = "missing_columns"
+
+    # The error code is returned when ALL features required for predictions are
+    # missing from the scoring dataset.
+    MISSING_ALL_COLUMNS = "missing_all_columns"
+
+    # The error code is returned when the request waited in uWSGI listen queue too
+    # long, and there's no need to process it anymore. Normally we have a 600
+    # seconds timeout on ALB, which means connections that are idling longer will be
+    # closed. Unfortunately the request could not be removed from uWSGI listen,
+    # hence the application can check the request start time and reject expired
+    # requests in order avoid computing something that could not be returned to a
+    # client anyway.
+    REQUEST_EXPIRED = "request_expired"
+
+
 # When running in the VSCode debugger, `JAVA_HOME` isn't being set and is needed
 # by `jpype.startJVM()` but we can derive it by looking for the `java` command
 # in the PATH.
 def set_java_home():
     if "JAVA_HOME" not in os.environ:
         java_path = shutil.which("java")
         # If we didn't find java, don't raise an error yet and let jpype have
@@ -104,14 +136,21 @@
         # has the wrong ID (mainly during testing).
         _model_id = os.getenv("MLOPS_MODEL_ID", _model.model_id)
 
     logging.info("Model Info: %s", _model.model_info)
     return _model, _model_id
 
 
+def read_feature_types():
+    default_feature_types_path = Path(__file__).parent / "feature_types.json"
+    feature_types_path = os.getenv("MLOPS_MODEL_FEATURE_TYPES_PATH", default_feature_types_path)
+    with open(feature_types_path, "r") as f:
+        return json.load(f)
+
+
 def get_mlops(
     model_id, feature_types=None, deployment_id=DEPLOYMENT_ID, enabled=MONITORING_ENABLED
 ):
     global _mlops
 
     if enabled and _mlops is None:
         if model_id is None:
@@ -127,36 +166,43 @@
         )
         if feature_types:
             _mlops.set_feature_types(feature_types)
         _mlops.init()
     return _mlops
 
 
+def get_model_id():
+    return _model_id
+
+
 def report_prediction_server_error_via_tracking_agent(
     mlops_sdk: Optional[MLOps],
     message: str,
-    model_id: str,
+    status_code: int,
+    model_id: Optional[str] = None,
     deployment_id=DEPLOYMENT_ID,
-    status_code: Optional[int] = None,
-    error_code: Optional[int] = None,
-    response_data: Optional[dict] = None,
+    error_code: Optional[ErrorCodes] = None,
 ):
     """Report pred server error to Tracking Agent."""
     if mlops_sdk is None:
         return
 
+    response_data = {"message": message}
+    if error_code is not None:
+        response_data["error_code"] = str(error_code.value)
+
     error_event = Event(
         event_type=EventType.PRED_REQUEST_FAILED,
         message=message,
         entity_id=deployment_id,
         data={
             "status_code": status_code,
-            "error_code": error_code,
-            "model_id": model_id,
-            "response_body": response_data,
+            "response_body": json.dumps(response_data),
+            "model_id": model_id or get_model_id(),
+            "error_code": error_code.value if error_code else None,
         },
     )
     mlops_sdk.report_event(event=error_event)
 
 
 def report_service_health_via_tracking_agent(
     mlops_sdk: Optional[MLOps],
```

## bosun/plugin/azureml/templates/online_score.py

```diff
@@ -5,14 +5,15 @@
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
+import http.client as http_codes
 import logging
 import os
 import time
 from pathlib import Path
 from typing import Optional
 from typing import Tuple
 from typing import Type
@@ -64,47 +65,65 @@
 
     try:
         if request.mimetype == "text/csv":
             df, params = _handle_csv_content(request, model, param_validator)
         elif request.mimetype == "application/json":
             df, params = _handle_json_content(request, param_validator)
         else:
-            return AMLResponse(
-                'Unsupported Content-Type; please use "application/json" or "text/csv"', 422
+            msg = 'Unsupported Content-Type; please use "application/json" or "text/csv"'
+            status_code = http_codes.UNPROCESSABLE_ENTITY
+            report_prediction_server_error_via_tracking_agent(  # noqa: F821
+                mlops_sdk,
+                msg,
+                status_code,
             )
+            return AMLResponse(msg, status_code)
     except HTTPException as err:
         logging.exception("Aborted while processing request")
+        report_prediction_server_error_via_tracking_agent(  # noqa: F821
+            mlops_sdk,
+            err.response.response[0].decode("UTF-8"),
+            err.code,
+        )
         return err.response
     except ValidationError as err:
         logging.exception("User param validation failed")
-        return AMLResponse(f"Request parameters are incorrect: {err}", 422)
+        msg = f"Request parameters are incorrect: {err}"
+        status_code = http_codes.UNPROCESSABLE_ENTITY
+        report_prediction_server_error_via_tracking_agent(  # noqa: F821
+            mlops_sdk,
+            msg,
+            status_code,
+        )
+        return AMLResponse(msg, status_code)
 
     return make_prediction(model, df, params, mlops_sdk, start_time)
 
 
 def _handle_json_content(
     request: AMLRequest, param_validator: Type[BaseModel]
 ) -> Tuple[pd.DataFrame, BaseModel]:
     # To avoid confusion, don't support both query params and params from the JSON payload.
     if request.args:
         abort(
             AMLResponse(
-                'Query parameters are not supported for "application/json" Content-Type', 422
+                'Query parameters are not supported for "application/json" Content-Type',
+                http_codes.UNPROCESSABLE_ENTITY,
             )
         )
     if (
         not (input_data := request.json.get("inputData"))
         or not isinstance(input_data, dict)
         or not all(field in input_data for field in ("columns", "index", "data"))
     ):
         abort(
             AMLResponse(
                 '"inputData" field is missing from the payload or not in the correct format.'
                 ' The payload should be of the form: {"inputData": df.to_dict(orient="split")}',
-                422,
+                http_codes.UNPROCESSABLE_ENTITY,
             )
         )
 
     inference_data = request.json.pop("inputData")
     df = pd.DataFrame(**inference_data)
     params = param_validator.parse_obj(request.json)
     return df, params
@@ -112,15 +131,15 @@
 
 def _handle_csv_content(
     request: AMLRequest, model: ScoringCodeModel, param_validator: Type[BaseModel]
 ) -> Tuple[pd.DataFrame, BaseModel]:
     try:
         df = pd.read_csv(request.stream, dtype=model.features)
     except pd.errors.ParserError as err:
-        abort(AMLResponse(f"CSV input is malformed: {err}", 400))
+        abort(AMLResponse(f"CSV input is malformed: {err}", http_codes.BAD_REQUEST))
     params = param_validator.parse_obj(request.args)
     return df, params
 
 
 def make_prediction(
     model: ScoringCodeModel,
     scoring_data: pd.DataFrame,
@@ -131,14 +150,17 @@
     # Delay importing this exception until we know jpype has been loaded
     from java.lang import IllegalArgumentException
 
     try:
         results = model.predict(scoring_data, **params.dict())
     except (ValueError, IllegalArgumentException) as err:
         logging.exception("Failed to make prediction")
-        return AMLResponse(f"Unable to compute prediction with given params: {err}", 422)
+        msg = f"Unable to compute prediction with given params: {err}"
+        status_code = http_codes.UNPROCESSABLE_ENTITY
+        report_prediction_server_error_via_tracking_agent(mlops_sdk, msg, status_code)  # noqa: F821
+        return AMLResponse(msg, status_code)
 
     report_service_health_via_tracking_agent(mlops_sdk, start_time, results)  # noqa: F821
     report_predictions_data_via_tracking_agent(  # noqa: F821
         mlops_sdk, model, results, scoring_data, params
     )
     return results.to_dict(orient="list")
```

## bosun/plugin/docker/docker_plugin.py

```diff
@@ -441,15 +441,15 @@
 
         containers = docker_helper.get_running_deployment_containers(deployment_id=di.id)
 
         if len(containers) == 0:
             final_status = ActionStatusInfo(
                 ActionStatus.ERROR,
                 msg=f"Error: could not find a container for deployment {di.id}",
-                state="errored",
+                state=DeploymentState.ERROR,
             )
         elif len(containers) > 1:
             # In case of model replacement it is possible that more than 1 containers are
             # running for the same deployment.  As long as at least one container is in OK
             # state, we will return that status.  It is possible that model replacement may
             # fail, and that status will be captured in the subsequent status request
             found_one_good_container = False
@@ -458,18 +458,20 @@
             for index, container in enumerate(containers):
                 cont_status = self._get_deployment_status(docker_helper, di.id, container)
                 msg += f" - Container {index} id {container.id}: {cont_status.msg}"
                 if cont_status.status == ActionStatus.OK:
                     found_one_good_container = True
                     status_data = cont_status.data
             if not found_one_good_container:
-                final_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
+                final_status = ActionStatusInfo(
+                    ActionStatus.ERROR, msg=msg, state=DeploymentState.ERROR
+                )
             else:
                 final_status = ActionStatusInfo(
-                    ActionStatus.OK, msg=msg, state="ready", data=status_data
+                    ActionStatus.OK, msg=msg, state=DeploymentState.READY, data=status_data
                 )
         else:
             final_status = self._get_deployment_status(docker_helper, di.id, containers[0])
         self._logger.info(final_status.msg)
         return final_status
 
     def _get_deployment_status(self, docker_helper, deployment_id, container):
@@ -530,12 +532,12 @@
                 self._logger.warn(
                     f"This plugin does not support model of type: {model_execution_type}"
                 )
                 continue
 
             deployments_map[deployment_id] = self._get_deployment_status(
                 docker_helper, deployment_id, deployment_container
-            ).__dict__
+            ).to_dict()
 
         self._logger.info(status_msg)
         self._logger.info("Containers: " + str(deployments_map))
         return ActionStatusInfo(status, msg=status_msg, data=deployments_map)
```

## bosun/plugin/filesystem/filesystem_plugin.py

```diff
@@ -242,15 +242,15 @@
         )
 
         for deployment_dir in list_deployment:
             deployments_status = self._deployment_status(deployment_dir)
             deployment_id = os.path.basename(deployment_dir).replace(
                 self._config.deployment_dir_prefix, ""
             )
-            deployments_map[deployment_id] = deployments_status.__dict__
+            deployments_map[deployment_id] = deployments_status.to_dict()
 
         if len(list_deployment) == 0:
             status_msg = "No containers running"
         else:
             status_msg = f"Number of deployments: {len(list_deployment)}"
 
         self._logger.info(status_msg)
```

## bosun/plugin/k8s/config.py

```diff
@@ -283,15 +283,15 @@
         # tracking-agent runs in the same pod as the prediction server we also need requests there
         # too if tracking is enabled.
         # See https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale/
         # TODO: when `Container Resource Metrics` goes beta/GA we can simplify the logic if we
         #       update our HPA spec.
         if self.pps_cpu_utilization is None:
             return False
-        if self.do_mlops_monitoring:
+        if self.do_mlops_monitoring and self.agent_sidecar:
             return self._has_pps_cpu_request and self._has_agent_cpu_request
         else:
             return self._has_pps_cpu_request
 
     @property
     def pps_pod_security_context(self):
         return self._config[KubernetesPluginConfig.PPS_POD_SECURITY]
```

## bosun/plugin/s3/s3_plugin.py

```diff
@@ -267,15 +267,15 @@
         deployment_set = self._get_deployment_dirs()
 
         for deployment_dir in deployment_set:
             deployments_status = self._deployment_status(deployment_dir)
             deployment_id = os.path.basename(deployment_dir).replace(
                 self._config.deployment_dir_prefix, ""
             )
-            deployments_map[deployment_id] = deployments_status.__dict__
+            deployments_map[deployment_id] = deployments_status.to_dict()
 
         if len(deployment_set) == 0:
             status_msg = "No containers running"
         else:
             status_msg = f"Number of deployments: {len(deployment_set)}"
 
         self._logger.info(status_msg)
```

## bosun/plugin/snowflake/snowflake_plugin.py

```diff
@@ -106,15 +106,15 @@
             status_msg = "No scoring code UDFs deployed"
             deployment_udfs = []
 
         self._logger.info(status_msg)
         self._logger.info("Deployed Scoring Code UDFs: " + str(deployment_udfs))
 
         deployments_map = {}
-        deployment_ready = ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY).__dict__
+        deployment_ready = ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY).to_dict()
 
         for udf_name, _ in deployment_udfs:
             # UDF name structure: <udf_name_prefix>_<deployment_id>
             deployment_id = udf_name.split("_")[-1].lower()
             # A UDF in Snowflake either exists or doesn't, so if it's there, then it is ready
             deployments_map[deployment_id] = deployment_ready
```

## Comparing `datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner` & `datarobot_bosun-9.1.3.data/scripts/bosun-plugin-runner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.1.1rc1.data/scripts/mcrunner` & `datarobot_bosun-9.1.3.data/scripts/mcrunner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner` & `datarobot_bosun-9.1.3.data/scripts/plugin-runner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.1.1rc1.dist-info/METADATA` & `datarobot_bosun-9.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-bosun
-Version: 9.1.1rc1
+Version: 9.1.3
 Summary: datarobot-bosun module providing MLOps Management framework and plug-ins
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: info@datarobot.com
 License: DataRobot
 Project-URL: Documentation, https://docs.datarobot.com/en/docs/release/public-preview/mlops-preview/mgmt-agent.html#mlops-management-agent
 Platform: UNKNOWN
@@ -23,14 +23,15 @@
 Requires-Dist: pytz
 Requires-Dist: python-dateutil
 Requires-Dist: schema
 Requires-Dist: datarobot-mlops-connected-client (>=7.1)
 Provides-Extra: azureml
 Requires-Dist: azure-ai-ml (>=1.3) ; extra == 'azureml'
 Requires-Dist: azure-identity (>=1.12) ; extra == 'azureml'
+Requires-Dist: datarobot-mlops-stats-aggregator (>=8.2.4) ; extra == 'azureml'
 Provides-Extra: docker
 Requires-Dist: requests ; extra == 'docker'
 Requires-Dist: docker ; extra == 'docker'
 Provides-Extra: kubernetes
 Requires-Dist: jinja2 ; extra == 'kubernetes'
 Requires-Dist: requests ; extra == 'kubernetes'
 Requires-Dist: kubernetes (!=25.*,>=19.15) ; (python_version < "3.9") and extra == 'kubernetes'
```

## Comparing `datarobot_bosun-9.1.1rc1.dist-info/RECORD` & `datarobot_bosun-9.1.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -5,48 +5,48 @@
 bosun/model_connector/mc_bosun.py,sha256=lCo6xyXg6YfwsP8Oh2UmFVQgusLwUpDcD98qyEFHACA,7190
 bosun/model_connector/mc_runner.py,sha256=xFxhvllb0W--AoP7m1aN0GyCY2eOQBk4e9D0heKm5R8,5269
 bosun/model_connector/model_connector_base.py,sha256=DSV1DI9n6bPk0J5dzQjQQCRHsIpawGF5miBX3f2hRMY,5433
 bosun/model_connector/s3_uri_fetcher.py,sha256=MAhtLIBhy8T-ACUFQ_-OyRl-Dm4UEpyq2ZlXO210dS4,2334
 bosun/model_connector/uri_fetcher_base.py,sha256=03RVfWSkb_jIa6EpIIwmIOfcw-6EMcW5wzwmIHnvB0Y,894
 bosun/plugin/__init__.py,sha256=jpqAqC1Ils82n2QssUt_W0fcKI6z6JUz4KJ-tyMWTro,583
 bosun/plugin/action_status.py,sha256=WWgF7KlMZLZN3iKHfPBRHvqNGey-SDZQIIp0aVXWHw0,2260
-bosun/plugin/bosun_plugin_base.py,sha256=H36wBTOyTdvx6qeYD1I8nPAR3IXn4uw0x_YR5cXk56s,6147
-bosun/plugin/bosun_test_plugin.py,sha256=W97oxU9Y__d5e_LGkPV6f2UtZvj3cuyHkZ1AKq1D7Mw,11466
+bosun/plugin/bosun_plugin_base.py,sha256=8i2dJ90RL6WuzO3YWfcT1F_npHMAE8JU6ZZTbRp3Yoc,6240
+bosun/plugin/bosun_test_plugin.py,sha256=kg9_jV5mUpPm9BxjzQyJA8REp0JyVki3azp6cLnN6eI,11492
 bosun/plugin/constants.py,sha256=EC8rwSudYn9Nj0htnue1gEXjivqEVUlz8FdHASoTW7E,2833
-bosun/plugin/deployment_info.py,sha256=lJOP2S9sQC-bw-X5rMHw3IZbBV4-DcKH2vvGe9OF4QE,3354
+bosun/plugin/deployment_info.py,sha256=6cEV6yF7OYkCkk48G7dFrLf1fQHqukmlHAli7rpmLjY,3745
 bosun/plugin/exceptions.py,sha256=XiPxJWyRd50MBAO3Ztu4KrlL5oSBjcPBK8IDD1sWHo0,1047
 bosun/plugin/pe_info.py,sha256=ey2Ef1zzK1jHO705xlpZo3jmdA5UW2S6e99mf_Xy4YI,2493
-bosun/plugin/plugin_runner.py,sha256=KpV3LKIYnqdTMaGgGMABiBdRZzTyB3hmjG4mek4Tng4,16799
+bosun/plugin/plugin_runner.py,sha256=-TcXsUS96ZtVFSWJqg61jCQuKxI6lfWgBVx893GfKyM,16892
 bosun/plugin/azureml/__init__.py,sha256=w0FppK0OReL18im5hlOAeWB_NYCFPFaSmnbqIxIspj4,640
-bosun/plugin/azureml/azureml_plugin.py,sha256=sfF2miMrgviV12u-u3jkX3iAHc7Xp2CBszpFbvSZ5NM,12218
+bosun/plugin/azureml/azureml_plugin.py,sha256=svxWH0yhrJLqv0KEHqJxnXN91x2LQwtCeaJTYkZzLXA,12219
 bosun/plugin/azureml/azureml_status_reporter.py,sha256=62KW9cDxvqKXgsXpbvIQnq28d54h7_xzYA_IjAFv7p4,3313
 bosun/plugin/azureml/template_renderer.py,sha256=IKm8M_4h1CvMN-Ujx3t_EiDMVugmVNUs8DlZqJnT51Q,1516
-bosun/plugin/azureml/client/base_endpoint_client.py,sha256=C6l-Pv1NMQ91AiXrtrt6k6c-V-XsfogeLRjM_SdisIY,18410
-bosun/plugin/azureml/client/batch_endpoint_client.py,sha256=mZV7GddP3RE3IwN54V6kmeqDFxE2ZQsL8hbnukhxBZY,6743
+bosun/plugin/azureml/client/base_endpoint_client.py,sha256=QdmZ49WWa1hMCWPscc2WKHdPj2aKYo8DFVY21meNafU,20318
+bosun/plugin/azureml/client/batch_endpoint_client.py,sha256=QyN7JFNis_i2gDirByAJ2A_G305fAImOVzUIda1aqO4,6797
 bosun/plugin/azureml/client/online_endpoint_client.py,sha256=Po6920-XaJh4NqR-MgUmhRs52tTT5qJO4C1oJ9RmUwY,17972
 bosun/plugin/azureml/client/scoring_snippets.py,sha256=DhIxVo2jpKg6F_p5d1fuqNOQQ_pFHYjHyIbDGtUc2bA,1394
 bosun/plugin/azureml/config/__init__.py,sha256=5LKBu0qgbs3MEvPz1MWIyivQ_LsncJV9bDTFdIEqoJk,583
 bosun/plugin/azureml/config/azureml_client_config.py,sha256=wBgvfEckS-wP-WNxPU6WrS_bzhc53_1CQt9jRRIvH7w,11520
 bosun/plugin/azureml/config/config_keys.py,sha256=IMKpnVT6Z2NPbc7Q230MZgbckJIw5wqmFCYI0IAOLSQ,3420
-bosun/plugin/azureml/templates/batch_score.py,sha256=aPULuPwZtHRz3ZzykiDbvsrFyVTxOqGlqIMBsJMOPKI,3767
-bosun/plugin/azureml/templates/common.py,sha256=VoN1HfviW9MmPFa9jdgexM2EMRBa7i9ZmNY7FAIN5ck,9634
+bosun/plugin/azureml/templates/batch_score.py,sha256=J3oiQt6z-QeSKOVUnzSwjF3Jq6s_NCKPx4SQmjEjSQE,4719
+bosun/plugin/azureml/templates/common.py,sha256=zzlhFXfGuf6pvACmrEg6sXkPVRo-0Y_SGdZSis89vfI,11617
 bosun/plugin/azureml/templates/conda.yml,sha256=RxGpt6rw4DizjDPht5YWp1p5i0Dx0HCSiIVQXCamYHE,697
-bosun/plugin/azureml/templates/online_score.py,sha256=BeZscUL5Wk0HHX3vb3jmb3B0xEDet3nPIoa24H50EhE,5452
+bosun/plugin/azureml/templates/online_score.py,sha256=QryEPfP2eIiTJYvwIkc0dBlcSWglKrkySXqVSuKvF2A,6394
 bosun/plugin/azureml/templates/scoring_script_builder.py.j2,sha256=ggw_rSteAoJM9tNLJxCdu-jjGzC62b7DnL2pUnHj3aI,963
 bosun/plugin/config_samples/__init__.py,sha256=sAc8oDBMnbrQI82jZrO-TKBO4JwXaMPLnO7cZw6GkxM,702
 bosun/plugin/docker/__init__.py,sha256=HBnE1c15RavjXjjlGCEqQm7PgKETJl1cLW3othCfBPU,757
 bosun/plugin/docker/docker_helper.py,sha256=fubvtoFhsJihzazfLk2gsfD_1YgxE0B_aJSoacQEcKU,14934
-bosun/plugin/docker/docker_plugin.py,sha256=LCoEkUCfaVKf4VcGrSM7wWVnRcWMazNBCj2tKPNzFek,23290
+bosun/plugin/docker/docker_plugin.py,sha256=b5MBVo-t3WftBqaO13ow0Fi4yAvnkRgIvZJlkuWo_ps,23367
 bosun/plugin/docker/docker_plugin_config.py,sha256=haxXV6dkolVNXXxy1uG7e3O7xV32ALibwDVwye2234U,5419
 bosun/plugin/docker/mlops_monitoring.py,sha256=UXtIj4Uybr9SY4m1uFZAoiRpsOAii343rYPpVt2trZ0,7897
 bosun/plugin/filesystem/__init__.py,sha256=DS_gsVTXiCIXCKL6eJe14Jye0Q08EvJoQaFagwvzTJI,646
-bosun/plugin/filesystem/filesystem_plugin.py,sha256=PB675cG9e59i1qSzEd2CbCjXXHRYZrp08X9p-bFXKk0,14021
+bosun/plugin/filesystem/filesystem_plugin.py,sha256=5qYRF0htIfEJm0bRUh9rCDtvIfMWSzGBbeNnTtuC2TY,14022
 bosun/plugin/k8s/__init__.py,sha256=AfSBWxZWkUluB4pI2V6dlvZ1znEdTT8wDx4QHxSQIZ8,646
 bosun/plugin/k8s/client.py,sha256=TX0Zz3z6VPypQLeh5nyIwWF9AjJ2rlMHzRq6XQ2uPSU,37071
-bosun/plugin/k8s/config.py,sha256=nGS-Ica0jsElogxiU6sPyQ26Hf_p60qPCfunfUjyx-w,20247
+bosun/plugin/k8s/config.py,sha256=MhsEVi38WKNwzO-LhpMg5za5m3XomDLBzmtGqTIF4Zk,20270
 bosun/plugin/k8s/kubernetes_plugin.py,sha256=-PjgQtmJivFQlSG1AGa6MlvnZDKUoF5brCnNfdDAzEk,28225
 bosun/plugin/k8s/manifests.py,sha256=j0IesWl7nnOAvwphIIYSACrzM6JoGNqBK4tteQxInKg,9170
 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2,sha256=i9mZbUArvs1q4N6z9vtB5CHqya3USqRzK17Zwl-6w1k,303
 bosun/plugin/k8s/templates/_helpers.j2,sha256=arpcrQvzhk-ZH7pyIpNXPqIf1NZ2RlrZxfyuY3DAfZs,2263
 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2,sha256=L5F7pP4M_HqsNP2wTqMMiNDbWB5pndHQi2vHlr4mCDo,4603
 bosun/plugin/k8s/templates/image-builder.yaml.j2,sha256=DjYTQSHq2uSxC0bOPr-fp6nrZEFi1tcmTVIkwpt2dRM,1393
 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2,sha256=RgnvF5CGVBsq3ThtKU3MjjlALUqD-w1xjkEjZ0sR14g,356
@@ -54,19 +54,19 @@
 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2,sha256=xWJR6dxoL-_-_BwpVdv9WDqqw4X8v97tymUi5nJrQRo,4929
 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2,sha256=1LRvU1g2owLignZ9bjefrVkrzk_Tlap5yVX8evk2Kz4,119
 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2,sha256=6qlsvgIUeV7GcMjEPWpPKPrVCETSTmUcq184O_NiKGU,842
 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2,sha256=b3K54nLIDeeHJp2mn9VzMM45Z8x0NVGRrhm0YTz3PT0,1253
 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2,sha256=Uu_JR1FDrMOSgdROcaDpDkfSQzVaSYrrVxJfV6-LtPk,484
 bosun/plugin/k8s/templates/model-resources/service.yaml.j2,sha256=uvp3IeGLMR1slrY9S5jlPH8lm4tRwm1lD3HnAm36jU0,547
 bosun/plugin/s3/__init__.py,sha256=K1whUFDQfXk5zzO_B7cdIf5rFBhBXkKveGb2utt5OAo,630
-bosun/plugin/s3/s3_plugin.py,sha256=EF-orhokbNFCev9P1liSroojc6TdT3A-2wdPGO79CEI,11175
+bosun/plugin/s3/s3_plugin.py,sha256=BmxeW4RKMI8FnMz1eeDClV5XNT7BW4jXtJwAowTIg_8,11176
 bosun/plugin/s3/s3_plugin_config.py,sha256=bDKpMgdCEXSiLiAmKlEcw5DP0ShrTZmUbJuA3U6VbRs,2705
 bosun/plugin/snowflake/__init__.py,sha256=DP4zjkZvK-kb975NTxg1HF_UTQYbwQPszpI2QJUbdR8,644
-bosun/plugin/snowflake/snowflake_plugin.py,sha256=HE308wrkeS5Ie1kMrDTKx7KbsRNuDX1qjPapozdaYck,10034
+bosun/plugin/snowflake/snowflake_plugin.py,sha256=WoOw9YzqYkrHp8bq0vDsxhUEYoWAhgHXla9lWJSmHjQ,10035
 bosun/plugin/snowflake/snowflake_plugin_config.py,sha256=KclEb3I9xEkJPf-0ZZcH2QCNI1bCRKhmYWy9-aW-GmE,5491
-datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner,sha256=e8YQBceK8QeD8EFh1q5Vb-jlAYxlrzvZllDq3LNnVPg,671
-datarobot_bosun-9.1.1rc1.data/scripts/mcrunner,sha256=FPqMPz123TVvMrWf1bBsu17RSoJJwXA0-M9EG5IdpXg,676
-datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner,sha256=pe1lGnDyvW82cBjewuRhb6ad6q3j4TYEJLurzG6GNdk,671
-datarobot_bosun-9.1.1rc1.dist-info/METADATA,sha256=BI-jmSlV9Qpw4mbjZsfspWwsBxyP2hccV9_htvisUJw,4471
-datarobot_bosun-9.1.1rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datarobot_bosun-9.1.1rc1.dist-info/top_level.txt,sha256=zNJvGsG32_zF72Xl_00PTybDZE3u5FXDSxJiFEekRd4,6
-datarobot_bosun-9.1.1rc1.dist-info/RECORD,,
+datarobot_bosun-9.1.3.data/scripts/bosun-plugin-runner,sha256=e8YQBceK8QeD8EFh1q5Vb-jlAYxlrzvZllDq3LNnVPg,671
+datarobot_bosun-9.1.3.data/scripts/mcrunner,sha256=FPqMPz123TVvMrWf1bBsu17RSoJJwXA0-M9EG5IdpXg,676
+datarobot_bosun-9.1.3.data/scripts/plugin-runner,sha256=pe1lGnDyvW82cBjewuRhb6ad6q3j4TYEJLurzG6GNdk,671
+datarobot_bosun-9.1.3.dist-info/METADATA,sha256=JJ8KBqrfQvsfMqjWem2ZpCHX4tc1IaHzZZtzAbKd6Ts,4547
+datarobot_bosun-9.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_bosun-9.1.3.dist-info/top_level.txt,sha256=zNJvGsG32_zF72Xl_00PTybDZE3u5FXDSxJiFEekRd4,6
+datarobot_bosun-9.1.3.dist-info/RECORD,,
```

