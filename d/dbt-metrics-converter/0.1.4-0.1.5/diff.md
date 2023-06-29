# Comparing `tmp/dbt_metrics_converter-0.1.4.tar.gz` & `tmp/dbt_metrics_converter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_metrics_converter-0.1.4.tar", max compression
+gzip compressed data, was "dbt_metrics_converter-0.1.5.tar", max compression
```

## Comparing `dbt_metrics_converter-0.1.4.tar` & `dbt_metrics_converter-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1823 2023-06-29 20:23:23.759876 dbt_metrics_converter-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-27 22:07:13.604392 dbt_metrics_converter-0.1.4/converter/__init__.py
--rw-r--r--   0        0        0     2888 2023-06-27 22:07:13.605469 dbt_metrics_converter-0.1.4/converter/dbt_metrics_to_semantic_model_converter.py
--rwxr-xr-x   0        0        0     1120 2023-06-29 20:23:23.763066 dbt_metrics_converter-0.1.4/converter/main.py
--rw-r--r--   0        0        0     3378 2023-06-29 20:23:23.763615 dbt_metrics_converter-0.1.4/converter/spec_upgrade.py
--rw-r--r--   0        0        0        0 2023-06-27 22:07:13.606341 dbt_metrics_converter-0.1.4/metricflow_parsing/__init__.py
--rw-r--r--   0        0        0     1807 2023-06-27 22:07:13.606510 dbt_metrics_converter-0.1.4/metricflow_parsing/dbt_dir_to_model.py
--rw-r--r--   0        0        0    19978 2023-06-27 22:07:13.606691 dbt_metrics_converter-0.1.4/metricflow_parsing/dbt_to_metricflow.py
--rw-r--r--   0        0        0      614 2023-06-29 20:25:23.920377 dbt_metrics_converter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 dbt_metrics_converter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1823 2023-06-29 20:27:21.644370 dbt_metrics_converter-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 22:07:13.604392 dbt_metrics_converter-0.1.5/converter/__init__.py
+-rw-r--r--   0        0        0     2888 2023-06-27 22:07:13.605469 dbt_metrics_converter-0.1.5/converter/dbt_metrics_to_semantic_model_converter.py
+-rwxr-xr-x   0        0        0     1120 2023-06-29 20:23:23.763066 dbt_metrics_converter-0.1.5/converter/main.py
+-rw-r--r--   0        0        0     3378 2023-06-29 20:23:23.763615 dbt_metrics_converter-0.1.5/converter/spec_upgrade.py
+-rw-r--r--   0        0        0        0 2023-06-27 22:07:13.606341 dbt_metrics_converter-0.1.5/metricflow_parsing/__init__.py
+-rw-r--r--   0        0        0     1807 2023-06-27 22:07:13.606510 dbt_metrics_converter-0.1.5/metricflow_parsing/dbt_dir_to_model.py
+-rw-r--r--   0        0        0    19978 2023-06-27 22:07:13.606691 dbt_metrics_converter-0.1.5/metricflow_parsing/dbt_to_metricflow.py
+-rw-r--r--   0        0        0      616 2023-06-29 20:27:27.678703 dbt_metrics_converter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 dbt_metrics_converter-0.1.5/PKG-INFO
```

### Comparing `dbt_metrics_converter-0.1.4/README.md` & `dbt_metrics_converter-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+Metadata-Version: 2.1
+Name: dbt-metrics-converter
+Version: 0.1.5
+Summary: Easily convert out of date, or unsported metrics spec into the latest suported metrics spec in dbt
+Author: Jordan Stein
+Author-email: jordan.stein77@gmail.com
+Requires-Python: >=3.9,<3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: dbt-core (>=1.5.0,<2.0.0)
+Requires-Dist: dbt-semantic-interfaces (==0.1.0.dev4)
+Requires-Dist: metricflow (==0.200.0.dev4)
+Description-Content-Type: text/markdown
+
 The dbt converter is a CLI tool that simplifies the process of migrating from the metrics spec supported in dbt v1.5 and earlier to the metrics specification supported in dbt ≥v1.6.
 
 **Installing dbt converter**
 
 ```sql
-pip install dbt-converter
+pip install dbt-metrics-converter
 ```
 
 **Upgrading to dbt v1.6 spec**
 
 1. Navigate to the root of your dbt project.
-2. Install the `dbt-converter` package using pip. Note that the converter requires `dbt-core==1.5`. You may need to update the version range for the `dbt_metrics` package.
-3. Run `dc convert-metrics`. The converter assumes you are in the root of your dbt project. Optionally, you can pass the project path `-dbt-project-path path/to/dbt_project`. NOTE: All metrics must have a timestamp for the upgrade to run. If your metrics do not have a timestamp, add one before running the converter.
+2. `pip install dbt-metrics-converter`. Note that the converter requires `dbt-core==1.5`. You may need to update the version range for the `dbt_metrics` package.
+3. Run `dbtc convert-metrics`. The converter assumes you are in the root of your dbt project. Optionally, you can pass the project path `-dbt-project-path path/to/dbt_project`. NOTE: All metrics must have a timestamp for the upgrade to run. If your metrics do not have a timestamp, add one before running the converter.
 4. Semantic models and metrics files will be created in the `semantic_models` and `metrics` directories. Move these folders into your model path.
 5. Delete the `metrics` package, move the old metrics configs out of your model path, or delete them.
 
 **Testing your metrics in dbt v1.6**
 
 1. Upgrade to dbt v1.6, and `pip install dbt-metricflow`
 2. Remove the old metrics package from your `dbt_packages` and run `dbt clean && dbt deps`. 
