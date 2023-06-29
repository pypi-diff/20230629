# Comparing `tmp/warpzone_sdk-8.0.0.tar.gz` & `tmp/warpzone_sdk-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-8.0.0.tar", max compression
+gzip compressed data, was "warpzone_sdk-8.1.0.tar", max compression
```

## Comparing `warpzone_sdk-8.0.0.tar` & `warpzone_sdk-8.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1071 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     1279 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2844 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3419 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1910 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/db/__init__.py
--rw-r--r--   0        0        0     1604 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/db/client.py
--rw-r--r--   0        0        0     1330 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/db/client_async.py
--rw-r--r--   0        0        0       47 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/__init__.py
--rw-r--r--   0        0        0     2916 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client.py
--rw-r--r--   0        0        0     2516 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client_async.py
--rw-r--r--   0        0        0      521 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/helpers.py
--rw-r--r--   0        0        0     2470 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/operations.py
--rw-r--r--   0        0        0      219 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2939 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/transform/data.py
--rw-r--r--   0        0        0     1833 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1279 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     2108 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3419 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     2105 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/process.py
+-rw-r--r--   0        0        0       46 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      781 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/processors/dependencies.py
+-rw-r--r--   0        0        0     1910 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/signature.py
+-rw-r--r--   0        0        0      547 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1604 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1330 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       47 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      521 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2470 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      219 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2939 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1833 2023-06-29 11:52:17.904246 warpzone_sdk-8.1.0/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.1.0/PKG-INFO
```

### Comparing `warpzone_sdk-8.0.0/pyproject.toml` & `warpzone_sdk-8.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "8.0.0"
+version = "8.1.0"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-8.0.0/warpzone/__init__.py` & `warpzone_sdk-8.1.0/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/blobstorage/client.py` & `warpzone_sdk-8.1.0/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/function/functionize.py` & `warpzone_sdk-8.1.0/warpzone/function/functionize.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from typing import Callable
 
 import typeguard
 
-from warpzone.function import monitor, process, signature
-from warpzone.function.processors import outputs, triggers
+from warpzone.function import monitor, process, signature, types
+from warpzone.function.processors.dependencies import DependencyProcessor
+from warpzone.function.processors.outputs import OutputProcessor
+from warpzone.function.processors.triggers import TriggerProcessor
 from warpzone.function.types import SingleArgumentCallable
 
 
 def functionize(
     f: SingleArgumentCallable,
-    trigger: triggers.TriggerProcessor,
-    output: outputs.OutputProcessor,
+    trigger: TriggerProcessor,
+    output: OutputProcessor,
+    dependencies: list[DependencyProcessor] = None,
 ) -> Callable:
     """Wrap function as an Azure function.
 
     Args:
         f (SingleArgumentCallable): Function with
             - argument of type specified in trigger processor
             - return value of type specified in output processor
-        trigger (triggers.TriggerProcessor): Trigger processor
-        output (outputs.OutputProcessor): Output processor
+        trigger (TriggerProcessor): Trigger processor
+        output (OutputProcessor): Output processor
+        dependencies (list[DependencyProcessor], optional): Dependency processors.
+            Defaults to None.
 
     Returns:
         Callable: Azure function with
             - argument
                 name: "<trigger.binding_name>"
                 annotation: "<trigger.arg_type>"
                 description: pre-argument of the original function
@@ -31,14 +36,22 @@
                 name: "context"
                 annotation: "azure.functions.Context"
                 description: Azure function context
             - return value
                 annotation: "<output.return_type>"
                 description: post-return value of the original function
     """
-    typeguard.check_type(f, SingleArgumentCallable)
+    if not dependencies:
+        dependencies = list()
 
-    main = process.pre_and_post_process(f, trigger, output)
+    # check types
+    typeguard.check_type(trigger, TriggerProcessor)
+    typeguard.check_type(output, OutputProcessor)
+    typeguard.check_type(dependencies, list[DependencyProcessor])
+    function_type = types.get_function_type(trigger, output, dependencies)
+    typeguard.check_type(f, function_type)
+
+    main = process.pre_and_post_process(f, trigger, output, dependencies)
 
     main = monitor.monitor(main)
     main = signature.redefine_signature(main, trigger, output)
     return main
```

### Comparing `warpzone_sdk-8.0.0/warpzone/function/integrations.py` & `warpzone_sdk-8.1.0/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/function/monitor.py` & `warpzone_sdk-8.1.0/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/function/processors/outputs.py` & `warpzone_sdk-8.1.0/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/function/processors/triggers.py` & `warpzone_sdk-8.1.0/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/function/signature.py` & `warpzone_sdk-8.1.0/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/healthchecks/__init__.py` & `warpzone_sdk-8.1.0/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/healthchecks/model.py` & `warpzone_sdk-8.1.0/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/monitor/logs.py` & `warpzone_sdk-8.1.0/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/monitor/traces.py` & `warpzone_sdk-8.1.0/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/servicebus/data/client.py` & `warpzone_sdk-8.1.0/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/servicebus/events/client.py` & `warpzone_sdk-8.1.0/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/tablestorage/db/client.py` & `warpzone_sdk-8.1.0/warpzone/tablestorage/db/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/tablestorage/db/client_async.py` & `warpzone_sdk-8.1.0/warpzone/tablestorage/db/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client.py` & `warpzone_sdk-8.1.0/warpzone/tablestorage/tables/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client_async.py` & `warpzone_sdk-8.1.0/warpzone/tablestorage/tables/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/helpers.py` & `warpzone_sdk-8.1.0/warpzone/tablestorage/tables/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/operations.py` & `warpzone_sdk-8.1.0/warpzone/tablestorage/tables/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/testing/assertions.py` & `warpzone_sdk-8.1.0/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/testing/data.py` & `warpzone_sdk-8.1.0/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/transform/data.py` & `warpzone_sdk-8.1.0/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/warpzone/transform/schema.py` & `warpzone_sdk-8.1.0/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.0.0/PKG-INFO` & `warpzone_sdk-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 8.0.0
+Version: 8.1.0
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

