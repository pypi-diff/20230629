# Comparing `tmp/datarobot_mlops_connected_client-9.1.1rc1-py3-none-any.whl.zip` & `tmp/datarobot_mlops_connected_client-9.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 42665 bytes, number of entries: 13
--rw-r--r--  2.0 unx      597 b- defN 23-May-18 21:10 datarobot/mlops/__init__.py
--rw-r--r--  2.0 unx      532 b- defN 23-May-18 21:10 datarobot/mlops/connected/__init__.py
--rw-r--r--  2.0 unx   106180 b- defN 23-May-18 21:10 datarobot/mlops/connected/client.py
--rw-r--r--  2.0 unx     1231 b- defN 23-May-18 21:10 datarobot/mlops/connected/enums.py
--rw-r--r--  2.0 unx      900 b- defN 23-May-18 21:10 datarobot/mlops/connected/exception.py
--rw-r--r--  2.0 unx   110928 b- defN 23-May-18 21:10 datarobot/mlops/connected/mlops_cli.py
--rw-r--r--  2.0 unx     2646 b- defN 23-May-18 21:10 datarobot/mlops/connected/upload_tracker.py
--rw-r--r--  2.0 unx    11367 b- defN 23-May-18 21:10 datarobot/mlops/connected/url_helper.py
--rw-r--r--  2.0 unx     1537 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1282 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD
-13 files, 237374 bytes uncompressed, 40457 bytes compressed:  83.0%
+Zip file size: 43553 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      597 b- defN 23-Jun-29 21:29 datarobot/mlops/__init__.py
+-rw-r--r--  2.0 unx      532 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/__init__.py
+-rw-r--r--  2.0 unx   109951 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/client.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/enums.py
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/exception.py
+-rw-r--r--  2.0 unx   115239 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/mlops_cli.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/upload_tracker.py
+-rw-r--r--  2.0 unx    11911 b- defN 23-Jun-29 21:29 datarobot/mlops/connected/url_helper.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-Jun-29 21:34 datarobot_mlops_connected_client-9.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 21:34 datarobot_mlops_connected_client-9.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-29 21:34 datarobot_mlops_connected_client-9.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-29 21:34 datarobot_mlops_connected_client-9.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1267 b- defN 23-Jun-29 21:34 datarobot_mlops_connected_client-9.1.3.dist-info/RECORD
+13 files, 246015 bytes uncompressed, 41375 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: datarobot/mlops/connected/upload_tracker.py
 Comment: 
 
 Filename: datarobot/mlops/connected/url_helper.py
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA
+Filename: datarobot_mlops_connected_client-9.1.3.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/WHEEL
+Filename: datarobot_mlops_connected_client-9.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/entry_points.txt
+Filename: datarobot_mlops_connected_client-9.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/top_level.txt
+Filename: datarobot_mlops_connected_client-9.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD
+Filename: datarobot_mlops_connected_client-9.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datarobot/mlops/connected/client.py

