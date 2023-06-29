# Comparing `tmp/pulumi_opsgenie-1.3.0a1687799894.tar.gz` & `tmp/pulumi_opsgenie-1.3.0a1688042112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.3.0a1687799894.tar", last modified: Mon Jun 26 17:22:31 2023, max compression
+gzip compressed data, was "pulumi_opsgenie-1.3.0a1688042112.tar", last modified: Thu Jun 29 12:39:25 2023, max compression
```

## Comparing `pulumi_opsgenie-1.3.0a1687799894.tar` & `pulumi_opsgenie-1.3.0a1688042112.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179600 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   160301 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 17:22:31.000000 pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:22:31.105456 pulumi_opsgenie-1.3.0a1687799894/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 17:22:30.000000 pulumi_opsgenie-1.3.0a1687799894/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:25.158597 pulumi_opsgenie-1.3.0a1688042112/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-29 12:39:25.158597 pulumi_opsgenie-1.3.0a1688042112/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:25.158597 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179600 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:25.158597 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160301 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:25.158597 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-29 12:39:25.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-29 12:39:25.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:25.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:25.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 12:39:25.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 12:39:25.000000 pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:39:25.158597 pulumi_opsgenie-1.3.0a1688042112/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-29 12:39:24.000000 pulumi_opsgenie-1.3.0a1688042112/setup.py
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/PKG-INFO` & `pulumi_opsgenie-1.3.0a1688042112/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.3.0a1687799894
+Version: 1.3.0a1688042112
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/README.md` & `pulumi_opsgenie-1.3.0a1688042112/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/api_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/email_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_escalation.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,20 +134,20 @@
     __args__['ownerTeamId'] = owner_team_id
     __args__['repeats'] = repeats
     __args__['rules'] = rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getEscalation:getEscalation', __args__, opts=opts, typ=GetEscalationResult).value
 
     return AwaitableGetEscalationResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        name=__ret__.name,
-        owner_team_id=__ret__.owner_team_id,
-        repeats=__ret__.repeats,
-        rules=__ret__.rules)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        owner_team_id=pulumi.get(__ret__, 'owner_team_id'),
+        repeats=pulumi.get(__ret__, 'repeats'),
+        rules=pulumi.get(__ret__, 'rules'))
 
 
 @_utilities.lift_output_func(get_escalation)
 def get_escalation_output(description: Optional[pulumi.Input[Optional[str]]] = None,
                           name: Optional[pulumi.Input[str]] = None,
                           owner_team_id: Optional[pulumi.Input[Optional[str]]] = None,
                           repeats: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetEscalationRepeatArgs']]]]] = None,
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,24 +192,24 @@
     __args__['intervalUnit'] = interval_unit
     __args__['name'] = name
     __args__['ownerTeamId'] = owner_team_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getHeartbeat:getHeartbeat', __args__, opts=opts, typ=GetHeartbeatResult).value
 
     return AwaitableGetHeartbeatResult(
-        alert_message=__ret__.alert_message,
-        alert_priority=__ret__.alert_priority,
-        alert_tags=__ret__.alert_tags,
-        description=__ret__.description,
-        enabled=__ret__.enabled,
-        id=__ret__.id,
-        interval=__ret__.interval,
-        interval_unit=__ret__.interval_unit,
-        name=__ret__.name,
-        owner_team_id=__ret__.owner_team_id)
+        alert_message=pulumi.get(__ret__, 'alert_message'),
+        alert_priority=pulumi.get(__ret__, 'alert_priority'),
+        alert_tags=pulumi.get(__ret__, 'alert_tags'),
+        description=pulumi.get(__ret__, 'description'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        interval=pulumi.get(__ret__, 'interval'),
+        interval_unit=pulumi.get(__ret__, 'interval_unit'),
+        name=pulumi.get(__ret__, 'name'),
+        owner_team_id=pulumi.get(__ret__, 'owner_team_id'))
 
 
 @_utilities.lift_output_func(get_heartbeat)
 def get_heartbeat_output(alert_message: Optional[pulumi.Input[Optional[str]]] = None,
                          alert_priority: Optional[pulumi.Input[Optional[str]]] = None,
                          alert_tags: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          description: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,20 +132,20 @@
     __args__['name'] = name
     __args__['ownerTeamId'] = owner_team_id
     __args__['timezone'] = timezone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getSchedule:getSchedule', __args__, opts=opts, typ=GetScheduleResult).value
 
     return AwaitableGetScheduleResult(
-        description=__ret__.description,
-        enabled=__ret__.enabled,
-        id=__ret__.id,
-        name=__ret__.name,
-        owner_team_id=__ret__.owner_team_id,
-        timezone=__ret__.timezone)
+        description=pulumi.get(__ret__, 'description'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        owner_team_id=pulumi.get(__ret__, 'owner_team_id'),
+        timezone=pulumi.get(__ret__, 'timezone'))
 
 
 @_utilities.lift_output_func(get_schedule)
 def get_schedule_output(description: Optional[pulumi.Input[Optional[str]]] = None,
                         enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                         name: Optional[pulumi.Input[str]] = None,
                         owner_team_id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__['description'] = description
     __args__['name'] = name
     __args__['teamId'] = team_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getService:getService', __args__, opts=opts, typ=GetServiceResult).value
 
     return AwaitableGetServiceResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        name=__ret__.name,
-        team_id=__ret__.team_id)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        team_id=pulumi.get(__ret__, 'team_id'))
 
 
 @_utilities.lift_output_func(get_service)
 def get_service_output(description: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        team_id: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceResult]:
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_team.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,18 +100,18 @@
     __args__['description'] = description
     __args__['members'] = members
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getTeam:getTeam', __args__, opts=opts, typ=GetTeamResult).value
 
     return AwaitableGetTeamResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        members=__ret__.members,
-        name=__ret__.name)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        members=pulumi.get(__ret__, 'members'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_team)
 def get_team_output(description: Optional[pulumi.Input[Optional[str]]] = None,
                     members: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetTeamMemberArgs']]]]] = None,
                     name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTeamResult]:
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/get_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,20 +132,20 @@
     __args__['role'] = role
     __args__['timezone'] = timezone
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        full_name=__ret__.full_name,
-        id=__ret__.id,
-        locale=__ret__.locale,
-        role=__ret__.role,
-        timezone=__ret__.timezone,
-        username=__ret__.username)
+        full_name=pulumi.get(__ret__, 'full_name'),
+        id=pulumi.get(__ret__, 'id'),
+        locale=pulumi.get(__ret__, 'locale'),
+        role=pulumi.get(__ret__, 'role'),
+        timezone=pulumi.get(__ret__, 'timezone'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(full_name: Optional[pulumi.Input[Optional[str]]] = None,
                     locale: Optional[pulumi.Input[Optional[str]]] = None,
                     role: Optional[pulumi.Input[Optional[str]]] = None,
                     timezone: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/incident_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/integration_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/schedule_rotation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opsgenie
-Version: 1.3.0a1687799894
+Version: 1.3.0a1688042112
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_opsgenie-1.3.0a1687799894/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.3.0a1688042112/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1687799894/setup.py` & `pulumi_opsgenie-1.3.0a1688042112/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1687799894"
-PLUGIN_VERSION = "1.3.0-alpha.1687799894+4e4f7c35"
+VERSION = "1.3.0a1688042112"
+PLUGIN_VERSION = "1.3.0-alpha.1688042112+d2a0f5f9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opsgenie', PLUGIN_VERSION])
         except OSError as error:
```

