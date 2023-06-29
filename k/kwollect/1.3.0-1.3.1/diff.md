# Comparing `tmp/kwollect-1.3.0.tar.gz` & `tmp/kwollect-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwollect-1.3.0.tar", last modified: Tue Mar 28 07:12:25 2023, max compression
+gzip compressed data, was "kwollect-1.3.1.tar", last modified: Thu Jun 29 10:35:10 2023, max compression
```

## Comparing `kwollect-1.3.0.tar` & `kwollect-1.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.911564 kwollect-1.3.0/
--rw-r--r--   0 simfu     (1000) simfu     (1000)      218 2022-03-21 15:15:12.000000 kwollect-1.3.0/.gitignore
--rw-r--r--   0 simfu     (1000) simfu     (1000)     1490 2023-02-27 13:57:51.000000 kwollect-1.3.0/.gitlab-ci.yml
--rw-r--r--   0 simfu     (1000) simfu     (1000)     1102 2021-06-18 10:03:24.000000 kwollect-1.3.0/LICENSE.txt
--rw-r--r--   0 simfu     (1000) simfu     (1000)    15124 2023-03-28 07:12:25.911564 kwollect-1.3.0/PKG-INFO
--rw-r--r--   0 simfu     (1000) simfu     (1000)    14715 2022-03-21 15:15:12.000000 kwollect-1.3.0/README.md
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.907561 kwollect-1.3.0/debian/
--rw-r--r--   0 simfu     (1000) simfu     (1000)     7255 2023-03-28 07:07:05.000000 kwollect-1.3.0/debian/changelog
--rw-r--r--   0 simfu     (1000) simfu     (1000)        2 2021-07-23 13:49:03.000000 kwollect-1.3.0/debian/compat
--rw-r--r--   0 simfu     (1000) simfu     (1000)      473 2021-07-23 13:49:03.000000 kwollect-1.3.0/debian/control
--rw-r--r--   0 simfu     (1000) simfu     (1000)      248 2021-07-23 13:49:03.000000 kwollect-1.3.0/debian/kwollect.links
--rw-r--r--   0 simfu     (1000) simfu     (1000)      309 2021-07-23 13:49:03.000000 kwollect-1.3.0/debian/kwollect.triggers
--rw-r--r--   0 simfu     (1000) simfu     (1000)      168 2021-07-23 13:49:03.000000 kwollect-1.3.0/debian/kwollector.service
--rwxr-xr-x   0 simfu     (1000) simfu     (1000)      429 2022-03-21 15:15:12.000000 kwollect-1.3.0/debian/rules
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.907561 kwollect-1.3.0/devel/
--rw-r--r--   0 simfu     (1000) simfu     (1000)      798 2022-03-21 15:15:12.000000 kwollect-1.3.0/devel/README.md
--rw-r--r--   0 simfu     (1000) simfu     (1000)      458 2023-03-28 07:08:11.000000 kwollect-1.3.0/devel/Vagrantfile
--rwxr-xr-x   0 simfu     (1000) simfu     (1000)     3896 2023-03-28 07:08:11.000000 kwollect-1.3.0/devel/install.sh
--rwxr-xr-x   0 simfu     (1000) simfu     (1000)     3667 2023-03-27 14:35:01.000000 kwollect-1.3.0/devel/populate.sh
--rw-r--r--   0 simfu     (1000) simfu     (1000)     5358 2022-03-23 08:56:27.000000 kwollect-1.3.0/devel/test.py
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.907561 kwollect-1.3.0/kwollect/
--rw-r--r--   0 simfu     (1000) simfu     (1000)       22 2023-03-28 07:07:20.000000 kwollect-1.3.0/kwollect/__init__.py
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.911564 kwollect-1.3.0/kwollect/db/
--rw-r--r--   0 simfu     (1000) simfu     (1000)        1 2022-03-21 15:15:12.000000 kwollect-1.3.0/kwollect/db/__init__.py
--rw-r--r--   0 simfu     (1000) simfu     (1000)    16877 2023-03-28 07:08:11.000000 kwollect-1.3.0/kwollect/db/kwollect_setup_db.py
--rw-r--r--   0 simfu     (1000) simfu     (1000)     3321 2022-03-21 15:15:12.000000 kwollect-1.3.0/kwollect/db/kwollect_setup_db_oar.py
--rw-r--r--   0 simfu     (1000) simfu     (1000)    12503 2022-03-14 15:02:40.000000 kwollect-1.3.0/kwollect/db/old
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.911564 kwollect-1.3.0/kwollect/grafana/
--rw-r--r--   0 simfu     (1000) simfu     (1000)     7032 2023-03-28 07:08:11.000000 kwollect-1.3.0/kwollect/grafana/kwollect_dashboard.json
--rw-r--r--   0 simfu     (1000) simfu     (1000)    11430 2021-12-10 06:53:57.000000 kwollect-1.3.0/kwollect/grafana/kwollect_dashboard_new.json
--rw-r--r--   0 simfu     (1000) simfu     (1000)      828 2022-03-21 15:15:12.000000 kwollect-1.3.0/kwollect/grafana/kwollect_dashboardsource.yaml
--rw-r--r--   0 simfu     (1000) simfu     (1000)      345 2023-02-27 13:52:42.000000 kwollect-1.3.0/kwollect/grafana/postgres_datasource.yaml
--rwxr-xr-x   0 simfu     (1000) simfu     (1000)    24890 2022-03-21 15:15:12.000000 kwollect-1.3.0/kwollect/kwollector.py
--rwxr-xr-x   0 simfu     (1000) simfu     (1000)     8391 2022-05-03 10:38:11.000000 kwollect-1.3.0/kwollect/kwollector_wattmetre.py
-drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-03-28 07:12:25.907561 kwollect-1.3.0/kwollect.egg-info/
--rw-r--r--   0 simfu     (1000) simfu     (1000)    15124 2023-03-28 07:12:25.000000 kwollect-1.3.0/kwollect.egg-info/PKG-INFO
--rw-r--r--   0 simfu     (1000) simfu     (1000)      827 2023-03-28 07:12:25.000000 kwollect-1.3.0/kwollect.egg-info/SOURCES.txt
--rw-r--r--   0 simfu     (1000) simfu     (1000)        1 2023-03-28 07:12:25.000000 kwollect-1.3.0/kwollect.egg-info/dependency_links.txt
--rw-r--r--   0 simfu     (1000) simfu     (1000)      232 2023-03-28 07:12:25.000000 kwollect-1.3.0/kwollect.egg-info/entry_points.txt
--rw-r--r--   0 simfu     (1000) simfu     (1000)       76 2023-03-28 07:12:25.000000 kwollect-1.3.0/kwollect.egg-info/requires.txt
--rw-r--r--   0 simfu     (1000) simfu     (1000)        9 2023-03-28 07:12:25.000000 kwollect-1.3.0/kwollect.egg-info/top_level.txt
--rw-r--r--   0 simfu     (1000) simfu     (1000)       38 2023-03-28 07:12:25.911564 kwollect-1.3.0/setup.cfg
--rw-r--r--   0 simfu     (1000) simfu     (1000)     1454 2022-03-21 15:15:12.000000 kwollect-1.3.0/setup.py
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.007759 kwollect-1.3.1/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      218 2022-03-21 15:15:12.000000 kwollect-1.3.1/.gitignore
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     1490 2023-02-27 13:57:51.000000 kwollect-1.3.1/.gitlab-ci.yml
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     1102 2021-06-18 10:03:24.000000 kwollect-1.3.1/LICENSE.txt
+-rw-r--r--   0 simfu     (1000) simfu     (1000)    15124 2023-06-29 10:35:10.007759 kwollect-1.3.1/PKG-INFO
+-rw-r--r--   0 simfu     (1000) simfu     (1000)    14715 2022-03-21 15:15:12.000000 kwollect-1.3.1/README.md
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.003759 kwollect-1.3.1/debian/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     7534 2023-06-29 10:34:00.000000 kwollect-1.3.1/debian/changelog
+-rw-r--r--   0 simfu     (1000) simfu     (1000)        2 2021-07-23 13:49:03.000000 kwollect-1.3.1/debian/compat
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      473 2021-07-23 13:49:03.000000 kwollect-1.3.1/debian/control
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      248 2021-07-23 13:49:03.000000 kwollect-1.3.1/debian/kwollect.links
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      309 2021-07-23 13:49:03.000000 kwollect-1.3.1/debian/kwollect.triggers
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      168 2021-07-23 13:49:03.000000 kwollect-1.3.1/debian/kwollector.service
+-rwxr-xr-x   0 simfu     (1000) simfu     (1000)      429 2022-03-21 15:15:12.000000 kwollect-1.3.1/debian/rules
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.007759 kwollect-1.3.1/devel/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      798 2022-03-21 15:15:12.000000 kwollect-1.3.1/devel/README.md
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      540 2023-03-28 07:43:30.000000 kwollect-1.3.1/devel/Vagrantfile
+-rwxr-xr-x   0 simfu     (1000) simfu     (1000)     4111 2023-03-28 07:43:30.000000 kwollect-1.3.1/devel/install.sh
+-rwxr-xr-x   0 simfu     (1000) simfu     (1000)     3667 2023-03-27 14:35:01.000000 kwollect-1.3.1/devel/populate.sh
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     5358 2022-03-23 08:56:27.000000 kwollect-1.3.1/devel/test.py
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.007759 kwollect-1.3.1/kwollect/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)       22 2023-06-29 10:32:32.000000 kwollect-1.3.1/kwollect/__init__.py
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.007759 kwollect-1.3.1/kwollect/db/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)        1 2022-03-21 15:15:12.000000 kwollect-1.3.1/kwollect/db/__init__.py
+-rw-r--r--   0 simfu     (1000) simfu     (1000)    16981 2023-04-05 12:34:42.000000 kwollect-1.3.1/kwollect/db/kwollect_setup_db.py
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     3321 2022-03-21 15:15:12.000000 kwollect-1.3.1/kwollect/db/kwollect_setup_db_oar.py
+-rw-r--r--   0 simfu     (1000) simfu     (1000)    12503 2022-03-14 15:02:40.000000 kwollect-1.3.1/kwollect/db/old
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.007759 kwollect-1.3.1/kwollect/grafana/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     7032 2023-06-29 08:48:33.000000 kwollect-1.3.1/kwollect/grafana/kwollect_dashboard.json
+-rw-r--r--   0 simfu     (1000) simfu     (1000)    11430 2021-12-10 06:53:57.000000 kwollect-1.3.1/kwollect/grafana/kwollect_dashboard_new.json
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      828 2022-03-21 15:15:12.000000 kwollect-1.3.1/kwollect/grafana/kwollect_dashboardsource.yaml
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      345 2023-02-27 13:52:42.000000 kwollect-1.3.1/kwollect/grafana/postgres_datasource.yaml
+-rwxr-xr-x   0 simfu     (1000) simfu     (1000)    24892 2023-06-20 11:20:46.000000 kwollect-1.3.1/kwollect/kwollector.py
+-rwxr-xr-x   0 simfu     (1000) simfu     (1000)     8391 2022-05-03 10:38:11.000000 kwollect-1.3.1/kwollect/kwollector_wattmetre.py
+drwxr-xr-x   0 simfu     (1000) simfu     (1000)        0 2023-06-29 10:35:10.007759 kwollect-1.3.1/kwollect.egg-info/
+-rw-r--r--   0 simfu     (1000) simfu     (1000)    15124 2023-06-29 10:35:09.000000 kwollect-1.3.1/kwollect.egg-info/PKG-INFO
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      827 2023-06-29 10:35:09.000000 kwollect-1.3.1/kwollect.egg-info/SOURCES.txt
+-rw-r--r--   0 simfu     (1000) simfu     (1000)        1 2023-06-29 10:35:09.000000 kwollect-1.3.1/kwollect.egg-info/dependency_links.txt
+-rw-r--r--   0 simfu     (1000) simfu     (1000)      232 2023-06-29 10:35:09.000000 kwollect-1.3.1/kwollect.egg-info/entry_points.txt
+-rw-r--r--   0 simfu     (1000) simfu     (1000)       76 2023-06-29 10:35:09.000000 kwollect-1.3.1/kwollect.egg-info/requires.txt
+-rw-r--r--   0 simfu     (1000) simfu     (1000)        9 2023-06-29 10:35:09.000000 kwollect-1.3.1/kwollect.egg-info/top_level.txt
+-rw-r--r--   0 simfu     (1000) simfu     (1000)       38 2023-06-29 10:35:10.007759 kwollect-1.3.1/setup.cfg
+-rw-r--r--   0 simfu     (1000) simfu     (1000)     1454 2022-03-21 15:15:12.000000 kwollect-1.3.1/setup.py
```

### Comparing `kwollect-1.3.0/.gitlab-ci.yml` & `kwollect-1.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/LICENSE.txt` & `kwollect-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/PKG-INFO` & `kwollect-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwollect
-Version: 1.3.0
+Version: 1.3.1
 Summary: Kwollect framework for metrics collection
 Home-page: https://gitlab.inria.fr/delamare/kwollect
 Author: Simon Delamare
 Author-email: simon.delamare@ens-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `kwollect-1.3.0/README.md` & `kwollect-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/debian/changelog` & `kwollect-1.3.1/debian/changelog`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+kwollect (1.3.1) unstable; urgency=medium