```diff
@@ -19,14 +19,15 @@
 import time
 import warnings
 from contextlib import suppress
 from functools import partial
 
 import aiohttp
 import requests
+from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from datarobot.mlops.common.aggregation_util import convert_aggregated_stats_features_to_dr_format
 from datarobot.mlops.common.aggregation_util import (
     convert_aggregated_stats_predictions_to_dr_format,
 )
 from datarobot.mlops.common.aggregation_util import (
     convert_aggregated_stats_segment_attr_to_dr_format,
@@ -100,14 +101,15 @@
     RESPONSE_TARGET_TYPE_KEY = "type"
     RESPONSE_MODEL_TARGET_TYPE_KEY = "targetType"
     RESPONSE_LOCATION_KEY = "Location"
     RESPONSE_FULL_API_VERSION = "versionString"
     RESPONSE_API_MAJOR_VERSION = "major"
     RESPONSE_API_MINOR_VERSION = "minor"
     RESPONSE_CUSTOM_METRIC_ID_KEY = "id"
+    RESPONSE_MONITORING_JOB_ID_KEY = "id"
 
     ASYNC_STATUS_ACTIVE = "active"
     ASYNC_STATUS_ERROR = "error"
     ASYNC_STATUS_ABORT = "abort"
     ASYNC_STATUS_INITIALIZED = "initialized"
     ASYNC_STATUS_RUNNING = "running"
     ASYNC_WAIT_SLEEP_TIME = 2
@@ -317,32 +319,38 @@
         """
 
         try:
             url = self._url_builder.upload_dataset()
             headers = dict(self._common_headers)
             if dry_run:
                 return "dummy-catalog-id-dry-run"
-            with open(dataset_filepath) as dataset_file:
-                response = requests.post(
-                    url,
-                    files={"file": (dataset_filepath, dataset_file)},
-                    headers=headers,
-                    verify=self._verify,
+
+            fields = {
+                "file": (
+                    os.path.basename(dataset_filepath),
+                    open(dataset_filepath, "rb"),  # pylint: disable=consider-using-with
                 )
-                if response.ok:
-                    self._wait_for_async_completion(
-                        response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
-                    )
-                    return response.json()[MLOpsClient.RESPONSE_CATALOG_ID_KEY]
-                else:
-                    raise DRMLOpsConnectedException(
-                        "Call {} with filename {} failed; text:[{}]".format(
-                            url, dataset_filepath, response.text
-                        )
+            }
+
+            encoder = MultipartEncoder(fields=fields)
+            headers["Content-Type"] = encoder.content_type
+
+            response = requests.post(url, headers=headers, data=encoder, timeout=timeout)
+
+            if response.ok:
+                self._wait_for_async_completion(
+                    response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
+                )
+                return response.json()[MLOpsClient.RESPONSE_CATALOG_ID_KEY]
+            else:
+                raise DRMLOpsConnectedException(
+                    "Call {} with filename {} failed; text:[{}]".format(
+                        url, dataset_filepath, response.text
                     )
+                )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def upload_dataframe(self, df, filename=None, timeout=180, dry_run=False):
         """
@@ -1341,14 +1349,86 @@
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
+    def create_monitoring_job(self, job_info):
+        try:
+            url = self._url_builder.create_monitoring_job()
+
+            headers = dict(self._common_headers)
+            headers.update({"Content-Type": "application/json"})
+            response = requests.post(
+                url, data=json_dumps_bytes(job_info), headers=headers, verify=self._verify
+            )
+            if response.ok:
+                return response.json()[MLOpsClient.RESPONSE_MONITORING_JOB_ID_KEY]
+            else:
+                raise DRMLOpsConnectedException(
+                    f"Call {url} with payload {job_info} failed; text: [{response.text}]"
+                )
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
+    def get_monitoring_job(self, monitoring_job_id):
+        try:
+            url = self._url_builder.get_monitoring_job(monitoring_job_id)
+            response = self._get_url_request_response(url)
+            if response.ok:
+                return response.json()
+            if response.status_code == HTTPStatus.NOT_FOUND:
+                raise DRNotFoundException(f"Monitoring Job with ID {monitoring_job_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
+    def upload_input_file_to_monitoring_job(self, monitoring_job_id, data_filepath):
+        try:
+            url = self._url_builder.upload_file_to_monitoring_job(monitoring_job_id)
+            headers = dict(self._common_headers)
+            headers["Content-Type"] = "text/csv"
+
+            with open(data_filepath, "rb") as dataset_file:
+                response = requests.put(
+                    url,
+                    data=dataset_file,
+                    headers=headers,
+                    verify=self._verify,
+                )
+                if not response.ok:
+                    raise DRMLOpsConnectedException(
+                        "Call {} with filename {} failed; text:[{}]".format(
+                            url, data_filepath, response.text
+                        )
+                    )
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
+    def abort_running_monitoring_job(self, monitoring_job_id):
+        try:
+            url = self._url_builder.get_monitoring_job(monitoring_job_id)
+            response = requests.delete(url, headers=self._common_headers, verify=self._verify)
+            if response.ok:
+                return response.json()
+            if response.status_code == HTTPStatus.NOT_FOUND:
+                raise DRNotFoundException(f"Monitoring Job with ID {monitoring_job_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
     def payload_report_deployment_stats(
         self, model_id, timestamp, num_predictions, execution_time_ms=None, batch_name=None
     ):
         deployment_stats = DeploymentStats(num_predictions, execution_time_ms)
         deployment_stats_container = DeploymentStatsContainer(
             GeneralStats(model_id, timestamp, batch_name), deployment_stats
         )
@@ -1453,23 +1533,23 @@
             else:
                 feature_data = data
 
         assoc_id_list = None
         if association_ids is not None:
             assoc_id_list = association_ids
         elif assoc_id:
-            if assoc_id not in feature_data.columns:
+            if feature_data is None or assoc_id not in feature_data.columns:
                 raise Exception(f"Error: assoc_id column '{assoc_id}' is not present in DataFrame")
             assoc_ids = feature_data[assoc_id].tolist()
             assoc_id_list = list(map(str, assoc_ids))
 
-        if assoc_id is not None and assoc_id in feature_data.columns:
+        if assoc_id is not None and feature_data is not None and assoc_id in feature_data.columns:
             feature_data = feature_data.drop(columns=assoc_id)
 
-        nr_lines = len(data)
+        nr_lines = len(data) if data is not None else len(predictions)
         max_lines_per_chunk = get_config_default(
             ConfigConstants.MLOPS_SAMPLES_GROUP_SIZE_FOR_MLOPS_API_ENDPOINT,
             MMMLimits.DATA_REPORTING_MAX_LINES_PER_CHUNK,
         )
         nr_chunks = math.ceil(nr_lines / max_lines_per_chunk)
         max_chunks = get_config_default(
             ConfigConstants.MLOPS_MAX_GROUPS_FOR_MLOPS_API_ENDPOINT,
@@ -1487,15 +1567,15 @@
             if to_line > nr_lines:
                 to_line = nr_lines
 
             assoc_id_list_section = None
             if assoc_id_list:
                 assoc_id_list_section = assoc_id_list[from_line:to_line]
             features_df = None
-            if len(feature_data.columns) > 0:
+            if feature_data is not None and len(feature_data.columns) > 0:
                 features_df = feature_data[from_line:to_line]
             predictions_data = PredictionsData(
                 features_df,
                 predictions[from_line:to_line],
                 association_ids=assoc_id_list_section,
                 class_names=class_names,
             )
@@ -1596,15 +1676,15 @@
         :returns: Tuple (response from MLOps, size of payload sent)
         :rtype: Tuple
         :raises DRMLOpsConnectedException: if request fails
         """
         url = self._url_builder.report_prediction_data(deployment_id)
         headers = dict(self._common_headers)
         headers.update({"Content-Type": "application/json"})
-        input_row_count = data.shape[0]
+        input_row_count = data.shape[0] if data is not None else len(predictions)
         start = 0
         max_lines_per_chunk = get_config_default(
             ConfigConstants.MLOPS_SAMPLES_GROUP_SIZE_FOR_MLOPS_API_ENDPOINT,
             MMMLimits.DATA_REPORTING_MAX_LINES_PER_CHUNK,
         )
         max_chunks = get_config_default(
             ConfigConstants.MLOPS_MAX_GROUPS_FOR_MLOPS_API_ENDPOINT,
@@ -1614,15 +1694,15 @@
 
         aggregate_payload_size = 0
         last_response = {}
         while start < input_row_count:
             end = start + size
             if end > input_row_count:
                 end = input_row_count
-            data_chunk = data[start:end]
+            data_chunk = data[start:end] if data is not None else None
             payload = self.payload_report_prediction_data(
                 model_id=model_id,
                 data=data_chunk,
                 association_ids=association_ids,
                 assoc_id=assoc_id_col,
                 predictions=predictions,
                 prediction_cols=prediction_cols,
```

