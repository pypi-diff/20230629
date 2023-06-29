# Comparing `tmp/peek-field-service-3.4.5.tar.gz` & `tmp/peek-field-service-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-field-service-3.4.5.tar", last modified: Wed Jun 28 07:26:55 2023, max compression
+gzip compressed data, was "peek-field-service-3.4.6.tar", last modified: Thu Jun 29 10:20:44 2023, max compression
```

## Comparing `peek-field-service-3.4.5.tar` & `peek-field-service-3.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:55.249084 peek-field-service-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-28 07:26:55.249084 peek-field-service-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:55.248084 peek-field-service-3.4.5/peek_field_service/
--rw-r--r--   0 root         (0) root         (0)     1506 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/PeekClientConfig.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/PeekClientConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:55.249084 peek-field-service-3.4.5/peek_field_service/backend/
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/backend/ClientObservable.py
--rw-r--r--   0 root         (0) root         (0)     2247 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/backend/SiteRootResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:55.249084 peek-field-service-3.4.5/peek_field_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/plugin/ClientFrontendBuildersMixin.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/plugin/ClientPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/plugin/ClientPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/plugin/PeekClientPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9797 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/run_peek_field_service.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/run_peek_field_service_build_only.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/run_peek_field_service_offline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:55.249084 peek-field-service-3.4.5/peek_field_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      792 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-28 07:25:24.000000 peek-field-service-3.4.5/peek_field_service/winsvc_peek_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:55.248084 peek-field-service-3.4.5/peek_field_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1199 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/peek_field_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:55.249084 peek-field-service-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3259 2023-06-28 07:26:55.000000 peek-field-service-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:44.239447 peek-field-service-3.4.6/peek_field_service/
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/PeekClientConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/PeekClientConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/peek_field_service/backend/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/backend/ClientObservable.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/backend/SiteRootResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/peek_field_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/plugin/ClientFrontendBuildersMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/plugin/ClientPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/plugin/ClientPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/plugin/PeekClientPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9797 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/run_peek_field_service.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/run_peek_field_service_build_only.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/run_peek_field_service_offline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/peek_field_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-29 10:19:15.000000 peek-field-service-3.4.6/peek_field_service/winsvc_peek_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/peek_field_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/peek_field_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:44.240447 peek-field-service-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-29 10:20:44.000000 peek-field-service-3.4.6/setup.py
```

### Comparing `peek-field-service-3.4.5/peek_field_service/PeekClientConfig.py` & `peek-field-service-3.4.6/peek_field_service/PeekClientConfig.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/PeekClientConfigTest.py` & `peek-field-service-3.4.6/peek_field_service/PeekClientConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/backend/SiteRootResource.py` & `peek-field-service-3.4.6/peek_field_service/backend/SiteRootResource.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/plugin/ClientFrontendBuildersMixin.py` & `peek-field-service-3.4.6/peek_field_service/plugin/ClientFrontendBuildersMixin.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/plugin/ClientPluginLoader.py` & `peek-field-service-3.4.6/peek_field_service/plugin/ClientPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/plugin/ClientPluginLoaderTest.py` & `peek-field-service-3.4.6/peek_field_service/plugin/ClientPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/plugin/PeekClientPlatformHook.py` & `peek-field-service-3.4.6/peek_field_service/plugin/PeekClientPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/run_peek_field_service.py` & `peek-field-service-3.4.6/peek_field_service/run_peek_field_service.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/run_peek_field_service_build_only.py` & `peek-field-service-3.4.6/peek_field_service/run_peek_field_service_build_only.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/run_peek_field_service_offline.py` & `peek-field-service-3.4.6/peek_field_service/run_peek_field_service_offline.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/sw_install/PeekSwInstallManager.py` & `peek-field-service-3.4.6/peek_field_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service/winsvc_peek_client.py` & `peek-field-service-3.4.6/peek_field_service/winsvc_peek_client.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/peek_field_service.egg-info/SOURCES.txt` & `peek-field-service-3.4.6/peek_field_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.5/setup.py` & `peek-field-service-3.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_field_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Field Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

