# Comparing `tmp/gardener-cicd-cli-1.2101.0.tar.gz` & `tmp/gardener-cicd-cli-1.2102.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2101.0.tar", last modified: Wed Jun 28 12:19:43 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2102.0.tar", last modified: Thu Jun 29 14:31:52 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2101.0.tar` & `gardener-cicd-cli-1.2102.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:19:43.098311 gardener-cicd-cli-1.2101.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-28 12:19:43.098311 gardener-cicd-cli-1.2101.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:19:43.090310 gardener-cicd-cli-1.2101.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:19:43.094310 gardener-cicd-cli-1.2101.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     8114 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11329 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8618 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     8141 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12219 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/productutil_v2.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:19:43.098311 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-28 12:19:43.000000 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      937 2023-06-28 12:19:43.000000 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 12:19:43.000000 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-28 12:19:43.000000 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-28 12:19:43.000000 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-28 12:19:43.000000 gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 12:19:43.098311 gardener-cicd-cli-1.2101.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-06-28 12:18:24.000000 gardener-cicd-cli-1.2101.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:31:52.280129 gardener-cicd-cli-1.2102.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-29 14:31:52.280129 gardener-cicd-cli-1.2102.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:31:52.276129 gardener-cicd-cli-1.2102.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:31:52.276129 gardener-cicd-cli-1.2102.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     8114 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/productutil_v2.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:31:52.280129 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-29 14:31:52.000000 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-06-29 14:31:52.000000 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:31:52.000000 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-29 14:31:52.000000 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-29 14:31:52.000000 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-29 14:31:52.000000 gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 14:31:52.280129 gardener-cicd-cli-1.2102.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-06-29 14:18:03.000000 gardener-cicd-cli-1.2102.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2101.0/bin/component-cli` & `gardener-cicd-cli-1.2102.0/bin/component-cli`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2102.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/bin/purge_history` & `gardener-cicd-cli-1.2102.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2102.0/gardener_ci/productutil_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 CliHint = ci.util.CliHint
 
 parse = yaml.safe_load
 
 
 def _raw_component_dep_to_v2(raw: dict):
   if not 'componentName' in raw:
-    component_name = raw['name']
+    component_name = raw['name'].strip()
     name = product.v2.mangle_name(component_name)
   else:
-    component_name = raw['componentName']
-    name = raw['name']
+    component_name = raw['componentName'].strip()
+    name = raw['name'].strip()
+
+  version = raw['version'].strip()
 
   args = {
     'componentName': component_name,
     'name': name,
-    'version': raw['version'],
+    'version': version,
   }
 
   if 'labels' in raw:
     args['labels'] = raw['labels']
 
   return cm.ComponentReference(**args)
```

### Comparing `gardener-cicd-cli-1.2101.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2102.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2101.0/setup.py` & `gardener-cicd-cli-1.2102.0/setup.py`

 * *Files identical despite different names*