## datarobot/mlops/connected/mlops_cli.py

```diff
@@ -21,14 +21,15 @@
 from argparse import RawTextHelpFormatter
 from contextlib import closing
 from enum import Enum
 
 import pandas as pd
 
 from datarobot.mlops.common import config
+from datarobot.mlops.common.aggregation_util import convert_feature_format
 from datarobot.mlops.common.enums import DataType
 from datarobot.mlops.common.enums import MLOpsSpoolAction
 from datarobot.mlops.common.enums import SpoolerType
 from datarobot.mlops.common.exception import DRCommonException
 from datarobot.mlops.common.exception import DRNotFoundException
 from datarobot.mlops.constants import Constants
 from datarobot.mlops.metric import SerializationConstants
@@ -53,14 +54,15 @@
     MLOPS_MODEL_PACKAGE_ID = "MLOPS_MODEL_PACKAGE_ID"
     MLOPS_DATASET_ID = "MLOPS_DATASET_ID"
     MLOPS_TRAINING_DATASET_ID = "MLOPS_TRAINING_DATASET_ID"
     MLOPS_HOLDOUT_DATASET_ID = "MLOPS_HOLDOUT_DATASET_ID"
     MLOPS_DEPLOYMENT_ID = "MLOPS_DEPLOYMENT_ID"
     MLOPS_DEPLOYMENT_LABEL = "MLOPS_DEPLOYMENT_LABEL"
     MLOPS_PREDICTION_ENVIRONMENT_ID = "MLOPS_PREDICTION_ENVIRONMENT_ID"
+    MLOPS_MONITORING_JOB_ID = "MLOPS_MONITORING_JOB_ID"
     MLOPS_DATAROBOT_APP_VERSION = "MLOPS_DATAROBOT_APP_VERSION"
     MLOPS_BATCH_ID = "MLOPS_BATCH_ID"
     MLOPS_METRIC_ID = "MLOPS_METRIC_ID"
 
 
 class Subjects:
     MAIN_COMMAND = "mlops-cli"
@@ -70,40 +72,43 @@
     MODEL = "model"
     DATASET = "dataset"
     DEPLOYMENT = "deployment"
     PREDICTION_ENVIRONMENT = "prediction-environment"
     SERVICE_STATS = "service-stats"
     BATCH = "batch"
     CUSTOM_METRICS = "custom_metric"
+    MONITORING_JOB = "monitoring-job"
 
     ALL_SUBJECTS = [
         PERF_TEST,
         PREDICTIONS,
         ACTUALS,
         MODEL,
         DATASET,
         DEPLOYMENT,
         PREDICTION_ENVIRONMENT,
         SERVICE_STATS,
         BATCH,
         CUSTOM_METRICS,
+        MONITORING_JOB,
     ]
 
 
 class Actions:
     UPLOAD = "upload"
     DOWNLOAD = "download"
     CREATE = "create"
     GET = "get"
     FEATURES = "features"
     LIST = "list"
     DELETE = "delete"
     REPLACE = "replace"
     REPORT = "report"
     RUN = "run"
+    CANCEL = "cancel"
     DEPLOY = "deploy"
     GET_MODEL = "get-model"
     COUNT = "count"
 
     ALL_ACTIONS = [
         UPLOAD,
         DOWNLOAD,
@@ -111,14 +116,15 @@
         GET,
         FEATURES,
         LIST,
         DELETE,
         REPLACE,
         REPORT,
         RUN,
+        CANCEL,
         DEPLOY,
         GET_MODEL,
         COUNT,
     ]
 
     PERF_ACTIONS = [RUN]
     PREDICTIONS_ACTIONS = [UPLOAD, GET, REPORT, COUNT]
@@ -126,36 +132,39 @@
     MODEL_ACTIONS = [DOWNLOAD, CREATE, GET, LIST, DELETE, REPLACE, DEPLOY]
     DATASET_ACTIONS = [UPLOAD, GET, LIST, DELETE]
     DEPLOYMENT_ACTIONS = [GET, LIST, DELETE, GET_MODEL]
     PREDICTION_ENVIRONMENT_ACTIONS = [CREATE, GET, LIST, DELETE]
     SERVICE_STATS_ACTIONS = [GET]
     BATCH_ACTIONS = [GET, LIST]
     CUSTOM_METRICS_ACTIONS = [CREATE, GET, LIST, REPORT]
+    MONITORING_JOBS_ACTIONS = [CREATE, GET, LIST, CANCEL, UPLOAD]
 
 
 SUPPORTED_ACTIONS = {
     Subjects.PERF_TEST: Actions.PERF_ACTIONS,
     Subjects.PREDICTIONS: Actions.PREDICTIONS_ACTIONS,
     Subjects.ACTUALS: Actions.ACTUALS_ACTIONS,
     Subjects.MODEL: Actions.MODEL_ACTIONS,
     Subjects.DATASET: Actions.DATASET_ACTIONS,
     Subjects.DEPLOYMENT: Actions.DEPLOYMENT_ACTIONS,
     Subjects.PREDICTION_ENVIRONMENT: Actions.PREDICTION_ENVIRONMENT_ACTIONS,
     Subjects.SERVICE_STATS: Actions.SERVICE_STATS_ACTIONS,
     Subjects.BATCH: Actions.BATCH_ACTIONS,
     Subjects.CUSTOM_METRICS: Actions.CUSTOM_METRICS_ACTIONS,
+    Subjects.MONITORING_JOB: Actions.MONITORING_JOBS_ACTIONS,
 }
 
 
 class ArgumentsOptions:
     VERBOSE = "--verbose"
     QUIET = "--quiet"
     JSON = "--json"
     TERSE = "--terse"
     PREDICTION_ENVIRONMENT_ID = "--prediction-environment-id"
+    MONITORING_JOB_ID = "--monitoring-job-id"
     DEPLOYMENT_ID = "--deployment-id"
     MODEL_ID = "--model-id"
     MODEL_PACKAGE_ID = "--model-package-id"
     DEPLOYMENT_LABEL = "--deployment-label"
     DATASET_ID = "--dataset-id"
     TRAINING_DATASET_ID = "--training-dataset-id"
     HOLDOUT_DATASET_ID = "--holdout-dataset-id"
@@ -206,14 +215,15 @@
     MODEL = Subjects.MODEL
     DATASET = Subjects.DATASET
     DEPLOYMENT = Subjects.DEPLOYMENT
     PREDICTION_ENVIRONMENT = Subjects.PREDICTION_ENVIRONMENT
     SERVICE_STATS = Subjects.SERVICE_STATS
     BATCH = Subjects.BATCH
     CUSTOM_METRICS = Subjects.CUSTOM_METRICS
+    MONITORING_JOBS = Subjects.MONITORING_JOB
 
     @staticmethod
     def list_all():
         all_subjects = ""
         for m in RunMode:
             all_subjects = f"{all_subjects} {m.value}"
         return all_subjects
@@ -336,14 +346,23 @@
                 ArgumentsOptions.PREDICTION_ENVIRONMENT_ID,
                 default=os.environ.get(EV.MLOPS_PREDICTION_ENVIRONMENT_ID, None),
                 help="Prediction Environment ID "
                 "(env: {})".format(EV.MLOPS_PREDICTION_ENVIRONMENT_ID),
             )
 
     @staticmethod
+    def _register_arg_monitoring_job_id(*parsers):
+        for parser in parsers:
+            parser.add_argument(
+                ArgumentsOptions.MONITORING_JOB_ID,
+                default=os.environ.get(EV.MLOPS_MONITORING_JOB_ID, None),
+                help="Monitoring Job ID " "(env: {})".format(EV.MLOPS_MONITORING_JOB_ID),
+            )
+
+    @staticmethod
     def _register_arg_deployment_label(*parsers):
         for parser in parsers:
             parser.add_argument(
                 ArgumentsOptions.DEPLOYMENT_LABEL,
                 default=os.environ.get(EV.MLOPS_DEPLOYMENT_LABEL, None),
                 help="Deployment label to use when creating a deployment "
                 "(env: {})".format(EV.MLOPS_DEPLOYMENT_LABEL),
@@ -903,14 +922,15 @@
         MLOpsCliArgParser._register_arg_action(parser)
 
         MLOpsCliArgParser._parsers = parser
 
         # multi-use parameters
         MLOpsCliArgParser._register_arg_deployment_id(parser)
         MLOpsCliArgParser._register_arg_pe_id(parser)
+        MLOpsCliArgParser._register_arg_monitoring_job_id(parser)
         MLOpsCliArgParser._register_arg_model_id(parser)
         MLOpsCliArgParser._register_arg_model_package_id(parser)
         MLOpsCliArgParser._register_target_col(parser)
         MLOpsCliArgParser._register_prediction_cols(parser)
         MLOpsCliArgParser._register_class_names(parser)
         MLOpsCliArgParser._register_dry_run(parser)
         MLOpsCliArgParser._register_status_file(parser)
@@ -1333,14 +1353,15 @@
                 self.event_loop.run_until_complete(self._spool_data_dispatcher(spooler))
         finally:
             self.delete_mclient()
 
     async def _spool_data_dispatcher(self, spooler):
         tasks = list()
         total_records = 0
+        failed_records = 0
         log_interval_sec = 180
         start_time = time.time()
         next_log_time = start_time + log_interval_sec
 
         while not spooler.empty():
             record_list = spooler.dequeue()
             total_records += len(record_list)
@@ -1350,14 +1371,17 @@
                 )
             if len(tasks) == self.options.num_concurrent_requests:
                 break
 
         while not spooler.empty() and tasks:
             done, _ = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
             for task in done:
+                if task.exception():
+                    failed_records += 1
+                    logger.error(f"Failed to process task: {task.exception()}")
                 tasks.remove(task)
                 record_list = spooler.dequeue()
                 total_records += len(record_list)
                 for record in record_list:
                     new_task = asyncio.create_task(
                         self._report_predictions_from_spooler(record, spooler)
                     )
@@ -1366,14 +1390,15 @@
                 elapsed = time.time() - start_time
                 logger.info("Records processed so far: %s", total_records)
                 logger.info("Current Throughput: %.02f (records/s)", total_records / elapsed)
                 next_log_time = time.time() + log_interval_sec
 
         runtime = time.time() - start_time
         logger.info("Runtime: %.02f minutes", runtime / 60)
+        logger.info("Total failed records: %s", failed_records)
         logger.info("Total records processed: %s", total_records)
         logger.info("Overall Throughput: %.02f (records/s)", total_records / runtime)
         # No more data to report, all tasks submitted, but let's wait for their completion
         logger.info("Done with submitting all tasks; waiting for them to finish now.")
 
         if tasks:
             await asyncio.wait(tasks)
@@ -1832,52 +1857,27 @@
             self.options.deployment_id, self.options.output_dir
         )
 
         logger.debug(f"Model Package path     {mlpkg_path}")
 
         self.delete_mclient()
 
-    @staticmethod
-    def _convert_feature_format(feature):
-        # FeatureType is defined in mlops-stats-aggregator library and are the types
-        # currently supported, this mostly correspond to EdaTypeEnum in DR side.
-        # Note: types not cover here (percentage, length, currency) are mapped to numeric after
-        # formatting.
-        from datarobot.mlops.stats_aggregator.types import FeatureType
-
-        feature_type = feature.get("featureType")
-
-        if feature_type == "Categorical":
-            feature_type = FeatureType.CATEGORY
-        elif feature_type == "Numeric":
-            feature_type = FeatureType.NUMERIC
-        elif feature_type == "Text":
-            feature_type = FeatureType.TEXT_WORDS
-        elif feature_type == "Date":
-            feature_type = FeatureType.DATE
-
-        return {
-            "name": feature.get("name"),
-            "feature_type": feature_type,
-            "format": feature.get("dateFormat"),
-        }
-
     def get_features_from_model_package(self):
         check_required_parameter(
             self.options.model_package_id,
             EV.MLOPS_MODEL_PACKAGE_ID,
             ArgumentsOptions.MODEL_PACKAGE_ID,
         )
         self.create_mclient()
         self._log_get_action("model package", self.options.model_package_id)
         try:
             info = self.mclient.get_features_from_model_package(
                 self.options.model_package_id, params={"offset": 0, "limit": 0}
             )
-            feature_types = [self._convert_feature_format(f) for f in info]
+            feature_types = [convert_feature_format(f) for f in info]
 
             if self.options.output_file:
                 with open(self.options.output_file, "w") as f:
                     json.dump(feature_types, f)
 
             self._print_resource_received(self.options.model_package_id, feature_types)
         except DRNotFoundException as e:
@@ -2193,14 +2193,96 @@
         except DRMLOpsConnectedException as e:
             self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
         except Exception as e:
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
         finally:
             self.delete_mclient()
 
+    def create_monitoring_job(self):
+        check_required_parameter(self.options.json_config, None, ArgumentsOptions.JSON_CONF)
+        try:
+            info = self._read_json_config(self.options.json_config)
+            if self.options.deployment_id:
+                # if deployment id is provided, use it to create the monitoring job
+                info["deploymentId"] = self.options.deployment_id
+
+            self.create_mclient()
+            job_id = self.mclient.create_monitoring_job(info)
+            self._print_resource_generic_action(job_id)
+            logger.info(f"Created monitoring job ID {job_id}.")
+        except FileNotFoundError as e:
+            self._log_error_and_exit(e, ExitCode.FILE_NOT_FOUND.value)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    def get_monitoring_job(self):
+        check_required_parameter(
+            self.options.monitoring_job_id,
+            EV.MLOPS_MONITORING_JOB_ID,
+            ArgumentsOptions.MONITORING_JOB_ID,
+        )
+        self.create_mclient()
+        self._log_get_action("monitoring job", self.options.monitoring_job_id)
+        try:
+            info = self.mclient.get_monitoring_job(self.options.monitoring_job_id)
+            self._print_resource_received(self.options.monitoring_job_id, info)
+        except DRNotFoundException as e:
+            self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    def abort_running_monitoring_job(self):
+        check_required_parameter(
+            self.options.monitoring_job_id,
+            EV.MLOPS_MONITORING_JOB_ID,
+            ArgumentsOptions.MONITORING_JOB_ID,
+        )
+        self.create_mclient()
+        self._log_delete_action("monitoring job", self.options.monitoring_job_id)
+        try:
+            self.mclient.abort_running_monitoring_job(self.options.monitoring_job_id)
+            self._print_resource_generic_action(self.options.monitoring_job_id)
+        except DRNotFoundException as e:
+            self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    def upload_input_file_to_monitoring_job(self):
+        check_required_parameter(
+            self.options.monitoring_job_id,
+            EV.MLOPS_MONITORING_JOB_ID,
+            ArgumentsOptions.MONITORING_JOB_ID,
+        )
+        check_required_parameter(self.options.input, None, ArgumentsOptions.INPUT)
+
+        self.create_mclient()
+        logger.info(f"Uploading data - {self.options.input}.")
+        try:
+            self.mclient.upload_input_file_to_monitoring_job(
+                self.options.monitoring_job_id, self.options.input
+            )
+            logger.info("Dataset uploaded.")
+        except Exception as e:
+            logger.error("Dataset upload failed.")
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED)
+        finally:
+            self.delete_mclient()
+
     @staticmethod
     def _print_supported_actions(subject):
         actions = SUPPORTED_ACTIONS[subject]
         if len(actions) == 1:
             print(f"Supported {subject} action is: {actions[0]}")
         else:
             print("Supported {} actions are: {}".format(subject, ", ".join(actions)))
@@ -2283,14 +2365,26 @@
         elif self.options.action == Actions.LIST:
             self.list_prediction_environments()
         elif self.options.action == Actions.CREATE:
             self.create_prediction_environment()
         else:
             self._print_supported_actions(Subjects.PREDICTION_ENVIRONMENT)
 
+    def handle_monitoring_jobs(self):
+        if self.options.action == Actions.CREATE:
+            self.create_monitoring_job()
+        elif self.options.action == Actions.GET:
+            self.get_monitoring_job()
+        elif self.options.action == Actions.CANCEL:
+            self.abort_running_monitoring_job()
+        elif self.options.action == Actions.UPLOAD:
+            self.upload_input_file_to_monitoring_job()
+        else:
+            self._print_supported_actions(Subjects.MONITORING_JOB)
+
     def handle_service_stats(self):
         if self.options.action == Actions.GET:
             self.get_service_stats()
         else:
             self._print_supported_actions(Subjects.SERVICE_STATS)
 
     def create_custom_metric(self):
@@ -2645,14 +2739,16 @@
             self.handle_prediction_environment()
         elif self.run_mode == RunMode.SERVICE_STATS:
             self.handle_service_stats()
         elif self.run_mode == RunMode.BATCH:
             self.handle_batch()
         elif self.run_mode == RunMode.CUSTOM_METRICS:
             self.handle_custom_metrics()
+        elif self.run_mode == RunMode.MONITORING_JOBS:
+            self.handle_monitoring_jobs()
         else:
             print("No valid subject provided")
             raise SystemExit(ExitCode.INVALID_CLI_INPUT.value)
 
 
 def check_required_parameter(option, env_name, parameter_name):
     if option is None:
```

