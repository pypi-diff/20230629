# Comparing `tmp/openmldb_tool-0.7.3-py3-none-any.whl.zip` & `tmp/openmldb_tool-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,18 @@
-Zip file size: 26350 bytes, number of entries: 20
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-22 12:33 diagnostic_tool/__init__.py
--rw-r--r--  2.0 unx     9672 b- defN 23-Mar-22 12:33 diagnostic_tool/collector.py
--rw-r--r--  2.0 unx    11416 b- defN 23-Mar-22 12:33 diagnostic_tool/conf_validator.py
--rw-r--r--  2.0 unx     2027 b- defN 23-Mar-22 12:33 diagnostic_tool/connector.py
--rw-r--r--  2.0 unx     9598 b- defN 23-Mar-22 12:33 diagnostic_tool/diagnose.py
--rw-r--r--  2.0 unx     9205 b- defN 23-Mar-22 12:33 diagnostic_tool/dist_conf.py
--rw-r--r--  2.0 unx     4958 b- defN 23-Mar-22 12:33 diagnostic_tool/log_analyzer.py
--rw-r--r--  2.0 unx     5466 b- defN 23-Mar-22 12:33 diagnostic_tool/server_checker.py
--rw-r--r--  2.0 unx     3042 b- defN 23-Mar-22 12:33 diagnostic_tool/util.py
--rw-r--r--  2.0 unx      571 b- defN 23-Mar-22 12:33 tests/__init__.py
--rw-r--r--  2.0 unx      705 b- defN 23-Mar-22 12:33 tests/case_conf.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Mar-22 12:33 tests/cmd_test.py
--rw-r--r--  2.0 unx     1274 b- defN 23-Mar-22 12:33 tests/conf_validator_test.py
--rw-r--r--  2.0 unx     2005 b- defN 23-Mar-22 12:33 tests/dist_conf_test.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Mar-22 12:33 tests/static_check_test.py
--rw-r--r--  2.0 unx      440 b- defN 23-Mar-22 12:47 openmldb_tool-0.7.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-22 12:47 openmldb_tool-0.7.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-22 12:47 openmldb_tool-0.7.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Mar-22 12:47 openmldb_tool-0.7.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1662 b- defN 23-Mar-22 12:47 openmldb_tool-0.7.3.dist-info/RECORD
-20 files, 68355 bytes uncompressed, 23638 bytes compressed:  65.4%
+Zip file size: 25497 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      571 b- defN 23-Jun-15 09:19 diagnostic_tool/__init__.py
+-rw-r--r--  2.0 unx     9672 b- defN 23-Jun-15 09:19 diagnostic_tool/collector.py
+-rw-r--r--  2.0 unx    11416 b- defN 23-Jun-15 09:19 diagnostic_tool/conf_validator.py
+-rw-r--r--  2.0 unx     2027 b- defN 23-Jun-15 09:19 diagnostic_tool/connector.py
+-rw-r--r--  2.0 unx    12128 b- defN 23-Jun-16 09:47 diagnostic_tool/diagnose.py
+-rw-r--r--  2.0 unx     9205 b- defN 23-Jun-15 09:19 diagnostic_tool/dist_conf.py
+-rw-r--r--  2.0 unx     4958 b- defN 23-Jun-15 09:19 diagnostic_tool/log_analyzer.py
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-16 09:47 diagnostic_tool/parser.py
+-rw-r--r--  2.0 unx     7914 b- defN 23-Jun-15 09:19 diagnostic_tool/server_checker.py
+-rw-r--r--  2.0 unx     5153 b- defN 23-Jun-16 09:47 diagnostic_tool/table_checker.py
+-rw-r--r--  2.0 unx     3042 b- defN 23-Jun-15 09:19 diagnostic_tool/util.py
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1365 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/RECORD
+16 files, 70771 bytes uncompressed, 23233 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -15,47 +15,35 @@
 
 Filename: diagnostic_tool/dist_conf.py
 Comment: 
 
 Filename: diagnostic_tool/log_analyzer.py
 Comment: 
 
-Filename: diagnostic_tool/server_checker.py
-Comment: 
-
-Filename: diagnostic_tool/util.py
-Comment: 
-
-Filename: tests/__init__.py
+Filename: diagnostic_tool/parser.py
 Comment: 
 
