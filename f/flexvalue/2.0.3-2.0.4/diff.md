# Comparing `tmp/flexvalue-2.0.3.tar.gz` & `tmp/flexvalue-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexvalue-2.0.3.tar", last modified: Wed Jun 28 23:18:24 2023, max compression
+gzip compressed data, was "flexvalue-2.0.4.tar", last modified: Thu Jun 29 05:53:59 2023, max compression
```

## Comparing `flexvalue-2.0.3.tar` & `flexvalue-2.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:18:24.796315 flexvalue-2.0.3/
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-28 23:18:24.796315 flexvalue-2.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    30648 2023-06-27 21:15:27.000000 flexvalue-2.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:18:24.760311 flexvalue-2.0.3/flexvalue/
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      984 2023-06-28 23:17:36.000000 flexvalue-2.0.3/flexvalue/__version__.py
--rw-rw-r--   0 root         (0) root         (0)    14642 2023-01-19 00:54:27.000000 flexvalue-2.0.3/flexvalue/cet_flexvalue_compare.py
--rw-rw-r--   0 root         (0) root         (0)    10248 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/cli.py
--rw-rw-r--   0 root         (0) root         (0)     6030 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/config.py
--rw-rw-r--   0 root         (0) root         (0)    50314 2023-06-28 22:28:35.000000 flexvalue-2.0.3/flexvalue/db.py
--rw-rw-r--   0 root         (0) root         (0)     3440 2023-01-19 00:54:27.000000 flexvalue-2.0.3/flexvalue/examples.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/flexvalue.py
--rw-rw-r--   0 root         (0) root         (0)     2198 2023-01-31 00:43:43.000000 flexvalue-2.0.3/flexvalue/report.py
--rw-rw-r--   0 root         (0) root         (0)     1446 2023-01-19 00:54:27.000000 flexvalue-2.0.3/flexvalue/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:18:24.784314 flexvalue-2.0.3/flexvalue/sql/
--rw-rw-r--   0 root         (0) root         (0)      569 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/create_elec_av_cost.sql
--rw-rw-r--   0 root         (0) root         (0)      269 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/create_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      311 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/create_gas_av_cost.sql
--rw-rw-r--   0 root         (0) root         (0)      439 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/create_project_info.sql
--rw-rw-r--   0 root         (0) root         (0)      162 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/create_therms_profile.sql
--rw-rw-r--   0 root         (0) root         (0)      125 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/elec_av_costs_index.sql
--rw-rw-r--   0 root         (0) root         (0)      109 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/elec_load_shape_index.sql
--rw-rw-r--   0 root         (0) root         (0)      219 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/gas_av_costs_index.sql
--rw-rw-r--   0 root         (0) root         (0)      520 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/postgres_indexes.sql
--rw-rw-r--   0 root         (0) root         (0)       90 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/project_info_dates_index.sql
--rw-rw-r--   0 root         (0) root         (0)       66 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/project_info_index.sql
--rw-rw-r--   0 root         (0) root         (0)      119 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/sql/therm_profile_index.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:18:24.796315 flexvalue-2.0.3/flexvalue/templates/
--rw-rw-r--   0 root         (0) root         (0)      242 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/bq_create_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      186 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/bq_create_therms_profile.sql
--rw-rw-r--   0 root         (0) root         (0)      603 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/bq_populate_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      664 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/bq_populate_metered_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      571 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/bq_populate_therms_profile.sql
--rw-rw-r--   0 root         (0) root         (0)    12645 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/calculation.sql
--rw-rw-r--   0 root         (0) root         (0)     6677 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/elec_calculation.sql
--rw-rw-r--   0 root         (0) root         (0)     6250 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/gas_calculation.sql
--rw-rw-r--   0 root         (0) root         (0)      101 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/get_project_info.sql
--rw-rw-r--   0 root         (0) root         (0)      117 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/get_therms_profiles.sql
--rw-rw-r--   0 root         (0) root         (0)      693 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/load_elec_av_costs.sql
--rw-rw-r--   0 root         (0) root         (0)      291 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/load_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      296 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/load_gas_av_costs.sql
--rw-rw-r--   0 root         (0) root         (0)      565 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/load_project_info.sql
--rw-rw-r--   0 root         (0) root         (0)      201 2023-06-27 21:15:27.000000 flexvalue-2.0.3/flexvalue/templates/load_therms_profiles.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:18:24.768312 flexvalue-2.0.3/flexvalue.egg-info/
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-28 23:18:24.000000 flexvalue-2.0.3/flexvalue.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1589 2023-06-28 23:18:24.000000 flexvalue-2.0.3/flexvalue.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 23:18:24.000000 flexvalue-2.0.3/flexvalue.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-28 23:18:24.000000 flexvalue-2.0.3/flexvalue.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-28 23:18:24.000000 flexvalue-2.0.3/flexvalue.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-28 23:18:24.000000 flexvalue-2.0.3/flexvalue.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       63 2023-06-28 23:18:24.804316 flexvalue-2.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3536 2023-06-28 23:08:42.000000 flexvalue-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:53:59.097863 flexvalue-2.0.4/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 05:53:59.097863 flexvalue-2.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    30648 2023-06-29 00:17:22.000000 flexvalue-2.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:53:59.085862 flexvalue-2.0.4/flexvalue/
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      984 2023-06-29 05:52:35.000000 flexvalue-2.0.4/flexvalue/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)    14642 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/cet_flexvalue_compare.py
+-rw-rw-r--   0 root         (0) root         (0)    10248 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/cli.py
+-rw-rw-r--   0 root         (0) root         (0)     6030 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/config.py
+-rw-rw-r--   0 root         (0) root         (0)    51618 2023-06-29 05:42:03.000000 flexvalue-2.0.4/flexvalue/db.py
+-rw-rw-r--   0 root         (0) root         (0)     3440 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/examples.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/flexvalue.py
+-rw-rw-r--   0 root         (0) root         (0)     2198 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/report.py
+-rw-rw-r--   0 root         (0) root         (0)     1446 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:53:59.093862 flexvalue-2.0.4/flexvalue/sql/
+-rw-rw-r--   0 root         (0) root         (0)      569 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/create_elec_av_cost.sql
+-rw-rw-r--   0 root         (0) root         (0)      269 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/create_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      311 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/create_gas_av_cost.sql
+-rw-rw-r--   0 root         (0) root         (0)      439 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/create_project_info.sql
+-rw-rw-r--   0 root         (0) root         (0)      162 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/create_therms_profile.sql
+-rw-rw-r--   0 root         (0) root         (0)      125 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/elec_av_costs_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      109 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/elec_load_shape_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      219 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/gas_av_costs_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      520 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/postgres_indexes.sql
+-rw-rw-r--   0 root         (0) root         (0)       90 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/project_info_dates_index.sql
+-rw-rw-r--   0 root         (0) root         (0)       66 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/project_info_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      119 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/sql/therm_profile_index.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:53:59.097863 flexvalue-2.0.4/flexvalue/templates/
+-rw-rw-r--   0 root         (0) root         (0)      242 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/bq_create_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      186 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/bq_create_therms_profile.sql
+-rw-rw-r--   0 root         (0) root         (0)      603 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/bq_populate_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      664 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/bq_populate_metered_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      571 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/bq_populate_therms_profile.sql
+-rw-rw-r--   0 root         (0) root         (0)    12645 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/calculation.sql
+-rw-rw-r--   0 root         (0) root         (0)     6677 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/elec_calculation.sql
+-rw-rw-r--   0 root         (0) root         (0)     6289 2023-06-29 04:31:43.000000 flexvalue-2.0.4/flexvalue/templates/gas_calculation.sql
+-rw-rw-r--   0 root         (0) root         (0)      101 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/get_project_info.sql
+-rw-rw-r--   0 root         (0) root         (0)      117 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/get_therms_profiles.sql
+-rw-rw-r--   0 root         (0) root         (0)      693 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/load_elec_av_costs.sql
+-rw-rw-r--   0 root         (0) root         (0)      291 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/load_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      296 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/load_gas_av_costs.sql
+-rw-rw-r--   0 root         (0) root         (0)      565 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/load_project_info.sql
+-rw-rw-r--   0 root         (0) root         (0)      201 2023-06-29 00:17:22.000000 flexvalue-2.0.4/flexvalue/templates/load_therms_profiles.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:53:59.089862 flexvalue-2.0.4/flexvalue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 05:53:58.000000 flexvalue-2.0.4/flexvalue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-29 05:53:58.000000 flexvalue-2.0.4/flexvalue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 05:53:58.000000 flexvalue-2.0.4/flexvalue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-29 05:53:58.000000 flexvalue-2.0.4/flexvalue.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-29 05:53:58.000000 flexvalue-2.0.4/flexvalue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-29 05:53:58.000000 flexvalue-2.0.4/flexvalue.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       63 2023-06-29 05:53:59.097863 flexvalue-2.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3536 2023-06-29 00:17:22.000000 flexvalue-2.0.4/setup.py
```

### Comparing `flexvalue-2.0.3/PKG-INFO` & `flexvalue-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: flexvalue
-Version: 2.0.3
+Version: 2.0.4
 Summary: FLEXvalue: a tool for calculating avoided costs
 Home-page: http://github.com/recurve-methods/flexvalue
 Author: Recurve Analytics, Inc.
 Author-email: support@recurve.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `flexvalue-2.0.3/README.rst` & `flexvalue-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/__init__.py` & `flexvalue-2.0.4/flexvalue/__init__.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/__version__.py` & `flexvalue-2.0.4/flexvalue/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,12 +16,12 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 """
 __title__ = "FLEXvalue"
 __description__ = "FLEXvalue: a tool for calculating avoided costs"
 __url__ = "http://github.com/recurve-methods/flexvalue"
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 __author__ = "Recurve Analytics, Inc."
 __author_email__ = "support@recurve.com"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2021 Recurve Analytics, Inc."
```