## datarobot/mlops/connected/url_helper.py

```diff
@@ -38,14 +38,16 @@
 
 
 class MMMEndpointPrefix:
     DEPLOYMENT = "api/v2/deployments"
     DATASET = "api/v2/datasets"
     MODEL_PACKAGE = "api/v2/modelPackages"
     PREDICTION_ENV = "api/v2/predictionEnvironments"
+    BATCH_MONITORING = "api/v2/batchMonitoring"
+    BATCH_JOBS = "api/v2/batchJobs"
 
 
 class MMMEndpoint:
     ARCHIVE = "archive"
     FEATURES = "features"
     FROM_FILE = "fromFile"
     PREDICTION_DATASET = "predictionInputs/fromDataset/"
@@ -66,14 +68,15 @@
     PREDICTION_STATS = "predictionsOverTime"
     TARGET_DRIFT = "targetDrift"
     PREDICTIONS_ACTUALS_STATS = "predictionsVsActualsOverTime"
     MONITORING_BATCHES = "monitoringBatches"
     PREDICTIONS_OVER_BATCH = "predictionsOverBatch"
     CUSTOM_METRICS = "customMetrics"
     SUMMARY = "summary"
+    CSV_UPLOAD = "csvUpload"
 
 
 class URLBuilder:
     def __init__(self, service_url):
         self._service_url = service_url
 
     def deployment(self, deployment_id, force_delete=False):
@@ -259,14 +262,25 @@
 
     def get_prediction_environment(self, pe_id):
         return build_url(self._service_url, MMMEndpointPrefix.PREDICTION_ENV, pe_id)
 
     def list_prediction_environments(self):
         return build_url(self._service_url, MMMEndpointPrefix.PREDICTION_ENV)
 
+    def create_monitoring_job(self):
+        return build_url(self._service_url, MMMEndpointPrefix.BATCH_MONITORING, None)
+
+    def get_monitoring_job(self, job_id):
+        return build_url(self._service_url, MMMEndpointPrefix.BATCH_JOBS, job_id)
+
+    def upload_file_to_monitoring_job(self, job_id):
+        return build_url(
+            self._service_url, MMMEndpointPrefix.BATCH_JOBS, job_id, MMMEndpoint.CSV_UPLOAD
+        )
+
     def get_service_stats(self, deployment_id):
         return build_url(
             self._service_url,
             MMMEndpointPrefix.DEPLOYMENT,
             deployment_id,
             MMMEndpoint.SERVICE_STATS,
         )
```