-Filename: tests/case_conf.py
-Comment: 
-
-Filename: tests/cmd_test.py
-Comment: 
-
-Filename: tests/conf_validator_test.py
+Filename: diagnostic_tool/server_checker.py
 Comment: 
 
-Filename: tests/dist_conf_test.py
+Filename: diagnostic_tool/table_checker.py
 Comment: 
 
-Filename: tests/static_check_test.py
+Filename: diagnostic_tool/util.py
 Comment: 
 
-Filename: openmldb_tool-0.7.3.dist-info/METADATA
+Filename: openmldb_tool-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: openmldb_tool-0.7.3.dist-info/WHEEL
+Filename: openmldb_tool-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: openmldb_tool-0.7.3.dist-info/entry_points.txt
+Filename: openmldb_tool-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: openmldb_tool-0.7.3.dist-info/top_level.txt
+Filename: openmldb_tool-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: openmldb_tool-0.7.3.dist-info/RECORD
+Filename: openmldb_tool-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## diagnostic_tool/diagnose.py

```diff
@@ -11,24 +11,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
+import os
 import textwrap
+import time
+
 from diagnostic_tool.connector import Connector
 from diagnostic_tool.dist_conf import read_conf
 from diagnostic_tool.conf_validator import (
     DistConfValidator,
     ClusterConfValidator,
 )
 from diagnostic_tool.log_analyzer import LogAnalyzer
 from diagnostic_tool.collector import Collector
 import diagnostic_tool.server_checker as checker
+from diagnostic_tool.table_checker import TableChecker
+from diagnostic_tool.parser import LogParser
 
 from absl import app
 from absl import flags
 from absl.flags import argparse_flags
 from absl import logging  # --verbosity --log_dir
 
 # only some sub cmd needs dist file
@@ -39,14 +44,19 @@
     short_name="f",
 )
 flags.DEFINE_bool(
     "local",
     False,
     "If set, all server in config file will be treated as local server, skip ssh.",
 )
+flags.DEFINE_string(
+    "db",
+    "",
+    "Specify databases to diagnose, split by ','. Only used in inspect online.",
+)
 
 flags.DEFINE_string("collect_dir", "/tmp/diag_collect", "...")
 
 
 def check_version(version_map: dict):
     # cluster must have nameserver, so we use nameserver version to be the right version
     version = version_map["nameserver"][0][1]
@@ -59,30 +69,34 @@
                 )
                 flag = False
     return version, flag
 
 
 def status(args):
     """use OpenMLDB Python SDK to connect OpenMLDB"""
-    conn = Connector()
-    status_checker = checker.StatusChecker(conn)
-    assert status_checker.check_components(), "some components is offline"
+    connect = Connector()
+    status_checker = checker.StatusChecker(connect)
+    if not status_checker.check_components():
+        print("some components is offline")
 
     # --diff with dist conf file, conf_file is required
     if args.diff:
         assert flags.FLAGS.conf_file, "need --conf_file"
         print(
             "only check components in conf file, if cluster has more components, ignore them"
         )
         dist_conf = read_conf(flags.FLAGS.conf_file)
         assert status_checker.check_startup(
             dist_conf
         ), f"not all components in conf file are online, check the previous output"
         print(f"all components in conf file are online")
 
+    if args.conn:
+        status_checker.check_connection()
+
 
 def inspect(args):
     insepct_online(args)
     inspect_offline(args)
 
 
 def insepct_online(args):
@@ -96,42 +110,73 @@
     for t in rs:
         if t[13]:
             print(f"unhealthy table {t[2]}.{t[1]}:\n {t[:13]}")
             # sqlalchemy truncated ref https://github.com/sqlalchemy/sqlalchemy/commit/591e0cf08a798fb16e0ee9b56df5c3141aa48959
             # so we print warnings alone
             print(f"full warnings:\n{t[13]}")
             fails.append(f"{t[2]}.{t[1]}")
-    
+
     assert not fails, f"unhealthy tables: {fails}"
     print(f"all tables are healthy")
 
+    if getattr(args, 'dist', False):
+        table_checker = TableChecker(conn)
+        table_checker.check_distribution(dbs=flags.FLAGS.db.split(","))
+
 
 def inspect_offline(args):
     """scan jobs status, show job log if failed"""
+    final_failed = ["failed", "killed", "lost"]
+    total, num, jobs = _get_jobs(final_failed)
+    # TODO some failed jobs are known, what if we want skip them?
+    print(f"inspect {total} offline jobs")
+    if num:
+        failed_jobs_str = "\n".join(jobs)
+        raise AssertionError(f"{num} offline final jobs are failed\nfailed jobs:\n{failed_jobs_str}")
+    print("all offline final jobs are finished")
+
+
+def _get_jobs(states=None):
     assert checker.StatusChecker(Connector()).offline_support()
     conn = Connector()
     jobs = conn.execfetch("SHOW JOBS")
-    # TODO some failed jobs are known, what if we want skip them?
-    print(f"inspect {len(jobs)} offline jobs")
-    fails = []
+    total_num = len(jobs)
     # jobs sorted by id
     jobs.sort(key=lambda x: x[0])
-    # only FINAL_STATE "finished", "failed", "killed", "lost"
-    final_failed = ["failed", "killed", "lost"]
-    for row in jobs:
-        if row[2].lower() in final_failed:
-            fails.append(" ".join([str(x) for x in row]))
-            # DO NOT try to print rs in execfetch, it's too long
-            std_output = conn.execfetch(f"SHOW JOBLOG {row[0]}")
-            # log rs schema is FORMAT_STRING_KEY
-            assert len(std_output) == 1 and len(std_output[0]) == 1
-            print(f"{row[0]}-{row[1]} failed, job log:\n{std_output[0][0]}")
-    fails_total = "\n".join(fails)
-    assert not fails, f"failed jobs:\n{fails_total}"
-    print("all offline final jobs are finished")
+    show_jobs = [_format_job_row(row) for row in jobs if not states or row[2].lower() in states]
+    return total_num, len(show_jobs), show_jobs
+
+
+def _format_job_row(row):
+    row = list(row)
+    row[3] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(row[3] / 1000))
+    row[4] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(row[4] / 1000))
+    return " ".join(map(str, row))
+
+
+def inspect_job(args):
+    if not args.id:
+        states = args.state.split(",") if args.state != "all" else None
+        total, num, jobs = _get_jobs(states)
+        print(f"inspect {total} offline jobs")
+        if args.state != "all":
+            print(f"{num} {args.state} jobs")
+        print(*jobs, sep="\n")
+        return
+    conn = Connector()
+    std_output = conn.execfetch(f"SHOW JOBLOG {args.id}")
+    assert len(std_output) == 1 and len(std_output[0]) == 1
+    detailed_log = std_output[0][0]
+    if args.detail:
+        print(detailed_log)
+    else:
+        parser = LogParser()
+        if args.conf_update or not os.path.exists(parser.conf_file):
+            parser.update_conf_file(args.conf_url)
+        parser.parse_log(detailed_log)
 
 
 def test_sql(args):
     conn = Connector()
     status_checker = checker.StatusChecker(conn)
     if not status_checker.check_components():
         logging.warning("some server is unalive, be careful")
@@ -190,32 +235,69 @@
         "status", help="check the OpenMLDB server status"
     )
     status_parser.add_argument(
         "--diff",
         action="store_true",
         help="check if all endpoints in conf are in cluster. If set, need to set `--conf_file`",
     )  # TODO action support in all python 3.x?
+    status_parser.add_argument(
+        "--conn",
+        action="store_true",
+        help="check network connection of all servers",
+    )
     status_parser.set_defaults(command=status)
 
     # sub inspect
     inspect_parser = subparsers.add_parser(
         "inspect",
         help="Inspect online and offline. Use `inspect [online/offline]` to inspect one.",
     )
     # inspect online & offline
     inspect_parser.set_defaults(command=inspect)
     inspect_sub = inspect_parser.add_subparsers()
     # inspect online
-    online = inspect_sub.add_parser("online", help="only inspect online table")
+    online = inspect_sub.add_parser("online", help="only inspect online table.")
     online.set_defaults(command=insepct_online)
+    online.add_argument(
+        "--dist",
+        action="store_true",
+        help="Inspect online distribution."
+    )
     # inspect offline
     offline = inspect_sub.add_parser(
-        "offline", help="only inspect offline jobs, check the job log"
+        "offline", help="only inspect offline jobs."
     )
     offline.set_defaults(command=inspect_offline)
+    # inspect job
+    ins_job = inspect_sub.add_parser("job", help="show jobs by state, show joblog or parse joblog by id.")
+    ins_job.set_defaults(command=inspect_job)
+    ins_job.add_argument(
+        "--state",
+        default="all",
+        help="Specify which state offline jobs, split by ','"
+    )
+    ins_job.add_argument(
+        "--id",
+        help="inspect joblog by id"
+    )
+    ins_job.add_argument(
+        "--detail",
+        action="store_true",
+        help="show detailed joblog information, use with `--id`"
+    )
+    ins_job.add_argument(
+        "--conf-url",
+        default="https://raw.githubusercontent.com/4paradigm/OpenMLDB/main/python/openmldb_tool/diagnostic_tool/common_err.yml",
+        help="url used to update the log parser configuration. If downloading is slow, you can try mirror source 'https://openmldb.ai/download/diag/common_err.yml'"
+    )
+    ins_job.add_argument(
+        "--conf-update",
+        action="store_true",
+        help="update the log parser configuration"
+    )
 
     # sub test
     test_parser = subparsers.add_parser(
         "test",
         help="Do simple create&insert&select test in online, select in offline(if taskmanager exists)",
     )
     test_parser.set_defaults(command=test_sql)
```