### Comparing `flexvalue-2.0.3/flexvalue/cet_flexvalue_compare.py` & `flexvalue-2.0.4/flexvalue/cet_flexvalue_compare.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/cli.py` & `flexvalue-2.0.4/flexvalue/cli.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/config.py` & `flexvalue-2.0.4/flexvalue/config.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/db.py` & `flexvalue-2.0.4/flexvalue/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1123,14 +1123,27 @@
             if len(table.schema) == len(original_schema) + 1 == len(new_schema):
                 print("A new column has been added.")
             else:
                 raise FLEXValueException(
                     f"Unable to add a datetime column to {table_name}; can't process gas avoided costs."
                 )
 
+    def _copy_table(self, source_table, target_table):
+        """source_table and target_table must include the dataset in their values, like {dataset}.{table}.
+        This deletes target_table before copying source_table to it.
+        """
+        self.client.delete_table(target_table, not_found_ok=True)
+        job_config = bigquery.CopyJobConfig()
+        job_config.write_disposition = bigquery.WriteDisposition.WRITE_TRUNCATE
+        job_config.create_disposition = bigquery.CreateDisposition.CREATE_IF_NEEDED
+        copy_job = self.client.copy_table(
+            source_table, target_table, job_config=job_config
+        )
+        copy_job.result()
+
     def process_elec_load_shape(self, elec_load_shapes_path: str, truncate=False):
         """Transforms data in the table specified by config.elec_load_shape_table, and loads it into `elec_load_shape`."""
         dataset = self._get_target_dataset()
         self._prepare_table(
             f"{dataset}.elec_load_shape", "bq_create_elec_load_shape.sql", truncate=True
         )
         template = self.template_env.get_template("bq_populate_elec_load_shape.sql")