## Comparing `datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA` & `datarobot_mlops_connected_client-9.1.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-mlops-connected-client
-Version: 9.1.1rc1
+Version: 9.1.3
 Summary: datarobot-mlops-connected-client client to communicate with DataRobot MLOps service
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: support@datarobot.com
 Maintainer: DataRobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
@@ -20,14 +20,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: pandas
 Requires-Dist: requests
+Requires-Dist: requests-toolbelt
 Requires-Dist: datarobot-mlops (>=9.1.1b1)
 
 # DataRobot MLOps Connected client (mlops-cli)
 
 This is the Python client used to communicate with the
 DataRobot MLOps service. It can be used to upload datasets,
 create and deploy model packages, report predictions files, etc.
```

## Comparing `datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD` & `datarobot_mlops_connected_client-9.1.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 datarobot/mlops/__init__.py,sha256=AKjMKTNwSwhUBVbzAe95rrPT428dkII5aszufDWlEYw,597
 datarobot/mlops/connected/__init__.py,sha256=gtaquSkCXoIY93Uy5hmlx-TbK6pSnDoGPwV-KeoM-DU,532
-datarobot/mlops/connected/client.py,sha256=TVxqXOa4Yl4yMfU_n76gsuBfH6TpWOos0aSWP9OsqSU,106180
+datarobot/mlops/connected/client.py,sha256=1FhNJqFAzusvvXF8gFMk0TN3k7Xu3BQrb4lXuDjPsd4,109951
 datarobot/mlops/connected/enums.py,sha256=ygJSPeoZjdYGWMBGJ3X18RumXqCEsnEdGQB6yqpI77g,1231
 datarobot/mlops/connected/exception.py,sha256=2Y-nd3Lbo6abhvyS3nTUPwnS8sGTdk29-kl3gsuUihA,900
