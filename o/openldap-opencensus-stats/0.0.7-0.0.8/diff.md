# Comparing `tmp/openldap-opencensus-stats-0.0.7.tar.gz` & `tmp/openldap-opencensus-stats-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openldap-opencensus-stats-0.0.7.tar", last modified: Fri Mar 31 19:48:44 2023, max compression
+gzip compressed data, was "openldap-opencensus-stats-0.0.8.tar", last modified: Thu Jun 29 15:48:22 2023, max compression
```

## Comparing `openldap-opencensus-stats-0.0.7.tar` & `openldap-opencensus-stats-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:48:44.335333 openldap-opencensus-stats-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-31 19:48:44.335333 openldap-opencensus-stats-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:48:44.335333 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:48:44.335333 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/child_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/copy_for_each_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_dn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_name_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_query_dn.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/snake_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/ldap_metric_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/ldap_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/ldap_statistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:48:44.335333 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-31 19:48:44.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-31 19:48:44.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:48:44.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 19:48:44.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-31 19:48:44.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-31 19:48:44.000000 openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-31 19:48:44.335333 openldap-opencensus-stats-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-31 19:48:32.000000 openldap-opencensus-stats-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:48:22.297345 openldap-opencensus-stats-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-29 15:48:22.297345 openldap-opencensus-stats-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap-opencensus-stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:48:22.293345 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:48:22.297345 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/child_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/copy_for_each_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_name_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_query_dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/snake_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_metric_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_sync_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/sync_metric_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:48:22.297345 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-29 15:48:22.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-29 15:48:22.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:48:22.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 15:48:22.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 15:48:22.000000 openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 15:48:22.297345 openldap-opencensus-stats-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-29 15:48:05.000000 openldap-opencensus-stats-0.0.8/setup.py
```

### Comparing `openldap-opencensus-stats-0.0.7/LICENSE` & `openldap-opencensus-stats-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/PKG-INFO` & `openldap-opencensus-stats-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openldap-opencensus-stats
-Version: 0.0.7
+Version: 0.0.8
 Summary: OpenLDAP OpenCensus Statistics
 Author: Mark Donnelly
 Author-email: mark@painless-security.com
 License: AGPL 3.0
 Keywords: openldap opencensus metrics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
```

### Comparing `openldap-opencensus-stats-0.0.7/README.md` & `openldap-opencensus-stats-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/__init__.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/base.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/base.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/child_object.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/child_object.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_dn.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_dn.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_name.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_name.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_name_interpolation.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_name_interpolation.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/metric_query_dn.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/metric_query_dn.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/config_transformers/snake_case.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/config_transformers/snake_case.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/configuration.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging.config
 
 import yaml
 from time import sleep
 
 from openldap_opencensus_stats.config_transformers.base import ConfigurationTransformationChainSingleton
 from openldap_opencensus_stats.ldap_metric_set import MetricSet
+from openldap_opencensus_stats.sync_metric_set import SyncMetricSet
 from openldap_opencensus_stats.ldap_server import LdapServerPool
 from openldap_opencensus_stats.ldap_statistic import LdapStatistic
 
 from opencensus.stats import stats
 from opencensus.ext.prometheus import stats_exporter
 import opencensus.ext.stackdriver.stats_exporter
 
@@ -25,14 +26,15 @@
     def __init__(self, config_file_name):
         if config_file_name is None:
             raise ValueError("Config file name must be supplied")
         self._config_file_name = config_file_name
         self._configuration_dict = {}
         self._sleep_time = 5
         self._metric_sets = []