+
+  * db: update move_chunk_to_archive to not reorder index
+  * db: order metric output from api.available_metrics
+  * db: enable compression on metrics_summary and change policy scheduling
+  * kwollector: Use more IPMI worker processes
+
 kwollect (1.3.0) unstable; urgency=medium
 
   * db: Fix as_rate calculation in get_metrics function
   * db: Fix summarized aggregation for counters metrics
   * kwollector_wattmetre: make v3 parsing more robust
   * ci: fix g5k-deploy-files options
   * grafana: update datasource for PG 12+ and recent grafana versions
```

### Comparing `kwollect-1.3.0/devel/README.md` & `kwollect-1.3.1/devel/README.md`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/devel/install.sh` & `kwollect-1.3.1/devel/install.sh`

 * *Files 16% similar despite different names*

```diff
@@ -14,30 +14,34 @@
 # apt install -y kwollect
 apt install -y --no-install-recommends python3-pip python3-setuptools python3-yarl
 pip3 install -U pip
 pip3 install -e /vagrant
 cat /vagrant/debian/kwollector.service | sed 's,bin/kwollector,local/bin/kwollector,g' > /etc/systemd/system/kwollector.service
 
 # Database
+pg_dropcluster --stop 13 main || true
+pg_createcluster 13 main
+systemctl restart postgresql
+
 wget --quiet -O - https://packagecloud.io/timescale/timescaledb/gpgkey | apt-key add -
 echo 'deb https://packagecloud.io/timescale/timescaledb/debian/ bullseye main' > /etc/apt/sources.list.d/timescaledb.list
 apt update
-apt-get install -y --no-install-recommends postgresql postgresql-client libpq-dev timescaledb-2-postgresql-13 timescaledb-tools postgresql-plpython3-13
+apt-get install -y --no-install-recommends postgresql postgresql-client libpq-dev timescaledb-2-postgresql-13 timescaledb-toolkit-postgresql-13 timescaledb-tools postgresql-plpython3-13
 
 ## TimescaleDB comes with a script to tune Postgres configuration that you might want to use:
 cp /etc/postgresql/13/main/postgresql.conf /etc/postgresql/13/main/postgresql.conf-timescaledb_tune.backup
 timescaledb-tune -yes -quiet
 echo 'timescaledb.telemetry_level=off' >> /etc/postgresql/13/main/postgresql.conf
 
 sed -i 's/max_connections.*/max_connections = 1000/g' /etc/postgresql/13/main/postgresql.conf
 
 systemctl restart postgresql
 
 # API
-wget -q https://github.com/PostgREST/postgrest/releases/download/v8.0.0/postgrest-v8.0.0-linux-x64-static.tar.xz -O /tmp/postgrest.txz
+[ -f /tmp/postgrest.txz ] || wget -q -O /tmp/postgrest.txz https://github.com/PostgREST/postgrest/releases/download/v10.1.2/postgrest-v10.1.2-linux-static-x64.tar.xz
 cd /tmp
 tar xf postgrest.txz
 chmod +x ./postgrest
 mv ./postgrest /usr/local/bin/
 
 cat > /etc/postgrest.conf << EOF
 db-uri = "postgres://kwuser:changeme@localhost/kwdb"
@@ -90,32 +94,34 @@
 - name: snmp_template
   device_id: local
   url: snmp://public@127.0.0.1/1.3.6.1.2.1.1.9.1.4.{{ 1.3.6.1.2.1.1.9.1.3 == The SNMP Management Architecture MIB. }}
   update_every: 5000
 
 - name: prom_default_metric
   device_id: local
-  url: prometheus://localhost:9100/node_load1-node_load5-node_load15
+  url: prometheus://localhost:9100/node_load1-node_load5-node_load15-node_cpu_total
   update_every: 15000
 
 - name: prom_all_metrics
   device_id: local
   url: prometheus://localhost:9100/
   update_every: 15000
   optional: true
 EOF
 
 apt install -y --no-install-recommends prometheus-node-exporter snmpd
 systemctl enable kwollector
 
 
 # Grafana
+
+
 apt-get install -y --no-install-recommends apt-transport-https software-properties-common wget
-echo "deb https://packages.grafana.com/oss/deb stable main" > /etc/apt/sources.list.d/grafana.list
-wget -q -O - https://packages.grafana.com/gpg.key | apt-key add -
+wget -q -O /usr/share/keyrings/grafana.key https://apt.grafana.com/gpg.key
+echo "deb [signed-by=/usr/share/keyrings/grafana.key] https://apt.grafana.com stable main" > /etc/apt/sources.list.d/grafana.list
 apt-get update
 apt-get install grafana
 
 sed -i 's/.*http_port.*/http_port = 3003/g' /etc/grafana/grafana.ini
 cp /vagrant/kwollect/grafana/postgres_datasource.yaml /etc/grafana/provisioning/datasources/postgres.yaml
 cp /vagrant/kwollect/grafana/kwollect_dashboardsource.yaml /etc/grafana/provisioning/dashboards/kwollect.yaml
 mkdir -p /etc/grafana/kwollect_dashboard
```