-datarobot/mlops/connected/mlops_cli.py,sha256=vqSeMdyFpKfBPvukaC7fiErqDVw8zKiJwRDgNzYHYK4,110928
+datarobot/mlops/connected/mlops_cli.py,sha256=vf046PT_W4ICqULDU_tOWsqAuOfQulOsSxVDfQQdM6A,115239
 datarobot/mlops/connected/upload_tracker.py,sha256=sgMVqBgI7xvXtpLYINqnxaw4AljraDVg5Gg3An8pq3A,2646
-datarobot/mlops/connected/url_helper.py,sha256=hlQP_JC4ACMKqXaN_R6a91M3vUq97aAsVuTRCIZ3vMs,11367
-datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA,sha256=FsimiGR4Inq0O84Sr42Jq2tBVnWap-jNG0VehOwSRoo,1537
-datarobot_mlops_connected_client-9.1.1rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datarobot_mlops_connected_client-9.1.1rc1.dist-info/entry_points.txt,sha256=pjOHN_gQuYzuqbf0AL5S5lcGhDfIlOGElQU2Qduh2mg,72
-datarobot_mlops_connected_client-9.1.1rc1.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
-datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD,,
+datarobot/mlops/connected/url_helper.py,sha256=BfLk1BIP2-Sx0S2FWzzDy13w4iB6fZhF_DChYStdmSM,11911
+datarobot_mlops_connected_client-9.1.3.dist-info/METADATA,sha256=kg_YKCGJSZKJRxQo6XL1q9Knqa3ipa6xEGyRJDZ8S3o,1567
+datarobot_mlops_connected_client-9.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_mlops_connected_client-9.1.3.dist-info/entry_points.txt,sha256=pjOHN_gQuYzuqbf0AL5S5lcGhDfIlOGElQU2Qduh2mg,72
+datarobot_mlops_connected_client-9.1.3.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
+datarobot_mlops_connected_client-9.1.3.dist-info/RECORD,,
```

