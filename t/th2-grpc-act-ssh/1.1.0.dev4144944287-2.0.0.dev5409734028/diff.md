# Comparing `tmp/th2_grpc_act_ssh-1.1.0.dev4144944287.tar.gz` & `tmp/th2_grpc_act_ssh-2.0.0.dev5409734028.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_ssh-1.1.0.dev4144944287.tar", last modified: Fri Feb 10 14:46:11 2023, max compression
+gzip compressed data, was "dist/th2_grpc_act_ssh-2.0.0.dev5409734028.tar", last modified: Thu Jun 29 07:47:22 2023, max compression
```

## Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287.tar` & `th2_grpc_act_ssh-2.0.0.dev5409734028.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2796 2023-02-10 14:45:30.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-02-10 14:45:31.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4543 2023-02-10 14:45:30.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-02-10 14:45:30.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14283 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5008 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-02-10 14:45:56.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh_service.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-02-10 14:46:11.000000 th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-06-29 07:46:30.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-29 07:46:31.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4522 2023-06-29 07:46:30.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-06-29 07:46:30.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-29 07:47:06.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-29 07:47:22.000000 th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/PKG-INFO` & `th2_grpc_act_ssh-2.0.0.dev5409734028/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_ssh
-Version: 1.1.0.dev4144944287
+Version: 2.0.0.dev5409734028
 Summary: th2_grpc_act_ssh
 Home-page: https://github.com/th2-net/th2-grpc-act-ssh
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC act template library (1.1.0)
+Description: # th2 gRPC act template library (2.0.0)
         
         This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j"). See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for details. <br>
         Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
         
         ## How to transform template
         1. Create a directory with the same name as project name (use underscores instead of dashes) under `src/main/proto` directory (remove other files and directories if they exist).
         2. Place your custom `.proto` files in created directory. Pay attention to `package` specifier and `import` statements.
@@ -52,14 +52,18 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release Notes
         
+        ### 2.0.0
+        
+        + Migrate to book and pages
+        
         ### 1.1.0
         
         + Update grpc-common version
         
         ### 1.0.0
         
         + Up major version for common V3 component
```

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/README.md` & `th2_grpc_act_ssh-2.0.0.dev5409734028/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# th2 gRPC act template library (1.1.0)
+# th2 gRPC act template library (2.0.0)
 
 This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j"). See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for details. <br>
 Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
 
 ## How to transform template
 1. Create a directory with the same name as project name (use underscores instead of dashes) under `src/main/proto` directory (remove other files and directories if they exist).
 2. Place your custom `.proto` files in created directory. Pay attention to `package` specifier and `import` statements.
@@ -44,14 +44,18 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release Notes
 
+### 2.0.0
+
++ Migrate to book and pages
+
 ### 1.1.0
 
 + Update grpc-common version
 
 ### 1.0.0
 
 + Up major version for common V3 component