### Comparing `kwollect-1.3.0/devel/populate.sh` & `kwollect-1.3.1/devel/populate.sh`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/devel/test.py` & `kwollect-1.3.1/devel/test.py`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/kwollect/db/kwollect_setup_db.py` & `kwollect-1.3.1/kwollect/db/kwollect_setup_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 sql_conn.autocommit = True
 sql_cur = sql_conn.cursor()
 
 print("Creating or updating database schema...")
 cmd = f"""
 SET LOCAL SESSION AUTHORIZATION DEFAULT;
 CREATE EXTENSION IF NOT EXISTS timescaledb CASCADE;
+CREATE EXTENSION IF NOT EXISTS timescaledb_toolkit;
 
 SET LOCAL SESSION AUTHORIZATION {kwollect_user};
 
 ALTER DEFAULT PRIVILEGES IN SCHEMA public GRANT SELECT ON TABLES TO {kwollect_user}_ro;
 ALTER DEFAULT PRIVILEGES IN SCHEMA _timescaledb_internal GRANT SELECT ON TABLES TO {kwollect_user}_ro;
 
 CREATE TABLE IF NOT EXISTS metrics (
@@ -142,18 +143,29 @@
     CASE WHEN metrics.metric_id ~ '_total$' THEN MAX(value) ELSE AVG(value) END AS value,
     labels - '_metric_scrape_time' AS labels
   FROM metrics
   GROUP BY time_bucket(INTERVAL '5 minute', timestamp), device_id, metric_id, labels - '_metric_scrape_time'
   WITH NO DATA;
 
 SELECT add_continuous_aggregate_policy('metrics_summary',
-    start_offset => INTERVAL '1 day',
+    start_offset => INTERVAL '12 hour',
     end_offset => INTERVAL '10 minute',
-    schedule_interval => INTERVAL '1 minute',
+    schedule_interval => INTERVAL '5 minute',
     if_not_exists => true);
+
+DO $$
+BEGIN
+  BEGIN ALTER MATERIALIZED VIEW metrics_summary SET (
+      timescaledb.compress
+      );
+  EXCEPTION WHEN OTHERS THEN RAISE NOTICE 'Compression already enabled';
+  END;
+END $$;
+SELECT add_compression_policy('metrics_summary', INTERVAL '2 day', if_not_exists => true);
+
 """
 sql(cmd)
 
 for suffix in ['', '_summary']:
   cmd = f"""
 SET LOCAL SESSION AUTHORIZATION {kwollect_user};
 CREATE OR REPLACE VIEW metrics_by_device{suffix} AS
@@ -263,36 +275,31 @@
     (tsi.chunk_tablespace IS NULL OR tsi.chunk_tablespace != destination)
   LOOP
     RAISE LOG 'Moving chunk: %', chunk::text;
     EXECUTE format('
       SELECT move_chunk(
         chunk => ''%s'',
         destination_tablespace => ''%I'',
-        index_destination_tablespace => ''%I'',
-        reorder_index => (
-          SELECT CONCAT(materialization_hypertable_schema, ''.'', materialization_hypertable_name, ''_device_id_timestamp_idx'')
-          FROM timescaledb_information.continuous_aggregates
-          WHERE view_name = ''%I''
-          )
-        )', chunk, destination, destination, ht);
+        index_destination_tablespace => ''%I''
+      )', chunk, destination, destination);
   END LOOP;
 END
 $$;
 
 DO $$
   DECLARE j record;
 BEGIN
   FOR j IN SELECT job_id FROM timescaledb_information.jobs WHERE proc_name = 'move_chunks_to_archive'
     LOOP PERFORM delete_job(j.job_id);
   END LOOP;
 END
 $$;
 SELECT add_job(
   'move_chunks_to_archive', '1d',
-  config => '{"hypertable":"metrics_summary", "lag":"14d", "tablespace":"archive"}',
+  config => '{"hypertable":"metrics_summary", "lag":"8d", "tablespace":"archive"}',
   initial_start => CURRENT_DATE + TIME '23:59:59' AT TIME ZONE current_setting('TIMEZONE')
   );
 """
     sql(cmd)
 
 cmd = f"""
 SET LOCAL SESSION AUTHORIZATION default;
@@ -442,14 +449,15 @@
 ordered_metrics AS (
   SELECT DISTINCT ON (idx1, idx2, idx3, metric_id)
     metrics.device_id, metrics.metric_id,
     CASE WHEN metrics.device_id ~ '^[a-z]+-\d+$' THEN '1' ELSE '2' END AS idx1,
     (STRING_TO_ARRAY(metrics.device_id, '-'))[1] AS idx2,
     COALESCE(SUBSTRING((STRING_TO_ARRAY(metrics.device_id, '-'))[2] FROM '([0-9]+)')::INTEGER, 0) as idx3
   FROM av_metrics AS metrics
+  ORDER BY idx1, idx2, idx3, metric_id
 )
 SELECT m.device_id, m.metric_id FROM ordered_metrics AS m;
 END;
 $$ LANGUAGE plpgsql IMMUTABLE;
 
 
 CREATE OR REPLACE FUNCTION api.insert_metrics(
```

### Comparing `kwollect-1.3.0/kwollect/db/kwollect_setup_db_oar.py` & `kwollect-1.3.1/kwollect/db/kwollect_setup_db_oar.py`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/kwollect/db/old` & `kwollect-1.3.1/kwollect/db/old`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/kwollect/grafana/kwollect_dashboard.json` & `kwollect-1.3.1/kwollect/grafana/kwollect_dashboard.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999007936507937%*

 * *Differences: {"'templating'": "{'list': {2: {'sort': 1}}}"}*

```diff
@@ -218,15 +218,15 @@
                 "multi": true,
                 "name": "metric_id",
                 "options": [],
                 "query": "SELECT DISTINCT metric_id FROM api.available_metrics(at => to_timestamp($__unixEpochTo()), params => '{\"devices\": [${device_id:doublequote}], \"job_id\": \"$job_str\"}') WHERE CASE WHEN '${device_id:raw}' = '' OR '${device_id:raw}' = 'Select...' THEN FALSE ELSE TRUE END",
                 "refresh": 1,
                 "regex": "",
                 "skipUrlSync": false,
-                "sort": 0,
+                "sort": 1,
                 "tagValuesQuery": "",
                 "tags": [],
                 "tagsQuery": "",
                 "type": "query",
                 "useTags": false
             }
         ]
```

### Comparing `kwollect-1.3.0/kwollect/grafana/kwollect_dashboard_new.json` & `kwollect-1.3.1/kwollect/grafana/kwollect_dashboard_new.json`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/kwollect/grafana/kwollect_dashboardsource.yaml` & `kwollect-1.3.1/kwollect/grafana/kwollect_dashboardsource.yaml`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/kwollect/kwollector.py` & `kwollect-1.3.1/kwollect/kwollector.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,15 +705,15 @@
 
 
 ipmi_executor = None
 
 
 def init_ipmi():
     global ipmi_executor
-    ipmi_executor = concurrent.futures.ProcessPoolExecutor(max_workers=config["worker"])
+    ipmi_executor = concurrent.futures.ProcessPoolExecutor(max_workers=4*config["worker"])
 
 
 async def make_snmp_request(
     host, snmp_command, oids, community="public", timeout=30, retries=1
 ):
     """aiosnmp glue"""
     try:
```

### Comparing `kwollect-1.3.0/kwollect/kwollector_wattmetre.py` & `kwollect-1.3.1/kwollect/kwollector_wattmetre.py`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/kwollect.egg-info/PKG-INFO` & `kwollect-1.3.1/kwollect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwollect
-Version: 1.3.0
+Version: 1.3.1
 Summary: Kwollect framework for metrics collection
 Home-page: https://gitlab.inria.fr/delamare/kwollect
 Author: Simon Delamare
 Author-email: simon.delamare@ens-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `kwollect-1.3.0/kwollect.egg-info/SOURCES.txt` & `kwollect-1.3.1/kwollect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwollect-1.3.0/setup.py` & `kwollect-1.3.1/setup.py`

 * *Files identical despite different names*

