# Comparing `tmp/redhat_qe_cloud_tools-1.0.7.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.7.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.8.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.7.tar` & `redhat_qe_cloud_tools-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/LICENSE
--rw-r--r--   0        0        0      852 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/__init__.py
--rw-r--r--   0        0        0     4478 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     4317 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      455 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/README.md
--rw-r--r--   0        0        0        0 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/roles.py
--rw-r--r--   0        0        0      554 2023-06-27 10:39:32.777041 redhat_qe_cloud_tools-1.0.7/clouds/aws/session_clients.py
--rw-r--r--   0        0        0     7805 2023-06-27 10:39:32.777041 redhat_qe_cloud_tools-1.0.7/clouds/aws/utilities/delete_aws_resources.py
--rw-r--r--   0        0        0      815 2023-06-27 10:39:32.777041 redhat_qe_cloud_tools-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/LICENSE
+-rw-r--r--   0        0        0      852 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/__init__.py
+-rw-r--r--   0        0        0     4478 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     4317 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      455 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/roles.py
+-rw-r--r--   0        0        0      554 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/session_clients.py
+-rw-r--r--   0        0        0     8197 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/utilities/delete_aws_resources.py
+-rw-r--r--   0        0        0      815 2023-06-29 14:06:23.153726 redhat_qe_cloud_tools-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.8/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.7/LICENSE` & `redhat_qe_cloud_tools-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/README.md` & `redhat_qe_cloud_tools-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.8/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.8/clouds/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.8/clouds/aws/delete_s3_velero_bucket.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/roles.py` & `redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/roles.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/clouds/aws/session_clients.py` & `redhat_qe_cloud_tools-1.0.8/clouds/aws/session_clients.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.7/clouds/aws/utilities/delete_aws_resources.py` & `redhat_qe_cloud_tools-1.0.8/clouds/aws/utilities/delete_aws_resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import multiprocessing
 import re
 import shlex
 import shutil
 
 import click
 from ocp_utilities.utils import run_command
 from simple_logger.logger import get_logger
@@ -77,15 +78,15 @@
     _iam_client = iam_client(region_name=region_name)
     roles_dict = _iam_client.list_roles(MaxItems=MAX_ITEMS)
     attached_role_policies_dict = {}
     detached_policy_names_dict = {}
     for role in roles_dict["Roles"]:
         role_name = role["RoleName"]
         if not re.search(
-            r"ManagedOpenShift|AWS|OrganizationAccountAccessRole|pco-|RedHatIT",
+            r"ManagedOpenShift|AWS|OrganizationAccountAccessRole|pco-|RedHatIT|RH-",
             role_name,
         ):
             # Need to iterate over both list_attached_role_policies and list_role_policies
             # For attached policies, we need to detach them using ARN
             attached_role_policies_dict = _iam_client.list_attached_role_policies(
                 RoleName=role_name, MaxItems=1000
             )
@@ -166,49 +167,65 @@
         click.echo(
             "cloud-nuke is not installed; install from https://github.com/gruntwork-io/cloud-nuke"
         )
         raise click.Abort()
 
     set_and_verify_aws_credentials()
 
-    rerun_cleanup_list = clean_aws_resources(aws_regions=_aws_regions)
-    while rerun_cleanup_list:
-        rerun_cleanup_list = clean_aws_resources(aws_regions=rerun_cleanup_list)
+    clean_aws_resources(aws_regions=_aws_regions)
 
 
 def clean_aws_resources(aws_regions):
+    rerun_cleanup_regions_list = []
+    jobs = []
+    cleanup_queue = multiprocessing.Queue()
+
+    for region in aws_regions:
+        job = multiprocessing.Process(
+            name=f"--- Clean up {region} ---",
+            target=clean_aws_region,
+            kwargs={"aws_region": region, "queue": cleanup_queue},
+        )
+        jobs.append(job)
+        job.start()
+
+    while not cleanup_queue.empty():
+        rerun_cleanup_regions_list.append(cleanup_queue.get())
+
+    for _job in jobs:
+        _job.join()
+
+    if rerun_cleanup_regions_list:
+        clean_aws_resources(aws_regions=rerun_cleanup_regions_list)
+
+
+def clean_aws_region(aws_region, queue):
     """Deletes AWS resources.
 
     Deletes open id connector providers, instance profiles and roles.
     (calls rds instances and vpc peerings connections - currently to only log data).
     Runs `cloud-nuke` utility - https://github.com/gruntwork-io/cloud-nuke
     Deletes S2 buckets.
+    Adds aws_region to queue in case additional cleanup is needed.
 
     Args:
-        aws_regions (list): list of AWS region names
+        aws_region (str): AWS region name
+        queue (Queue): multiprocessing queue to pass result
 
-    Returns:
-        list: list of cleanup functions return values
     """
-    rerun_cleanup_regions_list = []
-
-    for region_name in aws_regions:
-        LOGGER.info(f"Deleting resources in region {region_name}")
-        rerun_results = [
-            delete_rds_instances(region_name=region_name),
-            delete_vpc_peering_connections(region_name=region_name),
-            delete_open_id_connect_providers(region_name=region_name),
-            delete_instance_profiles(region_name=region_name),
-            delete_roles(region_name=region_name),
-        ]
-        run_command(
-            command=shlex.split(f"cloud-nuke aws --region {region_name} --force")
-        )
-        rerun_results.append(delete_buckets(region_name=region_name))
-        if any(rerun_results):
-            rerun_cleanup_regions_list.append(region_name)
+    LOGGER.info(f"Deleting resources in region {aws_region}")
+    rerun_results = [
+        delete_rds_instances(region_name=aws_region),
+        delete_vpc_peering_connections(region_name=aws_region),
+        delete_open_id_connect_providers(region_name=aws_region),
+        delete_instance_profiles(region_name=aws_region),
+        delete_roles(region_name=aws_region),
+    ]
+    run_command(command=shlex.split(f"cloud-nuke aws --region {aws_region} --force"))
+    rerun_results.append(delete_buckets(region_name=aws_region))
 
-    return rerun_cleanup_regions_list
+    if any(rerun_results):
+        queue.put(aws_region)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `redhat_qe_cloud_tools-1.0.7/pyproject.toml` & `redhat_qe_cloud_tools-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.7"
+version = "1.0.8"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
```

### Comparing `redhat_qe_cloud_tools-1.0.7/PKG-INFO` & `redhat_qe_cloud_tools-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