@@ -1146,22 +1159,25 @@
         )
         # fmt: on
         logging.info(f"elec_load_shape sql = {sql}")
         query_job = self.client.query(sql)
         result = query_job.result()
 
     def process_metered_load_shape(self, metered_load_shapes_path: str, truncate=False):
-        """Transforms data in the table specified by config.metered_load_shape_table, and loads it into `elec_load_shape`."""
+        """Transforms data in the table specified by config.metered_load_shape_table, and
+        loads it into `elec_load_shape`. First copies the specified elec_load_shape table
+        into {target_dataset}.elec_load_shape."""
         dataset = self._get_target_dataset()
         self._prepare_table(
             f"{dataset}.elec_load_shape",
             "bq_create_elec_load_shape.sql",
             truncate=truncate,
         )
 
+        self._copy_table(self.config.elec_load_shape_table, f"{self._get_target_dataset()}.elec_load_shape")
         template = self.template_env.get_template("bq_populate_metered_load_shape.sql")
         # Black ruins readability here, disable
         # fmt: off
         sql = template.render(
             {
                 "source_dataset": ".".join(self.config.metered_load_shape_table.split(".")[:-1]),
                 "target_dataset": dataset,
@@ -1195,26 +1211,36 @@
             }
         )
         # fmt: on
         logging.debug(f"therms_profile sql = {sql}")
         query_job = self.client.query(sql)
         result = query_job.result()
 