+        self._ldap_metrics = {}
 
         self.reconfigure()
 
     def reconfigure(self):
         self._configuration_dict = read_yaml_file(self._config_file_name)
         normalized_configuration = ConfigurationTransformationChainSingleton().transform_configuration(
             self._configuration_dict
@@ -43,20 +45,31 @@
         if log_config and isinstance(log_config, dict):
             log_config['version'] = log_config.get('version', 1)
             logging.config.dictConfig(log_config)
         for exporter_config in normalized_configuration.get('exporters', []):
             exporter = create_exporter(exporter_config)
             stats.stats.view_manager.register_exporter(exporter)
 
-        for ldap_server_config in normalized_configuration.get('ldap_servers'):
+        for ldap_server_config in normalized_configuration.get('ldap_servers', []):
             metric_set = self.generate_metric_set(ldap_server_config)
             self._metric_sets.append(metric_set)
 
-    @staticmethod
-    def generate_metric_set(ldap_server_config):
+        for base_dn, ldap_server_names in normalized_configuration.get('sync', {}).items():
+            ldap_servers = [
+                LdapServerPool().get_ldap_server(**server)
+                for server in normalized_configuration.get('ldap_servers', [])
+                if server['database'] in ldap_server_names
+            ]
+            sync_metric_set = SyncMetricSet(
+                base_dn=base_dn,
+                ldap_servers=ldap_servers
+            )
+            self._metric_sets.append(sync_metric_set)
+
+    def generate_metric_set(self, ldap_server_config):
         args = copy.deepcopy(ldap_server_config.get('connection', {}))
         args['database'] = ldap_server_config.get('database')
         ldap_server = LdapServerPool().get_ldap_server(**args)
         metric_set = MetricSet(ldap_server=ldap_server)
         configs = [ldap_server_config.get('object')]
         while configs:
             config = configs.pop()
@@ -68,23 +81,27 @@
                 name = config.get('metric_name')
                 attribute = config.get('attribute')
                 unit = config.get('unit')
                 description = config.get('description', '')
                 value_function = config.get('func', 'value')
                 query_dn = config.get('query_dn')
                 if dn and name and attribute and unit and query_dn:
-                    stat = LdapStatistic(
-                        dn=dn,
-                        name=name,
-                        attribute=attribute,
-                        description=description,
-                        unit=unit,
-                        value_function=value_function,
-                        query_dn=query_dn,
-                    )
+                    stat = self._ldap_metrics.get(name)
+                    if not stat:
+                        stat = LdapStatistic(
+                            dn=dn,
+                            name=name,
+                            attribute=attribute,
+                            description=description,
+                            unit=unit,
+                            value_function=value_function,
+                            query_dn=query_dn,
+                            tag_keys=['database']
+                        )
+                        self._ldap_metrics[name] = stat
                     metric_set.add_statistic(stat)
                 for key, value in config.items():
                     configs.insert(0, value)
         return metric_set
 
     def metric_sets(self):
         return self._metric_sets
```

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/ldap_metric_set.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_metric_set.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/ldap_server.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,17 @@
 
         try:
             if self._sasl_uri_scheme:
                 self.connection.sasl_external_bind_s()
             else:
                 self.connection.simple_bind_s(self.user_dn, self.user_password)
             return self.connection.search_s(dn, scope=scope, attrlist=attr_list)
-        except (ldap.SERVER_DOWN, ldap.NO_SUCH_OBJECT, ldap.TIMEOUT):
+        except (ldap.SERVER_DOWN, ldap.NO_SUCH_OBJECT, ldap.TIMEOUT) as error:
+            logging.error('Could not query LDAP:')
+            logging.exception(error)
             return []
 
     def query_dn_and_attribute(self, dn, attribute):
         results = self.query(dn, scope=ldap.SCOPE_BASE)
         if not results:
             return None
```

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats/ldap_statistic.py` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats/ldap_statistic.py`

 * *Files identical despite different names*

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/PKG-INFO` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openldap-opencensus-stats
-Version: 0.0.7
+Version: 0.0.8
 Summary: OpenLDAP OpenCensus Statistics
 Author: Mark Donnelly
 Author-email: mark@painless-security.com
 License: AGPL 3.0
 Keywords: openldap opencensus metrics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
```

### Comparing `openldap-opencensus-stats-0.0.7/openldap_opencensus_stats.egg-info/SOURCES.txt` & `openldap-opencensus-stats-0.0.8/openldap_opencensus_stats.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE
 README.md
+openldap-opencensus-stats.py
 setup.cfg
 setup.py
 openldap_opencensus_stats/__init__.py
 openldap_opencensus_stats/configuration.py
 openldap_opencensus_stats/ldap_metric_set.py
 openldap_opencensus_stats/ldap_server.py
 openldap_opencensus_stats/ldap_statistic.py
+openldap_opencensus_stats/ldap_sync_statistic.py
+openldap_opencensus_stats/sync_metric_set.py
 openldap_opencensus_stats.egg-info/PKG-INFO
 openldap_opencensus_stats.egg-info/SOURCES.txt
 openldap_opencensus_stats.egg-info/dependency_links.txt
-openldap_opencensus_stats.egg-info/entry_points.txt
 openldap_opencensus_stats.egg-info/requires.txt
 openldap_opencensus_stats.egg-info/top_level.txt
 openldap_opencensus_stats/config_transformers/__init__.py
 openldap_opencensus_stats/config_transformers/base.py
 openldap_opencensus_stats/config_transformers/child_object.py
 openldap_opencensus_stats/config_transformers/copy_for_each_database.py
 openldap_opencensus_stats/config_transformers/metric_dn.py
```

### Comparing `openldap-opencensus-stats-0.0.7/setup.py` & `openldap-opencensus-stats-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'OpenLDAP OpenCensus Statistics'
 LONG_DESCRIPTION = 'A package to gather statistics for OpenLDAP and publish via OpenCensus.'
 
 
 setup(
     name="openldap-opencensus-stats",
     version=VERSION,
@@ -19,19 +19,15 @@
         'opencensus-ext-stackdriver==0.8.0',
         'opencensus-ext-prometheus',
         'opencensus==0.10.0',
         'python-ldap',
         'pyyaml',
     ],
     keywords='openldap opencensus metrics',
-    entry_points={
-        'console_scripts': [
-            'openldap_opencensus_stats = openldap_opencensus_stats.openldap_opencensus_stats:main'
-        ]
-    },
+    scripts=['openldap-opencensus-stats.py'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: No Input/Output (Daemon)",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         "Programming Language :: Python :: 3",
```