@@ -22,8 +37,8 @@
 4. View the metrics in your dbt project by running `mf list metrics`
 5. Run `mf validate-configs —skip-dw` to validate metrics configs. 
 6. To run a test query, run `mf query --metrics <metric_name>`
 
 **Gotchas:**
 
 - Some packages, like fivetran/ad_reporting have metrics defined in them using the v1.5 spec, this may cause an error if you try to run your project after upgrading to v1.6
-- Make sure to delete any calls of `metrics.calculate` or `metrics.develop` they won’t work without the dbt_metrics package
+- Make sure to delete any calls of `metrics.calculate` or `metrics.develop` they won’t work without the dbt_metrics package
```

### Comparing `dbt_metrics_converter-0.1.4/converter/dbt_metrics_to_semantic_model_converter.py` & `dbt_metrics_converter-0.1.5/converter/dbt_metrics_to_semantic_model_converter.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.4/converter/main.py` & `dbt_metrics_converter-0.1.5/converter/main.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.4/converter/spec_upgrade.py` & `dbt_metrics_converter-0.1.5/converter/spec_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.4/metricflow_parsing/dbt_dir_to_model.py` & `dbt_metrics_converter-0.1.5/metricflow_parsing/dbt_dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.4/metricflow_parsing/dbt_to_metricflow.py` & `dbt_metrics_converter-0.1.5/metricflow_parsing/dbt_to_metricflow.py`

 * *Files identical despite different names*

### Comparing `dbt_metrics_converter-0.1.4/pyproject.toml` & `dbt_metrics_converter-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-metrics-converter"
-version = "0.1.4"
+version = "0.1.5"
 description = "Easily convert out of date, or unsported metrics spec into the latest suported metrics spec in dbt"
 authors = ["Jordan Stein <jordan.stein77@gmail.com>"]
 readme = "README.md"
 packages = [{include = "converter"},{include = "metricflow_parsing"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
@@ -15,9 +15,9 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
- dc= 'converter.main:cli'
+ dbtc= 'converter.main:cli'
```

### Comparing `dbt_metrics_converter-0.1.4/PKG-INFO` & `dbt_metrics_converter-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-Metadata-Version: 2.1
-Name: dbt-metrics-converter
-Version: 0.1.4
-Summary: Easily convert out of date, or unsported metrics spec into the latest suported metrics spec in dbt
-Author: Jordan Stein
-Author-email: jordan.stein77@gmail.com
-Requires-Python: >=3.9,<3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: dbt-core (>=1.5.0,<2.0.0)
-Requires-Dist: dbt-semantic-interfaces (==0.1.0.dev4)
-Requires-Dist: metricflow (==0.200.0.dev4)
-Description-Content-Type: text/markdown
-
 The dbt converter is a CLI tool that simplifies the process of migrating from the metrics spec supported in dbt v1.5 and earlier to the metrics specification supported in dbt ≥v1.6.
 
 **Installing dbt converter**
 
 ```sql
-pip install dbt-converter
+pip install dbt-metrics-converter
 ```
 
 **Upgrading to dbt v1.6 spec**
 
 1. Navigate to the root of your dbt project.
-2. Install the `dbt-converter` package using pip. Note that the converter requires `dbt-core==1.5`. You may need to update the version range for the `dbt_metrics` package.
-3. Run `dc convert-metrics`. The converter assumes you are in the root of your dbt project. Optionally, you can pass the project path `-dbt-project-path path/to/dbt_project`. NOTE: All metrics must have a timestamp for the upgrade to run. If your metrics do not have a timestamp, add one before running the converter.
+2. `pip install dbt-metrics-converter`. Note that the converter requires `dbt-core==1.5`. You may need to update the version range for the `dbt_metrics` package.
+3. Run `dbtc convert-metrics`. The converter assumes you are in the root of your dbt project. Optionally, you can pass the project path `-dbt-project-path path/to/dbt_project`. NOTE: All metrics must have a timestamp for the upgrade to run. If your metrics do not have a timestamp, add one before running the converter.
 4. Semantic models and metrics files will be created in the `semantic_models` and `metrics` directories. Move these folders into your model path.
 5. Delete the `metrics` package, move the old metrics configs out of your model path, or delete them.
 
 **Testing your metrics in dbt v1.6**
 
 1. Upgrade to dbt v1.6, and `pip install dbt-metricflow`
 2. Remove the old metrics package from your `dbt_packages` and run `dbt clean && dbt deps`. 
@@ -37,8 +22,8 @@
 4. View the metrics in your dbt project by running `mf list metrics`
 5. Run `mf validate-configs —skip-dw` to validate metrics configs. 
 6. To run a test query, run `mf query --metrics <metric_name>`
 
 **Gotchas:**
 
 - Some packages, like fivetran/ad_reporting have metrics defined in them using the v1.5 spec, this may cause an error if you try to run your project after upgrading to v1.6
-- Make sure to delete any calls of `metrics.calculate` or `metrics.develop` they won’t work without the dbt_metrics package
+- Make sure to delete any calls of `metrics.calculate` or `metrics.develop` they won’t work without the dbt_metrics package
```