## diagnostic_tool/server_checker.py

```diff
@@ -12,14 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from absl import flags
 from absl import logging
+from prettytable import PrettyTable
+import re
+import requests
 import time
 
 from .connector import Connector
 from .dist_conf import DistConf, COMPONENT_ROLES, ServerInfo
 
 # rename to checker?
 
@@ -29,14 +32,66 @@
         self.conn = conn
 
     def check_components(self):
         """ensure all components in cluster is online"""
         components_map = self._get_components(show=True)
         return self._check_status(components_map)
 
+    def check_connection(self):
+        """check all compontents connections"""
+        component_map = self._get_components(show=False)
+        t = PrettyTable()
+        t.title = "Connections"
+        t.field_names = ["Endpoint", "Version", "Cost_time", "Extra"]
+        err = ""
+        taskmanager = component_map.pop("taskmanager")  # extract taskmanager
+        other_components = [component for role in component_map.values() for component in role]  # extract other components
+        for (endpoint, _) in other_components:
+            version, response_time, ex, e = self._get_information(endpoint)
+            t.add_row([endpoint, version, response_time, ex])
+            err += e
+        for (endpoint, _) in taskmanager:
+            version, response_time, ex, e = self._get_information_taskmanager(endpoint)
+            t.add_row([endpoint, version, response_time, ex])
+            err += e
+        print(t)
+        if err:
+            print(err)
+
+    def _get_information(self, endpoint):
+        """get informations from components except taskmanager"""
+        try:
+            response = requests.get(f"http://{endpoint}/status", timeout=1)  # the connection timeout is 1 second
+            response.raise_for_status()
+        except Exception as e:
+            err = endpoint + "\n" + str(e) + "\n"
+            return "-", "timeout", "Error: See below", err
+        text = response.text
+        regex = re.compile("version: (.*?)\\n")
+        match = re.search(regex, text)
+        version = match.group(1)
+        ex = ""
+        response_time = str(response.elapsed.microseconds / 1000) + "ms"
+        return version, response_time, ex, ""
+
+    def _get_information_taskmanager(self, endpoint):
+        """get informations from taskmanager"""
+        try:
+            response = requests.post(f"http://{endpoint}/openmldb.taskmanager.TaskManagerServer/GetVersion", json={})
+            response.raise_for_status()
+        except Exception as e:
+            err = endpoint + "\n" + str(e) + "\n"
+            return "-", "timeout", "Error: See below", err
+        js = response.json()
+        version = js["taskmanagerVersion"]
+        ex = "batchVersion: " + js["batchVersion"][:-1]
+        response = requests.get(f"http://{endpoint}", timeout=1)
+        response_time = str(response.elapsed.microseconds / 1000) + "ms"
+        return version, response_time, ex, ""
+
     def offline_support(self):
         """True if have taskmanager, else False"""
         components_map = self._get_components(show=False)
         return "taskmanager" in components_map
 
     def _get_components(self, show=False):
         component_list = self.conn.execfetch("SHOW COMPONENTS", show=show)
```

