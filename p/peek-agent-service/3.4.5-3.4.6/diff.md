# Comparing `tmp/peek-agent-service-3.4.5.tar.gz` & `tmp/peek-agent-service-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-agent-service-3.4.5.tar", last modified: Wed Jun 28 07:26:10 2023, max compression
+gzip compressed data, was "peek-agent-service-3.4.6.tar", last modified: Thu Jun 29 10:19:59 2023, max compression
```

## Comparing `peek-agent-service-3.4.5.tar` & `peek-agent-service-3.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:10.299069 peek-agent-service-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-28 07:26:10.299069 peek-agent-service-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:10.298069 peek-agent-service-3.4.5/peek_agent_service/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/PeekAgentConfig.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/PeekAgentConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:10.298069 peek-agent-service-3.4.5/peek_agent_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     1629 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/plugin/AgentPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/plugin/AgentPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/plugin/PeekAgentPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7053 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/run_peek_agent_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:10.298069 peek-agent-service-3.4.5/peek_agent_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-06-28 07:25:23.000000 peek-agent-service-3.4.5/peek_agent_service/winsvc_peek_agent_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:10.298069 peek-agent-service-3.4.5/peek_agent_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/peek_agent_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:10.299069 peek-agent-service-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2023-06-28 07:26:10.000000 peek-agent-service-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:59.657361 peek-agent-service-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-29 10:19:59.657361 peek-agent-service-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:59.656360 peek-agent-service-3.4.6/peek_agent_service/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/PeekAgentConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/PeekAgentConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:59.657361 peek-agent-service-3.4.6/peek_agent_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/plugin/AgentPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/plugin/AgentPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/plugin/PeekAgentPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7053 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/run_peek_agent_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:59.657361 peek-agent-service-3.4.6/peek_agent_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-29 10:19:14.000000 peek-agent-service-3.4.6/peek_agent_service/winsvc_peek_agent_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:59.657361 peek-agent-service-3.4.6/peek_agent_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/peek_agent_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:19:59.657361 peek-agent-service-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-29 10:19:59.000000 peek-agent-service-3.4.6/setup.py
```

### Comparing `peek-agent-service-3.4.5/peek_agent_service/PeekAgentConfig.py` & `peek-agent-service-3.4.6/peek_agent_service/PeekAgentConfig.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/PeekAgentConfigTest.py` & `peek-agent-service-3.4.6/peek_agent_service/PeekAgentConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/plugin/AgentPluginLoader.py` & `peek-agent-service-3.4.6/peek_agent_service/plugin/AgentPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/plugin/AgentPluginLoaderTest.py` & `peek-agent-service-3.4.6/peek_agent_service/plugin/AgentPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/plugin/PeekAgentPlatformHook.py` & `peek-agent-service-3.4.6/peek_agent_service/plugin/PeekAgentPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/run_peek_agent_service.py` & `peek-agent-service-3.4.6/peek_agent_service/run_peek_agent_service.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/sw_install/PeekSwInstallManager.py` & `peek-agent-service-3.4.6/peek_agent_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service/winsvc_peek_agent_service.py` & `peek-agent-service-3.4.6/peek_agent_service/winsvc_peek_agent_service.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/peek_agent_service.egg-info/SOURCES.txt` & `peek-agent-service-3.4.6/peek_agent_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.5/setup.py` & `peek-agent-service-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_agent_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Agent Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