+    def _elec_load_shape_for_context(self):
+        if self.config.process_metered_load_shape or self.config.process_elec_load_shape:
+            return f"{self._get_target_dataset()}.elec_load_shape"
+        return self.config.elec_load_shape_table
+
+    def _therms_profile_for_context(self):
+        if self.config.process_therms_profiles:
+            return f"{self._get_target_dataset()}.therms_profile"
+        return self.config.therms_profiles_table
+
     def _get_calculation_sql_context(self, mode=""):
         elec_agg_columns = self._elec_aggregation_columns()
         gas_agg_columns = self._gas_aggregation_columns()
         elec_addl_fields = self._elec_addl_fields(elec_agg_columns)
         gas_addl_fields = self._gas_addl_fields(gas_agg_columns)
         # TODO double-check this: should the av_costs tables be treated the same as the load shapes?
         context = {
             "project_info_table": self.config.project_info_table,
             "eac_table": self.config.elec_av_costs_table,
-            "els_table": f"`{self._get_target_dataset()}.elec_load_shape`",
+            "els_table": self._elec_load_shape_for_context(),
             "gac_table": self.config.gas_av_costs_table,
-            "therms_profile_table": f"`{self._get_target_dataset()}.therms_profile`",
+            "therms_profile_table": self._therms_profile_for_context(),
             "float_type": self.config.float_type(),
             "database_type": self.config.database_type,
             "elec_components": self._elec_components(),
             "gas_components": self._gas_components(),
         }
         if mode == "electric":
             context["elec_aggregation_columns"] = elec_agg_columns
```

### Comparing `flexvalue-2.0.3/flexvalue/examples.py` & `flexvalue-2.0.4/flexvalue/examples.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/flexvalue.py` & `flexvalue-2.0.4/flexvalue/flexvalue.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/report.py` & `flexvalue-2.0.4/flexvalue/report.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/settings.py` & `flexvalue-2.0.4/flexvalue/settings.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/sql/create_elec_av_cost.sql` & `flexvalue-2.0.4/flexvalue/sql/create_elec_av_cost.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/sql/postgres_indexes.sql` & `flexvalue-2.0.4/flexvalue/sql/postgres_indexes.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/bq_populate_elec_load_shape.sql` & `flexvalue-2.0.4/flexvalue/templates/bq_populate_elec_load_shape.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/bq_populate_metered_load_shape.sql` & `flexvalue-2.0.4/flexvalue/templates/bq_populate_metered_load_shape.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/bq_populate_therms_profile.sql` & `flexvalue-2.0.4/flexvalue/templates/bq_populate_therms_profile.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/calculation.sql` & `flexvalue-2.0.4/flexvalue/templates/calculation.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/elec_calculation.sql` & `flexvalue-2.0.4/flexvalue/templates/elec_calculation.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/gas_calculation.sql` & `flexvalue-2.0.4/flexvalue/templates/gas_calculation.sql`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     , pcwdga.{{ field }}
     {% endfor -%}
     {%- for column in gas_aggregation_columns %}, pcwdga.{{ column }}{% endfor %}
 )
 
 SELECT
 gas_calculations.id
+, SUM(gas_calculations.total) as total
 {% if database_type == "postgresql" -%}
 , CASE
     WHEN MAX(gas_calculations.trc_costs) = 0 AND SUM(gas_calculations.gas_benefits) > 0 then FLOAT 'inf'
     WHEN MAX(gas_calculations.trc_costs) = 0 AND SUM(gas_calculations.gas_benefits) < 0 then FLOAT '-inf'
     WHEN MAX(gas_calculations.trc_costs) = 0 AND SUM(gas_calculations.gas_benefits) = 0 then 0.0
     ELSE SUM(gas_calculations.gas_benefits) / MAX(gas_calculations.trc_costs)
   END as trc_ratio
```

### Comparing `flexvalue-2.0.3/flexvalue/templates/load_elec_av_costs.sql` & `flexvalue-2.0.4/flexvalue/templates/load_elec_av_costs.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue/templates/load_project_info.sql` & `flexvalue-2.0.4/flexvalue/templates/load_project_info.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/flexvalue.egg-info/PKG-INFO` & `flexvalue-2.0.4/flexvalue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: flexvalue
-Version: 2.0.3
+Version: 2.0.4
 Summary: FLEXvalue: a tool for calculating avoided costs
 Home-page: http://github.com/recurve-methods/flexvalue
 Author: Recurve Analytics, Inc.
 Author-email: support@recurve.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `flexvalue-2.0.3/flexvalue.egg-info/SOURCES.txt` & `flexvalue-2.0.4/flexvalue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.3/setup.py` & `flexvalue-2.0.4/setup.py`

 * *Files identical despite different names*