## Comparing `openmldb_tool-0.7.3.dist-info/RECORD` & `openmldb_tool-0.8.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 diagnostic_tool/__init__.py,sha256=N0qwVVP92fAXFf_K7yoDGR-CK-YMuLzWeeKVnB5G9OE,571
 diagnostic_tool/collector.py,sha256=atUlOcIiBo5EqD64W80LXyh3AMeLqySO2Fl-mN50I2E,9672
 diagnostic_tool/conf_validator.py,sha256=TzAi5SYeHxsP6zkG5hZM5PXT3zIL45ZZk4Sv35IK54E,11416
 diagnostic_tool/connector.py,sha256=CIqA7Ly0hqUSm7l6JaTGtKvqipFUXACCozw2rhj_bkQ,2027
-diagnostic_tool/diagnose.py,sha256=23wkXBxj9Tc8TlDGs5D3OJ4Qk0nTFyiFqBAYeKFiEns,9598
+diagnostic_tool/diagnose.py,sha256=ERCACWEeCdCiIF9ulfJUTZEe3i7cLwMJAFr-kF-tLvk,12128
 diagnostic_tool/dist_conf.py,sha256=57NQjOZAJBp2zzTCP7nWMNBfnOOeEqOhrKNLKB2T3Kc,9205
 diagnostic_tool/log_analyzer.py,sha256=9-RT1oqUeAZGxey743_gZKBWO_8cROFerNyy_VRcADM,4958