```

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/setup.py` & `th2_grpc_act_ssh-2.0.0.dev5409734028/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.strict_mode = False
 
     def finalize_options(self):
         pass
 
     def run(self):
         proto_path = os.path.abspath('src/main/proto')
-        gen_path = os.path.abspath('src/gen/main/python')
+        gen_path = os.path.abspath('build/generated/source/proto/main/services/python')
 
         if not os.path.exists(gen_path):
             os.makedirs(gen_path)
 
         proto_files = []
         for root, _, files in os.walk(proto_path):
             for filename in files:
@@ -68,16 +68,15 @@
 
 
 class CustomDist(sdist):
 
     def run(self):
         copy_tree(f'src/main/proto/{package_name}', package_name)
 
-        copy_tree(f'src/gen/main/python/{package_name}', package_name)
-        copy_tree(f'src/gen/main/services/python/{package_name}', package_name)
+        copy_tree(f'build/generated/source/proto/main/services/python/{package_name}', package_name)
         Path(f'{package_name}/__init__.py').touch()
         Path(f'{package_name}/py.typed').touch()
 
         def make_packages(root_dir):
             for path in Path(root_dir).iterdir():
                 if path.is_dir():
                     path.joinpath('__init__.py').touch()
@@ -117,15 +116,15 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-act-ssh',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-common~=3.8.0'
+        'th2-grpc-common>=4,<5'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh.proto` & `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh_pb2.pyi` & `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -7,104 +7,100 @@
 import google.protobuf.empty_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
 import th2_grpc_common.common_pb2
 import typing
 import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class ExecutionRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class ParametersEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text = ...
-        value: typing.Text = ...
-
+        key: typing.Text
+        value: typing.Text
         def __init__(self,
             *,
-            key : typing.Text = ...,
-            value : typing.Text = ...,
+            key: typing.Text = ...,
+            value: typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     EVENT_INFO_FIELD_NUMBER: builtins.int
     EXECUTION_ALIAS_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     ENDPOINT_ALIAS_FIELD_NUMBER: builtins.int
-    execution_alias: typing.Text = ...
-    endpoint_alias: typing.Text = ...
-
     @property
     def event_info(self) -> global___EventInfo: ...
+    execution_alias: typing.Text
+    """The alias of the script or command described in the act-ssh settings"""
 
     @property
-    def parameters(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
+    def parameters(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]:
+        """The parameters that should be passed to the script"""
+        pass
+    endpoint_alias: typing.Text
+    """The alias for the endpoint to connect. If it is empty and the only one endpoint is define for the act that endpoint will be used"""
 
     def __init__(self,
         *,
-        event_info : typing.Optional[global___EventInfo] = ...,
-        execution_alias : typing.Text = ...,
-        parameters : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
-        endpoint_alias : typing.Text = ...,
+        event_info: typing.Optional[global___EventInfo] = ...,
+        execution_alias: typing.Text = ...,
+        parameters: typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
+        endpoint_alias: typing.Text = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"event_info",b"event_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"endpoint_alias",b"endpoint_alias",u"event_info",b"event_info",u"execution_alias",b"execution_alias",u"parameters",b"parameters"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["event_info",b"event_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["endpoint_alias",b"endpoint_alias","event_info",b"event_info","execution_alias",b"execution_alias","parameters",b"parameters"]) -> None: ...
 global___ExecutionRequest = ExecutionRequest
 
 class ExecutionResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
     EXIT_CODE_FIELD_NUMBER: builtins.int
     UNKNOWN_EXIT_CODE_FIELD_NUMBER: builtins.int
     OUTPUT_FIELD_NUMBER: builtins.int
     EMPTY_FIELD_NUMBER: builtins.int
     INTERUPTED_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
-    exit_code: builtins.int = ...
-    output: typing.Text = ...
-    interupted: builtins.bool = ...
-
+    exit_code: builtins.int
     @property
     def unknown_exit_code(self) -> google.protobuf.empty_pb2.Empty: ...
-
+    output: typing.Text
     @property
     def empty(self) -> google.protobuf.empty_pb2.Empty: ...
-
+    interupted: builtins.bool
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
-
     def __init__(self,
         *,
-        exit_code : builtins.int = ...,
-        unknown_exit_code : typing.Optional[google.protobuf.empty_pb2.Empty] = ...,
-        output : typing.Text = ...,
-        empty : typing.Optional[google.protobuf.empty_pb2.Empty] = ...,
-        interupted : builtins.bool = ...,
-        status : typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
+        exit_code: builtins.int = ...,
+        unknown_exit_code: typing.Optional[google.protobuf.empty_pb2.Empty] = ...,
+        output: typing.Text = ...,
+        empty: typing.Optional[google.protobuf.empty_pb2.Empty] = ...,
+        interupted: builtins.bool = ...,
+        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"empty",b"empty",u"exit_code",b"exit_code",u"exit_code_value",b"exit_code_value",u"output",b"output",u"result",b"result",u"status",b"status",u"unknown_exit_code",b"unknown_exit_code"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"empty",b"empty",u"exit_code",b"exit_code",u"exit_code_value",b"exit_code_value",u"interupted",b"interupted",u"output",b"output",u"result",b"result",u"status",b"status",u"unknown_exit_code",b"unknown_exit_code"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["empty",b"empty","exit_code",b"exit_code","exit_code_value",b"exit_code_value","output",b"output","result",b"result","status",b"status","unknown_exit_code",b"unknown_exit_code"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["empty",b"empty","exit_code",b"exit_code","exit_code_value",b"exit_code_value","interupted",b"interupted","output",b"output","result",b"result","status",b"status","unknown_exit_code",b"unknown_exit_code"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"exit_code_value",b"exit_code_value"]) -> typing_extensions.Literal["exit_code","unknown_exit_code"]: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["exit_code_value",b"exit_code_value"]) -> typing.Optional[typing_extensions.Literal["exit_code","unknown_exit_code"]]: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"result",b"result"]) -> typing_extensions.Literal["output","empty"]: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["result",b"result"]) -> typing.Optional[typing_extensions.Literal["output","empty"]]: ...
 global___ExecutionResponse = ExecutionResponse
 
 class EventInfo(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
-    description: typing.Text = ...
-
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
-
+    description: typing.Text
     def __init__(self,
         *,
-        parent_event_id : typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
-        description : typing.Text = ...,
+        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
+        description: typing.Text = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"description",b"description",u"parent_event_id",b"parent_event_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description",b"description","parent_event_id",b"parent_event_id"]) -> None: ...
 global___EventInfo = EventInfo
```

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh/act_ssh_pb2_grpc.py` & `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh/act_ssh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_ssh-1.1.0.dev4144944287/th2_grpc_act_ssh.egg-info/PKG-INFO` & `th2_grpc_act_ssh-2.0.0.dev5409734028/th2_grpc_act_ssh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-ssh
-Version: 1.1.0.dev4144944287
+Version: 2.0.0.dev5409734028
 Summary: th2_grpc_act_ssh
 Home-page: https://github.com/th2-net/th2-grpc-act-ssh
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC act template library (1.1.0)
+Description: # th2 gRPC act template library (2.0.0)
         
         This is the template project for creating custom gRPC act libraries. It contains proto messages and `Act` service that are used [th2 act template](https://github.com/th2-net/th2-act-template-j "th2-act-template-j"). See [act_template.proto](src/main/proto/th2_grpc_act_template/act_template.proto "act_template.proto") file for details. <br>
         Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
         
         ## How to transform template
         1. Create a directory with the same name as project name (use underscores instead of dashes) under `src/main/proto` directory (remove other files and directories if they exist).
         2. Place your custom `.proto` files in created directory. Pay attention to `package` specifier and `import` statements.
@@ -52,14 +52,18 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release Notes
         
+        ### 2.0.0
+        
+        + Migrate to book and pages
+        
         ### 1.1.0
         
         + Update grpc-common version
         
         ### 1.0.0
         
         + Up major version for common V3 component
```