-diagnostic_tool/server_checker.py,sha256=K64fyUk9jROB0J5C9XraNyjqjEqyBAoKerXms19366U,5466
+diagnostic_tool/parser.py,sha256=kW7tYXXrt7eln0W6Kkg-irNgJj6W0k4II3uO5uEFWBk,2657
+diagnostic_tool/server_checker.py,sha256=QpPiPHEqa_Bx3-NUa_bEyxFKJVuHXVj0J9NnETy5L1Q,7914
+diagnostic_tool/table_checker.py,sha256=E99BizQfwfKtVh5mF7WyULuv8jnOy4sgV_xD4bDQShU,5153
 diagnostic_tool/util.py,sha256=rj21SHz8vhLoWGTakmd7grlqym0AWRpDShaoqA83XJ4,3042
-tests/__init__.py,sha256=N0qwVVP92fAXFf_K7yoDGR-CK-YMuLzWeeKVnB5G9OE,571
-tests/case_conf.py,sha256=scWBSwzqFZ0Csj9iNBQkQpOKsYAGI_T9hPDVohqNB_c,705
-tests/cmd_test.py,sha256=4vSZNp1RcaCcGNLOFklKAhxirrXbUTg1iqQ0ivvoQjQ,2525
-tests/conf_validator_test.py,sha256=o1MCK0vCFIrKXwa758abze3g7H6ts21WtCoKSfdWbfA,1274
-tests/dist_conf_test.py,sha256=JraagUc0pjMM6CZHirlhnNMDLvg8rAueO4kbFtE8kFE,2005
-tests/static_check_test.py,sha256=ns0dbaBF7YuTzWzNTrVn0uLCa6ZAjCgklX1wQmYa1xI,3040
-openmldb_tool-0.7.3.dist-info/METADATA,sha256=a5vqjt7GDHIhBaiASwv-X0U9xmnvCrcLZqGNxBHQthc,440
-openmldb_tool-0.7.3.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-openmldb_tool-0.7.3.dist-info/entry_points.txt,sha256=aUVKKZotgPl1Tb82p74g-W1ARley8qP0CXvjXL3jmNg,64
-openmldb_tool-0.7.3.dist-info/top_level.txt,sha256=MuwA0DwuKJiTd4srl0NHucbhyKsVouMbuCOwpodylVQ,22
-openmldb_tool-0.7.3.dist-info/RECORD,,
+openmldb_tool-0.8.1.dist-info/METADATA,sha256=Wo3D84SEQ-ausPHCsSQMXt6FW2P8EUirmD6oHCIAaDA,491
+openmldb_tool-0.8.1.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+openmldb_tool-0.8.1.dist-info/entry_points.txt,sha256=aUVKKZotgPl1Tb82p74g-W1ARley8qP0CXvjXL3jmNg,64
+openmldb_tool-0.8.1.dist-info/top_level.txt,sha256=l3w2A2Oy57wqrgi95wfEAxdmJsz7Umeoxf5WMObkJb4,16
+openmldb_tool-0.8.1.dist-info/RECORD,,
```

